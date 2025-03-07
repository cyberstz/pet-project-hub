<template>
	<div class="bg-white p-4 rounded-lg shadow-md">
		<h3 class="font-semibold">{{ title }}</h3>
		<p class="text-gray-500">{{ description }}</p>
		<div class="flex justify-between items-center mt-2">
			<span>🔥 {{ likes }}</span>
			<span>💬 {{ comments }}</span>
		</div>
	</div>
</template>

<script>
export default {
	name: 'ProjectCard',
	props: {
		title: String,
		description: String,
		likes: Number,
		comments: Number
	}
};
</script>
