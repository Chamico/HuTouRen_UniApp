<template>
	<view class="content">
		<view class="border">
			<view>
				
			</view>			
		</view>

		<view class="sender">
			<view style="width: 80%; height: 100%;">
				<input class="input" focus placeholder="请输入需要发送的内容" />
			</view>
			<view>
				<button type="primary">发送</button>
			</view>
		</view>
	</view>
	
</template>

<script>
</script>

<style scoped>
	.content{
		padding: 0 5px;
	}
	.border{
		width: 99%;
		height: 100px;
		border: 1px solid red;
	}
	.input{ 
		width: 100%;
		height: inherit;
		border: 1px solid gray;
		border-radius: 5px;
	}
	.sender{
		height: 50px;
		margin-top: 10px;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
</style>