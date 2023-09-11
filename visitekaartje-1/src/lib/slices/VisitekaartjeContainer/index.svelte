<script>
	/** @type {import("@prismicio/client").Content.MijnFotosSlice} */
	export let slice;

	console.log(slice);
</script>

<section data-slice-type={slice.slice_type} data-slice-variation={slice.variation}>
	<!-- <img src={slice.primary.profileImage.url} alt="" /> -->

	<h1>{slice.primary.nameTitle}</h1>

	<section class="style-container">
		<h2>{slice.primary.experienceTitle}</h2>
		<p>{slice.primary.experienceContent}</p>

		<h2>{slice.primary.aboutTitle}</h2>
		<p>{slice.primary.aboutContent}</p>

		<div class="center-container">
			<button>Follow on Github</button>
		</div>

	</section>


</section>

<style>
	:global(body){
		min-height: 100vh;
		width: 100%;
		background-size: cover;
		background-position: center;
		background-image: url(https://images.prismic.io/visitekaartje-1/cf4ce052-9d21-4257-86c9-1e7388a0cbab_patrickBateman.png?auto=compress,format);
	}

	h1 {
		margin: 0.5em 0;
		padding: 0 0 0.25em 0.5em;
		font-size: 2.25em;
		font-weight: 800;
	}

	.style-container{
		background-color: rgba(159, 159, 159, 0.5);
		padding: 2em;
		backdrop-filter: blur(10px);
		border-radius: 20px 20px 0 0;
	}

	h2 {
		font-size: 1.25em;
		font-weight: 700;
		margin-bottom: 0;
	}

	h2:nth-child(1){
		margin-top: 0;
	}

	h2:nth-child(3){
		margin-top: 1.5em;
	}

	p {
		margin-top: 0.5em;
		font-size: 1em;
		font-weight: 400;
	}

	/* img {
		height: 60vh;
		max-width: 100%;
		object-fit: cover;
	} */

	.center-container{
		display: flex;
		justify-content: center;
	}

	button{
		background-color: rgba(255, 255, 255, 0.4);
		font-size: 1em;
		font-weight: 700;
		color: white;
		padding: 0.9em 3em;
		border: none;
		border-radius: 20px;
		margin-top: 1.25em;
	}


</style>
