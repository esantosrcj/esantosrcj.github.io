<svelte:head>
	<title>Eddie Santos - Software Engineer</title>
	<meta name="description" content="Senior Software Engineer with 9+ years of expertise in building scalable web applications and distributed systems." />
</svelte:head>

<header>
	<h1>Eddie Santos</h1>
	<p>Senior Software Engineer</p>
</header>

<nav>
	<ul>
		<li><a href="#about">About</a></li>
		<li><a href="#skills">Skills</a></li>
		<li><a href="#projects">Projects</a></li>
		<li><a href="#experience">Experience</a></li>
		<li><a href="#contact">Contact</a></li>
	</ul>
</nav>

<div class="container">
	<section id="about">
		<h2>About Me</h2>
		<p>Experienced software engineer with 9+ years of expertise in building scalable web applications and distributed systems. Passionate about clean code, system design, and mentoring junior developers. Proven track record of delivering high-impact solutions in fast-paced environments.</p>
		<p>Currently focusing on cloud-native architectures, microservices, and DevOps practices. Always eager to learn new technologies and solve complex problems.</p>
	</section>

	<section id="skills">
		<h2>Technical Skills</h2>
		<div class="skills">
			<div class="skill-category">
				<h3>Languages</h3>
				<ul>
					<li>JavaScript/TypeScript</li>
					<li>Python</li>
					<li>Java</li>
					<li>SQL</li>
				</ul>
			</div>
			<div class="skill-category">
				<h3>Frontend</h3>
				<ul>
					<li>React, Svelte</li>
					<li>Next.js, SvelteKit</li>
					<li>HTML/CSS</li>
					<li>Tailwind CSS</li>
				</ul>
			</div>
			<div class="skill-category">
				<h3>Backend</h3>
				<ul>
					<li>Node.js, Express</li>
					<li>FastAPI, Flask</li>
					<li>Spring Boot</li>
					<li>REST APIs</li>
				</ul>
			</div>
			<div class="skill-category">
				<h3>Database & Cloud</h3>
				<ul>
					<li>PostgreSQL, MySQL, MongoDB</li>
					<li>Redis</li>
					<li>AWS, Google Cloud</li>
					<li>Docker, CI/CD</li>
				</ul>
			</div>
		</div>
	</section>

	<section id="projects">
		<h2>Featured Projects</h2>
		<div class="projects">
			<div class="project">
				<h3>Fantasy Sports Draft Board</h3>
				<div class="tech-stack">Svelte • SvelteKit • Tailwind CSS • CI/CD</div>
				<p>Built a fantasy sports draft board application with real-time updates and seamless user experience.</p>
				<div class="project-links">
					<a href="#live">Live Demo</a>
					<a href="#github">GitHub</a>
				</div>
			</div>

			<div class="project">
				<h3>Daily Workout Logger</h3>
				<div class="tech-stack">Svelte • Python • PocketBase • FastAPI • Docker</div>
				<p>Developed a daily workout logging application with real-time data synchronization and personalized analytics.</p>
				<div class="project-links">
					<a href="#live">Live Demo</a>
					<a href="#github">GitHub</a>
				</div>
			</div>
		</div>
	</section>

	<section id="experience">
		<h2>Work Experience</h2>
		
		<div class="experience-item">
			<div class="role">Software Engineer</div>
			<h3>PrestoSports</h3>
			<div class="duration">August 2021 - November 2025</div>
			<ul>
				<li>Led full-stack development for key features, enhancing user engagement and system performance</li>
			</ul>
		</div>
	</section>

	<section id="contact">
		<h2>Get In Touch</h2>
		<div class="contact">
			<a href="mailto:your.email@example.com">Email</a>
			<a href="https://github.com/yourusername" target="_blank" rel="noopener noreferrer">GitHub</a>
			<a href="https://linkedin.com/in/yourprofile" target="_blank" rel="noopener noreferrer">LinkedIn</a>
			<a href="https://twitter.com/yourhandle" target="_blank" rel="noopener noreferrer">Twitter</a>
		</div>
	</section>
</div>

<footer>
	<p>&copy; 2026 Eddie Santos. All rights reserved.</p>
</footer>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
		line-height: 1.6;
		color: #333;
		background: #f5f5f5;
	}

	header {
		background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
		color: white;
		padding: 4rem 2rem;
		text-align: center;
	}

	header h1 {
		font-size: 2.5rem;
		margin-bottom: 0.5rem;
	}

	header p {
		font-size: 1.2rem;
		opacity: 0.9;
	}

	nav {
		background: white;
		padding: 1rem 2rem;
		box-shadow: 0 2px 4px rgba(0,0,0,0.1);
		position: sticky;
		top: 0;
		z-index: 100;
	}

	nav ul {
		list-style: none;
		display: flex;
		justify-content: center;
		gap: 2rem;
		flex-wrap: wrap;
		margin: 0;
		padding: 0;
	}

	nav a {
		color: #667eea;
		text-decoration: none;
		font-weight: 500;
		transition: color 0.3s;
	}

	nav a:hover {
		color: #764ba2;
	}

	.container {
		max-width: 1100px;
		margin: 0 auto;
		padding: 3rem 2rem;
	}

	section {
		background: white;
		margin-bottom: 2rem;
		padding: 2.5rem;
		border-radius: 8px;
		box-shadow: 0 2px 8px rgba(0,0,0,0.1);
	}

	h2 {
		color: #667eea;
		margin-bottom: 1.5rem;
		font-size: 2rem;
		border-bottom: 3px solid #667eea;
		padding-bottom: 0.5rem;
	}

	.skills {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
		gap: 1.5rem;
	}

	.skill-category h3 {
		color: #764ba2;
		margin-bottom: 0.8rem;
		font-size: 1.2rem;
	}

	.skill-category ul {
		list-style: none;
		padding: 0;
		margin: 0;
	}

	.skill-category li {
		padding: 0.4rem 0;
		padding-left: 1.5rem;
		position: relative;
	}

	.skill-category li:before {
		content: "▹";
		position: absolute;
		left: 0;
		color: #667eea;
		font-weight: bold;
	}

	.projects {
		display: grid;
		gap: 2rem;
	}

	.project {
		border-left: 4px solid #667eea;
		padding-left: 1.5rem;
	}

	.project h3 {
		color: #333;
		margin-bottom: 0.5rem;
		font-size: 1.4rem;
	}

	.project .tech-stack {
		color: #667eea;
		font-size: 0.9rem;
		margin-bottom: 0.8rem;
		font-weight: 500;
	}

	.project p {
		margin-bottom: 0.8rem;
		color: #555;
	}

	.project-links {
		display: flex;
		gap: 1rem;
		margin-top: 1rem;
	}

	.project-links a {
		color: #667eea;
		text-decoration: none;
		font-weight: 500;
		padding: 0.5rem 1rem;
		border: 2px solid #667eea;
		border-radius: 4px;
		transition: all 0.3s;
	}

	.project-links a:hover {
		background: #667eea;
		color: white;
	}

	.experience-item {
		margin-bottom: 2rem;
		padding-bottom: 2rem;
		border-bottom: 1px solid #eee;
	}

	.experience-item:last-child {
		border-bottom: none;
		margin-bottom: 0;
		padding-bottom: 0;
	}

	.experience-item h3 {
		color: #333;
		font-size: 1.3rem;
	}

	.experience-item .role {
		color: #667eea;
		font-weight: 600;
		margin-bottom: 0.3rem;
	}

	.experience-item .duration {
		color: #888;
		font-size: 0.9rem;
		margin-bottom: 1rem;
	}

	.experience-item ul {
		margin-left: 1.5rem;
	}

	.experience-item li {
		margin-bottom: 0.5rem;
		color: #555;
	}

	.contact {
		display: flex;
		justify-content: center;
		gap: 2rem;
		flex-wrap: wrap;
	}

	.contact a {
		color: #667eea;
		text-decoration: none;
		font-size: 1.1rem;
		transition: color 0.3s;
	}

	.contact a:hover {
		color: #764ba2;
	}

	footer {
		text-align: center;
		padding: 2rem;
		color: #888;
		background: white;
	}

	@media (max-width: 768px) {
		header h1 {
			font-size: 2rem;
		}

		nav ul {
			gap: 1rem;
		}

		section {
			padding: 1.5rem;
		}
	}
</style>
