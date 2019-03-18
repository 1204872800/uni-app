<template>
	<view class="content">
		<view class="taber">
			<view class="title" @click="change(index)" :class="{'active':curr==index}" v-for="(item,index) in list" :key="index">
				{{item}}
			</view>
		</view>
		
		<card :type="content" v-if="curr==0"></card>
	  <articles v-if="curr==1"></articles>
		 <shop v-if="curr==2"></shop>
	</view>
</template>

<script>
	// 商品
	 import card from "@/components/my-Collection/card.vue"
	 //文章
	 import articles from "@/components/my-Collection/articles.vue"
	 //店铺
	  import shop from "@/components/my-Collection/shop.vue"
	export default {
		components:{
			card,
			articles,
			shop
			
		},
		data() {
			return {
				 list:['商品','文章','店铺'],
				 curr:0,
				 content:'123123123'
			};
		},
		methods:{
			change(index){
				this.curr=index
			}
		}
	}
</script>

<style lang="less" scoped>
	.content {
		/*  #ifdef MP-WEIXIN  */
		height: 100vh;
		/*  #endif  */
		/*  #ifdef H5  */
		height: calc(100vh - 45px);
		/*  #endif  */
		width: 100%;
		background-color: #F3F3F3;
		  
      .taber{
		  height: 50px;
		  width: 100%;
		  background-color: white;
		  display: flex;
		  .title{
			  flex: 1;
			  text-align:center;
			  line-height: 50px;
			  margin: 0 20px;
		  }
		  .title.active{
			  color: red;
			  border-bottom: 2px solid red;
			  
		  }
		}

	}
</style>
