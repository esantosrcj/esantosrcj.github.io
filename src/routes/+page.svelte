<script lang="ts">
	import Navbar from './Navbar.svelte';
</script>

<svelte:head>
	<title>Eddie Santos - Software Engineer</title>
	<meta
		name="description"
		content="Senior Software Engineer with 9+ years of expertise in building scalable web applications and distributed systems."
	/>
</svelte:head>

<!-- Hero Section -->
<div
	class="hero hidden min-h-100 bg-linear-to-br from-primary to-secondary lg:flex lg:items-center lg:justify-center"
>
	<div class="hero-content text-center text-primary-content">
		<div class="max-w-md">
			<h1 class="mb-4 text-5xl font-bold">Eddie Santos</h1>
			<p class="text-xl opacity-90">Senior Software Engineer</p>
		</div>
	</div>
</div>

<!-- Navigation -->
<Navbar />

<!-- Main Content -->
<div class="mx-auto max-w-7xl space-y-8 px-4 py-12">
	<!-- About Section -->
	<section id="about" class="card border-base-300 bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">About Me</h2>
			<p class="mb-4">
				Experienced software engineer with 9+ years of expertise in building scalable web
				applications and distributed systems. Passionate about clean code, system design, and
				mentoring junior developers. Proven track record of delivering high-impact solutions in
				fast-paced environments.
			</p>
			<p>
				Currently focusing on cloud-native architectures, microservices, and DevOps practices.
				Always eager to learn new technologies and solve complex problems.
			</p>
		</div>
	</section>

	<!-- Skills Section -->
	<section id="skills" class="card border-base-300 bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Technical Skills
			</h2>

			<!-- Skills Snippet -->
			{#snippet skills(category: string, items: string[])}
				{#snippet listItem(item: string)}
					<li class="flex items-center gap-2">
						<span class="font-bold text-primary">▹</span>
						<span>{item}</span>
					</li>
				{/snippet}

				<h3 class="mb-3 text-xl font-bold text-secondary">{category}</h3>
				<ul class="space-y-2">
					{#each items as item}
						{@render listItem(item)}
					{/each}
				</ul>
			{/snippet}

			<div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-4">
				<div>
					{@render skills('Languages', ['JavaScript/TypeScript', 'Python', 'Java', 'SQL'])}
				</div>
				<div>
					{@render skills('Frontend', [
						'React, Svelte',
						'Next.js, SvelteKit',
						'HTML/CSS',
						'Tailwind CSS'
					])}
				</div>
				<div>
					{@render skills('Backend', [
						'Node.js, Express',
						'FastAPI, Flask',
						'Spring Boot',
						'REST APIs'
					])}
				</div>
				<div>
					{@render skills('Database & Cloud', [
						'PostgreSQL, MySQL, MongoDB',
						'Redis',
						'AWS, Google Cloud',
						'Docker, CI/CD'
					])}
				</div>
			</div>
		</div>
	</section>

	<!-- Projects Section -->
	<section id="projects" class="card border-base-300 bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Featured Projects
			</h2>

			<!-- Project Snippet -->
			{#snippet project(
				name: string,
				techStack: string[],
				description: string,
				liveLink: string,
				githubLink: string
			)}
				{#snippet listItem(item: string)}
					<span class="badge badge-outline badge-info">{item}</span>
				{/snippet}

				<h3 class="mb-2 text-2xl font-bold">{name}</h3>
				<div class="mb-3 flex flex-wrap gap-2">
					{#each techStack as item}
						{@render listItem(item)}
					{/each}
				</div>
				<p class="mb-4 text-base-content/70">
					{description}
				</p>
				<div class="flex flex-wrap gap-3">
					<a href={liveLink} class="btn btn-primary">Live Demo</a>
					<a href={githubLink} class="btn btn-outline btn-secondary">GitHub</a>
				</div>
			{/snippet}

			<div class="space-y-6">
				<div class="border-l-4 border-primary pl-6">
					{@render project(
						'Fantasy Sports Draft Board',
						['Svelte', 'SvelteKit', 'Tailwind CSS', 'CI/CD'],
						'Built a fantasy sports draft board application with real-time updates and seamless user experience.',
						'#live',
						'#github'
					)}
				</div>

				<div class="border-l-4 border-primary pl-6">
					{@render project(
						'Daily Workout Logger',
						['Svelte', 'SvelteKit', 'Python', 'FastAPI', 'PocketBase', 'Docker'],
						'Developed a daily workout logging application with real-time data synchronization and personalized analytics.',
						'#live',
						'#github'
					)}
				</div>
			</div>
		</div>
	</section>

	<!-- Experience Section -->
	<section id="experience" class="card border-base-300 bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Work Experience
			</h2>
			<div class="space-y-6">
				<div class="border-b border-base-300 pb-6 last:border-0">
					<div class="mb-1 text-lg font-semibold text-primary">Software Engineer</div>
					<h3 class="text-xl font-bold">PrestoSports</h3>
					<div class="mb-3 text-sm text-base-content/70">August 2021 - November 2025</div>
					<ul class="list-inside list-disc space-y-2 text-base-content/70">
						<li>
							Led full-stack development for key features, enhancing user engagement and system
							performance
						</li>
					</ul>
				</div>
			</div>
		</div>
	</section>

	<!-- Contact Section -->
	<section id="contact" class="card border-base-300 bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Get In Touch
			</h2>
			<div class="grid grid-cols-2 gap-3 sm:flex sm:flex-wrap sm:justify-center sm:gap-4">
				<a
					href="mailto:your.email@example.com"
					class="btn btn-outline btn-sm btn-secondary sm:btn-md">Email</a
				>
				<a
					href="https://github.com/yourusername"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-outline btn-sm btn-secondary sm:btn-md">GitHub</a
				>
				<a
					href="https://linkedin.com/in/yourprofile"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-outline btn-sm btn-secondary sm:btn-md">LinkedIn</a
				>
				<a
					href="https://twitter.com/yourhandle"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-outline btn-sm btn-secondary sm:btn-md">Twitter</a
				>
			</div>
		</div>
	</section>
</div>

<!-- Footer -->
<footer class="footer-center footer bg-base-100 p-10">
	<aside>
		<p class="font-semibold">&copy; 2026 Eddie Santos. All rights reserved.</p>
	</aside>
</footer>
