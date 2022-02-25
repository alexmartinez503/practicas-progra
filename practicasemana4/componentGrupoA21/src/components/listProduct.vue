<template>
    <div id="container">
         <a href="#" class="btn btn-primary"  data-bs-toggle="modal" data-bs-target="#exampleModal">Shopping cart</a>
    <div class="row">
  <div class="col-sm-6" v-for="(item, index) in items" v-bind:key="index">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">{{item.productName}}</h5>
        <p class="card-text">{{item.description}}</p>
        <input type="number" v-model="item.quantity">
        <a href="#" class="btn btn-primary" @click="add(index)" >add card</a>
      </div>
    </div>
  </div>
  
    </div>

    <card-items cartProducts="cartProducts"/>
    </div>
</template>



<script>
import cardItems from '../components/cartimes.vue'
import products from'../data/products.json'
export default {
name: 'ListProducts',
components: {
    cardItems
},

data(){
    return{
        items: products
    }
},
methods:{
    add:function(index){
        this,cardItems.push({
            productName:this.cardItems[index].productName,
            description:this.cardItems[index].description,
            quantity:this.cardItems[index].quantity,
            price: this.cardItems[index].price


        })
    }
}
}
</script>