<template>
    <div>
        <table class="table">
            <thead>
                <tr>
                    <th scope="col">Author</th>
                    <th scope="col">Title</th>
                    <th scope="col">Description</th>
                    <th scope="col">Image</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="book in books" :key="book.author">
                    <td>{{ book.author }}</td>
                    <td>{{ book.title }}</td>
                    <td>{{ book.description }}</td>
                    <td><img :src="book.img_url" alt=""></td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script setup>
    import books from '@/bookdata';
</script>

<style scoped>
th {
    font-weight: bold;
}

img {
    width: 100px;
}
</style>