<template>
	<view class="goods">
		<view class="select"></view>
		<view class="image">
			<image src="../static/logo.png" mode=""></image>
		</view>
		<view class="content">
			<view class="name">
				产品名称产品名称
			</view>
			<!-- 规格 -->
			<view class="spec">
				规格：8GB+128GB
			</view>
			<view class="price-num">
				<view class="price">
					$88.88
				</view>
				<view class="num">
					<text class="but" @click="subtract">-</text>
					<text class="total">{{current}}</text>
					<text class="but" @click="add">+</text>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		name:"cartProduct",
		data() {
			return {
				current:1
			};
		},
		methods:{
			subtract(){
				if(this.current===1){
					console.log(123);
					return 
				}
				this.current--;
			},
			add(){
				this.current++
			}
		}
	}
</script>

<style lang="less">
.goods{
	display: flex;
	align-items: center;
	width: 100%;
	height: 180rpx;
	background-color: #FFFFFF;
	padding: 20rpx;
	.image{
		width: 208rpx;
		height: 140rpx;
		margin-right: 20rpx;
		image{
			width: 100%;
			height: 100%;
		}
	}
	.content{
		flex: 1;
		height: 100%;
		.name{
			font-size: 28rpx;
		}
		.spec{
			font-size: 22rpx;
			color: #a0a0a0;
			margin-top: 10rpx;
		}
		.price-num{
			position: relative;
			margin-top: 20rpx;
			display: flex;
			align-items: center;
			.price{
				font-size: 22rpx;
				color: #e53131;
			}
			.num{
				position: absolute;
				right: 0px;
				font-size: 24rpx;
				color: #666;
				text{
					display: inline-block;
				}
				.but{
					width: 48rpx;
					height: 48rpx;
					border-radius: 50%;
					text-align: center;
					line-height: 48rpx;
					background-color: #f2f3f5;
				}
				.total{
					margin: 0 18rpx;
				}
			}
			
		}
	}
}
</style>
