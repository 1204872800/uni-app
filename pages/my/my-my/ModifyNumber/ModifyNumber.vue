<template>
	<view class="content">


		<view style="padding: 90px 25px 0 25px;">
			<input class="input" type="number" focus placeholder="请输入手机号码" />
		</view>

		<view style="margin: 50px 25px 0 25px;position: relative;left: 0;top: 0;">
			<input class="input" maxlength="6" type="number" placeholder="请输入验证码" />
			<button class="mini-btn" type="default" size="mini">发送验证码</button>
		</view>


	</view>
</template>

<script>
	export default {
		data() {
			return {

			};
		}
	}
</script>

<style lang="less" scoped>
	.content {
		/*  #ifdef MP-WEIXIN  */
		height: 100vh;
		/*  #endif  */
		/*  #ifdef H5  */
		height: calc(100vh - 90px);
		/*  #endif  */
		width: 100%;
		background-color: #FFFFFF;

		.input {

			background-color: #EBEBEB;
			height: 55px;
			font-size: 24px;
			padding-left: 5px;
		}

		.mini-btn {
			position: absolute;
			right: 21px;
			top: 15px;
			z-index: 999;
			background-color: #F5B70C;
			color: white;
		}

	}
</style>
