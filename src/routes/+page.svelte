<script lang="ts">
	import Navbar from './Navbar.svelte';
	import profileImage from '$lib/assets/profile-me.jpg';
	import { ChevronRight, Github, Linkedin } from '@lucide/svelte';
</script>

<svelte:head>
	<title>Eddie Santos - Senior Software Engineer</title>
	<meta
		name="description"
		content="Senior Software Engineer with 9+ years of expertise in building scalable web applications and distributed systems."
	/>
</svelte:head>

<!-- Hero Section -->
<div
	class="hero hidden min-h-100 bg-linear-to-br from-primary to-secondary lg:flex lg:items-center lg:justify-center"
>
	<div class="hero-content flex-col gap-6 text-primary-content lg:flex-row">
		<img src={profileImage} alt="Eddie Santos" class="mask w-64 mask-squircle shadow-2xl" />
		<div class="text-center lg:text-left">
			<h1 class="mb-4 text-5xl font-bold">Eddie Santos</h1>
			<p class="text-lg opacity-90">Building reliable solutions behind great user experiences</p>
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
				applications and distributed systems across collegiate athletics, healthcare, and EdTech
				industries. Expert in full-stack development with proven ability to modernize legacy
				systems, optimize performance, and collaborate with cross-functional teams to deliver
				high-quality solutions.
			</p>
			<p>
				Currently focused on mobile app development while staying up to date with the latest
				advancements in artificial intelligence, including new models, tools, and industry best
				practices. Always eager to learn new technologies and tackle complex problems.
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
						<ChevronRight class="h-4 w-4 text-primary" />
						<span>{item}</span>
					</li>
				{/snippet}

				<h3 class="mb-3 text-xl font-bold">{category}</h3>
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
				<div class="mb-4 flex flex-wrap gap-2">
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

			<div class="space-y-8">
				<div class="border-l-4 border-primary pl-6">
					{@render project(
						'Fantasy Sports Draft Board',
						['Svelte', 'SvelteKit', 'Tailwind CSS', 'CI/CD'],
						'Built a fantasy sports draft board application designed to enhance in-person draft events by providing an interactive, engaging, and visually intuitive drafting experience for participants.',
						'https://fantyboard.app',
						'https://github.com/esantosrcj/fantyboard'
					)}
				</div>

				<div class="border-l-4 border-primary pl-6">
					{@render project(
						'Daily Workout Logger',
						['Svelte', 'SvelteKit', 'Tailwind CSS', 'PocketBase'],
						'Developed a daily workout logging application with structured workout entries and progress tracking to help users record exercises, sets, and reps while maintaining historical workout data.',
						'https://myfitwerk.com/',
						'https://github.com/esantosrcj/workout-notepad'
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
				<div class="border-b border-secondary pb-6 last:border-0">
					<div class="mb-1 text-lg font-semibold">Software Engineer</div>
					<h3 class="text-xl font-bold text-info">PrestoSports</h3>
					<div class="mb-3 text-sm text-base-content/70">August 2021 - November 2025</div>
					<p class="mb-3 text-base-content/70">
						Worked as a full-stack engineer on large-scale sports technology platforms supporting
						athletic organizations nationwide.
					</p>
					<ul class="list-inside list-disc space-y-2 text-base-content/70">
						<li>Assisted modernization efforts from a legacy CMS toward microservices</li>
						<li>
							Built revenue-generating features with Stripe integrations and redesigned product
							packaging system
						</li>
						<li>
							Designed and delivered systems for live event monitoring, geo-blocked content
							delivery, and athlete record management
						</li>
						<li>
							Acted as a technical leader through code reviews, mentorship, and maintaining
							engineering standards
						</li>
					</ul>
				</div>

				<div class="border-b border-secondary pb-6 last:border-0">
					<div class="mb-1 text-lg font-semibold">Developer II</div>
					<h3 class="text-xl font-bold text-info">Blue Cross & Blue Shield of Kansas</h3>
					<div class="mb-3 text-sm text-base-content/70">August 2020 - July 2021</div>
					<p class="mb-3 text-base-content/70">
						Focused on backend optimization for healthcare claims systems serving nearly one million
						members.
					</p>
					<ul class="list-inside list-disc space-y-2 text-base-content/70">
						<li>
							Improved validation logic and batch-processing workflows for a high-volume claims
							platform processing over 17 million claims annually, reducing errors and manual
							intervention
						</li>
						<li>
							Played a key role in guiding the organization’s transition from SVN to Git,
							modernizing development workflows
						</li>
					</ul>
				</div>

				<div class="border-b border-secondary pb-6 last:border-0">
					<div class="mb-1 text-lg font-semibold">Software Engineer</div>
					<h3 class="text-xl font-bold text-info">PowerSchool Group LLC</h3>
					<div class="mb-3 text-sm text-base-content/70">September 2016 - April 2020</div>
					<p class="mb-3 text-base-content/70">
						Contributed to enterprise-scale K–12 education platforms, including absence management
						and applicant tracking systems used by hundreds of school districts.
					</p>
					<ul class="list-inside list-disc space-y-2 text-base-content/70">
						<li>
							Designed and implemented REST APIs for mobile applications, enhancing user experience
							and functionality
						</li>
						<li>
							Led modernization of an IVR system using a scalable, message-driven architecture,
							improving system reliability and performance
						</li>
						<li>
							Supported CI/CD and testing practices, contributing to faster deployment cycles and
							improved code quality
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
					href="https://github.com/esantosrcj"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-outline btn-sm btn-secondary sm:btn-md"
				>
					<Github />
					GitHub
				</a>
				<a
					href="https://www.linkedin.com/in/santos-eddie/"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-outline btn-sm btn-secondary sm:btn-md"
				>
					<Linkedin />
					LinkedIn
				</a>
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
