<template>
    <form v-on:submit.prevent="bookSubmit()" class="" action="#" method="post" >
        <input v-model="bookTitle" type="text" name="title" value="" placeholder="Book Title">
        <input v-model="bookAuthor" type="text" name="author" value="" placeholder="Book Author">
        <button type="submit" name="button"  >Add Book</button>
    </form>
</template>

<script>
export default {
    name: 'BookForm',
    props: ['books'],
    data() {
        return {
            bookTitle: "",
            bookAuthor: ""
        }
    },
    methods: {
        bookSubmit: function(){
            console.log($bookTitle)
        }
    },
}
</script>

<style scoped>
li{
    display: block;
    margin: 0 10px;
}
</style>