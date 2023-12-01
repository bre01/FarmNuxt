<template>
    <div class="single-show" v-for="show in shows ">
        <div class=" card card-side bg-base-100 shadow-xl">
            <figure><img src="https://daisyui.com/images/stock/photo-1635805737707-575885ab0820.jpg" alt="Movie" /></figure>
            <div class="card-body">
                <h2 class="card-title">New movie is released!</h2>
                <p>Click the button to watch on Jetflix app.</p>
                <div class="card-actions justify-end">
                    <button class="btn btn-primary">Watch</button>
                </div>
            </div>
        </div>
    </div>
</template>
<script lang="ts" setup>
const shows = ref([]) 
shows.value = ["Vue", "react", "angular", "lit"]  
</script>
<style>
.single-show {
    margin: 20px;
    border: 1px solid black; 
    border-radius: 18px;
}
</style>