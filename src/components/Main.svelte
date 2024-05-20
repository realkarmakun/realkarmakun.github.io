<script>
    import Page from "../routes/+page.svelte";
    import Step from "./Step.svelte";

    
    let steps = [
        {name: "pterocli", icon: "fa-brands fa-github"}
    ]
    let benefits = [
        {name: 'a Computer Security degree', description: 'yes, really. I studied at Dostoevsky Omsk State University and after 5 and half years I finished my studies (this is just how some degrees in Russia work)'}
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
            href="/contacts"
            target="_blank">
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
        </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">still need to know more? </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                here is some stuff <span class="fira text-violet-400">about</span> me
            </h3>
        </div>

    </section>
    <section>
    
</main>