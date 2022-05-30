<template>
    <div class="grid md:grid-cols-3 text-gray-500 font-body body">
    <Navbar></Navbar>


        <!--content wrapper I-->
      <ProductSummaryCard ></ProductSummaryCard>

       
    </div>
        <Footer1></Footer1>

</template>

<style scoped>
.body{
    margin-top: -370px;
    width:100%;
    height:100%;
}

.nav{
    width:300px;
}
.navbarall{
    width:100%;
}
</style>



<script>
import Navbar from '../components/Navbar.vue'
import Footer1 from '../components/Footer.vue'
import ProductSummaryCard from '../components/products/ProductSummaryCard.vue'


export default {
  name: 'ProductView',
  components: { Navbar, Footer1, ProductSummaryCard },
  
//   data(){
//       return{
//          myJson: json,

//          addToCart: JSON.parse(localStorage.getItem("addToCart")) || {},
//          control: {
//             tab: "all"
//         },
//         json
//       };
//   },
//   methods:{
//     alert(msg){
//         window.alert(msg);
//     },
//     toggle_cart: function(uid){
//         this.addToCart[uid] = !this.addToCart[uid];
//         localStorage.setItem("addToCart", JSON.stringify(this.addToCart));
//         console.log(this.addToCart);
//     }
//   },
//   computed:{
//       myJson: function(){
//           let vm = this;
//           if(vm.control.tab === "all"){
//               return vm.json;
//           } else if (vm.control.tab === "cart"){
//                return vm.json.filter((item)=> vm.addToCart[item.uid]);
//           }
//       },
//       total: function () {}
//   }             

//   mounted(){
//       fetch('/products.json')
//       .then(function(response) {
//     return response.json();
//   })
//   .then(function(myJson) {
//     console.log(myJson);
//   });
      
//   }
    
}



</script>