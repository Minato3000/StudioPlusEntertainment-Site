<template>
<footer class="text-center lg:text-left bg-gradient-to-t from-green-500 to-emerald-500 text-black" id="footer">
    <div class="flex justify-center items-center text-center border-b border-green-600">
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
              text-xl
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
            <a href="https://www.youtube.com/c/StudioPlusEntertainment" class="text-black-600"><u>Studio Plus Entertainment</u></a>
          </p>
          <p class="mb-2">
            <a href="https://www.youtube.com/channel/UCwSqxN64xIErNIB9QNMvQ9Q" class="text-black-600"><u>Movies Park</u></a>
          </p>
          <p class="mb-2">
            <a href="https://www.youtube.com/channel/UCSz8cDJ3F48Ad9Eu3PD_YrA" class="text-black-600"><u>Video Park</u></a>
          </p>
          <p class="mb-2">
            <a href="https://www.youtube.com/channel/UCiCR5fA6-Vk_RX8wgc9po2Q" class="text-black-600"><u>Music Studio</u></a>
          </p>
          <p class="mb-2">
            <a href="https://www.youtube.com/channel/UC5ii-vTHcftOIA39u0E99WA" class="text-black-600"><u>Divine Studio</u></a>
          </p>
          <p class="mb-2">
            <a href="https://www.youtube.com/channel/UCdOHJnEku_1p8mR9tUpZdlw" class="text-black-600"><u>Meekaa TV</u></a>
          </p>
        </div>

        <div class="md:col-span-2 lg:col-span-1 md:mx-auto lg:mx-0">
          <h6 class="uppercase font-bold mb-4 flex justify-center lg:justify-start">
            contact
          </h6>
          <a href="https://www.facebook.com/profile.php?id=100084930345733" class="mr-6 text-black">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="facebook-f"
            class="w-2.5 lg:block inline-block" role="img" xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 320 512">
            <path fill="currentColor"
              d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z">
            </path>
          </svg>
        </a>
        <a href="https://instagram.com/studioplusentertainment?igshid=YmMyMTA2M2Y=" class="text-black-600">
          <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="instagram"
            class="w-3.5 lg:block inline-block" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">
            <path fill="currentColor"
              d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z">
            </path>
          </svg>
        </a>
        <MDBBtn tag="a" color="primary" href="#!" style="background-color: rgb(237, 48, 47);">
        <MDBIcon iconStyle="fab" icon="youtube"></MDBIcon>
      </MDBBtn>
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
              type: String,
              required: true,
            }
        }
    }
</script>

<style scoped>
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
