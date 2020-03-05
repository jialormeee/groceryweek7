<template>
  <div class="headerStyle">
        <nav>
          <h1>{{ title }}</h1>
          <ul>
             <li><router-link to="/" exact>List</router-link></li>
             <li><router-link to="/add" exact>Add Item</router-link></li>
          </ul>
        </nav>
  </div>
</template>

<script>
export default {
  
  data(){
    return{
        msg: 'Grocery List'
        }
  },
  props:{
    title:{
      type:String
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header{
    background:rgb(92, 252, 0);
    padding:6px;
    border-style: solid;
    border-color:black;
    border-width: 2px;
}
h1{
    color:ivory;
    background: rgb(128, 151, 160);
    font-size: 30px;
}
nav{
    background: rgb(128, 151, 160);
    padding: 14px 0;
    margin-bottom: 40px;
}
.router-link-active{
    background: rgb(236, 105, 18);
    color: #444;
}
ul{
    list-style-type: none;
    text-align: left;
    margin: 0;
}
li{
    
    display: inline-block;
    margin: 0 10px;
}
li a{
  
  font-size: 18px;
  color:ivory;
    
}
</style>