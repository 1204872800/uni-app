<template>

	<view class="home">
		<view class="shang">
			<view style="display:flex">
				<view class="z">我的</view>
				<view class="y">
					<!--修改号码-->
					<navigator url="/pages/my/my-my/ModifyNumber/ModifyNumber" style="display: inline-block;padding-right: 8px;">
						<image style="width: 23px;height: 25px;" mode="scaleToFill" src="../../static/my/me_inform@2x.png"></image>
					</navigator>
					<!--个人设置-->
					<navigator url="/pages/my/my-my/SetUp/SetUp" style="display: inline-block;">
						<image style="width: 23px;height: 25px;" mode="scaleToFill" src="../../static/my/me_set@2x.png"></image>
					</navigator>
				</view>
			</view>
			<view class="tx clearfix">
				<!--    <img src="" alt="" style="float: left"> -->
				<image style="width: 100px;height:100px;margin-left: 10px;" mode="aspectFill" src="../../static/tou.png"></image>
				<view class="name">
					<view>
						<text style="color:white;font-size: 20px;">飞鸟和鱼</text><text class="sj">LV3</text>
					</view>
					<view style="color:white;font-size: 20px;">1578239182</view>
				</view>
			</view>
			<view class="yh">
				<view class="zt">
					<navigator url="/pages/my/my-my/Collection/Collection">
						<h3 class="h3">收藏</h3>
						<h3 class="h3">12</h3>
					</navigator>
				</view>
				<text class="xian"></text>
				<view class="yt">
					<navigator url="/pages/my/my-my/SetUp/SetUp">
						<h3 class="h3">优惠券</h3>
						<h3 class="h3">11张</h3>
					</navigator>
				</view>
			</view>
		</view>
		<view class="zhong">
			<view class="zd">
				<text class="zd1" style="color:#313131">我的订单</text>
				<text class="zd2" style="color:#B4B4B4;display: flex;align-items:center;">
					查看全部订单<uni-icon type="arrowright" size="30"></uni-icon></text>
			</view>

			<view style="display: flex;height: 67px; padding-top: 13px;">
				<view class="li">
					<image style="width: 36px;height: 36px;" 
					mode="scaleToFill" src="../../static/my/me_pay@2x.png"></image>
					<h3 class="h3">待支付</h3>
				</view>
				<view class="li">
				<image style="width: 36px;height: 36px;" mode="scaleToFill" src="../../static/my/me_shipments@2x.png"></image>
					<h3 class="h3">待发货</h3>
				</view>
				<view class="li">
					<image style="width: 36px;height: 36px;" mode="scaleToFill" src="../../static/my/me_takedelivery@2x.png"></image>
					<h3 class="h3">待收货</h3>
				</view>
				<view class="li">
					<image style="width: 36px;height: 36px;" mode="scaleToFill" src="../../static/my/me_evaluate@2x.png"></image>
					<h3 class="h3">评价</h3>
				</view>
				<view class="li">
					<image style="width: 36px;height: 36px;" mode="scaleToFill" src="../../static/my/me_exchange@2x.png"></image>
					<h3 class="h3">待支付</h3>
				</view>
			</view>
		</view>

		<view class="xia">
			<navigator url="/pages/my/my-my/Address/Address" class="zd">
				<text class="zd1" style="color:#313131">收货地址管理</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
			<!-- 意见反馈 -->
			<navigator url="/pages/my/my-my/feedback/feedback" class="zd">
				<text class="zd1" style="color:#313131">意见反馈</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
			<navigator url="/pages/my/my-my/AboutUs/AboutUs" class="zd">
				<text class="zd1" style="color:#313131">关于我们</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
		</view>



<find></find>
	</view>
</template>

<script>
	import uniIcon from "@/components/uni-icon/uni-icon.vue"
 import find from '../../components/my-Collection/find.vue'
	export default {
		components: {
			uniIcon,
			find
		},
		data() {
			return {

			}
		}
	}
</script>

<style lang="less" scoped>
	
	@import '../../static/Share.css';


	.home {
		/*  #ifdef MP-WEIXIN  */
		height: 100vh;
		/*  #endif  */
		/*  #ifdef H5  */
		height: calc(100vh - 95px);
		/*  #endif  */
		width: 100%;
		background-color: #F3F3F3;

		.shang {

			/*  #ifdef MP-WEIXIN  */
			height: 220px;
			/*  #endif  */
			/*  #ifdef H5  */
			height: 250px;
			/*  #endif  */
			background-color: #FC4B65;
			padding-top: 27px;

			.z {
				flex: 1.2;
				text-align: right;
				color: white;
				font-size: 22px;
			}

			.y {
				flex: 1;
				text-align: right;
				padding-right: 10px;

				.colorIcons {
					color: white;
				}
			}

			.tx {
				display: flex;

				.name {
					float: left;
					padding-top: 25px;
					line-height: 26px;
					padding-left: 20px;

					.sj {
						display: inline-block;
						width: 50px;
						height: 26px;
						background-color: #FFC801;
						text-align: center;
						/* border-bottom: 22px; */
						border-radius: 4px;
						color: white;
						margin-left: 15px;
					}
				}
			}

			.yh {
				display: flex;
				height: 100px;
				align-items: center;

				.zt {
					flex: 1;
					padding-top: 5px;

					.h3 {
						font-weight: normal;
						color: white;
						text-align: center;
					}
				}

				.yt {
					flex: 1;
					padding-top: 5px;

					.h3 {
						font-weight: normal;
						color: white;
						text-align: center;

					}
				}

				.xian {
					height: 30px;
					width: 1px;
					background-color: white;

				}
			}
		}

		.zhong {
			margin: 10px 0px;
			height: 120px;
			background-color: white;

			padding-top: 4px;

			.zd {
				display: flex;
				/*  #ifdef MP-WEIXIN  */
				padding: 0px 8px 0 8px;
				/*  #endif  */
				/*  #ifdef H5  */
				padding: 8px 8px 0 8px;
				/*  #endif  */
				justify-content: space-between;

				.uni-icon-arrow {
					color: red;
				}
			}

			.li {
				flex: 1;
				text-align: center;
				list-style: none;

				.h3 {
					font-size: 14px;
					font-weight: normal;
				}
			}
		}

		.xia {}

	}
</style>
