<template>
    <div class="bg-gray-900">
        <Header />
        <Banner />
        <Horizontalgrid />
    </div>
</template>

<script>
import Header from '~/components/header.vue';
import Banner from '../components/banner.vue';
import Horizontalgrid from '../components/horizontalgrid.vue';

export default {
    name: "MoviesPage",
    components: {
    Header,
    Banner,
    Horizontalgrid
}
}
</script>