<template>
    <div class="bg-gray-900">
        <Header />
        <Banner v-bind:title="title" />
        <Horizontalgrid v-bind:channel_id="channel_id" />
        <Verticalgrid v-bind:channel_id="channel_id" />
        <Footer v-bind:title="title"/>
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
            title: "music studio",
            channel_dp: "~/static/images/musicstudio_dp.jpg",
        }
    }
}
</script>