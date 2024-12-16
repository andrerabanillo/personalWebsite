<script>
    import Step from "./Step.svelte";
  
    let steps = [
      {
        name: "Sportsbook Betting Line Analyzer",
        icon: "fa-solid fa-users-between-lines",
        description:
          "Utilizes the Odds API to access the betting lines for each major sportsbook worldwide, giving users the ability to compare lines and secure profit.",
      },
      {
        name: "Discord Music Bot",
        icon: "fa-brands fa-discord",
        description:
          "Created a discord bot that enables Discord participants in a voice chat to play audio from a YouTube video.",
      },
      {
        name: "Joke Generator",
        icon: "fa-regular fa-face-laugh",
        description:
          "Utilizes an api-ninjas API to generate a joke and display them on an html webpage.",
      },
      {
        name: "Baseball Reference Web Scraper",
        icon: "fa-solid fa-baseball",
        description:
          "A weather application that provides real-time weather data using the OpenWeather API.",
      },
    ];

    let benefits = [
       
        {
            name: "Minoring in Project Management ",
            description:
                "My project management minor has given me valuable abilities in project planning, execution, and supervision. Choosing the minor has been highly beneficial, as it has given me a strong foundation in project management principles, allowing me to successfully coordinate activities, manage resources, and ensure success - especially within a group environment.",
        },

        {
            metric: "10x",
            name: "Experience in the Industrial Distribution Workplace",
               
            description:  "As a Logistics Associate at RotoPrecision Inc. in Mississauga, Ontario, I am tasked with a wide variety of jobs such as receiving, counting, and organizing items, handling customer orders, and providing support during annual inventory. Because of this, I'm more than happy to take on any task that is given to me -and complete it precisely and efficiently. ",
                
        },
      
    ];

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
  
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my projects.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
  
      <div style="display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 40px; ">
        {#each steps as step}
          <Step {step}>
            <p class = "text-base">
                {#if step.name === "Sportsbook Betting Line Analyzer"}
                Utilizes <span class="poppins text-violet-400"> the Odds API </span>to access the betting lines for each major sportsbook worldwide, giving users the ability to compare lines and secure profit. 
                Proves further well with the arbitrage betting strategy. 
                    <p class="justify-end">
                        <a href="https://github.com/sebastiankula/historicalSportsbookAnalyzer" target="_blank" rel="">
                            Go to &rarr; 
                        </a>
                    </p>
                {/if}
                {#if step.name === "Discord Music Bot"}
                Utilizes the <span class="poppins text-violet-400"> youtube.dll, FFmpeg and asyncio</span> frameworks to create discord bot that enables Discord participants in a voice chat to play audio from a YouTube video.
                    <p class="justify-end">
                        <a href="https://github.com/andrerabanillo/discordMusicBot" target="_blank" rel="">
                            Go to &rarr; 
                        </a>
                    </p>

                {/if}
                {#if step.name === "Joke Generator"}
                Utilizes the <span class="poppins text-violet-400"> api-ninjas </span> API to generate a joke and display them on an HTML webpage. This project showcases my ability to integrate APIs and develop dynamic web content.
                    <p class="justify-end">
                        <a href="https://github.com/andrerabanillo/apiJokeGenerator" target="_blank" rel="">
                            Go to &rarr; 
                        </a>
                    </p>
                {/if}
                {#if step.name === "Baseball Reference Web Scraper"}
                Utilizes
                <span class="poppins text-violet-400"> BeautifulSoup </span>
                to scrape data from baseball-reference.com. The program will parse the data, allowing the user to search up for various stats of previous, and current baseball players.
                <p class="justify-end">
                    <a href="https://github.com/andrerabanillo/baseballReferenceWebScraper" target="_blank" rel="">
                        Go to &rarr; 
                    </a>
                </p>

              {/if}
            </p>
          </Step>
        {/each}
      </div>
    </section>
    
    <section

        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A little bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
       
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