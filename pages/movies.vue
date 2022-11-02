<template>
    <div class="bg-gray-900">
        <Header />
        <Banner :title="title" :channel_url="channel_url" :image-url="require('~/static/images/entertainment_dp.jpg')"/>
        <Horizontalgrid :channel_id="channel_id"/>
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
            channel_id: "UCMHOIyUg_zfISaetTM0N_SQ",
            channel_url: "https://www.youtube.com/channel/UCMHOIyUg_zfISaetTM0N_SQ",
            title: "studio plus entertainment",
        }
    }
}
</script>