<template>
  <div id=app>
    <h1>Add Item Page</h1>
    <form id="fm1">
        <label>Item Name</label>
        <input type="text"/>
        <label>Item Price</label>
        <input type="text"/>
        <label>Item Checkout Code</label>
        <input type="text"/>
        <button type = "button">Add to Cart</button>   
        <button type = "button">Remove from Cart</button>  
    </form>
  </div>
</template>

<script>

export default {
  
  data(){
    return{
        
        msg:"Please Add Item"
        }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app *{
    box-sizing: border-box;
}
#app{
    margin: 30px auto;
    max-width: 500px;
}

p{
    align-content: center;
    color:red;
}
label{
    display: inline-block;
    margin: 20px 0 10px;
    width:50%;
    align-content:left;

}
input[type="text"]{
    display: inline-block;
    padding: 8px;
    width:50%;
}
</style>