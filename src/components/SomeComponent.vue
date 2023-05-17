<template>
  
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({

  props: {
    someProp: String
  },

  data: () => ({ 
    someData: ''
  }),

  computed: {
    someComputed() {
      return this.someData
    }
  },

  methods: {
    someMethod() {
      this.someData
    }
  }
})
</script>

<style scoped>

</style>
