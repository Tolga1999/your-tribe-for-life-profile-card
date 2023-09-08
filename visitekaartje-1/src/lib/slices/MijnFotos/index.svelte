<script>

	/** @type {import("@prismicio/client").Content.MijnFotosSlice} */
	export let slice;

	console.log(slice)
</script>

<section data-slice-type={slice.slice_type} data-slice-variation={slice.variation}>
	<h1>{slice?.primary.title[0].text}</h1>

	<img src={slice.primary.image.url} >
</section>

<style>
	img{
		width: 50%;
	}
</style>
