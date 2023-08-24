<script lang="ts">
	let sliderValue = 1000;
	let sliderValuec = 3;
	import * as Icon from 'svelte-google-materialdesign-icons';
</script>

<section class="relative flex py-16 gap-10 lg:gap-5 flex-col lg:flex-row z-10">
	<div class="absolute inset-0 bg-cover bg-center z-[-1]">
		<div class="header" />
	</div>
	<div class="home-title mx-auto text-center lg:text-left flex flex-col justify-center lg:pl-[10%]">
		<h1 class="text-[40px] font-bold leading-10 text-white">Bienvenido a Fintech I n-Genius</h1>
		<span class="mt-4 sm:w-3/5 text-white">Tu plataforma financiera de confianza</span>
	</div>
	<div class="container relative mx-auto text-center flex justify-center lg:justify-left sm:w-3/5 ">
		<div
			class="card absolute p-4 w-3/5 lg:w-3/5 ml-[20%] flex flex-col items-center gap-1 inset-0 bg-gradient-to-r from-green-300 to-green-600 shadow-lg transform -skew-y-6 sm:skew-y-0 sm:-rotate-6 sm:rounded-3xl"
		/>
		<div class="card relative shadow p-4 w-3/5 lg:w-3/5 flex flex-col items-center gap-1">
			<span class="text-lg font-bold">Prestamo:</span>
			<span class="text-3xl max-sm:scale-[0.8] font-bold mb-2">S/. {sliderValue}</span>
			<input
				class="w-4/5 my-2"
				type="range"
				bind:value={sliderValue}
				min="1000"
				max="5000"
				step="100"
			/>
			<span class="text-lg font-bold mb-2">Cuotas</span>
			<span class="text-2xl font-bold">{sliderValuec}</span>
			<input class="w-4/5 my-2" type="range" bind:value={sliderValuec} min="3" max="12" />
			
			<div class="b mx-auto h-16 w-64 flex justify-center items-center mt-7 max-sm:scale-[0.7]">
				<div
					class="i h-16 w-64 bg-gradient-to-br from-green-400 to-green-600 items-center rounded-full shadow-2xl cursor-pointer absolute overflow-hidden transform hover:scale-x-110 hover:scale-y-105 transition duration-300 ease-out"
				/>
				<a href="/register" class="text-center text-white font-semibold z-10"
					>Solicitar Prestamo</a>
					
			</div>
		</div>
	</div>
</section>

<section id="services" class="py-16 px-3">
	<div class="container mx-auto">
		<h2 class="text-3xl font-bold mb-8">Beneficios</h2>
		<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-2xl font-bold text-center">Prestamos altoque</h3>
				<div class="flex justify-center mt-4">
					<Icon.Hourglass_empty size="80" class="text-sky-400" />
				</div>
				<p class="mt-4 text-center">
					¡Al instante! Solicita tu crédito online desde tu celular en minutos, evaluamos y
					aprobamos en segundos.
				</p>
			</div>
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Sin muchos requisitos</h3>
				<div class="flex justify-center mt-4">
					<Icon.Badge size="80" class="text-yellow-400 " />
				</div>
				<p class="mt-4 text-center">Solo debes tener a la mano tu documento de identidad.</p>
			</div>
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Facilidad de pagos</h3>
				<div class="flex justify-center mt-4">
					<Icon.Event_available size="80" class=" text-purple-500 " />
				</div>
				<p class="mt-4 text-center">
					Podrás realizar pagos anticipados de cuotas o saldos de forma total o parcial sin
					penalidades..
				</p>
			</div>
		</div>
	</div>
</section>

<section id="services" class="py-16 px-3">
	<div class="container mx-auto">
		<h2 class="text-3xl font-bold mb-8">¿Cómo solicitar tu préstamo?</h2>
		<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-8">
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Paso 1</h3>
				<div class="flex justify-center mt-4">
					<Icon.Price_change size="70" class="text-sky-400 " />
				</div>
				<p class="mt-4 text-center">Escoge el monto y el numero de cuotas</p>
			</div>
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Paso 2</h3>
				<div class="flex justify-center mt-4">
					<Icon.Touch_app size="70" class="text-orange-400 " />
				</div>
				<p class="mt-4 text-center">Dale a solicitar prestamo</p>
			</div>
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Paso 3</h3>
				<div class="flex justify-center mt-4">
					<Icon.Description size="70" class="text-purple-400 " />
				</div>
				<p class="mt-4 text-center">Registrar tus datos</p>
			</div>
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Paso 4</h3>
				<div class="flex justify-center mt-4">
					<Icon.Query_stats size="70" class="text-red-400" />
				</div>
				<p class="mt-4 text-center">Evaluacion crediticia</p>
			</div>
			<div class="bg-white dark:bg-surface-500 rounded p-8 shadow">
				<h3 class="text-xl font-bold text-center">Paso 5</h3>
				<div class="flex justify-center mt-4">
					<Icon.Check_circle size="70" class="text-green-400 " />
				</div>
				<p class="mt-4 text-center">Prestamo solicitado</p>
			</div>
		</div>
	</div>
</section>

<section id="contact" class="py-16 px-7 bg-gradient-to-br from-green-500 to-green-400 text-white">
	<div class="container mx-auto">
		<h2 class="text-3xl font-bold mb-8">Contacto</h2>
		<p>Para cualquier consulta o soporte, contáctanos:</p>
		<form class="mt-8">
			<input
				type="text"
				placeholder="Nombre"
				class="w-full border border-gray-300 px-4 py-2 rounded mt-4"
			/>
			<input
				type="email"
				placeholder="Correo electrónico"
				class="w-full border border-gray-300 px-4 py-2 rounded mt-4"
			/>
			<textarea
				placeholder="Mensaje"
				class="w-full border border-gray-300 px-4 py-2 rounded mt-4"
			/>
			<button
				type="submit"
				class="bg-blue-500 text-white px-6 py-3 rounded mt-4 inline-block hover:bg-blue-600"
				>Enviar</button
			>
		</form>
	</div>
</section>

<style>
	input[type='range'] {
		display: block;
		-webkit-appearance: none;
		background-color: #ffffff;

		height: 5px;
		border-radius: 5px;
		margin: 0 auto;
		outline: 0;
	}
	input[type='range']::-webkit-slider-thumb {
		-webkit-appearance: none;
		background-color: #0fa90f;
		width: 20px;
		height: 20px;
		border-radius: 50%;
		border: 2px solid white;
		cursor: pointer;
		transition: 0.3s ease-in-out;
	}
	​ input[type='range']::-webkit-slider-thumb:hover {
		background-color: white;
		border: 2px solid #0fa90f;
	}
	input[type='range']::-webkit-slider-thumb:active {
		transform: scale(1.2);
	}

	.header {
		height: 60vh;
		background-image: linear-gradient(to right bottom, rgba(61, 61, 61, 0.8), rgba(37, 37, 37, 0.8)),
			url('https://cdn-pe.comparabien.com/shared/images/fb_fotos/prestamos-rapidos.jpg');

		background-size: cover;
		background-position: top;
		position: relative;

		clip-path: polygon(0 0, 100% 0, 100% 52vh, 0 100%);
	}

	.home-title span {
		position: relative;
		overflow: hidden;
		display: block;
		line-height: 1.2;
	}

	.home-title span::after {
		content: '';
		position: absolute;
		top: 0;
		right: 0;
		width: 100%;
		height: 100%;
		background: rgb(29, 29, 29);
		animation: a-ltr-after 2s cubic-bezier(0.77, 0, 0.18, 1) forwards;
		transform: translateX(-101%);
	}

	.home-title span::before {
		content: '';
		position: absolute;
		top: 0;
		right: 0;
		width: 100%;
		height: 100%;
		background: #d8d8d8;
		animation: a-ltr-before 2s cubic-bezier(0.77, 0, 0.18, 1) forwards;
		transform: translateX(0);
	}

	.home-title span:nth-of-type(1)::before,
	.home-title span:nth-of-type(1)::after {
		animation-delay: 1s;
	}

	.home-title span:nth-of-type(2)::before,
	.home-title span:nth-of-type(2)::after {
		animation-delay: 1.5s;
	}

	@keyframes a-ltr-after {
		0% {
			transform: translateX(-100%);
		}
		100% {
			transform: translateX(101%);
		}
	}

	@keyframes a-ltr-before {
		0% {
			transform: translateX(0);
		}
		100% {
			transform: translateX(200%);
		}
	}

	.i::before {
		content: '';
		position: absolute;
		width: 0px;
		height: 0px;
		opacity: 20%;
		background: white;
		/*   background: #3B82F6; */
		/* Centering */
		top: 0;
		left: 0;
		bottom: 0;
		right: 0;
		margin: auto;
	}

	.i:hover:before {
		animation: anim-in 0.7s forwards ease-out;
	}

	@keyframes anim-in {
		100% {
			opacity: 0%;
			border-radius: 0;
			width: 600px;
			height: 600px;
		}
		0% {
			width: 0px;
			height: 0px;
			border-radius: 100%;
			opacity: 20%;
		}
	}
</style>
