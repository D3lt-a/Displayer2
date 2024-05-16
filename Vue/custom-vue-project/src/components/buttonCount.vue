<template>
    <button @click="increment">{{ label }}</button>
  </template>
  
  <script>
  export default {
    props: {
      label: {
        type: String,
        default: 'Click me'
      }
    },
    methods: {
      increment() {
        this.$emit('increment')
      }
    }
  }
  </script>
  
  <style scoped>
  </style>