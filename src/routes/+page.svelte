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
<div class="navbar sticky top-0 z-50 bg-base-100 shadow-lg">
	<!-- Mobile menu button -->
	<div class="navbar-start lg:hidden">
		<div class="dropdown">
			<div tabindex="0" role="button" class="btn btn-ghost">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="h-5 w-5"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M4 6h16M4 12h16M4 18h16"
					/>
				</svg>
			</div>
			<ul class="dropdown-content menu z-1 mt-3 w-52 menu-sm rounded-box bg-base-100 p-2 shadow">
				<li><a href="#about">About</a></li>
				<li><a href="#skills">Skills</a></li>
				<li><a href="#projects">Projects</a></li>
				<li><a href="#experience">Experience</a></li>
				<li><a href="#contact">Contact</a></li>
			</ul>
		</div>
	</div>
	<!-- Desktop navbar-start (empty for proper centering) -->
	<div class="navbar-start hidden lg:block"></div>
	<!-- Desktop menu -->
	<div class="navbar-center hidden lg:flex">
		<ul class="menu menu-horizontal gap-2 px-1">
			<li><a href="#about" class="btn btn-ghost">About</a></li>
			<li><a href="#skills" class="btn btn-ghost">Skills</a></li>
			<li><a href="#projects" class="btn btn-ghost">Projects</a></li>
			<li><a href="#experience" class="btn btn-ghost">Experience</a></li>
			<li><a href="#contact" class="btn btn-ghost">Contact</a></li>
		</ul>
	</div>
	<!-- Desktop navbar-end (empty for proper centering) -->
	<div class="navbar-end hidden lg:block"></div>
	<!-- Mobile title -->
	<div class="navbar-center lg:hidden">
		<span class="text-xl font-bold">Eddie Santos</span>
	</div>
</div>

<!-- Main Content -->
<div class="mx-auto max-w-7xl space-y-8 px-4 py-12">
	<!-- About Section -->
	<section id="about" class="card bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">About Me</h2>
			<p class="mb-4 text-base-content">
				Experienced software engineer with 9+ years of expertise in building scalable web
				applications and distributed systems. Passionate about clean code, system design, and
				mentoring junior developers. Proven track record of delivering high-impact solutions in
				fast-paced environments.
			</p>
			<p class="text-base-content">
				Currently focusing on cloud-native architectures, microservices, and DevOps practices.
				Always eager to learn new technologies and solve complex problems.
			</p>
		</div>
	</section>

	<!-- Skills Section -->
	<section id="skills" class="card bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Technical Skills
			</h2>
			<div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-4">
				<div>
					<h3 class="mb-3 text-xl font-bold text-secondary">Languages</h3>
					<ul class="space-y-2">
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>JavaScript/TypeScript</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Python</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Java</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>SQL</span>
						</li>
					</ul>
				</div>
				<div>
					<h3 class="mb-3 text-xl font-bold text-secondary">Frontend</h3>
					<ul class="space-y-2">
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>React, Svelte</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Next.js, SvelteKit</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>HTML/CSS</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Tailwind CSS</span>
						</li>
					</ul>
				</div>
				<div>
					<h3 class="mb-3 text-xl font-bold text-secondary">Backend</h3>
					<ul class="space-y-2">
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Node.js, Express</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>FastAPI, Flask</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Spring Boot</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>REST APIs</span>
						</li>
					</ul>
				</div>
				<div>
					<h3 class="mb-3 text-xl font-bold text-secondary">Database & Cloud</h3>
					<ul class="space-y-2">
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>PostgreSQL, MySQL, MongoDB</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Redis</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>AWS, Google Cloud</span>
						</li>
						<li class="flex items-center gap-2">
							<span class="font-bold text-primary">▹</span>
							<span>Docker, CI/CD</span>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</section>

	<!-- Projects Section -->
	<section id="projects" class="card bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Featured Projects
			</h2>
			<div class="space-y-6">
				<div class="border-l-4 border-primary pl-6">
					<h3 class="mb-2 text-2xl font-bold text-base-content">Fantasy Sports Draft Board</h3>
					<div class="mb-3 badge badge-outline badge-primary">
						Svelte • SvelteKit • Tailwind CSS • CI/CD
					</div>
					<p class="mb-4 text-base-content/70">
						Built a fantasy sports draft board application with real-time updates and seamless user
						experience.
					</p>
					<div class="flex flex-wrap gap-3">
						<a href="#live" class="btn btn-outline btn-primary">Live Demo</a>
						<a href="#github" class="btn btn-outline btn-primary">GitHub</a>
					</div>
				</div>

				<div class="border-l-4 border-primary pl-6">
					<h3 class="mb-2 text-2xl font-bold text-base-content">Daily Workout Logger</h3>
					<div class="mb-3 badge badge-outline badge-primary">
						Svelte • Python • PocketBase • FastAPI • Docker
					</div>
					<p class="mb-4 text-base-content/70">
						Developed a daily workout logging application with real-time data synchronization and
						personalized analytics.
					</p>
					<div class="flex flex-wrap gap-3">
						<a href="#live" class="btn btn-outline btn-primary">Live Demo</a>
						<a href="#github" class="btn btn-outline btn-primary">GitHub</a>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Experience Section -->
	<section id="experience" class="card bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Work Experience
			</h2>
			<div class="space-y-6">
				<div class="border-b border-base-300 pb-6 last:border-0">
					<div class="mb-1 text-lg font-semibold text-primary">Software Engineer</div>
					<h3 class="text-xl font-bold text-base-content">PrestoSports</h3>
					<div class="mb-3 text-sm text-base-content/60">August 2021 - November 2025</div>
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
	<section id="contact" class="card bg-base-100 shadow-xl">
		<div class="card-body">
			<h2 class="mb-6 card-title border-b-4 border-primary pb-2 text-3xl text-primary">
				Get In Touch
			</h2>
			<div class="grid grid-cols-2 gap-3 sm:flex sm:flex-wrap sm:justify-center sm:gap-4">
				<a href="mailto:your.email@example.com" class="btn btn-sm btn-primary sm:btn-md">Email</a>
				<a
					href="https://github.com/yourusername"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-sm btn-primary sm:btn-md">GitHub</a
				>
				<a
					href="https://linkedin.com/in/yourprofile"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-sm btn-primary sm:btn-md">LinkedIn</a
				>
				<a
					href="https://twitter.com/yourhandle"
					target="_blank"
					rel="noopener noreferrer"
					class="btn btn-sm btn-primary sm:btn-md">Twitter</a
				>
			</div>
		</div>
	</section>
</div>

<!-- Footer -->
<footer class="footer-center footer bg-base-200 p-10 text-base-content">
	<aside>
		<p class="font-semibold">&copy; 2026 Eddie Santos. All rights reserved.</p>
	</aside>
</footer>
