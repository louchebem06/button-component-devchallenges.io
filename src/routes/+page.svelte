<script lang="ts">
	import Button from "./Button.svelte";
</script>

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
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Ubuntu Mono:wght@400&display=swap');

	* {
		margin: 0;
		padding: 0;
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
</style>
