<template>

    <div :class="book.published ? 'green': 'red' ">
        <h2> {{book.name}}</h2>
        <h4> {{book.year}}</h4>
        <h4> {{book.country}}</h4>
        <h4> {{book.noofusers}}</h4>
        <h4> {{book.revenue}}</h4>


    </div>

</template>

<script>


export default{
    name: 'BookItem',
    props:{
        book: Array
    }
}


</script>

<style scoped>


h4{
    margin: 2px;
}

div{
    background-color: #ec815a;
    color: black;
    padding: 1em;
}

.red{
background-color: rgb(26, 232, 19) !important;

}
.green{
    color: white;
}


</style>