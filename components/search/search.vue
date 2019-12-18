<template>
	<view>
		<view class="header">
			<view class="header-lf">
				<text class="heade-tite">深圳市</text>
				<image src="../../static/images/center-0.png" mode="" class="heade-img"></image>
			</view>
			<view class="header-center">
				<input type="text" placeholder="请输入" class="search">
			</view>
			<view class="header-rt">
				<image src="../../static/images/index-0.png"></image>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style>
.header{display: flex;padding-left: 20upx;padding-right: 20upx;height: 100upx;padding-top:50upx;}
.header-lf{width: 16%;}
.heade-tite{font-size: 25upx;display: inline-block;}
.heade-img{width:30upx;height: 30upx;display: inline-block;vertical-align: middle;padding-left: 5upx;}
.header-center{width:77%;}
.search{border: 1upx solid #f5f4f4;background: #f5f4f4;height:60upx;margin: auto;width:90%;border-radius: 15upx;padding-left:10upx;padding-right:10upx;font-size:20upx;}
.header-rt{width: 7%;}
.header-rt image{width: 50upx;height: 50upx;display: block;vertical-align: middle;padding-top: 10upx;}
</style>
