<template>
    <div>
        <h1 class="
            main-title
            inline-block 
            px-4 py-2
            ml-10 my-6
            mr-auto
            bg-green-200 
            rounded-3xl
            text-green-700 
            text-lg md:text-2xl 
            font-semibold
            capitalize 
        ">all videos</h1>
        <div class="
            vertical-grid 
            mx-4
            h-auto 
            px-2
            grid
            grid-cols-2
            md:grid-cols-3
            lg:grid-cols-4
            overflow-x-hidden
            overflow-y-auto           
            ">
            <div class="m-5 hover:cursor-pointer" v-for="detail in details">
                <img :src="detail.snippet.thumbnails.high.url" class="
                    thumbnail
                    w-full
                    "
                    :alt="detail.snippet.title">
                <div class="content w-full p-2 flex">
                    <div class="info flex flex-col">
                        <h4 class="title w-full h-10 font-medium text-sm text-green-500 overflow-hidden">{{ detail.snippet.title }}</h4>
                        <p class="channel-name my-1 font-extralight text-xs text-green-200">{{ detail.snippet.channelTitle }}</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="text-center">
        <button class="all-videos-btn py-2 px-5 text-green-700 bg-green-300 my-4 capitalize font-semibold">View more</button>
        </div>
    </div> 
</template>

<script>
    export default {
        data() {
            return {
            alldetails: [],
            details: [],
            api_key: "AIzaSyCkzCAGvVt7fKE_un1wHKvy2NLns86p3jQ",  // Another API key
            // api_key: "AIzaSyB6CbQR3WNUzTnuTg5iPvwNDfAqmdXjfII", // Another API key
            // api_key: "AIzaSyBIEWv1CI8xRwkfqVxJhv48edsuR-OjHiQ", // Another API key
            channel_id: "UCMHOIyUg_zfISaetTM0N_SQ",

        }
    },
    async fetch() {
    this.alldetails = await fetch(
        'https://www.googleapis.com/youtube/v3/search?' + new URLSearchParams({
            key: this.api_key,
            channelId: this.channel_id,
            order: 'date',
            part: 'snippet',
            maxResults: 6,
        })
    )
        .then(response => response.json())
        .then(data => {
            this.details = data.items;
        })
        .catch(err => console.log(err));
}
}

</script>


<style scoped>
.vertical-grid::-webkit-scrollbar {
        display: none;
    }

    .thumbnail {
        height: 9rem;
        object-fit: cover;
        border-radius: 4px;
        transition: transform 400ms cubic-bezier(0.075, 0.82, 0.165, 1);
    }

    .thumbnail:hover {
        transform: scale(1.1);
    }

    .main-title {
        box-shadow: rgba(0, 0, 0, 0.4) 0px 2px 4px,
            rgba(0, 0, 0, 0.3) 0px 7px 13px -3px,
            rgba(0, 0, 0, 0.2) 0px -3px 0px inset;
    }

    .all-videos-btn {
        border-radius: 100px;
        box-shadow: rgba(44, 187, 99, .2) 0 -25px 18px -14px inset, rgba(44, 187, 99, .15) 0 1px 2px, rgba(44, 187, 99, .15) 0 2px 4px, rgba(44, 187, 99, .15) 0 4px 8px, rgba(44, 187, 99, .15) 0 8px 16px, rgba(44, 187, 99, .15) 0 16px 32px;
        cursor: pointer;
        transition: all 250ms;
        border: 0;
        user-select: none;
        -webkit-user-select: none;
        touch-action: manipulation;
    }

    .all-videos-btn:hover {
        box-shadow: rgba(44, 187, 99, .35) 0 -25px 18px -14px inset, rgba(44, 187, 99, .25) 0 1px 2px, rgba(44, 187, 99, .25) 0 2px 4px, rgba(44, 187, 99, .25) 0 4px 8px, rgba(44, 187, 99, .25) 0 8px 16px, rgba(44, 187, 99, .25) 0 16px 32px;
        transform: scale(1.05) rotate(-1deg);
    }
</style>