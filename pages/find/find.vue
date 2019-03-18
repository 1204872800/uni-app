<template>
	<view class="content">
		<view class="header">
			<view class="top">小工具</view>
			<view style="display: flex;margin: 20px 50px 0 50px;">
				<view class="feng">海关运费查询</view>
				<view class="feng">海关编码查询</view>
			</view>
			<view class="bottom">干货分享</view>
		</view>


		<view style="margin-top: 10px;">
			<uni-card title="Nike旗舰店" thumbnail="http://img-cdn-qiniu.dcloud.net.cn/new-page/uni.png" extra="2013-1-3发布" note="1235人阅读">
				<image class="img" mode="scaleToFill" src="../../static/Commoditclassification/cla_banner@3x.png"></image>
			</uni-card>
			<uni-card title="Nike旗舰店" thumbnail="http://img-cdn-qiniu.dcloud.net.cn/new-page/uni.png" extra="2013-1-3发布" note="1235人阅读">
				<image class="img" mode="scaleToFill" src="../../static/Commoditclassification/cla_banner@3x.png"></image>
			</uni-card>

		</view>





		<find></find>
	</view>
</template>

<script>
	import find from '../../components/my-Collection/find.vue'
	import uniCard from '../../components/uni-card/uni-card.vue'
	import api from '../../js/api.js'
	export default {
		components: {
			find,
			uniCard
		},
		data() {
			return {

			};
		},
		onLoad() {

		}
	}
</script>

<style lang="less" scoped>
	.content {
		width: 100%;
		background-color: #F3F3F3;

		.header {
			height: 170px;
			background-color: #FC4B65;

			.top {
				color: white;
				padding-top: 25px;
				padding-left: 20px;
			}

			.feng {
				flex: 1;
				text-align: center;
				color: #FC4B65;
				height: 30px;
				line-height: 30px;
				border-radius: 20px;
				background-color: white;
				margin: 0 10px;
				font-size: 16px;
			}

			.bottom {
				color: white;
				padding-top: 20px;
				padding-left: 20px;

			}
		}

		.uni-card {
			
			margin: 0 !important;
			border-bottom: 1px solid #F8F8F8;

			.uni-card__header:after {
				background-color: #F8F8F8;
			}

			.uni-card__header {
				background-color: #F8F8F8;
			}

			.uni-card__header-extra-text {
				color: #B7B7B7;
			}

			.img {
				height: 160px;
				/*  #ifdef MP-WEIXIN  */
				width: 335px;
				/*  #endif  */
				/*  #ifdef H5  */
				width: 360px;
				/*  #endif  */

			}
		}

		.uni-card:after {
			border: none;
		}

	}
		.uni-card {
		
		margin: 0 !important;
		border-bottom: 1px solid #F8F8F8;
		
		}
</style>
