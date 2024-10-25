<script>
  export let y;

  export let tabs = [
      { name: "Projects ", link: "#projects" },
      { name: "About me", link: "#about" },
      // { name: "Contact", link: "" },
      // {name: '', link: ''},
  ];
</script>

<header
  class={"sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border-b border-solid " +
      (y > 0
          ? " py-4 bg-slate-950 border-violet-950"
          : " py-6 bg-transparent border-transparent")}
>
  <h1 class="font-medium">
      <a href="#introPage"><b class="font-bold poppins">Fajar</b> <span class="">Gustiana</span></a>
  </h1>
  <div class="sm:flex items-center gap-4 hidden">
      {#each tabs as tab, index}
          <a
              href={tab.link}
              class="duration-200 hover:text-violet-400"
              target={index === 2 ? "_blank" : ""}
          >
              <p>{tab.name}</p>
          </a>
      {/each}
      <a href="#footer"
          class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950"
      >
          <!-- svelte-ignore element_invalid_self_closing_tag -->
          <div
              class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
          />
          <h4 class="relative z-9">Get in touch</h4>
        </a>
  </div>
</header>



<div class="lg:hidden md:hidden fixed z-50 w-[calc(100%-1rem)] h-12 max-w-lg -translate-x-1/2 border border-gray-200 rounded-full bottom-4 left-1/2 bg-black bg-opacity-70">
    <div class="grid h-full max-w-lg grid-cols-3 mx-auto">
        <a href="#introPage"  type="button" class="inline-flex flex-col items-center justify-center px-5 rounded-s-full hover:bg-gray-800 group">
            <i class="fa-solid fa-house"></i>
            <span>Home</span>
        </a>
        <a href="#projects"  type="button" class="inline-flex flex-col items-center justify-center px-5 hover:bg-gray-800 group">
           <i class="fa-solid fa-diagram-project"></i>
           <span>Projects</span>
        </a>
        <a href="#about" type="button" class="inline-flex flex-col items-center justify-center px-5 rounded-e-full  hover:bg-gray-800 group">
            <i class="fa-solid fa-user"></i>
            <span>About</span>
        </a>
    </div>
</div>

