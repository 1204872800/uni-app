<template>
	<view class="content">
		<view class="dp">
			<view style="display: flex;align-items: center;">
				<image style="width:30px;height:30px;margin:20px 10px;" mode="aspectFill" src="/static/Other/els_hot@2x.png"></image>
				<text>Nike旗舰店</text>
			</view>
			<view class="remove">取消关注</view>
		</view>

		<view class="dp">
			<view style="display: flex;align-items: center;">
				<image style="width:30px;height:30px;margin:20px 10px;" mode="aspectFill" src="/static/Other/els_hot@2x.png"></image>
				<text>Nike旗舰店</text>
			</view>
			<view class="remove">取消关注</view>
		</view>


	</view>
</template>

<script>
	import uniRate from "@/components/uni-rate/uni-rate.vue"
	export default {
		props: ['type'],

		components: {
			uniRate
		},

		data() {
			return {

			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="less" scoped>
	.content {
		margin-top: 5px;

		.dp {
			height: 60px;
			background-color: white;
			border-bottom: 1px solid #F8F8F8;
			display: flex;
			justify-content: space-between;
			align-items: center;

			.remove {
				height: 37px;
				width: 95px;
				border: 1px solid #F8BC24;
				color: #F8BC24;
				text-align: center;
				line-height: 37px;
				border-radius: 4px;
				margin-right: 10px;
			}
		}

	}
</style>
