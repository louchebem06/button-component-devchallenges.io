<script lang="ts">
	import Button from "./Button.svelte";
</script>

<svelte:head>
	<title>Button Composante</title>
</svelte:head>

<div class="content">
<div class="right">
	<h1>Buttons</h1>

	<section>
		<div class="element">
			<p>{"<Button />"}</p>
			<Button />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{"<Button variant=\"outline\" />"}</p>
			<Button variant="outline" />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{'<Button variant="text" />'}</p>
			<Button variant="text" />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{'<Button disableShadow />'}</p>
			<Button disableShadow />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{'<Button disabled />'}</p>
			<Button disabled />
		</div>
		<div class="element">
			<p>{'<Button variant="text" disabled />'}</p>
			<Button variant="text" disabled />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{'<Button startIcon="local_grocery_store" />'}</p>
			<Button startIcon="local_grocery_store" />
		</div>
		<div class="element">
			<p>{'<Button endIcon="local_grocery_store" />'}</p>
			<Button endIcon="local_grocery_store" />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{'<Button size="sm" />'}</p>
			<Button size="sm" />
		</div>
		<div class="element">
			<p>{'<Button size="md" />'}</p>
			<Button size="md" />
		</div>
		<div class="element">
			<p>{'<Button size="lg" />'}</p>
			<Button size="lg" />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{'<Button color=”default” />'}</p>
			<Button color="default" />
		</div>
		<div class="element">
			<p>{'<Button color=”primary” />'}</p>
			<Button color="primary" />
		</div>
		<div class="element">
			<p>{'<Button color=”secondary” />'}</p>
			<Button color="secondary" value="Secondary" />
		</div>
		<div class="element">
			<p>{'<Button color=”danger” />'}</p>
			<Button color="danger" value="Danger" />
		</div>
	</section>

	<p>Icons: https://material.io/resources/icons/?style=round</p>
	<footer>
		<p>created by <bold><a href="http://github.bryanledda.fr">louchebem06</a></bold> - devChallenges.io</p>
	</footer>
</div>
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Ubuntu Mono:wght@400&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500&display=swap');

	* {
		margin: 0;
		padding: 0;
	}

	.content {
		display: flex;
		height: calc(100vh - 16px);
		gap: 80px;
	}

	h1 {
		font-family: 'Poppins';
		font-style: normal;
		font-weight: 500;
		font-size: 24px;
		line-height: 36px;
		color: #4F4F4F;
	}

	section {
		display: flex;
		gap: 10%;
		align-items: center;
	}

	.right {
		display: flex;
		flex-direction: column;
		gap: 33px;
		padding: 50px;
	}

	.element {
		min-width: 190px;
	}

	.element p {
		font-family: 'Ubuntu Mono';
		font-style: normal;
		font-weight: 400;
		font-size: 12px;
		line-height: 12px;
		color: #333333;
		margin-bottom: 8px;
	}

	p {
		font-family: 'Ubuntu Mono';
		font-style: normal;
		font-weight: 400;
		font-size: 12px;
		line-height: 12px;
		color: #828282;
	}

	footer {
		padding-bottom: 50px;
	}

	footer p, footer a {
		font-family: 'Montserrat';
		font-style: normal;
		font-weight: 500;
		font-size: 14px;
		line-height: 17px;
		color: #A9A9A9;
	}
</style>
