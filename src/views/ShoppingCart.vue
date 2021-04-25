<template>
<div class="shopping">
  <headerShayna />

<!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section">
        <div class="container">
            <div class="row">
                <div class="col-lg-12 text-left">
                    <div class="breadcrumb-text product-more">

                        <router-link to="/" ><i class="fa fa-home"></i> Home</router-link>
                        <a href="./shop.html">Shop</a>
                        <span>Shopping Cart</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Shopping Cart Section Begin -->
    <section class="shopping-cart spad">
        <div class="container">
            <div class="row">
                <div class="col-lg-8">
                    <div class="cart-table">
                        <table>
                            <thead>
                                <tr>
                                    <th>Image</th>
                                    <th class="p-name">Product Name</th>
                                    <th>Price</th>
                                    <th>Action</th>
                                    
                                    <!-- <th><i class="ti-close"></i></th> -->
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td class="cart-pic first-row"><img src="img/cart-page/product-1.jpg" alt=""></td>
                                    <td class="cart-title first-row">
                                        <h5>Pure Pineapple</h5>
                                    </td>
                                    <td class="p-price first-row">$60.00</td>
                                    
                                    <td class="close-td first-row"><i class="ti-close"></i></td>
                                </tr>
                                <tr>
                                    <td class="cart-pic first-row"><img src="img/cart-page/product-1.jpg" alt=""></td>
                                    <td class="cart-title first-row">
                                        <h5>Pure Pineapple</h5>
                                    </td>
                                    <td class="p-price first-row">$60.00</td>
                                  
                                    <td class="close-td first-row"><i class="ti-close"></i></td>
                                </tr>
                              
                            </tbody>
                        </table>
                       
                       
                    
                    </div>
                       
                </div>
                <div class="col-lg-4">

                 <div class="row">
                <div class="col-lg-12">
                    
                    <div class="proceed-checkout text-left">
                        
                                <ul>
                                    <li class="subtotal">id transaksi <span>$240.00</span></li>
                                    <li class="subtotal mt-3">Subtotal <span>$240.00</span></li>
                                    <li class="subtotal mt-3">pajak <span>$240.00</span></li>
                                    <li class="subtotal mt-3">total biaya <span>$240.00</span></li>
                                    <li class="subtotal mt-3">Bank Transfer <span>$240.00</span></li>
                                    <li class="subtotal mt-3">No rekening <span>$240.00</span></li>
                                    <li class="subtotal mt-3">Nama penerima <span>shayna</span></li>

                                    <!-- <li class="cart-total">Total <span>$240.00</span></li> -->
                                </ul>
                               <router-link to="/success" ><a href="#" class="proceed-btn">PROCEED TO CHECK OUT</a> </router-link>
                            </div>
                    
                    </div>

                    </div>
                    </div>
                
            </div>
            <div class="col-lg-6">
                <h4 class="mb-4 text-left"> Informasi Pembeli:</h4>
                <div class="user-checkout text-left">
                    <form >
                        <div class="form-group tex">
                            <label for="namaLengkap"> Nama Lengkap</label>
                            <input type="text" class="form-control" id="namaLengkap"
                            placeholder="masukan nama"
                            />
                        </div>
                         <div class="form-group">
                            <label for="emailAddress"> Email Address</label>
                            <input type="email" class="form-control" id="emailAddress"
                            placeholder="masukan nama"
                            />
                        </div>
                        <div class="form-group">
                            <label for="noHp"> No. Hp</label>
                            <input type="email" class="form-control" id="noHp"
                            placeholder="masukan nama"
                            />
                        </div>
                        <div class="form-group">
                            <label for="noHp"> Alamat Lengkap</label>
                            <textarea type="email" class="form-control" id="noHp"
                            placeholder="masukan nama"
                            > </textarea>
                        </div>
                    </form>
                </div>
                
            </div>
        </div>
    </section>
    <!-- Shopping Cart Section End -->
</div>
  
</template>

<script>
import HeaderShayna from '../components/HeaderShayna.vue'
export default {
name: "cart",
components:{
    HeaderShayna
}
}
</script>


<style>

</style>