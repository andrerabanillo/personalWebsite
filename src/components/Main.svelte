<script>
    import Step from "./Step.svelte";

    let steps = [
        {name : 'Sportsbook Betting Line Analyzer', icon: 'fa-solid fa-users-between-lines'},
        {name: 'Discord Music Bot ', icon: 'fa-brands fa-discord'},
        {name: 'Joke Generator ', icon: ''}
    ]

</script> 

<main class = "flex flex-col flex-1 p-4">
    <section id = "introPage" class = "grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class = "flex flex-col lg:justify-center text center lg:text-left gap-6 md:gap-8 
        lg:gap-10">
            <h2 class = "font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class= "poppins text-violet-400"> Andre Rabanillo </span> <br>
                Computer Science @  <span class= "poppins text-violet-400"> <br>
                University of Guelph</span>
            </h2>
    
            <button
            class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
        >
            <div
                class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
            />
            <h4 class="relative z-9">Get in Touch With Me &rarr;</h4>
        </button>
    </div>
    </section>

    <section id = "projects" class = "py-20 lg:py-32 flex flex-col gap-24">
        <div class ="flex flex-col gap-2 text-center">
            <h6 class = "text-large sm:text-xl md:text-2xl">
                My Projects!
            </h6>
            <h3 class ="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class= "poppins text-violet-400"> See </span> my Work?
            </h3>

            <div class = "grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
                <Step steps={steps[0]}>

                </Step>
                <Step steps={steps[1]}>

                </Step>
                <Step step={steps[2]}>

                </Step>

               
        </div>
    </section>

</main>