<template>
  <div class="hello">
    <p>{{msg}}</p>
    <p>他是从{{here.pro}}来</p>
    <p>他是从{{here.type}}来</p>
    <p>他是从{{here.color}}来</p>
  </div>
</template>

<script>
export default {
  name: 'ChildCont',
  data () {
    return {
      msg: '我是子组件'
    }
  },
  props:['here']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
