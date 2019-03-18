<template>
	<view class="content">
		<view class="box" v-for="i in 2">
			<view class="box-li">
				<text>想想</text>
				<text>1386653294</text>
			</view>
			<view class="box-li">
				<text>广东省深圳市半点去操控性</text>
			</view>
			<view class="box-li">
				<view>
					<checkbox-group class="uni-list" @change="radioChange">
						<label class="uni-list-cell uni-list-cell-pd">
							<checkbox value="cb" checked="true" />
							<text>默认地址</text>
						</label>
					</checkbox-group>
				</view>
				<view style="display: flex;">


					<!-- 编辑地址 -->
					<navigator url="/pages/my/my-my/ModifyAddress/ModifyAddress" navigate>
						<text style="padding-right: 10px;">
							编辑
						</text>
					</navigator>

					<navigator url="/pages/my/my-my/ModifyAddress/ModifyAddress" navigate>
						<text style="padding-right: 10px;">
							删除
						</text>
					</navigator>
				</view>
			</view>
		</view>

		<view class="xx">

			<button type="primary" @click="dj">新增地址</button>
		</view>

	</view>
</template>

<script>
	export default {
		components: {

		},
		data() {
			return {
				zj: false
			};
		},
		methods: {
			radioChange(e) {
				// this.zj =  e.target.value
				console.log(1111)
			},
			//新增地址
			dj() {
				uni.navigateTo({
					url: '/pages/my/my-my/addAddress/addAddress'
				});
			}
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

		.box:nth-child(1) {
			height: 140px;
			display: flex;
			flex-direction: column;
			background-color: #ffffff;
		}


		.box {
			margin-top: 10px;
			height: 140px;
			display: flex;
			flex-direction: column;
			background-color: #ffffff;

			.box-li {
				flex: 1;
				display: flex;
				justify-content: space-between;
				align-items: center;
				padding: 0 10px;
			}

			.box-li:nth-child(3) {
				flex: 1;
				display: flex;
				border-top: 1px #F0F0F0 solid;
				justify-content: space-between;
				align-items: center;
				padding: 0 10px;
			}
		}
	}
</style>
