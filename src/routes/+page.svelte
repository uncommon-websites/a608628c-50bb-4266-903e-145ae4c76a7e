<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import Project from "$lib/components/Project.svelte";

	const projects = [
		{
			title: "SSS Showhouse",
			src: "https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?q=80&w=2000&auto=format&fit=crop", // Living room fireplace
			alt: "Minimal living room with fireplace"
		},
		{
			title: "Palm Beach Spanish Revival",
			src: "https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?q=80&w=2000&auto=format&fit=crop", // High ceiling living room
			alt: "Spanish revival living room"
		},
		{
			title: "Mulberry Modern",
			src: "https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?q=80&w=2000&auto=format&fit=crop", // Kitchen dining
			alt: "Modern kitchen with dining booth"
		},
		{
			title: "Furniture",
			src: "https://images.unsplash.com/photo-1596162954151-cd676000b3b8?q=80&w=2000&auto=format&fit=crop", // Furniture
			alt: "Geometric furniture pieces"
		},
		{
			title: "Woodland Post-Modern",
			src: "https://images.unsplash.com/photo-1600607687644-c7171b42498f?q=80&w=2000&auto=format&fit=crop", // Curved sofa
			alt: "Post-modern living space"
		},
		{
			title: "Woodland Bath",
			src: "https://images.unsplash.com/photo-1584622050111-993a426fbf0a?q=80&w=2000&auto=format&fit=crop", // Bathroom
			alt: "Bathroom with checkered tiles"
		},
		{
			title: "Moore's Mid-Century",
			src: "https://images.unsplash.com/photo-1600585154340-be6161a56a0c?q=80&w=2000&auto=format&fit=crop", // Kitchen marble
			alt: "Mid-century modern kitchen"
		}
	];
</script>

<Header />

<main class="w-full bg-[#F2F0EB]">
	{#each projects as project}
		<Project {...project} />
	{/each}
</main>


