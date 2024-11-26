<template>
    <div class="card" style="width: 14rem;">
        <img :src="book.img_url" class="card-img-top">
        <div class="card-body">
            <h5 class="card-title">{{ props['book'].title }}</h5>
            <p class="card-text">{{ props['book'].author }}</p>
            <p class="card-text">{{ props['book'].description }}</p>
        </div>
    </div>
</template>

<script setup>
    const props = defineProps(['book']);
</script>

<style lang="scss" scoped></style>