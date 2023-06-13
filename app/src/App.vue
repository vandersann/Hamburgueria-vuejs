<template>
  <div>
    <primeiro />
    <LifeCycle />
    <Pessoa/>
  </div>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue'
import  primeiro from './components/primeiro.vue'
import Pessoa from './components/Pessoa.vue'

export default {
  name: 'App',
  components: {
    primeiro,
    LifeCycle,
    Pessoa
  },
  data() {
    return {

    }
  }
}
</script>
