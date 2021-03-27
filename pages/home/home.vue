<template>
	<view class="shop-home">
		<view class="header">
			<view class="search">
				请输入商品名称
			</view>
		</view>
		<view class="fill"></view>
		<view class="shop-content">
			<product v-for="(i,index) in 10" :key="index "></product>
		</view>
	</view>
</template>

<script>
import product from '../../components/product.vue';
export default {
	data() {
		return {};
	},
	components: {
		product
	},
	methods: {},
	onPullDownRefresh() {
		console.log(123);
	}
};
</script>

<style lang="less">
.shop-home {
	width: 100%;
	letter-spacing: 1rpx;
	.header {
		position: fixed;
		min-width: 750rpx;
		height: 80rpx;
		padding: 10rpx 30rpx;
		background-color: #f2f3f5;
		.search {
			width: 100%;
			height: 100%;
			background-color: #ffffff;
			border-radius: 50rpx;
			padding: 16rpx 30rpx;
			font-size: 24rpx;
			color: #999999;
		}
	}
	.fill{
		height: 70rpx;
	}
}
</style>
