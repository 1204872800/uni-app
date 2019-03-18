<template>
	<view class="content">
		<view>
            <text class="title">{{title}}</text>
        </view>
		
		<find></find>
	</view>
</template>

<script>
	 import find from '../../components/my-Collection/find.vue'
	export default {
		components:{
			find
		},
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.content {
		text-align: center;
		height: 400upx;
	}
    .logo{
        height: 200upx;
        width: 200upx;
        margin-top: 200upx;
    }
	.title {
		font-size: 36upx;
		color: #8f8f94;
	}
</style>
