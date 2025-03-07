<template>
	<div class="bg-gray-100">
		<div class="container mx-auto px-4">
			<!-- Navbar -->
			<nav class="flex justify-between items-center py-4">
				<div class="text-2xl font-bold">Logo</div>
				<ul class="flex space-x-4">
					<li><a href="#" class="hover:underline">Home</a></li>
					<li><a href="#" class="hover:underline">Explore</a></li>
					<li><a href="#" class="hover:underline">About</a></li>
					<li><a href="#" class="hover:underline px-4 py-2 bg-blue-500 text-white rounded-lg">Login/Signup</a></li>
				</ul>
			</nav>
		</div>
	</div>

	<div class="bg-blue-100">
		<div class="container mx-auto px-4">
			<!-- Hero Section -->
			<section class="text-center py-16 bg-blue-100">
				<h1 class="text-4xl font-bold mb-4">🚀 Share Your Side Projects & Get Inspired!</h1>
				<div class="space-x-4">
					<button class="btn-green">Post a Project</button>
					<button class="btn-blue">Explore Projects</button>
				</div>
			</section>
		</div>
	</div>
	
	<div class="bg-gray-100">
		<div class="container mx-auto px-4">
			<!-- Trending & Latest Projects -->
			<section class="p-8">
				<div class="flex justify-between mb-4">
					<h2 class="text-2xl font-bold">🔥 Trending Projects</h2>
					<h2 class="text-2xl font-bold">🆕 Latest Projects</h2>
				</div>
				<div class="grid grid-cols-2 gap-4">
					<ProjectCard v-for="n in 6" :key="n" :title="'Project Title ' + n" description="Short project description..." :likes="120" :comments="45" />
				</div>
			</section>
		</div>
	</div>

	<div class="bg-yellow-100">
		<div class="container mx-auto px-4">
			<!-- Featured Project of the Week -->
			<section class="p-8">
				<h2 class="text-3xl font-bold mb-4">⭐ Featured Project of the Week</h2>
				<div class="bg-white p-6 rounded-lg shadow-lg">
					<h3 class="text-2xl font-semibold">Amazing Project Title</h3>
					<p class="text-gray-600">Detailed description of the featured project...</p>
				</div>
			</section>
		</div>
	</div>		

	<div class="bg-gray-100">
		<div class="container mx-auto px-4">
			<!-- Leaderboard & Top Contributors -->
			<section class="p-8">
				<div class="flex justify-between mb-4">
					<h2 class="text-2xl font-bold">🏆 Leaderboard</h2>
					<h2 class="text-2xl font-bold">🎖️ Top Contributors</h2>
				</div>
				<div class="grid grid-cols-2 gap-4">
					<ContributorCard v-for="i in 6" :key="i" :name="'User Name ' + i" :score="i * 100" />
				</div>
			</section>
		</div>
	</div>

	<div class="bg-green-100">
		<div class="container mx-auto px4">
			<!-- Call to Action -->
			<section class="text-center py-16 bg-green-100">
				<h2 class="text-3xl font-bold mb-4">📢 Join the Community & Share Your Ideas!</h2>
				<button class="btn-blue">Get Started for Free</button>
			</section>
		</div>
	</div>

	<div class="bg-gray-200 text-center">
		<div class="container mx-auto px4">
			<!-- Footer -->
			<footer class="p-4 bg-gray-200 text-center">
				<div class="flex justify-center space-x-4 mb-2">
					<a href="#" class="text-gray-600">About</a>
					<a href="#" class="text-gray-600">Contact</a>
					<a href="#" class="text-gray-600">Privacy Policy</a>
				</div>
				<p>&copy; 2025 Pet Project Hub. All rights reserved.</p>
			</footer>
		</div>
	</div>
</template>
  
<script>
import ProjectCard from '@/components/ProjectCard.vue';
import ContributorCard from '@/components/ContributorCard.vue';

export default {
	name: 'HomePage',
	components: {
		ProjectCard,
		ContributorCard
	}
};
</script>

<style scoped>
	.container {
		max-width: 1200px;
	}
	.btn-green {
		@apply bg-green-500 px-6 py-2 text-white rounded-lg;
	}
	.btn-blue {
		@apply bg-blue-500 px-6 py-2 text-white rounded-lg;
	}
</style>

