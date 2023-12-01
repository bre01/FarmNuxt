<template>
    <div>
        <div style="margin-left:20%">
            <form style="">
                <input type="text" placeholder="Type here" class="input input-bordered w-full max-w-xs" style="margin-right: 20px;"/>
                <button class="btn" style="margin-right:20px">Button</button>

            </form>
        </div>
        

        <div>
            <div class="keyword" v-for="keyword in keywords" style="display: inline; margin: 20px;">
                
            {{ keyword }}</div>
        </div>



        <div id="videos">
            <div class="single-video" v-for="video in videos">

                <video width="320" height="240" controls>
                    <source :src="video.videoUrl" type="video/mp4">
                </video>
            </div>
        </div>







    </div>
</template>
<style>
.single-video{
    display: inline-block;
    margin: 20px;
    border: 1px solid black; 

}
</style>

<script lang="ts" setup>
import type { Video } from "../interfaces/video.ts"
import { ref } from 'vue'
const keywords=ref([])
keywords.value=["Vue","react","angular","lit"]
const example: Video =
{
    id: '1',
    title: "Vue3",
    description: "Vue3 is awesome",
    videoUrl: "1.mkv",
}


const videos = ref([])
videos.value.push(example)
videos.value.push(example)
videos.value.push(example)
videos.value.push(example)
videos.value.push(example)
videos.value.push(example)
videos.value.push(example)
videos.value.push(example)
console.log(videos.value)
/*
fetch('http://localhost:3000/videos')
    .then(res => res.json())
    .then(res => {
        //videos.value=res
        console.log(videos.value)
    })

*/
</script>