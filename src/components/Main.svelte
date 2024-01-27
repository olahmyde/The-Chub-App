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
    import RoundCube from "../assets/RoundCube-White-Glossy.png";
    import DarkPhone1 from "../assets/main.png";
    import DarkPhone2 from "../assets/main-2.png";
    import iPhoneStock1 from "../assets/Challenges1.png";
    import iPhoneStock2 from "../assets/Challenges2.png";
    import SToroid from "../assets/SuperToroid-White-Glossy.png";
    function LearnMore(){
        location.href="#downloadApp";
    }
    
    function GoToReviews(){
        location.href="/reviews";
    }
</script>

<!-- Active menu -->
<menu>
    <!-- <a class="nav--active" href='#home'><i class="fa-solid fa-house"></i></a> -->
    <a class="nav--active" href='#home'>Home</a>
    <a href='#features'> Features</a>
    <a href='#integration'> Integration</a>
    <a href='#blog'> Blog</a>
    <a href='#about'> About</a>
</menu>

<main class="max-md:top-[80px] grid justify-center p-4 top-[293px] absolute w-full">
    
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
            
            <a href="https://apps.apple.com/app/chub/id6450390309">
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
        <div class="absolute md:w-[90vw] w-[100%]" id="shapes">
            
            <img src={CylinderImg} alt="" class="w-[250px] max-md:w-[130px] h-[400px] max-md:h-[150px] mix-blend-difference float-left rotate-[-70deg] relative top-[-280px] max-md:top-[-70px] left-[-10px] max-md:left-[-50px]">
            
            <!-- <img src={CylinderImg} alt="" class="w-[200px] h-[250px] mix-blend-difference float-left rotate-[1.05deg] relative top-[-100px] right-[-500px]"> -->
            
            <img src={EllipsesImg} alt="" class="size-[120px] max-md:size-[70px] bg-[#FD8C48] rounded-full mix-blend-difference float-right rotate-[1.05deg] relative top-[-80px] max-md:top-[-30px] right-[700px] max-md:right-[180px]">
            
            <div class="float-right rounded-[250px] bg-[#00CC99] relative h-[550px] max-md:h-[300px] w-[370px] max-md:w-[170px] top-[70px] max-md:top-[10px] right-[0px] max-md:right-[80px] max-lg:hidden"></div>
            
            <img src={BluePillImg} alt="" class="w-[200px] max-md:w-[100px] h-[250px] max-md:h-[120px] mix-blend-difference float-right rotate-[1.05deg] relative top-[-100px] max-md:top-[-45px] right-[-500px] max-md:right-[-35px]">
        </div>
        <div class="flex max-md:flex-col-reverse items-end pt-[50px] w-[90vw] justify-around px-10 bg-[#1e0a54] p-4 bg-blend-color-dodge text-white rounded-[60px]">
            <div class="md:w-[50%] items-center">
                <h1 class="max-md:text-[30px] mb-5 max-md:mx-5 max-md:leading-[1.2] md:w-[650px] text-[88px] leading-[90px] text-white">What <span class="text-[#FA6400] glancyr">People</span> say about Challenge Hub</h1>
                
                <p class="max-md:text-[15px] max-md:mx-5 max-md:leading-[1.2] md:w-[460px] text-white text-[20px] font-[100]">One of the things i loved most about ths website was the ability to easily search for and find books that interested and helped me to quickly find books in specific genres or by specific authors</p>
                
                <button on:click={GoToReviews} class="buttons header-button my-[50px] mr-[16px] self-center duration-200"> Reviews</button>
                
            </div>
            <div class="md:w-[50%] flex rounded-[60px]">
                <div class="md:hidden rounded-[250px] bg-[#00CC99] relative h-[300px] w-[170px] top-[0px] left-[100px]"></div>
                <img src={SalyImg} alt="" class="w-[600px] h-[600px] max-md:size-[350px] relative left-[100px] max-md:top-[20px] rounded-[20px] rotate-[1.647deg]">
            </div>
        </div>
    </section>
    
    <!-- SECTION FIVE -->
    <section id="preview" class="max-md:mt-[50px] h-[400px] mt-[250px] relative w-full grid justify-center  bg-[#1E0221]">
        
        <div class="flex w-[75vw] justify-between px-1 py-0 bg-[#3c0210] bg-blend-color-dodge gap-10 text-white rounded-[40px]">
            
            <div class="w-[60%] flex flex-row justify-left items-end relative">
                <img src={RoundCube} alt="" class="absolute w-[15%] h-[25%]">
                <img src={DarkPhone1} alt="" class="absolute w-[50%] h-[120%] ml-[70px] z-[3]">
                <img src={iPhoneStock1} alt="" class="absolute w-[46%] h-[116%] ml-[86px] z-[4]">
                <img src={DarkPhone2} alt="" class="absolute w-[46%] h-[85%] ml-[350px] z-[1]">
                <img src={iPhoneStock2} alt="" class="absolute w-[40%] h-[81%] ml-[380px] z-[2]">
            </div>
            
            <div class="w-[40%]">
                <h1 class="text-[40px] mt-[30%] w-[65%] leading-10 text-white">Create your world with <span class="text-[#F1BB30] glancyr">CHUB</span></h1>
                
                <img src={SToroid} alt="" class="absolute w-[7%] mix-blend-lighten top-[28%] ml-[10%] color-[red] rotate-[10deg] z-[1]">
                
                <div class="flex mt-5 gap-5">
                    <a href="https://play.google.com/store/apps/details?id=com.challenge365.app&hl=en&gl=US">
                        <button class="download-button max-md:h-[50%] max-md:w-[50%] h-[60px] w-[200px] flex gap-2 leading-[1] justify-center items-center font-[300]">
                            <img class="size-[32px] bg-transparent" src={PlaystoreImg} alt="playstore-logo">
                            <span class="text-left">Download on <br>Playstore</span>
                        </button>
                    </a>
                    
                    <a href="https://apps.apple.com/app/chub/id6450390309">
                        <button class="download-button max-md:h-[50%] max-md:w-[50%] h-[60px] w-[200px] flex gap-2 leading-[1] justify-center items-center font-[300]">
                            <img class="size-[32px] bg-transparent" src={AppstoreImg} alt="playstore-logo">
                            <span class="text-left">Download on <br>Appstore</span>
                        </button>
                    </a>
                </div>
            </div>
            
        </div>
    </section>
</main>