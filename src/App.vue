<script>
// un componente si importa in un altro in 3 passaggi:
//  1 - importo il file in cima al mio script e gli assegno un nome
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
// 2 - Lo inserisco nella lista dei componenti di questo componente
// 3 - Lo inserisco come un self-closing tag nell'html

export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>

<template>
  <div>
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
</template>

<style scoped>
</style>
