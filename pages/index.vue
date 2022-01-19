<template>
  <div>
    <Button />
    Hello, World!
    <div class="red-text">
      red text
    </div>
    <div class="green-text">
      {{ name }}
    </div>
    <div class="green-text">
      {{ surname }}
    </div>
    <div class="green-text">
      {{ age }}
    </div>
  </div>
</template>

<script>
  import Button from '@/components/Button'

  export default {
    name: 'IndexPage',
    components: {Button},
    data() {
      return {
        name: 'Marat',
        surname: 'Prokudin',
        age: '23'
      }
    },
    
  }
</script>

<style scoped>
  .red-text {
    color: crimson;
  }

  .green-text {
    color: green;
  }
</style>
