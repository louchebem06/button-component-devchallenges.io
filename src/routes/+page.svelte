<script lang="ts">
	import Button from "./Button.svelte";
</script>
<div class="content">
<div class="left">
	Wesh la zone
</div>
<div class="right">
	<h1>Buttons</h1>

	<section>
		<div class="element">
			<p>{"<Button />"}</p>
			<Button />
		</div>
		<div class="element">
			<p>&:hover, &:focus</p>
			<Button />
		</div>
	</section>

	<section>
		<div class="element">
			<p>{"<Button variant=\"outline\" />"}</p>
			<Button variant="outline" />
		</div>
		<div class="element">
			<p>&:hover, &:focus</p>
			<Button variant="outline" />
		</div>
	</section>

	<section>
		<Button variant="text" />
		<Button variant="text" />
	</section>

	<section>
		<Button disableShadow />
	</section>

	<section>
		<Button disabled />
		<Button variant="text" disabled />
	</section>

	<section>
		<Button startIcon="local_grocery_store" />
		<Button endIcon="local_grocery_store" />
	</section>

	<section>
		<Button size="sm" />
		<Button size="md" />
		<Button size="lg" />
	</section>

	<section>
		<Button color="default" />
		<Button color="primary" />
		<Button color="secondary" value="Secondary" />
		<Button color="danger" value="Danger" />
	</section>

	<section>
		<Button color="default" />
		<Button color="primary" />
		<Button color="secondary" value="Secondary" />
		<Button color="danger" value="Danger" />
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

	.left {
		padding: 50px;
		background: #FAFBFD;
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
