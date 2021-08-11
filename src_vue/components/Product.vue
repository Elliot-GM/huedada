<template>
    <div class="product">
        <div class="product-inner">
            <div class="product-detail">
                <h2>{{ product.title }}</h2>
            </div>
            <div class="product-image-wrap">
                <img :src="product.src" class="image" />
            </div>
            <div class="product-detail">
                <p>arfgqgzngjoiriabia</p>
            </div>
            <div class="product-text-wrap">
                <button type="button" class="bouton-r">réserver</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'product',
    props: ['product']
}
</script>

<style>
.product {
    flex: 1 1 33.333%;
    width: 100%;
    padding: 10px;
    overflow: hidden;
}

.product-inner {
    position: relative;
    padding: 25px;
    box-shadow: 0px 0px 32px rgba(0, 0, 0, 0.25);
}

.product-image-wrap .image {
    width: 100%;
    height: 300px;
}

.bouton-r {
    border-radius: 5px 5px 5px 5px;
    padding: 10px;
}

</style>