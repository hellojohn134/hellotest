<template>
  <div class="hello">
    <p>{{msg}}</p>
    <ChildCont :here='info'/>

  </div>
</template>

<script>
import ChildCont from './ChildCont'
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: '我是父组件',
      info:{
        pro:'四川',
        type:'熊猫',
        color:'黑白相间'
      }
    }
  },
  components:{
    ChildCont
  }
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
