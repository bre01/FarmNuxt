<template>
    <div>
        <div role="tablist" class="tabs tabs-lifted">
            <input type="radio" name="my_tabs_2" role="tab" class="tab" aria-label="关注" />
            <div role="tabpanel" class="tab-content bg-base-100 border-base-300 rounded-box p-6"><shows/></div>

            <input type="radio" name="my_tabs_2" role="tab" class="tab" aria-label="发现" checked />
            <div role="tabpanel" class="tab-content bg-base-100 border-base-300 rounded-box p-6"><shows/></div>

            <input type="radio" name="my_tabs_2" role="tab" class="tab" aria-label="本地" />
            <div role="tabpanel" class="tab-content bg-base-100 border-base-300 rounded-box p-6">
               <shows></shows> 
            </div>

        </div>
        <div id="show">
            <div v-for="content in contents">{{ content }}</div>
        </div>

    </div>
</template>
<script lang="ts" setup>
import { ref } from 'vue'
const contents = ref([]);

contents.value = ["Vue", "react", "angular", "lit"];


</script>
<style>
button {
    margin: 20px
}
</style>


