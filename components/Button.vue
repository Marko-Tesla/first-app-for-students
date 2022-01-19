<template>
  <div @click="logger" class="button">
    <div class="button-text">
        {{name}}
    </div>
  </div>
</template>

<script>
export default {
    name: 'Button',
    data() {
      return {
        name: 'Nurkhan',
        surname: 'Shakuali',
        age: '22'
      }
    },
    methods: {
        logger(){
            this.name = this.name + ' a'
            console.log(this.name, 'Button clicked');
        }
    }
}
</script>

<style scoped>
    .button {
        height: 30px;
        width: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
        border: 1px solid black;
    }
    .button-text {
        font-size: 12px;
        line-height: 19px;
        color: black;
    }
</style>
