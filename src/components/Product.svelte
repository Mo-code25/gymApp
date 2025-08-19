<script>
    import SectionWrapper from "./SectionWrapper.svelte";
    let productFeatures = [
        {
            featureList: [
                "Daily streak Counter",
                "Weights and reps tracker",
                "Community challenges",
            ],
            description:
                "Swoley moley ensures all users have the information they need to train safely and train effectively",
            imageUrl: [],
        },
        {
            featureList: [
                "Select your preferences",
                "Personalize your workouts",
                "Customize your training",
                "Gurantees progress on all your exercises",
            ],
            description:
                "Build you streaks and see your progress with your amazing tracking and analytics features",
            imageUrl: [],
        },
        {
            featureList: [
                "Elimainating guesswork",
                "Save time",
                "Load your own models",
                "Achievr the performancr you seek",
                "Builds functional strength",
            ],
            description:
                "Enter as much information about yourself as you desire to ensure all workouts are personalizes to your every need",
            imageUrl: [],
        },
    ];
</script>

<SectionWrapper id="project">
    <div
        class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:pb-24"
    >
        <div class="flex flex-col gap-2">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                Start your lifetime <span class="text-indigo-400">
                    gym streak
                </span> today
            </p>
            <h3
                class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
            >
                Features for everyone
            </h3>
        </div>
        {#each productFeatures as productFeature, index}
            <productCard {productFeature} {index}>
                {#if index === 0}
                    Experience a beginner exercise <span
                        class="text-indigo-400 font-medium">master</span
                    > class
                {:else if index === 1}
                    Lay the foundations for <span
                        class="text-indigo-400 font-medium">routine</span
                    > and consistency
                {:else}
                    Workouts specific to your <span
                        class="text-indigo-400 font-medium">enviroment</span
                    >
                    and
                    <span class="text-indigo-400 font-medium">expertise</span>
                {/if}
            </productCard>
        {/each}
    </div>
</SectionWrapper>
