<template>
    <div>
        <div style="margin-left:20%">
            <input class=" input input-primary" placeholder="今天你对什么感兴趣" />
            <button class="btn btn-primary" style="margin-left: 20px;">搜索</button>

        </div>
        <!--
        <div v-for="keyword in keywords">
            {{ keyword }}
        </div>
        -->
        <div style="display:flex; flex-wrap: wrap; row-gap: 5%;">
        <div style=" width:40%;margin:5%" v-for="content in contents" class="card w-96 bg-base-100 shadow-xl">
            <figure><img src="https://daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.jpg" alt="Shoes" /></figure>
            <div class="card-body">
                <h2 class="card-title">{{ content }}</h2>
                <p>If a dog chews shoes whose shoes does he choose?</p>
                <div class="card-actions justify-end">
                    <button class="btn btn-primary">Buy Now</button>
                </div>
            </div>
        </div>
        </div>
    </div>
</template>
<script langt="ts" setup>
const keywords = ref([])
const contents = ref([]);
keywords.value = ["Vue", "react", "angular", "lit"]
contents.value = ["Vue", "react", "angular", "lit"]

</script>

