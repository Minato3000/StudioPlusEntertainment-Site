<template>
    <div class="flex justify-center items-center flex-col">
        <img src="../static/images/entertainment_banner.jpg" alt="banner" class="
            w-screen
            opacity-70
        ">
        <div class="channel-details flex justify-center items-center py-4 mx-auto">
            <img src="../static/images/entertainment_dp.jpg" alt="channel icon" class="
                w-16
                md:w-20
                channel-dp
                rounded-[50%]
                mr-6
                md:mr-12
            ">
            <div class="info">
                <h4 class="
                    info-title
                    text-green-100
                    hover:text-green-500
                    hover:cursor-pointer
                    capitalize
                    text-xl
                    md:text-3xl
                    font-bold
                    tracking-wide
                    md:tracking-widest
                ">studio plus entertainment</h4>
                <p class="
                    info-extra
                    text-green-100
                    capitalize
                    text-md
                    md:text-lg
                ">99999 subscribers</p>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>

    .channel-dp {
        box-shadow: -6px 6px 8px black;
    }

    .info-title, .info-extra {
        text-shadow: -4px 4px 6px black;
    }

</style>