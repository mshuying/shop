<template>
	<view>
		<!-- 购物车商品数量 -->
		<view class="goods-number">
			<text class="icon"></text>
			<text>{{ '共' + total + '件商品' }}</text>
			<van-icon name="delete" class="delete" />
		</view>
		<!-- 购物车商品 -->
		<view class="cart-goods" v-for="(i,index) in 10" :key="index">
			<!-- 店家 -->
			<view class="goods-store">
				<storwname></storwname>
			</view>
			<!-- 商品内容信息 -->
			<view class="goods-content" v-for="(i,inde) in 4" :key="inde">
				<cartproduct></cartproduct>
			</view>
		</view>
	</view>
</template>

<script>
	import storwname from "../../components/storeName.vue"
	import cartproduct from "../../components/cartProduct.vue"
export default {
	data() {
		return {
			total: 4
		};
	},
	components:{
		storwname,cartproduct
	}
};
</script>

<style lang="less">
.goods-number {
	display: flex;
	align-items: center;
	width: 100%;
	height: 65rpx;
	font-size: 22rpx;
	color: #333333;
	background-color: #f2f3f5;
	position: relative;
	.icon {
		width: 10rpx;
		height: 28rpx;
		background-color: #4ca0ff;
		border-radius: 10rpx;
		margin-left: 30rpx;
		margin-right: 15rpx;
	}
	.delete {
		font-size: 28rpx;
		color: #666666;
		position: absolute;
		top: 17rpx;
		right: 30rpx;
	}
}
.cart-goods {
	margin-bottom: 20rpx;
}
</style>
