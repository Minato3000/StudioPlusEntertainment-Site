<template>
<footer class="text-center lg:text-left bg-gradient-to-t from-green-500 to-emerald-500 text-black" id="footer">
    <div class="flex justify-center items-center text-center p-6 border-b border-green-600">
      <div class="flex align-center text-center inline-block">
        <h4 class="inline-block capitalize text-2xl md:text-3xl font-bold hover:cursor-pointer tracking-wide md:tracking-widest">{{ title }}</h4>
      </div>
    </div>
    <div class="mx-6 py-10 text-center md:text-left">

    <div class="grid grid-1 md:grid-cols-2 lg:grid-cols-3 gap-8 lg:gap-48">

        <div class="">
          <h6 class="
              uppercase
              font-bold
              mb-4
              flex
              items-center
              justify-center
              lg:justify-start
            ">
            about us
          </h6>
          <p class="text-start">
            Studio Plus Entertainment is a Upcoming Production Company & Digital Media Company which brings in more content from Indian Movies. Watch Full Length Old And New Movies, Comedy , Scenes , Music & Devotional Content.
          </p>
        </div>

        <div class="md:mx-auto lg:mx-0">
          <h6 class="uppercase font-bold mb-4 flex justify-center md:justify-start">
            channels
          </h6>
          <p class="mb-2">
            <a href="#!" class="text-black-600">Studio Plus Entertainment</a>
          </p>
          <p class="mb-2">
            <a href="#!" class="text-black-600">Movies Park</a>
          </p>
          <p class="mb-2">
            <a href="#!" class="text-black-600">Video Park</a>
          </p>
          <p class="mb-2">
            <a href="#!" class="text-black-600">Music Studio</a>
          </p>
          <p class="mb-2">
            <a href="#!" class="text-black-600">Divine Studio</a>
          </p>
          <p class="mb-2">
            <a href="#!" class="text-black-600">Meeka TV</a>
          </p>
        </div>

        <div class="md:col-span-2 lg:col-span-1 md:mx-auto lg:mx-0">
          <h6 class="uppercase font-bold mb-4 flex justify-center lg:justify-start">
            contact
          </h6>
          <a href="#!" class="mr-6 text-black">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="facebook-f"
            class="w-2.5 lg:block inline-block" role="img" xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 320 512">
            <path fill="currentColor"
              d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z">
            </path>
          </svg>
        </a>
        <a href="#!" class="mr-6 text-black-600">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="twitter"
            class="w-4 lg:block inline-block" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
            <path fill="currentColor"
              d="M459.37 151.716c.325 4.548.325 9.097.325 13.645 0 138.72-105.583 298.558-298.558 298.558-59.452 0-114.68-17.219-161.137-47.106 8.447.974 16.568 1.299 25.34 1.299 49.055 0 94.213-16.568 130.274-44.832-46.132-.975-84.792-31.188-98.112-72.772 6.498.974 12.995 1.624 19.818 1.624 9.421 0 18.843-1.3 27.614-3.573-48.081-9.747-84.143-51.98-84.143-102.985v-1.299c13.969 7.797 30.214 12.67 47.431 13.319-28.264-18.843-46.781-51.005-46.781-87.391 0-19.492 5.197-37.36 14.294-52.954 51.655 63.675 129.3 105.258 216.365 109.807-1.624-7.797-2.599-15.918-2.599-24.04 0-57.828 46.782-104.934 104.934-104.934 30.213 0 57.502 12.67 76.67 33.137 23.715-4.548 46.456-13.32 66.599-25.34-7.798 24.366-24.366 44.833-46.132 57.827 21.117-2.273 41.584-8.122 60.426-16.243-14.292 20.791-32.161 39.308-52.628 54.253z">
            </path>
          </svg>
        </a>
        <a href="#!" class="mr-6 text-black-600">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="youtube"
            class="w-3.5 lg:block inline-block" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 488 512">
            <path fill="currentColor"
              d="M488 261.8C488 403.3 391.1 504 248 504 110.8 504 0 393.2 0 256S110.8 8 248 8c66.8 0 123 24.5 166.3 64.9l-67.5 64.9C258.5 52.6 94.3 116.6 94.3 256c0 86.5 69.1 156.6 153.7 156.6 98.2 0 135-70.4 140.8-106.9H248v-85.3h236.1c2.3 12.7 3.9 24.9 3.9 41.4z">
            </path>
          </svg>
        </a>
        <a href="#!" class="text-black-600">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="instagram"
            class="w-3.5 lg:block inline-block" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">
            <path fill="currentColor"
              d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z">
            </path>
          </svg>
        </a>
        </div>
      </div>

    </div>

    <div class="text-center p-6">
      <span>Developed by </span>
      <a class="text-black-600 font-semibold" href="https://www.wimax.live/">WiMaX CLUB</a>
    </div>
  </footer>
</template>

<script>
    export default {
        props: {
            title: {
                required: true,
            }
        }
    }
</script>

<style>
.footer {
    box-shadow: 0rem -1rem 8rem -4rem #34D399 ;
}

.links {
    margin-right: 2rem;
}

.links svg {
    transition: all 400ms ;
}

</style>