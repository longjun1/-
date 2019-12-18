<template>
	<view>
		<view class="nav">
			<view class="nav-lf">
				<text>可提现金额</text>
				<text>￥999</text>
			</view>
			<view class="nav-rt">
				<view class="nav-wrap"><image src="../../static/images/center-1.png"></image><text>立即提现</text></view>
			</view>
		</view>
		
		<view class="content-tit">
			<view class="content-tit-list">
				<text>5</text>
				<text>今日收益</text>
			</view>
			<view class="content-tit-list">
				<text>123</text>
				<text>累计收益</text>
			</view>
			<view class="content-tit-list">
				<text>99</text>
				<text>累计提现</text>
			</view>
		</view>
		<view>
			<view class="order-tab">
				<view v-for="(item,index) in order" :key="index" @click="gettab(index)" :class="{active:cur==index}">{{item}}</view>
			</view>
			<view>
				<view v-show="cur==0">
					<view class="personnel">
						<view>
							<image src="../../static/images/center-1.png" class="personnel-img"></image>
						</view>
						<view>
							<text class="username">小龙</text>
							<text class="oldday">代理有效期：442天</text>
						</view>
						<view>
							<text class="money">495￥</text>
							<text class="contribution">贡献金额</text>
						</view>
					</view>
					
					<view class="personnel">
						<view>
							<image src="../../static/images/center-1.png" class="personnel-img"></image>
						</view>
						<view>
							<text class="username">小龙</text>
							<text class="oldday">代理有效期：442天</text>
						</view>
						<view>
							<text class="money">495￥</text>
							<text class="contribution">贡献金额</text>
						</view>
					</view>
				</view>
				<view v-show="cur==1">2</view>
				<view v-show="cur==2">3</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				order:['直接推广订单','下级推广订单','下级代理人'],
				cur:0
			}
		},
		methods: {
			gettab(index){
				this.cur=index
			}
		}
	}
</script>

<style>
.nav{display: flex;background: #E7CB9C;height:300upx;}
.nav-lf{width: 50%;}
.nav-lf text{display: block;}
.nav-lf text:nth-child(1){font-size: 40upx;font-weight: 600;color: #876837;margin-top: 70upx;margin-left: 60upx;}
.nav-lf text:nth-child(2){font-size: 50upx;font-weight: 600;color: #876837;margin-top: 30upx;margin-left: 60upx;}
.nav-rt{width: 50%;}
.nav-wrap{height:60upx;width: 150upx;background: #8B6840;border-radius:30upx;padding: 0upx 20upx;margin-top: 150upx;margin-left: 150upx;}
.nav-wrap image{height:30upx;width: 30upx;display: inline-block;vertical-align: middle;}
.nav-wrap text{font-size:20upx;color: #fff;display: inline-block;padding-left: 15upx;}

.content-tit{display: flex;background: #ECDDC0;}
.content-tit-list{width: 33.33%;}
.content-tit-list text{display: block;font-size: 30upx; color: #876837;text-align: center;padding:15upx;}

.order-tab{display: flex;text-align: center;border-bottom:1upx solid #F1F1F1;}
.order-tab>view{width: 33.33%;font-size:30upx;height:100upx;line-height: 100upx;color: #999;}
.order-tab .active:after{content: '';width: 70upx;height: 8upx;background:#007AFF;display: block;margin:-10upx auto 0upx auto;}
.order-tab .active{color: #007AFF;}

.personnel{display:flex;padding:25upx 20upx;border-bottom:10upx solid #EEEEEE;}
.personnel>view:nth-child(1){width:20%;}
.personnel>view:nth-child(2){width:40%;}
.personnel>view:nth-child(3){width:40%;}
.personnel-img{height:100upx;width: 100upx;border-radius:50%;display: block;}
.username{display: block;font-size: 32upx;font-weight: bold;}
.oldday{font-size:20upx;color: #999;}
.money{display: block;font-size:35upx;color: #876837;text-align: right;}
.contribution{display: block;font-size:20upx;color: #999;text-align: right;}
</style>
