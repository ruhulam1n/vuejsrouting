<template>
  <header class="header">
    <h1><img alt="Vue logo" src="../assets/logo.png"></h1>
    <nav class="nav">
      <ul>
          <li v-for="nav in navLinks" :key="nav.id">
              <router-link :class="`${(nav.path).replace('#','')}`" :to="nav.path">{{nav.text}}</router-link>
          </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isfixed: 'asas',
      navLinks: [
        { id: 1, text: 'Home', path: '#home' },
        { id: 2, text: 'About', path: '#about'},
        { id: 3, text: 'Contact',path: '#contact'},
        { id: 4, text: 'Services',path: '#services'}
      ],
    }
  },
  mounted() {
    window.addEventListener('scroll', function(){
      //Its called sticky on the navigation
      let header = document.querySelector('.header');
      let headerOuterHeight = header.outerHeight()+15;
      header.classList.toggle('is-sticky', window.scrollY > 0);
      let el = document.querySelectorAll('.is-scrolled');
      for (var i = 0, len = el.length; i < len; i++) {
          let elementTop = el[i].offsetTop;
          let elementBottom = elementTop + el[i].offsetHeight
          let windowTop = window.pageYOffset+headerOuterHeight
          let windowBottom = windowTop + window.outerHeight 
          if(elementBottom > windowTop && elementTop < windowBottom) {
            const nodeList = document.querySelectorAll('.nav a')
            for (let i = 0; i < nodeList.length; i++) {
              nodeList[i].classList.remove('active')
            }
            let activeElem = el[i].getAttribute('id')
            document.querySelector('.nav a.'+activeElem).classList.add('active')
          }
        }

    })

  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
html { 
  scroll-behavior: smooth; 
}
h3 {
  margin: 40px 0 0;
}
header.is-sticky{
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  background-color: rgba(0,0,0,0.7);
}
nav{

}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 15px;
}
a {
  color: #42b983;
  display: inline-block;
  margin-left: 15px;
  margin-right: 15px;
  text-transform: uppercase;
  text-decoration: none;
}
a.active {
  border-bottom: solid 3px #a00404;
}
</style>
