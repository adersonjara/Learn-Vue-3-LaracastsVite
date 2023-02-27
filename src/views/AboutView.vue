<script>

	import flash from "@/mixins/flash";
	
	export default {
		mixins: [flash]
	}

</script>

<template>
  <div>
    <p>
    	<button @click="flash('It Works in the about page')">Click Me</button>
    </p>
  </div>
</template>

