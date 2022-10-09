<template>
    <div>
        <h1 class="
            main-title
            inline-block 
            px-4 py-2
            ml-10 my-6
            bg-green-200 
            rounded-3xl
            text-green-900 
            text-lg md:text-2xl 
            font-semibold
            capitalize 
        ">popular videos</h1>
        <div class="
            horizontal-grid 
            h-auto 
            px-5
            flex
            items-center 
            overflow-x-auto
            overflow-y-hidden           
            ">
            <div class="m-5 hover:cursor-pointer" v-for="detail in details" :click="redirect(detail)">
                <p>{{detail.id.videoId}}</p>
                <img :src="detail.snippet.thumbnails.high.url" class="thumbnail" :alt="detail.snippet.title">
                <div class="content w-full p-2 flex">
                    <div class="info flex flex-col">
                        <h4 class="title w-full h-10 font-medium text-sm text-green-500 overflow-hidden">{{
                        detail.snippet.title }}</h4>
                        <p class="channel-name my-1 font-extralight text-xs text-green-200">{{
                        detail.snippet.channelTitle }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        channel_id: {
            required: true,
        }
    },
    data() {
        return {
            alldetails: [],
            details: [],
            // api_key: "AIzaSyCkzCAGvVt7fKE_un1wHKvy2NLns86p3jQ",
            // api_key: "AIzaSyB6CbQR3WNUzTnuTg5iPvwNDfAqmdXjfII", // Another API key
            api_key: "AIzaSyBIEWv1CI8xRwkfqVxJhv48edsuR-OjHiQ", // Another API key

        }
    },
    methods: {
        redirect: function(detail) {
            window.location = "https://www.youtube.com/watch?v=" + detail.id.videoId;
        }
    },
    async fetch() {
        this.alldetails = await fetch(
            'https://www.googleapis.com/youtube/v3/search?' + new URLSearchParams({
                key: this.api_key,
                channelId: this.channel_id,
                order: 'viewCount',
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
.horizontal-grid::-webkit-scrollbar {
        height: 1em;
    }

    .horizontal-grid::-webkit-scrollbar-track {
        background-color: #15803D; 
        margin: 2em 20vw;
        border-radius: 100vh;
    }

    .horizontal-grid::-webkit-scrollbar-thumb {
        height: 2rem;
        border: 0.3em solid #15803D;
        border-radius: 100vh;
        background-color: #BBF7D0;
    }

    .horizontal-grid::-webkit-scrollbar-thumb:hover {
        background-color: #86EFAC;
    }

    .thumbnail {
        min-width: 17.5rem;
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
</style>