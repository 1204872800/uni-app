<template>
	<view class="content">
		<view style="text-align: center;padding: 20px 0;">
			   <image style="width: 200px;height: 200px;" mode="scaleToFill" src="../../../../static/tou.png"></image>
		</view>
				<view class="xia">
			<navigator url="#" class="zd">
				<text class="zd1" style="color:#313131">昵称</text>
				<view style="display: flex;align-items: center;color: #B4B4B4;">
					<text>
						往事随风
					</text>
					<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
				</view>
				
			</navigator>
			<navigator url="#" class="zd">
				<text class="zd1" style="color:#313131">性别</text>
					<view style="display: flex;align-items: center;color: #B4B4B4;">
					<text>
						男
					</text>
					<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
				</view>
			</navigator>
			<navigator url="#" class="zd">
				<text class="zd1" style="color:#313131">出生日期</text>
					<view style="display: flex;align-items: center;color: #B4B4B4;">
					<text>
						2018-9-2
					</text>
					<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
				</view>
			</navigator>
				<navigator url="#" class="zd">
				<text class="zd1" style="color:#313131">电子邮箱</text>
				<view style="display: flex;align-items: center;color: #B4B4B4;">
				<text>
					12024238@11.com
				</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</view>
			</navigator>
				<navigator url="#" class="zd">
				<text class="zd1" style="color:#313131">所属行业</text>
					<view style="display: flex;align-items: center;color: #B4B4B4;">
					<text>
						码农
					</text>
					<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
				</view>
			</navigator>
				<navigator url="#" class="zd">
				<text class="zd1" style="color:#313131">所在地区</text>
					<view style="display: flex;align-items: center;color: #B4B4B4;">
					<text>
						深圳市-坂田区-五河
					</text>
					<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
				</view>
			</navigator>
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
				
			};
		}
	}
</script>

<style lang="less" scoped>
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
		

	}


</style>
