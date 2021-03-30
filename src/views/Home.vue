<template>
	<div class="home">
		<img alt="Vue logo" src="../assets/logo.png" />
		<div class="counter">{{ $store.state.counter }}</div>
		<div class="buttons">
			<button @click="decreaseCounter">-</button>
			<button @click="increaseCounter">+</button>
		</div>
	</div>
</template>

<script>
// @ is an alias to /src

export default {
	name: "Home",

	methods: {
		decreaseCounter() {
			this.counter--;
		},
		increaseCounter() {
			this.counter++;
		},
	},
};
</script>

<style>
div {
	margin-bottom: 10px;
}
.counter {
	font-size: 80px;
}
.buttons button {
	font-size: 40px;
	width: 100px;
	margin: 0 10px;
}
</style>
