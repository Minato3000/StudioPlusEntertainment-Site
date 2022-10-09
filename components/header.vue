<template>
    <nav class="
        flex 
        justify-evenly md:justify-start 
        items-center 
        pt-6 pb-1 
        md:pt-10 md:pb-4 
        bg-gray-900 
        px-12
        md:px-40 
        z-10"
    >
        <a href="/" class="links md:mr-10 text-lg md:text-2xl capitalize md:tracking-wider text-green-100 hover:text-green-500">HOME</a>
        <a href="/movies" class="links md:mr-10 text-lg md:text-2xl capitalize md:tracking-wider text-green-100 hover:text-green-500">MOVIES</a>
        <a href="/songs" class="links md:mr-10 text-lg md:text-2xl capitalize md:tracking-wider text-green-100 hover:text-green-500">SONGS</a>
        <a href="/devotional" class="links md:mr-10 text-lg md:text-2xl capitalize md:tracking-wider text-green-100 hover:text-green-500">DEVOTIONAL</a>
    </nav>
</template>

<style scoped>
nav {
        box-shadow: -100px 0 100px black;
    }

    .links {
        transition: all 300ms cubic-bezier(0.35, 0.83, 0, 0.99);
    }
</style>