<template>
    <div class="bg-gray-900">
        <Header />
        <Banner />
        <Horizontalgrid />
        <Verticalgrid />
        <Footer />
    </div>
</template>

<script>
import Header from '~/components/header.vue';
import Banner from '../components/banner.vue';
import Horizontalgrid from '../components/horizontalgrid.vue';
import Verticalgrid from '~/components/verticalgrid.vue';
import Footer from '~/components/footer.vue';

export default {
    name: "MoviesPage",
    components: {
    Header,
    Banner,
    Horizontalgrid,
    Verticalgrid,
    Footer
}
}
</script>