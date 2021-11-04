<template>
<body>
  <div id ="app">
    <div id = "top=bar">
        <h1 class="name">Carvue</h1>
    </div>
    
</body>
 
</template>
<script>
export default {
  name:"App", 
  data(){
    return{
      store: [{
         item: "Vanilla",
         price:5.50 ,
         image:  require("./assets/vanillaaa.jpg"),
        
      },{
        item: "Chocolate", 
        price:5.50,
        image: require("./assets/choclate.jpg")
      }, 
      {
        item: "Cookie N Cream",
        price:6, 
        image: require("")
      },{
        item: "Pistachio", 
        price:6, 
        image: require("./assets/pisstachio.jpg")
      }, {
        item: "Cookie Dough", 
        price:6.50, 
        image: require("./assets/cookiedough.png")
      }, {
      }
      
      ],
    
       
        total:0,
        cart: 0
        
        
       
    }
  }, 
   methods: {
     cartValue(){
       this.cart += 1
    
     },
   
    newTotal(){
      this.total += 5
    }
     
  }}
</script>

<style>
html,
body {
  display: flex;
  justify-content: center;
  font-family: 'Courier New', Courier, monospace;
  box-sizing: border-box;
  padding: 0;
  margin: 0;
  background-color: #0C6E63;
  color: black;
  font-weight: 500;
}
.name {
  background-color: blanchedalmond;
  opacity: 1;
  color: black;
  font-family: 'Courier New', Courier, monospace;
  font-weight: bold;
  font-size: 2.5rem;
  border-radius: 1rem;
  border: solid .2rem #BD8775;
  padding-left: 1rem;
  padding-right: 1rem ;
 
}
.item {
  display: inline ;
}
.items-image{
  display: inline;
  color: white;
  font-family: 'Courier New', Courier, monospace;
  font-weight: 900;
  text-align: center;
}
.actual-image{
  width: 20rem;
  border: solid .2rem #BD8775;
  border-radius: 2rem;
}
.whole-container {
  display: flex;
  align-items: center;
}
.buy{
  border-radius: 2rem ;
  border: solid .2rem black ;
  color: #BD8775;
  font-size: 2rem;
  background-color: white;
  opacity: .7;
}
.buy:hover{
  transform: scale(1.2);
  transition: all .7s;
  cursor: pointer;
}
.cart{
    border-radius: 1rem ;
  border: solid .2rem white ;
  color: #BD8775;
  font-size: 1rem;
  background-color: black;
  opacity: .7;
}
.cart:hover{
   transform: scale(1.2);
  transition: all .7s;
  cursor: pointer;
}
.product-name{
  font: 900;
  font-size: 2.5rem;
  font-family: 'Courier New', Courier, monospace;
}
.price-sub{
  color: yellow;
  font-family: 'Courier New', Courier, monospace;
  font-size: 1.5rem;
  }
  .total-amount{
    color: white;
    text-align: center;
    display: flex;
    flex-direction: row-reverse;
    font-family: 'Courier New', Courier, monospace;
    font-size: 1.5rem;
  }
</style>