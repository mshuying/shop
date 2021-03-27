<template>
	<view>
		<product></product>
		<product></product>
		<product></product>
		<product></product>
	</view>
</template>

<script>
	import product from '../../components/product.vue';
	export default {
		data() {
			return {
				editorCtx:""
			}
		},
		components:{
			product
		},
		onLoad() {

		},
		onPullDownRefresh() {
			console.log(1111)
		},
		methods: {

		}
	}
</script>

<style>
</style>
