<script>
import products from '../products.js';
import AppProduct from './AppProduct.vue';
export default {

    name: 'AppProducts',

    data() {
        return {
            products //Objects Array
        }
    },
    components: {
        AppProduct
    }

}
</script>

<template>
    <section class="products_bg">
        <h5 class="section_title">CURRENT SERIES</h5>
        <div class="container d-flex">
            <div class="d-flex flex-wrap">
                <AppProduct v-for="product in products" 
                :img="product.thumb" 
                :price="product.price" 
                :series="product.series"
                :category="product.type" />
            </div>
        </div>
    </section>
</template>


<style lang="scss" scoped></style>