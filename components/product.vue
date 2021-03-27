<template>
	<!-- 商品信息 -->
	<view class="product">
		<!-- 商品图片 -->
		<image src="../static/logo.png" mode=""></image>
			<!-- 商品内容信息 -->
		<view class="product-content">
			<view class="content-title">
				产品名称产品名称产品名称产品名称
			</view>
			<view class="content">
				<span class="price">$888.88</span>
				<span class="number">已售12件</span>
				<span class="purchase">立即加购</span>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		name:"product",
		data() {
			return {
				
			};
		}
	}
</script>

<style lang="less">
	.product{
		margin-top: 10rpx;
		width: 100%;
		height: 550rpx;
		background-color: #FFFFFF;
		padding: 20rpx 30rpx;
		image{
			width: 100%;
			height: 400rpx;
			border-radius: 20rpx;
			background-color: #F0AD4E;
		}
		.content-title{
			font-size: 28rpx;
			font-weight: 700;
			color: #333333;
		}
		.content{
			width: 100%;
			height: 60rpx;
			display: flex;
			align-items: center;
			.price{
				flex: 2;
				color: #e53131;
				font-size: 24rpx;
			}
			.number{
				flex: 8;
				color: #adadad;
				font-size: 24rpx;
			}
			.purchase{
				text-align: center;
				width: 140rpx;
				height: 48rpx;
				line-height: 48rpx;
				background-color: #ffc868;
				border-radius: 20rpx 0rpx 20rpx 20rpx;
				font-size: 22rpx;
				color: #333333;
			}
		}
		
	}
</style>
