<script>
	const links = [{ id: 0, name: 'Study Pal', lead: './StudyPal' }];
</script>

<!-- :by Cristina Gottardi: https://images.unsplash.com/profile-1509140709644-5b9d6cd408f9?w=32&dpr=2&crop=faces&bg=%23fff&h=32&auto=format&fit=crop&q=60&ixlib=rb-4.0.3 -->

<div
	class="home relative grid h-screen w-screen grid-cols-12 grid-rows-12 gap-4 bg-[url('https://images.unsplash.com/photo-1522787345986-d5c7885a889e?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D')] bg-cover bg-center p-4"
	alt="Image of Pillars from Before created by Critstina Gottardi from Unsplash"
>
	<nav class="col-span-12 row-span-1 flex justify-between">
		<a href="/" aria-label="Home">Marici</a>

		<section>
			{#each links as link}
				<ul>
					<li class="underline">
						<a href={link.lead}>{link.name}</a>
					</li>
				</ul>
			{/each}
		</section>
	</nav>
	<article class="col-span-12 row-span-4 flex flex-col gap-2 text-center">
		<h1 class="text-6xl">
			Carving our path by Building the <span>Brighter</span> Future we always knew
		</h1>
		<p class="subtitle underline">Architects of a brandnew Realm</p>
		<p class="text-md m-auto w-2/3 rounded-sm bg-neutral-300/30 p-4 text-justify backdrop-blur-md">
			Together we may find lighter roads to travel. The future is ready to be built and we have
			every tool we need at our disposal. This is a place where you will realize your worth finding
			more reasons to explore this realm. Thank you.
		</p>
	</article>

	<form action="" method="post" class="col-span-12 row-span-1 text-center">
		<label for="email" class="block">Stay In tune to our TL</label>
		<input
			id="email"
			type="email"
			name="email"
			placeholder="Enter email"
			class="rounded-sm border border-blue-600 px-4 py-1"
		/>
		<input type="submit" value="submit" class="rounded-sm bg-yellow-500/60 px-4 py-2" />
	</form>
</div>

<style>
	* {
		color: midnightblue;
		font-family: 'reross-quadratic', sans-serif;
		font-weight: 400;
		font-style: normal;
	}

	h1 span {
		font-family: 'playwrite-cc-hr-lijeva', sans-serif;
		font-weight: 400;
		font-style: normal;
	}

	.subtitle {
		font-family: 'playwrite-cc-hr-lijeva', sans-serif;
		font-weight: 200;
		font-style: normal;
		font-size: 0.9em;
	}
</style>
