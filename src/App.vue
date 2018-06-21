<template>
  <div id="app">
    <router-view/>
    <banner-component/>
    <filter-component/>
    <data-stack/>
  </div>
</template>

<script>
import Banner from './components/Banner'
import Option from './components/Option'
import DataStack from './components/DataStack'

export default {
  name: 'App',
  components: {
    'banner-component': Banner,
    'filter-component': Option,
    'data-stack': DataStack
  }
}
</script>
