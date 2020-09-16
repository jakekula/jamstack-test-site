<template>
  <div>
    <header class="md:flex md:items-center md:justify-around p-4 shadow-lg md:pb-4">
      <nav class="flex flex-wrap item-center justify-around text-primary font-bold">
        <div>
          <ul class="list-reset md:flex md:items-center">
            <li class="md:ml-4">
              <g-link class="nav__link block no-underline py-2 hover:text-darkgray md:border-none md:p-0" to="/">Home</g-link>
            </li>
            <li class="md:ml-4">
              <g-link class="nav__link block no-underline py-2 hover:text-darkgray md:border-none md:p-0" to="/about/">About</g-link>
            </li>
            <li class="md:ml-4">

            </li>
            <li class="md:ml-4">

            </li>
          </ul>
        </div>
      </nav>
    </header>
    <!-- END NAVIGATION -->
    
    <slot/>

    <footer class="mt-20 font-light text-gray w-full text-center p-4 text-primary">
      <p class="text-sm">
        Copyright YOUR NAME 2020
      </p>
      <div>
        <p class="text-small font-light">
          Developed using Gridsome, Tailwindcss and Contenful
        </p>
      </div>
    </footer>

  </div>
</template>



<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

