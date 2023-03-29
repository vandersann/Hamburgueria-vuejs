<template>
  <div>
    <primeiro />
    <LifeCycle />
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import  primeiro from './components/primeiro.vue'

export default {
  name: 'App',
  components: {
    primeiro,
    LifeCycle
  },
  data() {
    return {

    }
  }
}
</script>
