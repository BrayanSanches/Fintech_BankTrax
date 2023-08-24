<script lang="ts">
	import { goto } from '$app/navigation';
	import * as Icon from 'svelte-google-materialdesign-icons';
	import { Stepper, Step } from '@skeletonlabs/skeleton';
	function onCompleteHandler() {
		goto('/dashboard');
	}
</script>

<div class="container flex justify-center flex-col items-center h-screen w-full max-w-full">
	<div class="card md:p-10 max-sm:scale-[0.9] p-5 bg-white w-2/5 h-2/3">
		<Stepper
			stepTerm="Paso"
			buttonCompleteLabel="Registrarse"
			buttonNextLabel="Siguiente →"
			buttonBackLabel="← Atras"
			on:complete={onCompleteHandler}
		>
			<Step>
				<svelte:fragment slot="header">Registro</svelte:fragment>
				<div class="h-[260px]">
					<label class="label mt-3">
						<span>DNI *</span>
						<div class="flex justify-between gap-3">
							<input class="input" title="Input (text)" type="text" placeholder="Ingrese DNI" />
							<a href="/register" class="btn max-sm:scale-[0.8] variant-filled">Validar</a>
						</div>
					</label>
					<label class="label mt-3">
						<span>Nombre *</span>
						<input
							class="input"
							title="Input (text)"
							type="text"
							placeholder="Ingrese nombre"
							disabled
						/>
					</label>
					<label class="label mt-3">
						<span>Apellidos *</span>
						<input
							class="input"
							title="Input (text)"
							type="text"
							placeholder="Ingrese apellido"
							disabled
						/>
					</label>
				</div>
			</Step>
			<Step>
				<svelte:fragment slot="header">Registro</svelte:fragment>
				<div class="h-[260px]">
					<label class="label mt-3">
						<span>Celular *</span>
						<input class="input" title="Input (text)" type="text" placeholder="Ingrese Celular" />
					</label>
					<label class="label mt-3">
						<span>Correo *</span>
						<input class="input" title="Input (text)" type="text" placeholder="Ingrese Correo" />
					</label>
				</div>
			</Step>
			<Step>
				<svelte:fragment slot="header">Registro</svelte:fragment>
				<div class="h-[260px]">
					<label class="label mt-3">
						<span>Contraseña *</span>
						<input
							class="input"
							title="Input (text)"
							type="password"
							placeholder="Ingrese contraseña"
						/>
					</label>

					<label class="label mt-3">
						<span>Confirmar Contraseña *</span>
						<input
							class="input"
							title="Input (text)"
							type="password"
							placeholder="Confirme contraseña"
						/>
					</label>
				</div>
			</Step>
		</Stepper>
	</div>
</div>

<style>
	.container {
		/* Add the URL of your background image here */
		background-image: linear-gradient(to right bottom, rgba(61, 61, 61, 0.8), rgba(37, 37, 37, 0.8)),
			url('https://i0.wp.com/cardbiss.com/wp-content/uploads/2022/11/Imagen-1-1-e1597769103370.jpg?ssl=1');
		/* You can adjust the background size, position, and other properties as needed */
		background-size: cover;
		background-position: center;
		/* Add more styling for the container if necessary */
	}
</style>
