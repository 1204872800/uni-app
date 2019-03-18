<template>
	<view class="content">
		<view class="xia">
			<navigator url="/pages/my/my-my/ModifyNumber/ModifyNumber" class="zd">
				<text class="zd1" style="color:#313131">
					<!-- 更换手机号 -->
						更换手机号
				</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
			<!-- 意见反馈 -->
			<navigator url="/pages/my/my-my/ModifyingData/ModifyingData" redirect class="zd">
				<text class="zd1" style="color:#313131">修改资料</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
			<navigator url="/pages/my/my-my/language/language" class="zd">
				<text class="zd1" style="color:#313131">语言</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
			<navigator url="/AboutUs" class="zd">
				<text class="zd1" style="color:#313131">清除缓存</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
			<navigator url="/AboutUs" class="zd">
				<text class="zd1" style="color:#313131">检查更新</text>
				<uni-icon type="arrowright" color="#B4B4B4" size="30"></uni-icon>
			</navigator>
		</view>

		<view class="xx">
			<button type="primary" @click="dj">退出登录</button>
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
				dj() {
					uni.switchTab({
						url: '/pages/my/my'
					});
				}
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
