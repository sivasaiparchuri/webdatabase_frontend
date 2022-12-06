<template>
    <div class="bookbox">


        

        <div v-for="book in books" :key="book.id" >
            <BookItem :book="book"/>
        </div>

    </div>
    


</template>

<script>

    import BookItem from "@/components/BookItem.vue";


    export default{
        name: 'BookBox',
        components: {
            BookItem
        },
        props:{
            
            books: Array
        }
    }

</script>

<style scoped>

.bookbox{

background-color: rgb(196, 231, 255);
padding: 1em;
color: gray;
}

</style>