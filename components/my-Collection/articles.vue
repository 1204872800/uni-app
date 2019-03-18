<template>
	<view class="content">
		<view class="card">
			<image style="width:130px;height:130px;margin:20px 10px;" mode="aspectFill" src="/static/Commoditclassification/cla_coat@2x.png"></image>
			<view class="left">
				<text @click="dj">2019夏季短袖型宽这是一件美丽的衣服,限时打折!</text>
		
				<view style="display: flex;align-items: center;margin-top: 60px;justify-content: space-between;">
					<view style="display: flex;align-items: center;">
					<image style="width:30px;height:30px;" mode="aspectFill" src="/static/Other/els_hot@2x.png"></image>	
					  <text style="padding-left: 10px;">Nike旗舰店</text>
					</view>
						<image style="width:30px;height:30px;margin-right:20px;" mode="aspectFill" src="/static/Other/els_like_s@2x.png"></image>
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
