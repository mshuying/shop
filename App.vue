<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/*每个页面公共css */
	page{
		margin: 0;
		padding: 0;
		background-color: #f2f3f5;
		color: #333333;
	}
	view{
		box-sizing: border-box;
	}
	.select{
		width: 34rpx;
		height: 34rpx;
		background-color: #f2f3f5;
		border: 1rpx solid #bbb;
		border-radius: 4rpx;
		margin-right: 40rpx;
	}
</style>
