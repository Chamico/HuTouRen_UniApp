<template>
	<view class="pages"> 
		<view class="pages-header"> 
			<view class="pages-header-body">
				<image class="pages-header-body-avtar" src="../../static/default.webp"></image>
				<view>
					<view class="pages-header-body-title">
						<text style="margin-right: 8rpx;">{{ userInfo.nickName }}</text>
					</view>
					<view class="pages-header-body-desc">{{ userInfo.title }}</view>
				</view>
			</view> 
		</view>

		<view class="pages-body"> 
			<view class="pages-section">
				<view class="pages-section-body">
					<view class="pages-cell">
						<view class="pages-cell-body">帮助与反馈</view>
						<view class="pages-cell-extra">
							<uni-icons type="right" color="#999999" size="24"/>
						</view>
					</view>
					<view class="pages-cell">
						<view class="pages-cell-body">隐私条款</view>
						<view class="pages-cell-extra">
							<uni-icons type="right" color="#999999" size="24"/>
						</view>
					</view>
					<view class="pages-cell">
						<view class="pages-cell-body">关于</view>
						<view class="pages-cell-extra">
							<uni-icons type="right" color="#999999" size="24" />
						</view>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>

export default {
	components: {
	},
	data() {
		return { 
			userInfo: { // 用户信息
				nickName: "Uniapp",  
				vipValidityDateStr: "2024-08-10"
			}
		}
	},
	onShow () {
	},
	methods: {
	}
}
</script>

<style lang="scss">
.pages {
  width: 100vw;
	height: calc(100vh - 50px);
	background: #F5F7F9;
	padding-bottom: 64rpx;

	&-header {
		position: relative;
    	z-index: 1;
		height: 360rpx; 
		background-image: url('../../static/bg.png');
		background-size: cover;
		padding: 48rpx 32rpx 0;
		display: flex;
		align-items: center;
		justify-content: space-between;
		color: #FFF;
		&-bg{
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 360rpx;
		}

		&-title {
			position: absolute;
			top: 107rpx;
			left: 0;
			width: 100%;
			display: flex;
			align-items: center;
			justify-content: center;
			font-size: 36rpx;
			font-weight: 500;
			color: #FFFFFF;
		}

		&-body {
			display: flex;
			align-items: center;

			&-avtar {
				width: 110rpx;
				height: 110rpx;
				margin-right: 22rpx;
				border-radius: 50%;
				overflow: hidden;
        		border: 2rpx solid #fff;
			}

			&-title {
				font-size: 36rpx;
				font-weight: 500;
				height: 40rpx;
				display: flex;
				align-items: center;
				white-space: nowrap;
			}

			&-desc {
				margin-top: 12rpx;
				font-size: 24rpx;
				line-height: 40rpx;
			}
		}
	}

	&-body {
		position: relative; 
		padding: 0 28rpx;
		border-radius: 16rpx 16rpx 0rpx 0rpx;
		background: #F5F7F9;
		display: flex;
		flex-direction: column;
	}
 

	&-section {
		margin-top: 20rpx;
		background: #FFFFFF;
		border-radius: 20rpx;
		padding: 40rpx 28rpx;

		&-title {
			height: 50rpx;
			font-size: 36rpx;
			font-weight: 500;
			color: #333333;
			line-height: 50rpx;
			margin-bottom: 20rpx;
		}
	}

	&-cell {
		height: 64rpx;
    	margin-top: 24rpx;
		display: flex;
		align-items: center;
		&:first-child{
		margin-top: 0;
		}
		&-body {
			flex: 1;
		}

		&-extra {
			flex: 0 0 auto;
			margin-left: 20rpx;
		}
	} 

  .follow{
    margin-top: 20rpx;
    width: 686rpx;
  }
}
</style>
