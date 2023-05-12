<script >

import AContattiAzienda from './components/AContattiAzienda.vue';
import BbHeaderComp from './components/BbHeaderComp.vue';
import BaNavComp from './components/BaNavComp.vue';
import CMainComp from './components/CMainComp.vue';
import DFooterComp from './components/DFooterComp.vue';


export default {
  components: {
    AContattiAzienda,
    BaNavComp,
    BbHeaderComp,
    CMainComp,
    DFooterComp,


  }
}

</script>

<template>
  <AContattiAzienda />
  <div>
    <BaNavComp />
    <BbHeaderComp />
  </div>
  <CMainComp />
  <DFooterComp />
</template>

<style lang="scss">
@use './style/main.scss';
</style>
