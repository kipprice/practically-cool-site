{#snippet comingSoon()}
	<div class="pointer-events-none text-xs opacity-0">Coming Soon</div>
	<div
		class="absolute top-[calc(100%-1.8rem)] left-[calc(100%-6rem)] rounded-md bg-amber-400 px-2 py-1 text-xs whitespace-nowrap text-black"
	>
		Coming Soon
	</div>
{/snippet}

<div class="rootContainer">
	<h1>Practically Cool</h1>
	<p>
		A collection of interesting things created by <a
			href="https://kipprice.dev"
			class="font-semibold underline">Kip Price</a
		>
	</p>

	<div class="flex min-h-0 flex-grow flex-col overflow-x-visible overflow-y-auto px-6">
		<h2 class="stickyHeader">Apps</h2>
		<div class="mt-4 grid w-full grow grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3">
			<a class="card text-[#136F63]" href="https://mossyvibes.com">
				<img
					src="/mossy-vibes.png"
					alt="screenshot of Mossy Vobes, a reading based meditation app"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">Mossy Vibes</h3>
				<p>Meditation for busy people</p>
			</a>
			<a class="card text-[#000]" href="https://spindle.practically.cool">
				<img src="/spindle.png" alt="screenshot of Spindle" class="max-w-72 rounded-md" />
				<h3 class="cardTitle">Spindle Campaign Manager</h3>
				<p>Run TTRPG games using the Spindle framework</p>
			</a>
			<a class="card text-[#000]" href="https://hf.practically.cool">
				<img
					src="/hocus-focus.png"
					alt="screenshot of hocus focus, a dynamic music generator"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">hocus focus</h3>
				<p>loop mixer and editor with a little bit of magic</p>
			</a>
			<a class="card text-rose-800" href="https://monochromatic.app">
				<img
					src="/monochrome.png"
					alt="screenshot of monochrome, a digital murder mystery game"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">Monochrome</h3>
				<p>Mobile mystery night</p>
			</a>

			<a class="card text-[#116A91]" href="https://bookdrop.io">
				<img
					src="/book-drop.png"
					alt="screenshot of Book Drop, a library-management tool for books and more"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">Book Drop</h3>
				<p>Organize your library</p>
			</a>
			<a class="card text-[#324472]" href="https://ummm.kipprice.com">
				<img
					src="/ummm.png"
					alt="screenshot of Ummm, a visual UML editor that can generate code"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">Ummm</h3>
				<p>Generate code from UML</p>
			</a>
			<a class="card text-[#D65108]" href="https://tv-roulette.netlify.app">
				<img
					src="/tv-roulette.png"
					alt="screenshot of TV Roulette, a tool that can suggest a random episode to watch"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">TV Roulette</h3>
				<p>Random episode suggester</p>
			</a>
			<a class="card text-[#3A10E5]" href="https://github.com/kipprice/github-search-extension">
				<img
					src="/gh-search.png"
					alt="screenshot of GitHub Search, a Chrome extension that allows you to search GitHub"
					class="max-h-48 rounded-md"
				/>
				<h3 class="cardTitle">GitHub Search</h3>
				<p>Find a PR anywhere</p>
			</a>
		</div>

		<h2 class="stickyHeader">Libraries</h2>
		<div class="mt-4 grid w-full grow grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3">
			<a class="card text-[#313D5A]" href="https://kipprice.github.io/flow-md/">
				<img
					src="/flow-md.png"
					alt="screenshot of Flow MD, a library that can convert markdown into flow charts"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">Flow MD</h3>
				<p>Build dynamic flows in React</p>
			</a>
			<a class="card text-[#10162F]" href="https://kipprice.github.io/markdown-matrix/">
				<img
					src="/markdown-matrix.png"
					alt="screenshot of Markdown to Matrix, a library that can convert markdown into interactive matrices"
					class="max-w-72 rounded-md"
				/>
				<h3 class="cardTitle">Markdown to Matrix</h3>
				<p>Build interactable matrices with Markdown</p>
			</a>
			<a class="card" href="https://github.com/kipprice/toolkip_module">
				<h3 class="cardTitle">Toolkip</h3>
				<p>Collection of various tools and helpers in typescript</p>
			</a>
		</div>

		<h2 class="stickyHeader">Underway</h2>
		<div class="mt-4 grid w-full grow grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-3">
			<div class="card text-[oklch(0.85_0.1378_182.15)]">
				<h3 class="cardTitle">Pizzazzium</h3>
				<p>Coordinate classes and lessons</p>
				{@render comingSoon()}
			</div>
		</div>
	</div>
</div>

<style>
	.rootContainer {
		display: flex;
		flex-direction: column;
		background-color: white;
		height: 100vh;
		width: 100vw;
		padding: 2rem;
		align-items: center;
		color: black;
		overflow: hidden;
	}

	h1 {
		font-size: 2rem;
		font-weight: 700;
	}

	h2 {
		font-size: 1.5rem;
		font-weight: 700;
	}

	.card {
		background-color: white;
		border: 1px solid black;
		border-radius: 4px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;
		padding: 1rem;
		cursor: pointer;
		position: relative;

		transition: all 0.1s ease-in-out;
	}

	.card * {
		color: black;
	}

	.card:hover {
		margin-left: -4px;
		margin-right: 4px;
		margin-top: -4px;
		margin-bottom: 4px;

		box-shadow: 4px 4px 0 0 currentColor;
	}

	.cardTitle {
		font-weight: 700;
		font-size: 1.3rem;
	}

	.stickyHeader {
		position: sticky;
		top: 0;
		z-index: 10;
		background-color: rgba(255, 255, 255, 0.9);
	}
</style>
