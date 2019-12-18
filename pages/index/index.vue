<template>
	<view class="content">
		<search-top></search-top>
		<view class="mian">
			<view class="share">
				<view class="share-lf">
					<image src="../../static/images/center-0.png"></image>
					<text>如何分享</text>
				</view>
				<view class="share-rt">
					<image src="../../static/images/center-0.png"></image>
					<text>如何分享</text>
				</view>
			</view>
			
			<view class="examination">
				<view><text class="examination-tit">科二考场</text></view>
				<view class="examination-box">
					<view>
						<image src="https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/shuijiao.jpg" class="examination-img"></image>
					</view>
					<view class="examination-tex">
						<text>西丽</text>
						<text>2999次播放</text>
						<text>9.9￥</text>
					</view>
					<view class="examination-share">
						<text>转发分享</text>
					</view>
				</view>
				
				<view class="examination-box">
					<view>
						<image src="https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/muwu.jpg" class="examination-img"></image>
					</view>
					<view class="examination-tex">
						<text>西丽考场一号线</text>
						<text>2999次播放</text>
						<text>9.9￥</text>
					</view>
					<view class="examination-share">
						<text>转发分享</text>
					</view>
				</view>
				
				<view class="examination-box">
					<view>
						<image src="https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/muwu.jpg" class="examination-img"></image>
					</view>
					<view class="examination-tex">
						<text>西丽考场一号线</text>
						<text>2999次播放</text>
						<text>9.9￥</text>
					</view>
					<view class="examination-share">
						<text>转发分享</text>
					</view>
				</view>
				
				<view class="examination-box">
					<view>
						<image src="https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/muwu.jpg" class="examination-img"></image>
					</view>
					<view class="examination-tex">
						<text>西丽考场一号线</text>
						<text>2999次播放</text>
						<text>9.9￥</text>
					</view>
					<view class="examination-share">
						<text>转发分享</text>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import SearchTop from '@/components/search/search.vue'; 
	export default {
		data() {
			return {
				
			}
		},
		onLoad() {

		},
		methods: {

		},
		components:{
			SearchTop
		}
	}
</script>

<style>
	.mian{padding-left: 10upx;padding-right: 10upx;}
	.share{display: flex;justify-content:space-around;}
	.share-lf{width:47%;border: 1upx solid #333333;border-radius:20upx;background-image:url("https://img-cdn-qiniu.dcloud.net.cn/uniapp/images/shuijiao.jpg");background-size: auto;}
	.share-rt{width:47%;border: 1upx solid #333333;border-radius:20upx;}
	.share-lf image{display: block;width:100upx;height: 100upx;margin: auto;}
	.share-lf text{font-size: 30upx;font-weight: 500;text-align: center;display: block;padding:10upx;}
	.share-rt image{display: block;width:100upx;height: 100upx;margin: auto;}
	.share-rt text{font-size: 30upx;font-weight: 500;text-align: center;display: block;padding:10upx;}
	
	.examination-tit{font-size: 30upx;color: #808080;padding: 20upx 10upx;display: block;}
	.examination-box{display: flex;justify-content:space-around;margin-bottom: 10upx;}
	.examination-tit view{width:31%;}
	.examination-img{width:290upx;height:190upx;display: block;border-radius: 15upx;}
	.examination-tex{display: flex;flex-direction:column;padding-top:20upx;padding-bottom: 20upx;}
	.examination-tex text:nth-child(1){font-size:35upx;font-weight: 600;width:240upx;text-overflow: ellipsis;overflow: hidden;white-space: nowrap;}
	.examination-tex text:nth-child(2){font-size:20upx;color: #808080;width:240upx;text-overflow: ellipsis;overflow: hidden;white-space: nowrap;}
	.examination-tex text:nth-child(3){font-size:40upx;color: #F0AD4E;width:240upx;text-overflow: ellipsis;overflow: hidden;white-space: nowrap;padding-top:35upx;}
	.examination-share {margin-top:100upx;}
	.examination-share  text{width: 160upx;height:60upx;background: #007AFF;color: #fff;font-size: 25upx;border-radius: 40upx;display: block;text-align: center;line-height: 60upx;}
</style>
