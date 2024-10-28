<script>
    let menuOpen = false;
  
    const toggleMenu = () => {
      menuOpen = !menuOpen;
    };

    /*
      <div class="text-xl font-semibold bg-gradient-to-r from-blue-600 via-purple-600 to-pink-500 bg-clip-text text-transparent">
        <a href="/">MooseCoding</a>
      </div>

    */
  </script>
  
  <nav class="bg-black shadow-md px-4 py-4">
    <div class="container mx-auto flex items-center justify-between">
      <!-- Logo -->
       <div class="text-xl font-semibold gradient-text">
          <a href="/">MooseCoding</a>
       </div>
  
      <!-- Desktop Navigation -->
      <div class="hidden md:flex space-x-6">
        <a href="/about" class="text-blue-600 hover:text-purple-400">About</a>
        <a href="/projects" class="text-purple-600 hover:text-pink-400">Projects</a>
        <a href="/contact" class="text-pink-400 hover:text-blue-600">Contact</a>
      </div>
  
      <!-- Mobile Menu Button -->
      <button class="md:hidden text-gray-800" on:click={toggleMenu}>
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
        </svg>
      </button>
    </div>
  
    <!-- Mobile Navigation -->
    {#if menuOpen}
      <div class="md:hidden flex flex-col items-center space-y-4 mt-4">
        <a href="/about" class="text-blue-600 hover:text-purple-600">About</a>
        <a href="/projects" class="text-purple-600 hover:text-pink-400">Projects</a>
        <a href="/contact" class="text-pink-400 hover:text-blue-600">Contact</a>
      </div>
    {/if}
  </nav>
  
  <style>
    nav {
      @apply bg-gray-900 shadow-md;
    }
    .container {
      @apply flex items-center justify-between;
    }

    .gradient-text {
    font-size: 1.7rem;
    font-weight: bold;
    background: linear-gradient(90deg, #0000ff 0%, #8a2be2 25%, #ff69b4 50%, #8a2be2 75%, #0000ff 100%);
    background-size: 600%;  /* Makes the gradient wider for smooth scrolling */
    background-clip: text;
    -webkit-background-clip: text;
    color: transparent;
    animation: gradient-animation 3s infinite linear;
  }



  @keyframes gradient-animation {
    0% {
      background-position: 0% 50%;
    }
    100% {
      background-position: 100% 50%;
    }
  }
  </style>

  