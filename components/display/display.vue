<template>
	<view class="display">
		<span @click='openCalculatorPopup()'>123</span>
		<uni-popup type="center" ref="calculator" :maskClick="false">
			<xl-calculator @closeCalculatorPopup="closeCalculatorPopup"></xl-calculator>
		</uni-popup>
	</view>
</template>

<script>
	export default {
		name: "display",
		data() {
			return {

			};
		},
		methods: {
			openCalculatorPopup() {
				this.$refs.calculator.open();
			}
		},
	}
</script>

<style>

</style>
