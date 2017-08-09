<template id="products_layout">
<div class="products">
  <div class="products-public">
    产品共用模版
  </div>

  <div class="products-content">
    <nuxt/>
  </div>

</div>
</template>

<style>
.products {
  display: flex;
}

.products-public {
  width: 200px;
}

.products-content {
  flex: 1;
}
</style>
