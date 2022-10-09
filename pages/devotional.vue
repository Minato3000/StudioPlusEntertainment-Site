<template>
    <div class="bg-gray-900">
        <Header />
        <Banner :title="title" :image-url="require('~/static/images/divinestudio_dp.jpg')"/>
        <Horizontalgrid :channel_id="channel_id" />
        <Verticalgrid :channel_id="channel_id" />
        <Footer :title="title"/>
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
    },
    data() {
        return {
            channel_id: "UC5ii-vTHcftOIA39u0E99WA",
            title: "divine studio",
        }
    },
}
</script>