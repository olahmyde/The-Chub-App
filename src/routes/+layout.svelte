<script>
   import "../app.css";
   import "../menu.css";
   import Header from "../components/Header.svelte";
   import Main from "../components/Main.svelte";
   import Footer from "../components/Main.svelte";
   let y;
   let innerHeight = 0;
   let innerWidth = 0;

   function goTop() {
      document.body.scrollIntoView();
   }
</script>

<div class="relative flex flex-col max-w-full mx-auto w-full text-sm sm:text-base min-h-screen">
   <div class={"fixed bottom-0 w-auto duration-200 flex p-10 z-[10] bg-transparent " +
         (y > 0
            ? "opacity-full pointer-events-auto"
            : "opacity-0 pointer-events-none")}
   >
      <button on:click={goTop} class="max-md:hidden arrow-button ml-auto rounded-full bg-slate-900 text-violet-400 px-3 sm:px-4 hover:bg-[#33023b] cursor-pointer bg-transparent">
         <i class="fa-solid fa-arrow-up grid place-items-center aspect-square" />
      </button>
   </div>
   <Header y={y}/>
   <slot />
   <Footer />
</div>

<svelte:window
   bind:scrollY={y}
   bind:innerHeight
   bind:innerWidth
/>
