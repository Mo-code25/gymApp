<script>
    export let dark;
</script>

<div class="flex items-center gap-4">
    <button
        class={"specialBtn " +
            (dark ? "bg-white text-[#181b34] border border-transparent" : " ")}
    >
        <p class="textbase sm:text-lg md:text-xl">Contact Us</p>
    </button>

    <button class="specialBtnDark">
        <p class="text-base sm:text-lg md:text-xl">Get Started &rarr;</p>
    </button>
</div>


