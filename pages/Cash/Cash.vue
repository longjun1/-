<template>
	<view>
		<view class="header">
			<text class="header-lt">总金额</text>
			<text class="header-rt">￥888</text>
		</view>
		<view class="content">
			<text class="content-tit">提现金额</text>
			<view class="content-money">
				<text>￥</text>
				<input type="text"  placeholder="请输入提现金额"/>
			</view>
			<view class="withdrawal">
				<view class="withdrawal-lt"><text>可提现金额:</text><text>12121</text></view>
				<view class="withdrawal-rt"><text>已提金额: 1231211</text></view>
			</view>
			<button class="tixian">提现</button>
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
.header{display: flex;border-top:1upx solid #C8C7CC;border-bottom:1upx solid #C8C7CC;}
.header-lt{width:50%;display: block;font-size: 35upx;height:130upx;line-height: 130upx;color: #000;padding-left:20upx;}
.header-rt{width:50%;display:block;text-align: right;color: #FFC881;font-size:45upx;height:130upx;line-height: 130upx;padding-right:20upx;}
.content{padding-left:20upx;padding-right: 20upx;}
.content-tit{padding:20upx 0upx;font-size: 35upx;display: block;}
.content-money{border-bottom:1upx solid #C8C7CC;}
.content-money text{font-size:50upx;font-weight:bold;height:130upx;line-height:130upx;display: inline-block;width:150upx;}
.content-money>input{height:;display: inline-block;}

.withdrawal{display: flex;padding:20upx 0upx;}
.withdrawal>view{width:50%;}
.withdrawal-lt>text:nth-child(1){font-size:30upx;color: #C5C5C5;}
.withdrawal-lt>text:nth-child(2){font-size:30upx;color: #FFC881;margin-left:5upx;}
.withdrawal-rt>text:nth-child(1){font-size:30upx;color: #C5C5C5;display:block;text-align:right;padding-top:10upx}
.tixian{width:80%;margin:auto;height:100upx;background:#04D0F7;color:#fff;margin-top:100upx;}


</style>
