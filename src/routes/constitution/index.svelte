<script>
	import { onMount } from "svelte";
	let PdfViewer;
  
	onMount(async () => {
	  const module = await import("svelte-pdf");
	  PdfViewer = module.default;
	});
</script>
  
<svelte:component this={PdfViewer} src="./constitution.pdf"/>
<iframe><a href="/"><img id="logo" alt="league logo" src="./badge.png" /></a></iframe>

