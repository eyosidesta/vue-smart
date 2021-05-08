<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <div>{{hello}} </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  data: () => ({
    books: 0,
    hello: "yes we do"
  }),
  beforeCreate() {
    console.log('beforCreate hook has been called');
      // alert('beforCreate hook has been called');
      console.log("books value is ", this.books)
      
    },
  
  created() {
    console.log('books value on created is: ', this.books)
    // alert('on create hook has been called');
    console.log('on create hook has been called');
  },

  beforeMount() {
    this.$data.hello = 'kakakakakakakakak'
    // alert('beforeMount has been called')
  },
  mounted() {
    this.$data.hello = 'lalalallalalalalala'
    // alert('mounted has been called')
  },
  beforeUpdate() {
    console.log('ggggggggggggggggggoooooooooooooodd before update')
    this.$data.hello = 'goooood'
  },
  // updated() {
  //   console.log('mmmmmmmmmmmmmmmmm updated')
  //   this.$data.hello = 'mmmmmmmmm'
  // },
  components: {
    HelloWorld
  }
}
</script>
