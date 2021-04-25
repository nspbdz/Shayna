<template>
  <div class="product">
   <HeaderShayna />

 <!-- Breadcrumb Section Begin -->
    <div class="breacrumb-section text-left">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="breadcrumb-text product-more">
                       <router-link to="/"><i class="fa fa-home"></i> Home</router-link >
                        <a href="./shop.html">Shop</a>
                        <span>Detail</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Breadcrumb Section Begin -->

    <!-- Product Shop Section Begin -->
    <section class="product-shop spad page-details">
        <div class="container">
            <div class="row">
               
                <div class="col-lg-12">
                    <div class="row">
                        <div class="col-lg-6">
                            <div class="product-pic-zoom">
                                <img class="product-big-img" :src="gambar_default" alt="">
                                <div class="zoom-icon">
                                    <i class="fa fa-search-plus"></i>
                                </div>
                            </div>
                            <div class="product-thumbs">
                                <carousel class="product-thumbs-track ps-slider"  :dots="false" :items="3" :nav="false" >
                                    <div class="pt" @click="changeImage(thumbs[0])" :class="thumbs[0] == gambar_default ? 'active' : '' "><img
                                            src="img/mickey4.jpg" alt=""></div>
                                    <div class="pt" @click="changeImage(thumbs[1])" :class="thumbs[1] == gambar_default ? 'active' : '' "><img
                                            src="img/mickey2.jpg" alt=""></div>
                                    <div class="pt" @click="changeImage(thumbs[2])" :class="thumbs[2] == gambar_default ? 'active' : '' "><img
                                            src="img/mickey3.jpg" alt=""></div>
                                    <div class="pt" @click="changeImage(thumbs[3])" :class="thumbs[3] == gambar_default ? 'active' : '' "><img
                                            src="img/mickey1.jpg" alt=""></div>
                                </carousel>
                            </div>
                        </div>
                        <div class="col-lg-6">
                            <div class="product-details text-left">
                                <div class="pd-title">
                                    <span>oranges</span>
                                    <h3>Pure Pineapple</h3>
                                    <a href="#" class="heart-icon"><i class="icon_heart_alt"></i></a>
                                </div>
                                <div class="pd-rating">
                                    <i class="fa fa-star"></i>
                                    <i class="fa fa-star"></i>
                                    <i class="fa fa-star"></i>
                                    <i class="fa fa-star"></i>
                                    <i class="fa fa-star-o"></i>
                                    <span>(5)</span>
                                </div>
                                <div class="pd-desc">
                                    <p>Lorem ipsum dolor sit amet, consectetur ing elit, sed do eiusmod tempor sum dolor
                                        sit amet, consectetur adipisicing elit, sed do mod tempor</p>
                                    <h4>$495.00 <span>629.99</span></h4>
                                </div>
                              
                               
                                <div class="quantity">
                                    
                                    <router-link to="cart"> <a href="#" class="primary-btn pd-cart">Add To Cart</a></router-link>
                                </div>
                               
                              
                            </div>
                        </div>
                    </div>
                   
                </div>
            </div>
        </div>
    </section>
    <!-- Product Shop Section End -->

   <RelatedShayna />
   <FooterShayna />
   
   
  
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderShayna from '../components/HeaderShayna.vue';
import FooterShayna from '../components/FooterShayna.vue';
import carousel from 'vue-owl-carousel';
import RelatedShayna from '../components/RelatedShayna.vue';





export default {
  name: 'product',
  components: {
    HeaderShayna,
    FooterShayna,
        carousel ,
        RelatedShayna
  },
  data() {
      return {
  gambar_default:"img/mickey1.jpg",
  thumbs:[
      "img/mickey1.jpg",
      "img/mickey2.jpg",
      "img/mickey3.jpg",
      "img/mickey4.jpg"
  ]

      }

  },
  methods:{
      changeImage(urlImage) {
          this.gambar_default =urlImage;
      }
  }
  
}
</script>
<style  scoped>
.pt{
    margin-right :14px;
}
</style>
