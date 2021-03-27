<template>
	<view class="store">
		<view class="select">
		</view>
		<view class="store-icon">
			<van-icon name="shop" />
		</view>
		<view class="store-name">
			华为品牌旗舰店
		</view>
	</view>
</template>

<script>
	export default {
		name:"storeName",
		data() {
			return {
				
			};
		},
		methods:{
			
		}
	}
</script>

<style lang="less">
.store{
	width: 100%;
	height: 64rpx;
	padding: 15rpx 20rpx;
	background-color: #FFFFFF;
	margin-bottom: 2rpx;
	display: flex;
	.store-icon{
		font-size: 30rpx;
		color: #4ca0ff;
		margin-right: 10rpx;
	}
	.store-name{
		font-size: 22rpx;
		color: #333;
	}
}
</style>
