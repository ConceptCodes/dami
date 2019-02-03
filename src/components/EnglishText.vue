<template>
  <div class="text">
   <p> {{ txt }} </p>
  </div>
</template>

<script>
  export default {
    name: 'EnglishText',
    props: {
      txt : String
    },
    data () {
      eng : []
    },
    methods: {
      getEngText: function() { this.eng = require('../static/eng.json'); },
      selectSnippet: function() { this.txt = this.eng[Math.floor(Math.random()*this.eng.length)]; },
      checkText: function() { return this.txt.length > 0 }
  },
  beforeCreate(){ this.getEngText(); },
  beforeMount(){ this.selectSnippet(); }
  }
</script>

<style scoped>
 p {
   font-size: 25px;
 }
</style>
