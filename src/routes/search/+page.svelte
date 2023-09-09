<script>
  import Select from 'svelte-select';

  let simple = ['one', 'two', 'three'];

  let collection = [
    { value: 1, label: 'one' },
    { value: 2, label: 'two' },
    { value: 3, label: 'three' },
  ];
</script>

<div class="grid place-items-center h-screen">
	<div class="w-[600px] mx-auto">
		<form class="flex items-center">
			<label for="simple-search" class="sr-only">Buscar Ação</label>
			<div class="relative w-full">
				<div class="flex absolute inset-y-0 left-0 items-center pl-3 pointer-events-none">
					<svg
						class="w-5 h-5 text-gray-500 dark:text-gray-300"
						fill="currentColor"
						viewBox="0 0 20 20"
						xmlns="http://www.w3.org/2000/svg"
						><path
							fill-rule="evenodd"
							d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
							clip-rule="evenodd"
						/></svg
					>
				</div>
				<input
					type="text"
					id="simple-search"
					class="bg-gray-50 border text-sm rounded-lg block w-full pl-10 p-2.5"
					placeholder="Digite o nome da ação. Ex.: petr4"
					required
				/>
			</div>
			<button
				type="submit"
				class="p-2.5 ml-2 text-sm font-medium text-white bg-blue-700 rounded-lg border border-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
			>
				Validar
			</button
			>
		</form>

		<p class="mt-5">
			Selecione no maximo 5 ações para validar.
		</p>
	</div>
</div>
