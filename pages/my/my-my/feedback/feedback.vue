<template>

	<view class="content">
		<view style="background-color: #FFFFFF;">
			<textarea class="sr" placeholder="请输入遇到的问题或建议..." autofocus></textarea>
			<view class="clearfix da">
				<view class="tt">
					<uni-icon type="camera" size="70"></uni-icon>
					<h4>添加图片</h4>
				</view>
				<view class="srk">
					<input type="text" class="uni-input" placeholder="添加图片说明">
				</view>

			</view>
		</view>

		<view class="xx">
			<button type="primary">提交</button>
		</view>


	</view>


</template>

<script>
	import uniIcon from "@/components/uni-icon/uni-icon.vue"
	export default {
		components: {
			uniIcon
		},
		data() {
			return {

			}
		}



	}
</script>

<style lang="less" scoped>
	.content {
		/*  #ifdef MP-WEIXIN  */
		height: 100vh;
		/*  #endif  */
		/*  #ifdef H5  */
		height: calc(100vh - 45px);
		/*  #endif  */
		width: 100%;
		background-color: #F3F3F3;
	}
	.da {
		position: relative;
		top: 0;
		left: 0;
		margin-top: 2px;
		background-color: #FFFFFF;
		height: 150px;

		.srk {
			font-size: 20px;
			border: navajowhite;
			padding-left: 14px;
			position: absolute;
			bottom: 10px;
			right: 0;

		}
	}

	.sr {
		width: 100%;
		height: 200px;
		font-size: 18px;
		text-indent: 20px;
		border: none;
		padding: 10PX;
	}

	.tt {
		border: 1px dashed #D9D9D9;
		display: inline-block;
		border: 1px dashed;
		padding: 20px;
		border-radius: 11px;
		margin-left: 22px;
		text-align: center;
		float: left;


	}



	.xx {
		margin-top: 20px;
		padding: 20px 45px 0 45px;
	}

	uni-button[type=primary] {
		background-color: #F7B90E !important;
	}
</style>
