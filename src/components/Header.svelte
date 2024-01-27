<script>
   export let y;
   import ArrowMenu from "../assets/menu-arrow.svg";
   import ChubLogo from "../assets/wLogo_white.png"
   
   function downloadApp(){
    location.href="#downloadApp";
   }
   
   function refreshPage(){
    window.location.reload();
   }
</script>

<header class="w-auto justify-center flex">
    
    <div class="header flex justify-between">
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
        <img on:click={refreshPage} class="my-[24px] ml-[80px] bg-transparent " src={ChubLogo} alt='CHUB logo'>
        
        <nav class="bg-transparent flex gap-20 my-[40px] self-center">
            <a class="nav-links" href=''>Home </a>
            <a class="nav-links flex gap-1" href='#features'>Features <img class="w-[20px]" src={ArrowMenu} /></a>
            <a class="nav-links flex gap-1" href='#integration'>Integration <img class="w-[20px]" src={ArrowMenu} /></a>
            <a class="nav-links flex gap-1" href='#blog'>Blog <img class="w-[20px]" src={ArrowMenu} /></a>
        </nav>
        <button on:click={downloadApp} class="buttons header-button my-[14px] mr-[16px] self-center duration-200"> Get Started</button>
    </div>
</header>
