<script lang="ts">
    import * as Icon from 'svelte-google-materialdesign-icons'
    import { goto } from '$app/navigation';
    function onCompleteHandler() {
		goto('/dashboard');
	}
</script>

<div class="container flex justify-center flex-col items-center h-screen w-full max-w-full">
   
    <div class="card md:p-10 max-sm:scale-[0.9] p-5">
        <div class="flex justify-center"> <Icon.Insights size="50" class="mt-1"  /></div>
		<h3 class="h3 text-center">Inicio de Sesión</h3>
		<label class="label mt-3">
			<span>Correo *</span>
			<input class="input" title="Input (text)" type="text" placeholder="Ingrese correo electronico" />
		</label>
		<label class="label mt-3">
			<span>Contraseña *</span>
			<input class="input" title="Input (text)" type="password" placeholder="Ingrese contraseña"  />
		</label>
        <div class="text-center mt-4">
		<button on:click={onCompleteHandler} type="button" class="btn bg-gradient-to-br variant-gradient-secondary-tertiary mt-3" >
			<span><Icon.Login /></span>
			<span>Login</span>
		</button>
        <div class="space-y-2 mt-3">
            <label class="flex items-center space-x-2">
                <input class="checkbox" type="checkbox"  />
                <p>Recordarme</p>
            </label>
        </div>
        </div>
	</div>
    
</div>

<style>
    .container {
        /* Add the URL of your background image here */
        background-image: 	  linear-gradient(to right bottom, 
     rgba(61, 61, 61, 0.8),
     rgba(37, 37, 37, 0.8)),url('https://i0.wp.com/cardbiss.com/wp-content/uploads/2022/11/Imagen-1-1-e1597769103370.jpg?ssl=1');
        /* You can adjust the background size, position, and other properties as needed */
        background-size: cover;
        background-position: center;
        /* Add more styling for the container if necessary */
    }

	
</style>