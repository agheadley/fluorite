<script>
import { onMount } from 'svelte';
import { marked } from 'marked';
let text='';

onMount(async () => {
		

});

</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>


<div class="row">
	<div class="col">
		/Home
	</div>
</div>


<div class="row">
	      <div class="col">
	            <textarea style="height:20rem;" bind:value={text} />
	      </div>
	</div>
	
	<div class="row">
	      <div class="col">
	            {@html marked(text)}
	      </div>
	</div>




<style>

</style>
