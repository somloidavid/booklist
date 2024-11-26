<template>
    <div class="container">
        <div class="row row-cols-1 row-cols-md-3 g-4">
            <div class="col" v-for="book in books" :key="book.title">
                <CardComponent :book="book"></CardComponent>
            </div>
        </div>
    </div>
</template>

<script setup>
import books from '@/bookdata';
import CardComponent from './Card.component.vue';


</script>

<style lang="scss" scoped>

</style>