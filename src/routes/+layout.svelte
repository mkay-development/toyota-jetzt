<script>
  import "../tailwind.css";
  import Fa from "svelte-fa";
  import {
    faHeart,
    faUser,
    faMagnifyingGlass,
  } from "@fortawesome/free-solid-svg-icons";
</script>

<header class="my-2 flex justify-between px-2 py-2">
  <div class="logo">
    <img
      src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5e/Toyota_EU.svg/2560px-Toyota_EU.svg.png"
      class="w-16 ml-5"
      alt="Toyota - Logo"
    />
  </div>
  <nav class="w-full mx-5 px-3 py-3 flex justify-between">
    <ul class="space-x-12 flex">
      <li>Neuwagen</li>
      <li>Angebote & Finanzierung</li>
      <li>Elektromobilität</li>
      <li>Gebrauchtwagen</li>
      <li>Zubehör & Service</li>
      <li>Geschäftskunden</li>
      <li>Entdecke Toyota</li>
    </ul>
    <ul class="space-x-5 flex">
      <li class="mr-12">
        <a href="https://www.toyota.de/startyourimpossible">
          <img
          src="https://www.toyota.de/content/dam/toyota/nmsc/glen/assets-without-car/image/logo-olympics.png"
          alt="Toyota Partner Olympic"
          class="h-8"
        />
        </a>
      </li>
      <li class="flex">
        <Fa icon={faUser} class="mr-3 mt-1" />
        <span>Konto</span>
      </li>
      <li class="flex">
        <Fa icon={faMagnifyingGlass} class="mr-3 mt-1" />
        <span>Suche</span>
      </li>
    </ul>
  </nav>
</header>

<main class="my-2 px-2 py-2"><slot /></main>

<footer class="my-2 px-2 py-2">
  <div class="grid grid-cols-6">
    <div class="col-span-6 md:col-span-2">
      <a href="/impressum">Impressum</a> &
      <a href="/data-privacy">Datenschutz</a>
    </div>
    <div class="col-span-6 md:col-span-2 flex">
      Made with <Fa icon={faHeart} class="mx-2 mt-1 text-red-400" /> by Jonathan
    </div>
    <div class="col-span-6 md:col-span-2">
      Copyright by <a
        href="https://www.mkay-development.de"
        class="text-blue-600">MkaY Development</a
      >
    </div>
  </div>
</footer>
