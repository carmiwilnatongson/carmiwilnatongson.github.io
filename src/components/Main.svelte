<script>    
    import Step from "./Step.svelte";
    import Exp from "./Exp.svelte";

    let steps = [
        {name:'Facebook', icon:'fa-solid fa-palette', link:"https://www.facebook.com/carmiwilna.tongson"}, 
        {name:'Phone Number', icon:'fa-solid fa-scroll ', link:"rghs"},
        {name:'Instagram', icon:'fa-solid fa-terminal', link:"https://www.ig.com"},
        {name:'GitHub', icon:'fa-brands fa-github', link:"carmiwilnatongson"},
    ];    
    
    let experiences = [
        {}, 
        {},
        {},
        {},
        {},
        {},
        {},
        {},
        {},
        
    ];

    let benefits = [
        {name:'3rdyear BSCS Student', description: 'Computer science student with a passion for problem-solving and innovation. Skilled in coding, data analysis, and eager to apply technical knowledge to real-world challenges. Thrives in collaborative settings and committed to continuous learning.'}, 
        {name:'A UI/UX Enthusiast', description: 'Computer science student specializing in UI/UX design, passionate about creating intuitive, user-centered digital experiences. Skilled in wireframing, prototyping, and user research, with a strong eye for detail and a commitment to seamless, functional design.'},
        {name:'Creativity', description: 'As a computer science student, I thrive on creativity, using it to craft innovative solutions and engaging digital experiences. I enjoy blending technical skills with imaginative thinking to design user-centered interfaces that are both functional and inspiring.'},
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8
        lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl text-orange-100">
                Hi! I'm <span class="poppins text-violet-400">Carmi Wilna</span> Tongson <br/>Computer Science
                <span class="poppins text-violet-400">Student</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                Dedicated <span class="text-violet-400"> BSCS </span> 
                student passionate about technology and programming,
                eager to create innovative solutions and enhance user experiences through design.
            </p>
            <a href="mailto:guhan.delta@gmail.com" class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins
            relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" target="_blank">
                <h4 class="relative z-9">Get in Touch &rarr;</h4>
            </a>
        </div>
        <div class="relative grid place-items-center shadow-2xl">
            <img src={"images/ming.png"} alt="Me" class="object-cover z-[2] max-h-[70vh]" />
        </div>
    </section>

    <section id="experience" class="py-20 lg:py-32 flex flex-col gap-24">
    </section>
    <hr class="">
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        
        <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
           My <span class="poppins text-violet-400">Contacts</span> & Social Media
            
        </h3>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p class="">Carmi Wilna Tongson </p>
                <strong class="text-violet-400"></strong>
            </Step>
            <Step step={steps[1]}>
                <p class="">09085565409</p>
                <strong class="text-violet-400"></strong>
            </Step>
            <Step step={steps[2]}>
                <p class="">wiln_01</p>
                <strong class="text-violet-400"></strong>
            </Step>
        </div>
        <Step step={steps[3]}>
            <p class="">GitHub</p>
            <strong class="text-violet-400"></strong>
        </Step>
    </section>
    <section id="about" class="relative flex flex-col pt-10 py-20 lg:pt-16 lg:py-32 gap-16 sm:gap-24 md:gap-24">

    <div
        class="flex flex-col gap-2 text-center relative before:absolute before:top-0
        before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute
        after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
        <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
        <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
            A bit <span class="poppins text-violet-400">about</span> me.
        </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am . . .</p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w- [800px]">
        {#each benefits as benefit, index}
            <div class="flex gap-6 sm:gap-8">
                <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">0{index+1}</p>
                <div class="flex flex-col gap-6 sm:gap-8">
                    <h3 class="text-2xl sm:text-2xl md:text-5xl">{benefit.name}</h3>
                    <p class="">{benefit.description}</p>
                </div>
            </div>
        {/each}
    </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
    </section>
</main>