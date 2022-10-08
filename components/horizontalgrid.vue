<template>
    <div>
        <h1 class="
            inline-block 
            px-4 py-2
            ml-10 my-6
            bg-green-200 
            rounded-3xl
            text-green-700 text-2xl 
            font-semibold
            capitalize 
            ">popular videos</h1>

        <div class="horizontal-grid">
            <div class="video"  v-for="detail in details">
                <img :src="detail.snippet.thumbnails.high.url" class="thumbnail" :alt="detail.snippet.title">
                <div class="content">
                    <div class="info">
                        <h4 class="title">{{ detail.snippet.title }}</h4>
                        <p class="channel-name">{{ detail.snippet.channelTitle }}</p>
                    </div>
                </div>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    data() {
        return {
            alldetails: [],
            details: [],
            api_key: "AIzaSyCkzCAGvVt7fKE_un1wHKvy2NLns86p3jQ",
            channel_id: "UCMHOIyUg_zfISaetTM0N_SQ",

        }
    },
    async fetch() {
        this.alldetails = await fetch(
            'https://www.googleapis.com/youtube/v3/search?' + new URLSearchParams({
                key: this.api_key,
                channelId: this.channel_id,
                order: 'viewCount',
                part: 'snippet',
                maxResults: 2,
            })
        ).then(response => response.json())
        .then(data => {
            this.details = data.items;
            console.log(this.details)
        })
    }
}

</script>

<style scoped>
    .horizontal-grid {
        width: 100%;
        height: auto;
        padding: 0 20px;
        display: flex;
        align-items: center;
        overflow-x: auto;
        overflow-y: hidden;
    }

    .horizontal-grid::-webkit-scrollbar {
        display: none;
    }

    .video {
        height: 250px;
        cursor: pointer;
        margin: 20px;
    }

    .thumbnail {
        width: 280px;
        height: 150px;
        object-fit: cover;
        border-radius: 4px;
        transition: transform 400ms cubic-bezier(0.075, 0.82, 0.165, 1);
    }

    .thumbnail:hover {
        transform: scale(1.1);
    }

    .content {
        width: 100%;
        height: 100px;
        padding: 10px;
        display: flex;
    }

    .info {
        display: flex;
        flex-direction: column;
    }

    .title {
        width: 100%;
        max-height: 40px;
        color: #cae962;
        font-size: 14px;
        overflow: hidden;
    }

    .channel-name {
        font-size: 12px;
        margin: 2px 0;
        color: rgba(202, 233, 98, 0.5);
    }
</style>