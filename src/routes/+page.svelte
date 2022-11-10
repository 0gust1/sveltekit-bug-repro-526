<script lang="ts">
	import { Editor, Viewer } from 'bytemd';
	import 'bytemd/dist/index.css';

	let editorContent = '# Hello';
	const handleChange = (event) => {
		editorContent = event.detail.value;
	};
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<p>ByteMD viewer component:</p>
<div class="box">
	<Viewer bind:value={editorContent} />
</div>

<p>ByteMD editor component:</p>
<div class="box">
	<Editor bind:value={editorContent} on:change={handleChange} />
</div>

<style>
	.box {
		border: 1px solid #555;
		padding: 2rem;
	}
</style>
