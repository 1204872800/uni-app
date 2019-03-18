<template>
	<view class="content">
		<view class="uni-common-mt">
			<view class="uni-form-item uni-column ss" style="display: flex;">
				<view class="title" style="font-size: 20px;">收货人</view>
				<input class="uni-input srk" focus />
			</view>
			<view class="uni-form-item uni-column ss" style="display: flex;">
				<view class="title" style="font-size: 20px;">联系电话</view>
				<input class="uni-input srk" />
			</view>

			<view class="zd" style="margin-left: 10px;">
				<text class="zd1" style="color:#313131;font-size: 20px;">所在地区</text>






				<!--  #ifdef H5-->
				<input maxlength="14" :value="array[index]" style="width: 200px;" />
				<picker @change="bindPickerChange" :value="index" :range="array">
					<view class="uni-input">请选择</view>
				</picker>
				<!--  #endif -->
				<!--  #ifdef MP-WEIXIN  -->

				<input maxlength="14" :value="region" style="width: 200px;" />


				<picker mode="region" @change="bindRegionChange" :range="region">
					<view class="uni-input">请选择</view>
				</picker>
				<!--  #endif -->




			</view>

			<view class="uni-form-item uni-column ss" style="display: flex;">
				<view class="title" style="font-size: 20px;">详细地址</view>
				<input class="uni-input srk" />
			</view>
		</view>

		<view class="checkbox">
			<checkbox value="123" checked="true" />
			<text style="margin-left: 10px;;">设为默认地址</text>
		</view>
		<view class="xx">
			<button type="warn" @click="dj">删除收货地址</button>
		</view>
		<view class="xx" style="margin-top: 8px;">
			<button type="primary" @click="dj">保存收货地址</button>
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
				array: ['中国', '美国', '巴西', '日本'],
				index: 0,
				region: '',
				customItem: '全部'
			};
		},
		methods: {
			bindRegionChange(e) {
				// console.log('picker发送选择改变，携带值为', e.detail.value)
				this.region = e.detail.value[0] + '/' + e.detail.value[1] + '/' + e.detail.value[2]
				console.log(this.region)
			},
			bindPickerChange: function(e) {
				console.log('picker发送选择改变，携带值为', e.target.value)
				this.index = e.target.value
			},
		}
	}
</script>

<style lang="less" scoped="">
	@import '../../../../static/Share.css';

	.content {
		/*  #ifdef MP-WEIXIN  */
		height: 100vh;
		/*  #endif  */
		/*  #ifdef H5  */
		height: calc(100vh - 45px);
		/*  #endif  */
		width: 100%;
		background-color: #F3F3F3;

		.uni-common-mt {
			background-color: #ffffff;

			.where {
				font-size: 20px;
				color: #C3C3C3;
				display: flex;
				justify-content: center;
				align-items: center;
			}

			.ss {
				border-bottom: 1px solid #EBEBEB;
				height: 50px;
				align-items: center;
				margin: 0 10px;

				.srk {
					font-size: 20px;
					margin-left: 5px;
				}
			}

		}

		uni-checkbox .uni-checkbox-input {
			background-color: #F3F3F3 !important;
		}

		.checkbox {
			display: flex;
			margin-top: 30px;
			margin-left: 20px;
			align-items: center;
		}
	}
</style>
