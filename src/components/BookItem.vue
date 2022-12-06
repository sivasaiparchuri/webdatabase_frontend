<template>

    <div>
        <h1 id="meal"> {{book.mealname}}</h1>
        <h2 id="breakfast"> {{book.type}}</h2>
        <h2> Protein : {{book.protein}} gm</h2>
        <h2> Carbohydrates : {{book.carbs}} gm</h2>
        <h2> Totalkcal : {{book.totalkcal}} Kcal</h2>
        
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

h2{
    text-align: center;
}

h1{
    text-align: center;
}
#meal{
  background-color: rgb(238, 193, 96);
  color: black;
    padding: 1em;
    text-align: center; 

}
#breakfast{
  background-color: rgb(96, 174, 238);
  color: black;
    padding: 1em;
    text-align: center; 

}
#body{
  background-color: #e6ff00;
}
div{
    background-color: #a1ff9e;
    color: black;
    padding: 1em;
}

.red{
background-color: orangered !important;

}
.green{
    color: white;
}


</style>
