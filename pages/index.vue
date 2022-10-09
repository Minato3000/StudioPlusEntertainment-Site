<template>
  <div class="bg-gray-900">
    <Header />
    <Homecontent />
    <Footer :title="title"/>
  </div>
</template>

<script>
import Header from '~/components/header.vue';
import Homecontent from '~/components/homecontent.vue';
import Footer from '~/components/footer.vue';


export default {
    name: "IndexPage",
    components: { Header, Homecontent, Footer },
    data() {
      return {
        title: "studio plus",
      }
    }
}
</script>
