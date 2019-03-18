<template>
	<view class="content">

		<image class="img" style="width:50px;height:50px;" mode="aspectFill" src="/static/tabar/tab_find@2x.png" @click="dj"></image>

	</view>
</template>

<script>
	export default {

		components: {

		},

		data() {
			return {

			}
		},
		onLoad() {

		},
		methods: {
			dj() {
				uni.switchTab({
					url: '/pages/find/find'
				});
			}
		}
	}
</script>

<style lang="less" scoped>
	.img {
		position: fixed;
		left: 45%;
		z-index: 999;
			/*  #ifdef MP-WEIXIN  */
			bottom:-100px;
			
		/*  #endif  */
		/*  #ifdef H5  */
			bottom: 20px;
		/*  #endif  */
	}
</style>
