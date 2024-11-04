<script>
    import Step from "./Step.svelte";

    let steps = [
        {
           
        },
        {
            
        },
        {
           
        },
    ];

    let benefits = [
        
        {
            name: "UI/UX Design ",
            description:
                "Computer science student specializing in UI/UX design, passionate about creating intuitive, user-centered digital experiences. Skilled in wireframing, prototyping, and user research, with a strong eye for detail and a commitment to seamless, functional design.",
        },
        {
            name: "Creativity",
            description:
                "As a computer science student, I thrive on creativity, using it to craft innovative solutions and engaging digital experiences. I enjoy blending technical skills with imaginative thinking to design user-centered interfaces that are both functional and inspiring. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-white-400">Carmi Wilna</span> Tongson
                <br />
                <span class="poppins text-red-400">3rd year BSCS Student</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
               <span class="text-blue-500"> </span>
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-red-500 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/ming.png"}
                alt=""
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
               
            </h6>
        </div>
        
    </section>
    <section
    id="about"
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
>
    <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
    <div
        class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-red-500 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
        <h6 class="text-large sm:text-xl md:text-2xl">
           To know more
        </h6>
        <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
             <span class="poppins text-red-500">about</span> me.
        </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
        I'm 
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
        {#each benefits as benefit, index}
            <div class="flex gap-6 sm:gap-8">
                <p
                    class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-00 font-semibold"
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
    <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
        <span class="text-red-500">About Me</span> 
    </h5>
    <div>
        <p class="mx-auto">Hi Im Carmi Wilna Tongson, I am a Bachelor of Science in Computer Science (BSCS) student specializing in UI/UX design. With a passion for creating intuitive and engaging user experiences, I thrive on the intersection of technology and design. I enjoy collaborating on projects that challenge my creativity and technical skills. In my free time, I explore emerging trends in technology and design, continuously seeking ways to improve my craft and stay ahead in the field.</p>
    </div>
    <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
        <p></p>
    </div>
    <p class="mx-auto"></p>
</section>
</main>