<script>
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';
    import '@splidejs/svelte-splide/css';
    import PlaystoreImg from "../assets/icons8-playstore-48.png";
    import AppstoreImg from "../assets/icons8-app-store-48.png";
    import ConnectDot from "../assets/connect-svg.png";
    import ChubLogo from "../assets/wLogo_white.png";
    import EmoticonImg from "../assets/emotion-smile.svg";
    import LockImg from "../assets/lock-2.svg";
    import ClockImg from "../assets/clock.svg";
    import CylinderImg from "../assets/7e12243d3becd9ddddaac792c62746cd.png";
    import EllipsesImg from "../assets/Mask_group.svg";
    import BluePillImg from "../assets/Pill-Blue-Glossy-2.png";
    import SalyImg from "../assets/Saly-35.png";
    function LearnMore(){
        location.href="#downloadApp";
    }
    
    function GoToReviews(){
        location.href="/reviews";
    }
</script>

<main class="max-md:top-[80px] grid justify-center p-4 top-[293px] absolute w-full">
    <menu>
        <!-- <a class="nav--active" href='#home'><i class="fa-solid fa-house"></i></a> -->
        <a class="nav--active" href='#home'>Home</a>
        <a href='#features'> Features</a>
        <a href='#integration'> Integration</a>
        <a href='#blog'> Blog</a>
        <a href='#about'> About</a>
    </menu>
    <!-- SECTION ONE-->
    <section id="title" class="max-md:mx-[20px] mx-[40px] grid grid-cols-1 bg-transparent">
        
        <div class="justify-center mb-4 flex lg:hidden">
            <img src="{ChubLogo}" alt="" class="w-[300px]">
        </div>
        <h1 class="max-md:text-[30px] max-md:leading-[1.2] text-[88px] leading-[100px] text-center">Master your goals with <span class="text-[#FA6400] glancyr">playful productivity</span></h1>
        
        <p class="text-center mt-1 font-[100]">Boost productivity and attain your set goals with our gamified aided by the power of community support and social networks</p>
        
        <div class="max-md:grid max-md:mt-8 flex justify-center max-md:gap-4 gap-10 mt-[75px]">
            <a href="https://play.google.com/store/apps/details?id=com.challenge365.app&hl=en&gl=US">
                <button class="download-button max-md:h-[70px] max-md:w-[300px] h-[80px] w-[320px] flex gap-2 leading-[2] justify-center items-center font-[300]">
                    <img class="size-[32px] bg-transparent" src={PlaystoreImg} alt="playstore-logo">Download on Playstore
                </button>
            </a>
            
            <a href="https://apps.apple.com/ng/app/chub/id6450390309">
                <button class="download-button max-md:h-[70px] max-md:w-[300px] h-[80px] w-[320px] flex gap-2 leading-[2] justify-center items-center font-[300]">
                    <img class="size-[32px] bg-transparent" src={AppstoreImg} alt="playstore-logo">Download on Appstore
                </button>
            </a>
        </div>
    </section>
    
    <!-- SECTION TWO-->
    <section id="about" class="max-md:hidden mt-[200px] h-[800px] overflow-x-scroll w-full flex gap-3 bg-[#1E0221]">
        <div class="carousel flex flex-row gap-3">
            <!-- Slide 1 -->
            <div class="grid grid-flow-row gap-3 bg-transparent w-[300px]">
                <div class="divided-grid rounded-md flex flex-cols-2 flex-rows-2 items-end justify-end bg-[#F07DBC]">
                    <h1 class="text-[30px]">Collaborate</h1>
                </div>
                <div class="divided-grid rounded-md flex flex-cols-2 flex-rows-2 items-end justify-end bg-[#F1BB30]">
                    <h1 class="text-[30px]">Conquer</h1>
                </div>
            </div>
            
            <!-- Slide 2 -->
            <div class="flex flex-col gap-3 bg-blend-overlay w-[600px] bg-[#3d0443] rounded-[40px]">
                <div class="mt-[40%] flex flex-col items-center mx-10 text-center">
                    <div class="rounded-full p-3 w-fit bg-blue-500">Simplify</div>
                    <h1 class="text-[30px] mt-4 mx-[50px] leading-[1]">Embrace your Achievements</h1>
                    <p class="text-center mt-1 font-[100] mx-[80px]">Earn your badges and showcase your journey, inspiring others to push their limits and be successful.</p>
                    <a href="#about" class="flex gap-2 mt-4">Learn more<svg xmlns="http://www.w3.org/2000/svg" width="16" height="10" viewBox="0 0 16 10" fill="none" class="block">
                        <path d="M14.9243 5.42426C15.1586 5.18995 15.1586 4.81005 14.9243 4.57574L11.1059 0.757359C10.8716 0.523045 10.4917 0.523045 10.2574 0.757359C10.023 0.991674 10.023 1.37157 10.2574 1.60589L13.6515 5L10.2574 8.39411C10.023 8.62843 10.023 9.00833 10.2574 9.24264C10.4917 9.47696 10.8716 9.47696 11.1059 9.24264L14.9243 5.42426ZM0.5 5.6H14.5V4.4H0.5V5.6Z" fill="white"/>
                        </svg>
                    </a>
                </div>
                <div class="mt-[30px] flex justify-center">
                    <img src={ConnectDot} alt="">
                </div>
            </div>
            
            <!-- Slide 3 -->
            <div class="flex flex-col gap-3 bg-blend-overlay w-[600px] bg-[#3c0213] rounded-[40px]">
                <div class="mt-[40%] flex flex-col items-center mx-10 text-center">
                    <div class="opacity-0 rounded-full p-3 w-fit bg-blue-500">Simplify</div>
                    <h1 class="text-[30px] mt-4 mx-[50px] leading-[1]">Embrace your Achievements</h1>
                    <p class="text-center mt-1 font-[100] mx-[80px]">Earn your badges and showcase your journey, inspiring others to push their limits and be successful.</p>
                    
                    <button on:click={LearnMore} class="buttons header-button my-[14px] mr-[16px] self-center duration-200"> Get Started</button>
                </div>
            </div>
            
            <!-- Slide 4 -->
            <div class="flex flex-col gap-3 bg-blend-overlay w-[600px] bg-[#3d0443] rounded-[40px]">
                <div class="mt-[40%] flex flex-col items-center mx-10 text-center">
                    <div class="rounded-full p-3 w-fit bg-blue-500">Simplify</div>
                    <h1 class="text-[30px] mt-4 mx-[50px] leading-[1]">Embrace your Achievements</h1>
                    <p class="text-center mt-1 font-[100] mx-[80px]">Earn your badges and showcase your journey, inspiring others to push their limits and be successful.</p>
                    <a href="#about" class="flex gap-2 mt-4">Learn more<svg xmlns="http://www.w3.org/2000/svg" width="16" height="10" viewBox="0 0 16 10" fill="none" class="block">
                        <path d="M14.9243 5.42426C15.1586 5.18995 15.1586 4.81005 14.9243 4.57574L11.1059 0.757359C10.8716 0.523045 10.4917 0.523045 10.2574 0.757359C10.023 0.991674 10.023 1.37157 10.2574 1.60589L13.6515 5L10.2574 8.39411C10.023 8.62843 10.023 9.00833 10.2574 9.24264C10.4917 9.47696 10.8716 9.47696 11.1059 9.24264L14.9243 5.42426ZM0.5 5.6H14.5V4.4H0.5V5.6Z" fill="white"/>
                        </svg>
                    </a>
                </div>
                <div class="mt-[30px] flex justify-center">
                    <img src={ConnectDot} alt="">
                </div>
            </div>
            
            <!-- Slide 5 -->
            <!-- <div class="flex flex-col gap-3 bg-blend-overlay w-[600px] bg-[#FD8C48] rounded-[40px]">
                <div class="mt-[40%] flex flex-col items-center mx-10 text-center">
                    <div class="opacity-0 rounded-full p-3 w-fit bg-blue-500">Simplify</div>
                    <h1 class="text-[30px] mt-4 mx-[50px] leading-[1]">Embrace your Achievements</h1>
                    <p class="text-center mt-1 font-[100] mx-[80px]">Earn your badges and showcase your journey, inspiring others to push their limits and be successful.</p>
                    
                    <button on:click={LearnMore} class="buttons header-button my-[14px] mr-[16px] self-center duration-200"> Get Started</button>
                </div>
            </div> -->
        </div>
    </section>
    
    <!-- SECTION THREE -->
    <section id="features" class="max-md:mt-[50px] mt-[160px] w-full grid justify-center">
        <center class="mx-10 max-md:mx-2">
            <h1 class="max-md:text-[30px] max-md:mx-5 max-md:leading-[1.2] md:w-[800px] text-[88px] leading-[100px] text-center">Reason Why You Should Use <span class="text-[#FA6400] glancyr">CHUB</span></h1>
            
            <p class="text-center mt-1 font-[100]">CHUB has several features that makes the go to for challenges</p>
            
            <div class="flex gap-3 my-10 max-md:mx-0 lg:gap-7">
                <div class="mini-features bg-[#33023a] lg:w-[260px]">
                    <img class="bg-[#3C0345]" src={EmoticonImg} alt="">
                    <h3 class="mt-2">Easy to use</h3>
                    <p>Easy to use for everyone and simple</p>
                </div>
                
                <div class="mini-features bg-[#690571] lg:w-[260px]">
                    <img class="bg-[#81108A]" src={ClockImg} alt="">
                    <h3 class="mt-2">Real time</h3>
                    <p>Connect with customer real time</p>
                </div>
                
                <div class="mini-features bg-[#33023a] lg:w-[260px]">
                    <img class="bg-[#3C0345]" src={LockImg} alt="">
                    <h3 class="mt-2">Safety & Privacy</h3>
                    <p>Easy to use for everyone and simple</p>
                </div>
            </div>
        </center>
    </section>
    
    <!-- SECTION FOUR -->
    <section id="feedbacks" class="max-md:mt-[50px] mt-[160px] w-full grid justify-center">
        <div class="absolute w-[90vw]" id="shapes">
            
            <img src={CylinderImg} alt="" class="w-[250px] h-[400px] mix-blend-difference float-left rotate-[-70deg] relative top-[-280px] left-[-10px]">
            
            <!-- <img src={CylinderImg} alt="" class="w-[200px] h-[250px] mix-blend-difference float-left rotate-[1.05deg] relative top-[-100px] right-[-500px]"> -->
            
            <img src={EllipsesImg} alt="" class="size-[120px] bg-[#FD8C48] rounded-full mix-blend-difference float-right rotate-[1.05deg] relative top-[-80px] right-[700px]">
            
            <div class="float-right rounded-[250px] bg-[#00CC99] relative h-[550px] w-[370px] top-[70px] right-[0px]"></div>
            
            <img src={BluePillImg} alt="" class="w-[200px] h-[250px] mix-blend-difference float-right rotate-[1.05deg] relative top-[-100px] right-[-500px]">
        </div>
        <div class="flex items-end pt-[50px] w-[90vw] justify-around px-10 bg-[#1e0a54] p-4 bg-blend-color-dodge text-white rounded-[60px]">
            <div class="w-50% z-10 items-center">
                <h1 class="max-md:text-[30px] max-md:mx-5 max-md:leading-[1.2] md:w-[650px] text-[88px] leading-[90px] text-white">What <span class="text-[#FA6400] glancyr">People</span> say about Challenge Hub</h1>
                
                <p class="max-md:text-[30px] max-md:mx-5 max-md:leading-[1.2] md:w-[460px] text-white text-[20px] font-[100]">One of the things i loved most about ths website was the ability to easily search for and find books that interested and helped me to quickly find books in specific genres or by specific authors</p>
                
                <button on:click={GoToReviews} class="buttons header-button my-[50px] mr-[16px] self-center duration-200"> Reviews</button>
                
            </div>
            <div class="w-50% rounded-[60px] z-10">
                <img src={SalyImg} alt="" class="w-[600px] h-[600px] rounded-[20px] rotate-[1.647deg]">
            </div>
        </div>
    </section>
</main>