<template>
	<view class="content">
		<view class="xia">

			<radio-group @change="radioChange">
				<label class="uni-list-cell uni-list-cell-pd zd" v-for="(item,index) in list" :key="item.value">
						<view>{{item.name}}</view>
					<view>
						<radio :value="item.value" :checked="index === current"/>
					</view>
				
				</label>
			</radio-group>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
              list:[{
				  name:'中文',
				  value:1
			  },
			  {
				  name:'英文',
				  value:2
			  }],
			  current:0
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

		uni-checkbox .uni-checkbox-input {
			border: none !important;
		}

	}
</style>
