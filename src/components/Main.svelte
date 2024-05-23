<script>
    import Page from "../routes/+page.svelte";
    import { base } from "$app/paths";
    import Step from "./Step.svelte";

    let steps = [
        {
            href: 'https://github.com/your-repo/pterocli',
            icon: 'fa-solid fa-terminal',  // Replace with the actual icon class
            name: 'pterocli',
            image: 'images/pterocli-screen.webp'  // Replace with the actual image URL
        },
        {
            href: 'https://github.com/your-repo/pvpflag',
            icon: 'fa-solid fa-skull',  // Replace with the actual icon class
            name: 'pvpflag',
            image: 'images/pvpflag-screen.webp'  // Replace with the actual image URL
        }
    ];
    let benefits = [
        {name: 'love for ML', description: 'I like Machine Learning, anything related to it. including but not limted to math behind it. obviously CI/CD processes for ML are the sweet spot for me. in terms of experience sadly I did not have a chance to work with ML in production yet'},
        {name: 'prefer backend', description: "if we talking developing I like backend and critical mission developing. you know, making sure nothing ever fails, databases, premature optimization is my guilty pleasure (when I'm allowed to do it)"},
        {name: 'GAMIN', description: "yeah... I'm a gamer...... (sorry) I do dip my toes in gamedev if that wasn't clear just yet. not only developing but general gamedev processes as well as DevOps side of things. collecting a ton of data in a big game through telemetry is my dream"}
        //{name: "Computer Security degree ", description: "so there is that I guess"}
    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                hey I'm <span class="fira text-violet-400">rkkm</span>_ I do, uh <span class="fira text-violet-400">DevOps</span> stuff, yes hello hi
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                Kinds of stuff related to <span class="fira text-violet-400">Linux, containerization, k8s, CI/CD</span>
                  and also weirdly enough <span class="fira text-violet-400">Minecraft</span>. Oh! And some <span class="fira text-violet-400">Java, Kotlin</span> on the side
            </p>
            <a 
            class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl fira relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            href="{base}/contacts"
            target="_self">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200" />
                <h4 class="relative z-9">send me a message &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src={"images/avatar1.webp"} alt="my many avatars you probably saw" class="object-cover z-[2] max-h-[70vh]">
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                anyway here is some of my least emberassing <span class="fira text-violet-400">Open Source</span> works (this is prob still at one link sorry)
            </h6>
        </div>
        
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>pterocli is CLI interface for game server orchestration software <strong class="text-violet-400">Pterodactyl</strong>.
                    it's written in <strong class="text-violet-400">Kotlin and uses GraalVM dark magic</strong> to make it build nativly. pretty cool</p>
            </Step>
            <Step step={steps[1]}>
                <p>pvpflag is a simple <strong class="text-violet-400">Minecraft</strong> mod written in <strong class="text-violet-400">Java</strong> using <strong class="text-violet-400">Fabric API</strong>.
                    just something I made to play with friends on my server. nothing groundbreaking, but I'm still proud of how simple it is.
            </Step>
        </div>
    </section>
    <!-- <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">still need to know more? </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                here is some stuff <span class="fira text-violet-400">about</span> me
            </h3>
        </div>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index} -->
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
                <!-- <div class="flex gap-6 sm:gap-8">
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
        </div> -->

    
  <section>
    <div class="flex flex-col gap-2 text-center items-center">
      <h6 class="text-lg sm:text-xl md:text-2xl">
        well this is more of a shitpost than a proper personal website so you might be intrested in my actual <span class="fira text-violet-400">CV</span> so here you go
      </h6>
      <a
        class="blueShadow text-base sm:text-lg md:text-xl fira relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 mt-2"
        href="{base}/cv"
        target="_self"
      >
        <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"></div>
        <h4 class="relative z-9">curriculum vitae &darr;</h4>
      </a>
    </div>
  </section>
    
</main>