<script setup>
import TheWelcome from "@/components/TheWelcome.vue";


let message = $ref("Hello, World");

setTimeout(() => {
	message = "I have Been Changed";
},2000);

let doSomething = () => {
	alert("doing it now");
};


//Sin colocar setup en <script setup>
/*export default {
	setup(){
		//onMounted(() => {
		//	alert("Hi there");
		//});

		let message = ref("Hello, World");

		setTimeout(() => {
			message.value = "I have Been Changed";
		},2000);

		return {
			message
		};
	}
};*/

</script>

<template>
  <main>
    <TheWelcome />
    {{ message }}
    <input type="text" v-model="message">
    <button @click="doSomething">Click me</button>
  </main>
</template>
