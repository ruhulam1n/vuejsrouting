<template>
    <div>
      <HeaderComp msg="This is header"/>   
      <h2>Home</h2>
      <div id="home" class="content is-scrolled">
        <p><span>Iure excepturi eligendi dolorem tempore deserunt maxime dolorum at pariatur reiciendis, nesciunt nam autem neque consectetur! Debitis, quisquam perspiciatis animi earum dolorum enim. Consectetur dignissimos veritatis eius doloremque ducimus esse.</span><span>Ullam doloribus quaerat id. Dolor iste illo illum, dolores eum est aliquam magni laborum? Cum aliquam tempora ut enim quam consequatur nulla, in itaque atque commodi id ipsam necessitatibus eaque?</span><span>Aperiam perspiciatis quas facere laudantium laboriosam voluptatum iusto explicabo iste quia magni nulla, eligendi dignissimos, quidem tenetur eos saepe dolorum reprehenderit possimus repellendus impedit provident ab corrupti voluptatibus culpa. Reprehenderit.</span><span>Totam odio officiis assumenda repudiandae quidem, doloribus eos ad maiores. Fugit animi sed eaque hic, molestiae tempora dolores quas eum neque asperiores, facere libero aspernatur dignissimos incidunt ducimus? Consequuntur, dicta?</span></p>
        <p><span>Iure excepturi eligendi dolorem tempore deserunt maxime dolorum at pariatur reiciendis, nesciunt nam autem neque consectetur! Debitis, quisquam perspiciatis animi earum dolorum enim. Consectetur dignissimos veritatis eius doloremque ducimus esse.</span><span>Ullam doloribus quaerat id. Dolor iste illo illum, dolores eum est aliquam magni laborum? Cum aliquam tempora ut enim quam consequatur nulla, in itaque atque commodi id ipsam necessitatibus eaque?</span><span>Aperiam perspiciatis quas facere laudantium laboriosam voluptatum iusto explicabo iste quia magni nulla, eligendi dignissimos, quidem tenetur eos saepe dolorum reprehenderit possimus repellendus impedit provident ab corrupti voluptatibus culpa. Reprehenderit.</span><span>Totam odio officiis assumenda repudiandae quidem, doloribus eos ad maiores. Fugit animi sed eaque hic, molestiae tempora dolores quas eum neque asperiores, facere libero aspernatur dignissimos incidunt ducimus? Consequuntur, dicta?</span></p>
        <p><span>Iure excepturi eligendi dolorem tempore deserunt maxime dolorum at pariatur reiciendis, nesciunt nam autem neque consectetur! Debitis, quisquam perspiciatis animi earum dolorum enim. Consectetur dignissimos veritatis eius doloremque ducimus esse.</span><span>Ullam doloribus quaerat id. Dolor iste illo illum, dolores eum est aliquam magni laborum? Cum aliquam tempora ut enim quam consequatur nulla, in itaque atque commodi id ipsam necessitatibus eaque?</span><span>Aperiam perspiciatis quas facere laudantium laboriosam voluptatum iusto explicabo iste quia magni nulla, eligendi dignissimos, quidem tenetur eos saepe dolorum reprehenderit possimus repellendus impedit provident ab corrupti voluptatibus culpa. Reprehenderit.</span><span>Totam odio officiis assumenda repudiandae quidem, doloribus eos ad maiores. Fugit animi sed eaque hic, molestiae tempora dolores quas eum neque asperiores, facere libero aspernatur dignissimos incidunt ducimus? Consequuntur, dicta?</span></p>
        <img src="https://picsum.photos/id/906/600/400" alt="">
        <img src="https://picsum.photos/id/112/600/400" alt="">
        <img src="https://picsum.photos/id/743/600/400" alt="">
      </div>
      <AboutView msg="This is header"/> 
      <ServicesView msg="This is header"/> 
      <ContactView msg="This is header"/> 
      <FooterComp msg="This is Footer"/>
    </div>
</template>

<script>
// @ is an alias to /src
import HeaderComp from '../components/HeaderComp.vue';
import FooterComp from '../components/FooterComp.vue';

import AboutView from '../views/AboutView.vue';
import ServicesView from '../views/ServicesView.vue';
import ContactView from '../views/ContactView.vue';


export default {
  components: {
    HeaderComp,
    AboutView,
    ServicesView,
    ContactView,
    FooterComp
  }
}
</script>
