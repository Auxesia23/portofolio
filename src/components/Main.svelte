<script>

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, cloud services and much much more.",
        },
        {
            name: "a backend enthusiast",
            description:
                "A passion for backend development and a growing interest in frontend technologies. I love building scalable, efficient systems and exploring the architecture that powers modern applications.",
        },
        {
            name: "full-stack explorer",
            description:
                "My focus is on backend technologies, but I enjoy working with frontend as well. I’m passionate about creating robust, efficient solutions and am constantly learning new tools and techniques..",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14 min-h-screen"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-blue-400">Fajar</span> Gustiana
               
            </h2>
            <h3 class="font-semibold text-3xl sm:text-5xl md:text-4xl">Informatics Engineering student</h3>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-blue-400"> favorite tech</span> includes Python + Django or FastAPI, JavaScript
                (SvelteKit) & PostgreSQL
                or MySQL
            </p>
            <a href="#footer"
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <!-- svelte-ignore element_invalid_self_closing_tag -->
                <div
                    class="absolute top-0 right-full w-full h-full bg-blue-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
        </a>
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24 min-h-screen" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my projects.
            </h6>   
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <!-- svelte-ignore a11y_invalid_attribute -->
            <a
                href="#"
                target="_blank"
                class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-violet-700 text-center cursor-pointer group hover:border-violet-400 duration-200"
            >
                <div
                    class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200"
                >
                    <!-- svelte-ignore element_invalid_self_closing_tag -->
                    <i class="fa fa-user"/>
                </div>
                <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
                    Persolan Website
                </h3>
                <p>This website serves as my portfolio, showcasing my journey in Informatics Engineering. Built with SvelteKit,
                     it highlights my skills, projects, and a bit of frontend work to demonstrate a well-rounded approach to web development.
                </p>
                <div class="flex-1 flex justify-betweeen gap-4 items-end">
                    <div
                        class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:top-0 after:h-0 after:right-full after:bg-white after:w-full after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden"
                    >
                        <p class="z-4">Go to &rarr;</p>
                    </div>
                </div>
            </a>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-blue-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-blue-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-blue-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
    </section>
</main>