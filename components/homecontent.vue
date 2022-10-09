<template>
    <div class="content flex justify-center items-start flex-col w-max mx-auto my-12 gap-6">
        <a class="studioplus flex justify-center items-center flex-col md:flex-row w-full bg-gray-800 p-4 md:p-8 border border-none rounded-lg hover:cursor-pointer">
            <img src="~/static/images/entertainment_dp.jpg" alt="" class="channeldp mr-8 w-24 my-4 md:my-0">
            <h4 class="channel-name text-green-200 text-2xl font-bold capitalize">studio plus entertainment</h4>
        </a>
        <a class="musicstudio flex justify-start items-center flex-col md:flex-row w-full bg-gray-800 p-4 md:p-8 border border-none rounded-lg hover:cursor-pointer">
            <img src="~/static/images/musicstudio_dp.jpg" alt="" class="channeldp mr-8 w-24 my-4 md:my-0">
            <h4 class="channel-name text-green-200 text-2xl font-bold capitalize">music studio</h4>
        </a>
        <a class="divinestudio flex justify-start items-center flex-col md:flex-row w-full bg-gray-800 p-4 md:p-8 border border-none rounded-lg hover:cursor-pointer">
            <img src="~/static/images/divinestudio_dp.jpg" alt="" class="channeldp mr-8 w-24 my-4 md:my-0">
            <h4 class="channel-name text-green-200 text-2xl font-bold capitalize">divine studio</h4>
        </a>
        <a class="moviespark flex justify-start items-center flex-col md:flex-row w-full bg-gray-800 p-4 md:p-8 border border-none rounded-lg hover:cursor-pointer">
            <img src="~/static/images/moviespark_dp.jpg" alt="" class="channeldp mr-8 w-24 my-4 md:my-0">
            <h4 class="channel-name text-green-200 text-2xl font-bold capitalize">movies park</h4>
        </a>
        <a class="videopark flex justify-start items-center flex-col md:flex-row w-full bg-gray-800 p-4 md:p-8 border border-none rounded-lg hover:cursor-pointer">
            <img src="~/static/images/videopark_dp.jpg" alt="" class="channeldp mr-8 w-24 my-4 md:my-0">
            <h4 class="channel-name text-green-200 text-2xl font-bold capitalize">video park</h4>
        </a>
        <a class="meekaatv flex justify-start items-center flex-col md:flex-row w-full bg-gray-800 p-4 md:p-8 border border-none rounded-lg hover:cursor-pointer">
            <img src="~/static/images/meekaatv_dp.jpg" alt="" class="channeldp mr-8 w-24 my-4 md:my-0">
            <h4 class="channel-name text-green-200 text-2xl font-bold capitalize">meeKaa TV</h4>
        </a>
    </div>
</template>

<script>
    export default {
        name: 'homecontent',
    }
</script>

<style scoped>
    .channeldp {
        border-radius: 50%;
    }
</style>