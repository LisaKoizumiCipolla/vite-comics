<script>
import NewHeader from './components/NewHeader.vue';
import NewMain from './components/NewMain.vue';
import NewFooter from './components/NewFooter.vue';

export default {
    name: 'App',
    components:{
      NewHeader,
      NewMain,
      NewFooter
    }
}
</script>

<template>
  <NewHeader />
  <NewMain />
  <NewFooter />
</template>

<style lang="scss">
@import "./styles/general.scss";
</style>
