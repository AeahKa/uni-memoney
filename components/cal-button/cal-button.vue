<template>
	<view>
		<button class="button" @click="$emit('click', $event)">
			<slot />
		</button>
	</view>
</template>

<script>
	export default {
		name: "button",
		data() {
			return {

			};
		}
	}
</script>

<style lang="scss">
	button {
		background: #767676;
		color: #e6e6e6;
		border: none;
		border-radius: 4px;
		padding: 0 16px;
		// height: 40px;
	}
</style>
