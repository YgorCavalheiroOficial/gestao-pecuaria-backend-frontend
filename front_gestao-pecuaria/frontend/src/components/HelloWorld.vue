<template>
  <div> 
  <h1>HelloWorld</h1>
  <P>Link da API: {{ url_api }}</P>
  <P>Modo: {{ modo_env }}</P>
  <p>token: {{ token }}</p>
  </div>
</template>

<script>
export default {
data:() =>({
url_api:process.env.VUE_APP_API_URL,
modo_env:process.env.VUE_APP_MODE,
token:process.env.VUE_APP_TOKEN,
}),
name:'HelloWorld'
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
