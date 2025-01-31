<template>
	<main>
		<section id="hero" class="relative h-[75vh] p-25 flex items-center justify-center">
			<img src="/hero.png" alt="Hero Image" class="absolute inset-0 w-full h-full object-cover opacity-50">
			<h1 class="relative text-7xl/24 font-bold text-center">Code, Creativity, and a Curiosity That Never Stops.
			</h1>
		</section>
		<section id="about" class="container mx-auto px-10 py-20 grid grid-cols-1 gap-10 md:grid-cols-2">
			<div class="w-[405px] h-[540px] bg-[#343434] mx-10 rounded-xl overflow-hidden -rotate-3">
				<img src="/me1.png" alt="About Image" class="w-full h-full p-5 rounded-3xl object-cover">
			</div>
			<div class="flex flex-col justify-center">
				<h2 class="text-4xl font-bold">About Me</h2>
				<p class="mt-5 text-lg">
					Ferdinan Kurnia Nugroho (a.k.a Ferdinan Iydheko), Lorem Ipsum is simply dummy text of the printing
					and
					typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
					when an
					unknown printer took a galley of type and scrambled it to make a type specimen book.
					<br>
					<br>
					It has survived not only five centuries, but also the leap into electronic typesetting, remaining
					essentially
					unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem
					Ipsum
					passages, and more recently with desktop publishing software like Aldus PageMaker including versions
					of Lorem
					Ipsum.
				</p>
			</div>
		</section>
		<section id="projects">
			<div class="container mx-auto px-10">
				<h2 class="text-4xl font-bold text-center">My Projects</h2>
				<div class="flex flex-wrap justify-center gap-10 mt-10">
					<div class="bg-[#343434] w-full rounded-xl overflow-hidden">
						<!-- <img src="/project-1.png" alt="Project 1 Image" class="w-full h-[300px] object-cover"> -->
						<div class="pt-15 pb-0 grid gap-8">
							<img src="/paperiteicon.png" alt="Paperite Icon" class="mx-auto">
							<div>
								<h3 class="font-['courgette'] text-3xl font-bold text-center">Paperite</h3>
								<p class="mt-2 text-lg text-center">Just another note-taking app.</p>
							</div>
							<img src="/paperitepreview.png" alt="Paperite App Preview" class="mx-auto px-15">
						</div>
					</div>
				</div>
			</div>
		</section>
		<section id="blog" class="py-20">
			<h2 class="text-4xl font-bold px-20">My Blog</h2>
			<div class="flex gap-10 mt-10 pb-2 px-20 overflow-x-auto hide-scrollbar">
				<a href="" v-for="n in 5" :key="n"
					class="flex-shrink-0 w-[350px] rounded-xl translate-y-1 hover:translate-y-0 transition-transform">
					<!-- Tambah flex-shrink-0 -->
					<img src="/mdnews.png" alt="Blog 1 Image" class="w-[350px] h-[200px] object-cover">
					<div class="py-5">
						<h3 class="text-xl font-bold">MD Shows is ended</h3>
						<p class="mt-2 text-sm text-gray-400 whitespace-normal">They ended this masterpiece shows.
							Here’s what we can do for keeping MD fandom alive.</p>
						<p class="mt-2 text-sm text-gray-400">Tue, 28 January 2025</p>
					</div>
				</a>
			</div>
		</section>
	</main>
</template>

<style>
/* Tambahkan CSS berikut */
.hide-scrollbar {
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}

.hide-scrollbar::-webkit-scrollbar {
  display: none;  /* Chrome, Safari, and Opera */
}
</style>