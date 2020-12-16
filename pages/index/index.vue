<template>
	<view class="content">
		<view class="title-area">
			<text class="title">{{title}}</text>
		</view>
		<view class="butten-array">
			<navigator class="button">
				<button>简介</button>
			</navigator>

			<navigator class="button">
				<button>开始</button>
			</navigator>

			<navigator class="button">
				<button>关于本程序</button>
			</navigator>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'International\nPhonetic\nAlphabet\n国际音标'
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
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		background-color: #ffffd7;
		width: 100%;
		height: 100%;
	}

	.title-area {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		text-align: center;
		background-color: #A0522D;
	}

	.title {
		font-size: xx-large;
		color: #e4e4e4;
	}
	
	.butten-array {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		background-color: #ffffd7;
		width: 100%;
		height: 100%;
	}
	
	.button {
		margin-top: 5%;
		margin-bottom: 5%;
		width: 100%;
	}
</style>
