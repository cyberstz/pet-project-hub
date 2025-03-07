<template>
	<div class="bg-white p-4 rounded-lg shadow-md">
		<div class="flex items-center space-x-4">
			<div class="w-10 h-10 bg-gray-300 rounded-full"></div>
			<div>
				<h4 class="font-semibold">{{ name }}</h4>
				<p class="text-gray-600">Score: {{ score }}</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'ContributorCard',
	props: {
		name: String,
		score: Number
	}
};
</script>
