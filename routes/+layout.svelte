<script lang="ts">
	import '../app.css';
	
	let { children } = $props();
</script>

{@render children()}

<head>
	<link
	rel="stylesheet"
	href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
	integrity="sha512-..."
	crossorigin="anonymous"
	referrerpolicy="no-referrer"
  />
  </head>
  <nav class="bg-white border-gray-200 dark:bg-gray-900 dark:border-gray-700">
	<div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
	  <a href="#" class="flex items-center space-x-3 rtl:space-x-reverse">
		  <img src="https://flowbite.com/docs/images/logo.svg" class="h-8" alt="Flowbite Logo" />
		  
		  <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">Water's Edge</span>
	  </a>
	  <button data-collapse-toggle="navbar-multi-level" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-multi-level" aria-expanded="false">
		  <span class="sr-only">Open main menu</span>
		  <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
			  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
		  </svg>
	  </button>
	  <div class="hidden w-full md:block md:w-auto" id="navbar-multi-level">
		<ul class="flex flex-col font-medium p-4 md:p-0 mt-4 border border-gray-100 rounded-lg bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
		  <li>
			<a href="#" class="block py-2 px-3 text-white bg-blue-700 rounded-sm md:bg-transparent md:text-blue-700 md:p-0 md:dark:text-blue-500 dark:bg-blue-600 md:dark:bg-transparent" aria-current="page">Home</a>
		  </li>
		  <li>
			  <button id="dropdownNavbarLink" data-dropdown-toggle="dropdownNavbar" class="flex items-center justify-between w-full py-2 px-3 text-gray-900 hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto dark:text-white md:dark:hover:text-blue-500 dark:focus:text-white dark:hover:bg-gray-700 md:dark:hover:bg-transparent">Dropdown <svg class="w-2.5 h-2.5 ms-2.5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 10 6">
	  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 4 4 4-4"/>
	</svg></button>
			  <!-- Dropdown menu -->
			  <div id="dropdownNavbar" class="z-10 hidden font-normal bg-white divide-y divide-gray-100 rounded-lg shadow-sm w-44 dark:bg-gray-700 dark:divide-gray-600">
				  <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownLargeButton">
					<li>
					  <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Dashboard</a>
					</li>
					<li aria-labelledby="dropdownNavbarLink">
					  <button id="doubleDropdownButton" data-dropdown-toggle="doubleDropdown" data-dropdown-placement="right-start" type="button" class="flex items-center justify-between w-full px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Dropdown<svg class="w-2.5 h-2.5 ms-2.5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 10 6">
	  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 4 4 4-4"/>
	</svg></button>
					  <div id="doubleDropdown" class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow-sm w-44 dark:bg-gray-700">
						  <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="doubleDropdownButton">
							<li>
							  <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Overview</a>
							</li>
							<li>
							  <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">My downloads</a>
							</li>
							<li>
							  <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Billing</a>
							</li>
							<li>
							  <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Rewards</a>
							</li>
						  </ul>
					  </div>
					</li>
					<li>
					  <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Earnings</a>
					</li>
				  </ul>
				  <div class="py-1">
					<a href="#" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Sign out</a>
				  </div>
			  </div>
		  </li>
		  <li>
			<a href="#" class="block py-2 px-3 text-gray-900 rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">FrontEnd Projects</a>
		  </li>
		  <li>
			<a href="#" class="block py-2 px-3 text-gray-900 rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">BackEnd Projects</a>
		  </li>
		  <li>
			<a href="#" class="block py-2 px-3 text-gray-900 rounded-sm hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent">Random Projects</a>
		  </li>
		</ul>
	  </div>
	</div>
  </nav>
  
  <div class="justify-center flex-row items-center bg-slate-950">
	<div class="justify-center">
	  <img src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/anne-sophie-benoit-JaNtL4uGvG8-unsplash.jpg" alt="Imagem" class="  rounded-2xl"/>
	</div>
	 
  
	 <div class="flex ">
	 
	   
	  <img class="rounded-2xl object-cover" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/s-alb-xYWMPwhQcDM-unsplash.jpg" alt="" />
			
  
	  <img class="rounded-t-lg max-w-sm max-h-sm object-cover" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/WhatsApp%20Image%202024-05-13%20at%2023.39.08.jpeg" alt="" />
			   
  
	  <img class="rounded-t-lg max-w-sm max-h-sm object-cover" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/luca-bravo-WeFDiEDModQ-unsplash.jpg" alt="" />
			 
  
	  <img class="rounded-t-lg max-w-sm max-h-sm object-cover" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/WhatsApp%20Image%202024-05-13%20at%2023.39.09.jpeg" alt="" />
			   
  
	  <img class="rounded-t-lg max-w-sm max-h-sm object-cover" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/louis-gaudiau-jloWf465qgU-unsplash.jpg" alt="" />
			  
	 </div>
	 
	 <div class="flex-row items-center">
	   <h2 class="text-white">FrontEnd Projects</h2>
  
		 
			  <a href="#" class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
				  <img class="object-cover w-full rounded-t-lg h-96 md:h-auto md:w-48 md:rounded-none md:rounded-s-lg" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/Captura%20de%20Tela%20(183).png" alt="">
				  <div class="flex flex-col justify-between p-4 leading-normal">
					  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">DoctorCare</h5>
					  <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
  A site made in the programming event NLW Return, it's a site made to ease people access to proper health care.</p>
				  </div>
			  </a>
  
			   <a href="#" class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
				  <img class="object-cover w-full rounded-t-lg h-96 md:h-auto md:w-48 md:rounded-none md:rounded-s-lg" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/Captura%20de%20Tela%20(184).png" alt="">
				  <div class="flex flex-col justify-between p-4 leading-normal">
					  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">MKJ Enterprises
  </h5>
					  <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">A collaborative site i made with two other people, João Gabriel Pereira Lopes and Erick de Castro, about an Enterprise that has two subsidiaries one which works with a luthier work and other which works with cealing lowering.</p>
				  </div>
			  </a>
  
			   <a href="#" class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
				  <img class="object-cover w-full rounded-t-lg h-96 md:h-auto md:w-48 md:rounded-none md:rounded-s-lg" src="https://asafesseidon.github.io/Asafesseidon-s_Website/Files/Images/Captura%20de%20Tela%20(185).png" alt="">
				  <div class="flex flex-col justify-between p-4 leading-normal">
					  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Hash Game</h5>
					  <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">
  Some quick example text to build on the card title and make up the bulk of the card's content.</p>
				  </div>
			  </a>
  
	 </div>
  
	 <div>
	   <h2 class="text-white">BackEnd Projects</h2>
  
		
			  <a href="#" class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
				 
				  <div class="flex flex-col justify-between p-4 leading-normal">
					  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
  RocketseatAuctionAPI</h5>
					  <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">A C# API that realizes and organizes auctions with automated bidding based on the maximum value the participants want to bid, it was made with an SQLite database.</p>
				  </div>
			  </a>
  
			   <a href="#" class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow-sm md:flex-row md:max-w-xl hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
				  
				  <div class="flex flex-col justify-between p-4 leading-normal">
					  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">PassInAPI</h5>
					  <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">A C# API that organizes events, made using the SQLite database.</p>
				  </div>
			  </a>
  
	 </div>
  
	 <div>
	   <h2 class="text-white">Random Projects</h2>
	 </div>
  
  </div>
  <footer class="bg-white rounded-lg shadow-sm  dark:bg-gray-800">
	  <div class="w-full mx-auto max-w-screen-xl p-4 md:flex md:items-center md:justify-between">
		<span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2023 <a href="https://flowbite.com/" class="hover:underline">Flowbite™</a>. All Rights Reserved.
	  </span>
	  <ul class="flex flex-wrap items-center mt-3 text-sm font-medium text-gray-500 dark:text-gray-400 sm:mt-0">
		  <li>
			  <a href="#" class="hover:underline me-4 md:me-6"><i class="fa-brands fa-github"></i> Github</a>
		  </li>
		  <li>
			  <a href="#" class="hover:underline me-4 md:me-6"><i class="fa-sharp fa-regular fa-envelope"></i> Email</a>
		  </li>
		  <li>
			  <a href="#" class="hover:underline me-4 md:me-6"><i class="fa-solid fa-phone"></i> Cellphone</a>
		  </li>
		  <li>
			  <a href="#" class="hover:underline"><i class="fa-brands fa-linkedin-in"></i> Linkedin</a>
		  </li>
	  </ul>
	  </div>
  </footer>
  