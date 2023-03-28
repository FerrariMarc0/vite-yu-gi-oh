<script>
  import axios from 'axios';
  import {store} from './store'
  import AppHeader from './components/AppHeader.vue'
  import AppMain from './components/AppMain.vue'
  import AppFooter from './components/AppFooter.vue'
  export default{
    name: 'app',
    components: {
      AppHeader,
      AppMain,
      AppFooter
    },
    data(){
      return{
        store
      }
    },
    methods: {
      search(){
        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php', {
          params: {
            status: store.searchStatus
          }
        }).then((response) => {
                
                this.store.characters = response.data.data;
                this.store.charactersFound = response.data.data.length;
            }).catch((error) => {
              this.store.characters = [];
              this.store.charactersFound = 0;
            })
      }
    },
    created(){
      this.search();
    }
  }
</script>

<template>
  <AppHeader/>
  <AppMain @find="search"/>
  <AppFooter/>
</template>
