<template>
<div>
    <h1>{{title}}</h1>
    <ul>
        <li>Book 1</li>
        <li>Book 2</li>
        <li>Book 3</li>
    </ul>
</div>    
</template>

<script>
export default {
    name: 'Booklist',
    data() {
        return {
            title: 'All Books'
        }
    }
}
</script>

<style>
h1, h2 {
    font-weight: normal;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: block;
    margin: 0 10px;
}
</style>