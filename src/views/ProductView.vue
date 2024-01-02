<script setup>

</script>

<template>
 <section class="products">
				<div class="container">

					<div class="products-wrapper" id="goods-container">
						<div class="products-card" v-for="good in goodsArray" :key="good.id" :to="`/good?id=${good.id}`">
							<div class="products-card__image">
								<img :src="getUrl(good.image)"  alt="Eel_roll_standard">
							</div>
							<div class="products-card_description">
								<div class="products-card_description-row">
									<h5 class="products-card_description-name">{{ good.title }}</h5>
								</div>
								<div class="products-card_description-row">
									<p class="products-card_description-text">{{ good.ingredients }}</p>
								</div>
								<div class="products-card_description-row">
									<div class="products-card_description-controls">
										<button class="btn btn-primary">
											В корзину
											<img src="../assets/img/icon/shopping-cart-white.svg" alt="cart-white" />
										</button>
										<span class="products-card_description-controls--price">{{ good.price }} ₽</span>
									</div>
								</div>
							</div>
						</div>
						
					</div>
				</div>
				<!-- /.container  -->
			</section>
</template>
<script setup>
import { goodsArray } from '../constants/goods'
const getUrl = (name) => {
  return new URL(`../assets/img/goods/${name}`, import.meta.url)
//   return `../assets/img/rests/pizza-plus.jpg`
}



</script>