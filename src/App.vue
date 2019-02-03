<template>
  <div id="app">
    <div id="msg">
      <h1>Welcome to Dami.io </h1>
      <h2>Machine Learning Translation</h2>
      <p>This is a <a href="vue.js">Vue.js</a> Web Application I built to help me crowdsource data <br>
      The data is snippets of dialog from the <a href="fraiser">Fraiser Show</a>. I want to use the data collected with this application to train a 
      Neural Network to do machine translation w/ ~>90% accuracy.<br>After that is done I can use the speech recording to train a model similar to googles wavenets<br>
      to detect yourba being spoken and translate it while also being able to synthesis yourba from english text.</p>
      <p>Here are the steps needed to help me collect data</p>
      <ol>
        <li>Translate the english snippet provided into yourba in the textfield below</li>
        <li>Record the translation you made using the audio recorder below</li>
        <li>When done refresh the page and continue again if you want</li>
      </ol>
      <br>
      <p>If you want to see some more of my projects <a href="www.github.com/conceptcodes">Click Me</a></p>
    </div>
    <EnglishText />
    <YorubaText />
    <Recording />
  </div>
</template>

<script>
  import EnglishText from './components/EnglishText.vue'
  import YorubaText from './componente/YorubaText.vue'
  import Recording from './componente/Recording.vue'

export default {
  name: 'app',
  components: {
    EnglishText,
    YorubaText,
    Recording
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
