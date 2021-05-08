<template>
 <div>
   <!-- <h1>{{msg}}</h1> -->
 </div>
</template>
<script>
export default {
 name: 'HelloWorld',
 beforeCreate() {
  alert('beforCreate hook has been called');
  console.log('beforCreate hook has been called');
 },
 created() {
   alert('on create hook has been called');
  console.log('on create hook has been called');
 },
 props: {
  msg: String
 }
}
</script>
<! — Add “scoped” attribute to limit CSS to this component only →
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
 

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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
