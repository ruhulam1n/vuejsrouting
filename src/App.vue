<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
//import { reactive } from 'vue'
export default{
  data: () => {
    return {
      name: 'Fired Vue.js',
    }
  },

    // data: ()=> ({
    //    items: {
    //     title: 'How to do lists in Vue',
    //     author: 'Jane Doe',
    //     publishedAt: '2016-04-10'
    //   }
    // }),

  // data: () => ({
  //     items: [
  //       { id: 1, title: 'My journey with Vue' },
  //       { id: 2, title: 'Blogging with Vue' },
  //       { id: 3, title: 'Why Vue is so fun' }
  //     ]
  // })

  // data: () => ({
  //   numbers: [ 1, 2, 3, 4, 5 ]
  // }),
  // computed: {
  //   evenNumbers: function(){
  //     return this.numbers.filter(function(number){
  //       return number % 2 === 0
  //     })
  //   }
  // }
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
