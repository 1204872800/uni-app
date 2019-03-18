<template>
	<view class="content">
		<view class="card">
			<image style="width:130px;height:130px;margin:20px 10px;" mode="aspectFill" src="/static/Commoditclassification/cla_coat@2x.png"></image>
			<view class="left">
				<text @click="dj">2019夏季短袖型宽这是一件美丽的衣服,限时打折!</text>
				<view style="margin-top: 40px;">
					<text style="color: red;">￥79.9</text>
					<text style="color: #7D7E80;text-decoration:line-through;">￥222</text>
				</view>
				<view style="display: flex;align-items: center;">
					<text style="color: red;">
						<uni-rate disabled="true" size="20" max="3" value="3"></uni-rate>
					</text>
					<text style="color: #7D7E80;font-size: 16px;">
						2101人收藏
					</text>
						<image style="width:30px;height:30px;margin-left:40px;" mode="aspectFill" src="/static/Other/els_like_s@2x.png"></image>
				</view>
			</view>
		</view>
	
		<view class="card">
		<image style="width:130px;height:130px;margin:20px 10px;" mode="aspectFill" src="/static/Commoditclassification/cla_dress@2x.png"></image>
		<view class="left">
			<text @click="dj">2019夏季短袖型宽这是一件美丽的衣服,限时打折!</text>
			<view style="margin-top: 40px;">
				<text style="color: red;">￥79.9</text>
				<text style="color: #7D7E80;text-decoration:line-through;">￥222</text>
			</view>
			<view style="display: flex;align-items: center;">
				<text style="color: red;">
					<uni-rate disabled="true" size="20" max="3" value="3"></uni-rate>
				</text>
				<text style="color: #7D7E80;font-size: 16px;">
					2101人收藏
				</text>
					<image style="width:30px;height:30px;margin-left:40px;" mode="aspectFill" src="/static/Other/els_like_s@2x.png"></image>
			</view>
		</view>
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
			dj() {
				console.log(12313)
			}
		}
	}
</script>

<style lang="less" scoped>
	.content {
		margin-top: 5px;

		.card {
			height: 180px;
			background-color: white;
			display: flex;
			border-bottom: 1px solid #F4F4F4;
		}

		.left {
			flex: 1;
			display: flex;
			flex-direction: column;
			margin: 14px 0;
		}
	}
</style>
