<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>Il a de trop grande jambe aimad :(
    </p>
    <h3>:)</h3>
    <p>{{coucou}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data : function() {
    return {
      coucou : "Merde Aimad tu saoules"
    }
  }
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
