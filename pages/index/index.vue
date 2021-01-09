<template>
	<view>
		整数 <long-num-box 
			v-model="count"
			@change="change"
		>
		</long-num-box>
		小数 <long-num-box
			v-model="count1"
			:step="0.1"
			@change="change"
		>
		</long-num-box>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				count: 0,
				count1: 0
			}
		},
		onLoad() {

		},
		methods: {
			change (val) {
				console.log(val)
			}
		}
	}
</script>
