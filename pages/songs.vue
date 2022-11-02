<template>
    <div class="bg-gray-900">
        <Header />
        <Banner :title="title" :channel_url="channel_url" :image-url="require('~/static/images/musicstudio_dp.jpg')"/>
        <Horizontalgrid :channel_id="channel_id" />
        <Verticalgrid :channel_id="channel_id" :channel_url="channel_url"/>
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
            channel_id: "UCiCR5fA6-Vk_RX8wgc9po2Q",
            channel_url: "https://www.youtube.com/channel/UCiCR5fA6-Vk_RX8wgc9po2Q",
            title: "music studio",
        }
    }
}
</script>