<script>
	import { onMount } from "svelte";
	let PdfViewer;
  
	onMount(async () => {
	  const module = await import("svelte-pdf");
	  PdfViewer = module.default;
	});
</script>
  
<svelte:component this={PdfViewer} url="./src/routes/constitution/constitution.pdf"/>

