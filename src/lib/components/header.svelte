<script lang="ts">
    import { LightSwitch } from '@skeletonlabs/skeleton';
    import Logo from './logo.svelte'
    import { Drawer, drawerStore } from '@skeletonlabs/skeleton';
    import type { DrawerSettings } from '@skeletonlabs/skeleton';
	const drawerSettings: DrawerSettings = {
		id: 'example-3',
        position: 'right',
		width: 'w-[230px] md:w-[300px]'
        
	};



	function drawerOpen(): void {
		drawerStore.open(drawerSettings);
	}
</script>
<Drawer >
	<h2 class="p-4">Menu</h2>
	<hr class="!border-dashed !border-t-2" />
    <ul class="m-4">
        <li>
            <a href="/" class="hover-3 mr-3">Iniciar Sesion</a>
        </li>
    <li>
   <a href="/" class="hover-3 mt-5 mr-3 dark:text-white font-bold">Servicios</a>
    
    </li>
    <li>
        <a href="/" class="hover-3  mt-5 mr-3 font-bold">Contacto</a>
    </li>
    </ul>

 
</Drawer>
<nav class=" drop-shadow-lg w-scream mr-0 flex justify-between items-center  bg-white dark:bg-surface-800 gap-4  h-[70px] ">
    <a href="/" class="flex items-center pt-2  ">
        <Logo  />
    </a>

<div class="flex items-center gap-4 mr-4">
    <a href="/" class="hover-3 hidden sm:inline-block max-md:hidden mr-3 dark:text-white font-bold">Servicios</a>
    <a href="/" class="hover-3 hidden sm:inline-block mr-3 font-bold">Contacto</a>
       
        <div class="flex items-center">
            <button class="sm:hidden btn btn-sm mr-4" on:click={drawerOpen}>
                <span>
                    <svg viewBox="0 0 100 80" class="fill-token w-4 h-4">
                        <rect width="100" height="20" />
                        <rect y="30" width="100" height="20" />
                        <rect y="60" width="100" height="20" />
                    </svg>
                </span>
            </button>
        </div>
    
    <a href="/login" class="btn py-1.5 variant-soft hover:variant-soft-primary hidden sm:inline-block">Iniciar Sesion</a>
</div>

</nav>  

<style>
    .hover-3 {
  --b: 0.1em;   /* the thickness of the line */
  --c: #10c13f; /* the color */
  
  color: #0000;
  padding-block: var(--b);
  background: 
    linear-gradient(var(--c) 50%,#000 0) 0% calc(100% - var(--_p,0%))/100% 200%,
    linear-gradient(var(--c) 0 0) 0% var(--_p,0%)/var(--_p,0%) var(--b) no-repeat;
  -webkit-background-clip: text,padding-box;
          background-clip: text,padding-box;
  transition: .3s var(--_s,0s) linear,background-size .3s calc(.3s - var(--_s,0s));
}
.hover-3:hover {
  --_p: 100%;
  --_s: .3s;
}
</style>