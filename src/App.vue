<template>
  <div id="app">
    <div id="he-plugin-standard"></div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      settings: ''
    }
  },
  mounted() {
    let settings = '<script> const WIDGET = { CONFIG: { "layout": 1, "width": 450, "height": 150, "background": 1, "dataColor": "FFFFFF", "borderRadius": 5, "key": "Your Key" } } <\/script>';
    $(settings).appendTo(document.body);
    $('<script src="https://widget.heweather.net/standard/static/js/he-standard-common.js?v=1.1" type="text/javascript"><\/script>').appendTo(document.body);
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
