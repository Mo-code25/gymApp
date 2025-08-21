<script>
    import FaQs from "../components/FAQs.svelte";
    import Hero from "../components/Hero.svelte";
    import Product from "../components/Product.svelte";
    import Reviews from "../components/Reviews.svelte";
</script>

<!-- <h1 class="text-green-400">Welcome to SvelteKit</h1>
<p>
    Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the
    documentation
</p>

<h1 class="text-1xl font-bold underline">Hello world!</h1> -->

<main class="flex flex-col">
    <Hero />
    <Product />
    <Reviews />
    <FaQs />
</main>

<style lang="postcss">
    @reference "tailwindcss";
    :global(html) {
        background-color: theme(--color-gray-100);
    }
</style>
