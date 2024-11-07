<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "X (Twitter) Clone",
            icon: "fa-brands fa-x-twitter",
            description:
                "Developed a Twitter clone using the MERN stack, with JWT-based authentication, user suggestions, and post interactions, including creating, liking, commenting, and conditional deletion by owners. Utilized React Query for efficient data fetching and caching, Cloudinary for image uploads, and implemented a notification system to enhance user engagement.",
            link: "https://twitter-asp.onrender.com/",    
        },
        {
            name: "Reddit Clone",
            icon: "fa-brands fa-reddit",
            description:
                "Developed a full-stack Reddit clone using Next.js 14 using Kinde for passwordless and OAuth authentication, with Prisma ORM and Supabase. Implemented core Reddit features including up-down voting, comment sections, subreddit creation, and username generation, along with pagination for smooth content browsing and interaction.",
                 link: "https://reddit-jm.vercel.app/",
        },
        {
            name: "Airbnb Clone",
            icon: "fa-brands fa-airbnb",
            description:
                "Developed an Airbnb clone with Next.js 14, using Kinde for passwordless and OAuth authentication, with Prisma ORM and Supabase. Implemented a multi-step search modal, filter bar, and calendar integration, along with dynamic map functionality for enhanced user experience.",
                 link: "https://airbnb-jm.vercel.app/",
        },
        {
            name: "Apple 15 Pro",
            icon: "fa-brands fa-apple",
            description:
                "This project showcases a sleek and modern Apple 15 Pro landing page. It combines cutting-edge design with seamless functionality by utilizing the power of Three.js for stunning 3D graphics and GSAP for smooth animations.",
                 link: "https://apple-15-jsm.netlify.app/",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                `I taught myself to code using free online resources and absolutely fell in love with programming and problem solving. Starting of with HTML, CSS, and JavaScript and evolving my knowledge to include Frontend libraries and frameworks (React + Svelte + Astro), backend development (Node + Express, Django), design, cloud services and much much more.`,
        },
        {
            name: "UX fanatic",
            description:
                "I love the challenge of learning new design concepts and enabling users with amazing online experiences.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-3xl sm:text-4xl md:text-5xl line leading-8">
                Hi! I'm <span class="poppins text-violet-400"> Jatesh</span> Parikh <br>
                Full Stack <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite tech</span> includes JavaScript
                (Next.js or SvelteKit), TailwindCSS, Node.js + Express.js, Django, MongoDB, Firebase and PostgreSQL
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-25 group-hover:translate-x-full z-0 duration-200"
                />
                <a href="#footer" class="relative z-9">Get in touch &rarr;</a>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile-pic.jpeg"}
                alt="profile"
                class="object-cover z-[2] max-h-[70vh] aspect-square rounded-md shadow-inner p-12"
            />
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
         <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-16 place-items-center">
            <Step step={steps[0]}>
                <p class="leading-8">
                    Developed a Twitter clone using the <strong
                        class="text-violet-400"
                        >MERN stack, with JWT-based authentication</strong
                    >, and deployment using render.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p class="leading-8">
                    Developed a full-stack Reddit clone using <strong
                        class="text-violet-400">Next.js, Kinde for authentication</strong
                    >, with Prisma ORM and Supabase.
                </p>
            </Step>
            <Step step={steps[3]}>
                <p class="leading-8">
                    This project combines cutting-edge design with seamless functionality by utilizing the power of <strong class="text-violet-400"
                        >Three.js + GSAP </strong
                    >for smooth animations.
                </p>
            </Step>
        </div>
   
    <section id="about" class="py-20 lg:py-12 pt-10 lg:pt-16 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl mt-8 mb-4">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl mb-8">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p class="opacity-80">{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
    </section>
</main>