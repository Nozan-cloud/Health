<template>
	<view class="container">
		<!-- 健康记录 -->
		<view class="header">
			<text class="time">9:41</text>
			<text class="title">健康记录</text>
		</view>
		<!-- BMI框 -->
		<view class="BMI">
			<view class="weight">
				<text class="label">体重</text>
				<text class="value">106斤</text>
				<text class="change">↓0.8斤</text>
				<text class="date">今天 08:52 对比昨天</text>
			</view>
			<view class="bmi">
		
				<text class="label">BMI</text>
				<text class="value">20.3</text>
				<text class="change">↓0.2</text>
			</view>
			<view class="fat">
				<text class="label">脂肪率</text>
				<text class="value">解锁更多</text>
			</view>
		</view>
		
		<!-- 计划 -->
		<view class="plan">
			<view class="improvement">
				<view class="improvement-header">
					<text class="title">计划</text>
				</view>
				<view class="improvement-body">
					<view class="improvement-item">
						<text class="label">周报</text>
						<text class="value">改善第一周</text>
					</view>
					<view class="improvement-item">
						<text class="label">体重</text>
						<text class="value">106.0斤</text>
					</view>
					<view class="improvement-item">
						<text class="label">BMI</text>
						<text class="value">20.3</text>
					</view>
					<view class="improvement-item">
						<text class="label">脂肪</text>
						<text class="value">解锁更多</text>
					</view>
				</view>
			</view>
			<view class="progress">
				<view class="progress-header">
					<text class="title">改善第一周</text>
				</view>
				<view class="progress-body">
					<view class="progress-item">
						<text class="label">改善前情况</text>
						<text class="value">106.0斤</text>
					</view>
					<view class="progress-item">
						<text class="label">改善后情况</text>
						<text class="value">103.0斤</text>
					</view>
				</view>
			</view>
		</view>
		
		<!-- 目标框 -->
		<view class="goals">
			<view class="row">
				<view class="goal">
					<view class="text">
						<text class="label">饮食</text>
						<text class="value">今天不超过1200千卡</text>
					</view>
					
				</view>
				<view class="goal">
					
					<text class="label">喝水</text>
					<text class="value">今天目标是2000毫升</text>
				</view>
			</view>
			<view class="row">
				<view class="goal">
					<text class="label">步数</text>
					<text class="value">每天目标8000步</text>
				</view>
				<view class="goal">
					<text class="label">睡眠时间</text>
					<text class="value">每天八小时</text>
				</view>
			</view>
		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				// 页面数据
			};
		},
		methods: {
			// 页面方法
		}
	};
</script>

<style scoped>
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 20px;
		background-color: #f5f5f5;
		
	}

	.header {
		margin-bottom: 20px;
		width: 100%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		border: 1px solid red;
	}

	.time {
		font-size: 14px;
		color: #888;
	}

	.title {
		font-size: 24px;
		font-weight: bold;
		margin-top: 5px;
	}

	.BMI {
		height: 350rpx;
		width: 100%;
		/* border: 1px solid #50c6d4; */
		border-radius: 5px;
		background-color: #50c6d4;
		margin-bottom: 10rpx;
		display: flex;
		flex-direction: column;
		align-items: center;
		/* border: 1px solid red; */
	}

	.weight,
	.bmi,
	.fat {
		width: 100%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-bottom: 10px;
	}

	.label {
		padding-left: 10rpx;
		padding-top: 5rpx;
		font-size: 16px;
		font-weight: bold;
		color: #fff;
	}

	.value {
		padding-left: 10rpx;
		padding-top: 5rpx;
		font-size: 12px;
		
		color: #fff;
	}

	.change {
		font-size: 14px;
		color:#888;
	}

	.date {
		font-size: 12px;
		color: #888;
	}

	.goals {
		width: 100%;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		/* border: 1px solid red; */
		
			
	}

	.row {
		display: flex;
		width: 100%;
		justify-content: space-between;
		margin-bottom: 5px;
		/* Adjusted margin for spacing */
	}

	.goal {
			
		height: 150rpx;
		width: calc(50% - 10px);
		border-radius: 5px;
		background-color: #fff;
		margin-bottom: 5px;
		.label {
		
			font-size: 16px;
			
			color: #333;
		}
		
		.value {
		
			font-size: 12px;
			
			color: #888;
		}
	}

	.label,
	.value {
		
		display: block;
	}

	.plan {
		
		
		display: flex;
		justify-content: space-between;
		align-items: flex-start;
		width: 100%;
	/* 	border: 1px solid red; */
		.label {
			font-size: 16px;
			font-weight: bold;
			color: #333;
		}
		
		.value {
			font-size: 12px;
			
			color: #888;
		}
	
	}

	.improvement,
	.progress {
		height: 300rpx;
		width: calc(50% - 10px);
		
		border-radius: 5px;
			background-color: #fff;
		margin-bottom: 10px;
		
		
	}

	.improvement-header,
	.progress-header {
		display: flex;
		justify-content: center;
		align-items: center;
		margin-bottom: 10px;
	}

	.improvement-body,
	.progress-body {
		display: flex;
		flex-direction: column;
		align-items: center;
		
	}

	.improvement-item,
	.progress-item {
		width: 100%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-bottom: 10px;
		
	}

	.title {
		font-size: 18px;
		font-weight: bold;
		color: #333;
	}



	
</style>