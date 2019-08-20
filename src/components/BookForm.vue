<template>
  <form v-on:submit.prevent="bookSubmit(bookTitle, bookAuthor)" class="" method="POST">
      <input v-model="bookTitle" type="text" name="title" placeholder="Book Title"/>
      <input v-model="bookAuthor" type="text" name="author" placeholder="Book Author"/>
      <button type="submit" name="button">Add Book</button>
  </form>
</template>

<script>
export default {
    name: 'BookForm',
    props: ['books'],
    data() {
        return {
            bookTitle: '',
            bookAuthor: ''
        }
    },
    methods: {
        bookSubmit(bookTitle, bookAuthor) {
            this.$emit('addBook', bookTitle, bookAuthor);
        }
    }
}
</script>

<style>

</style>