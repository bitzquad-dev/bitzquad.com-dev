<script>
  import Header from "../Header.svelte";
</script>

<svelte:head>
  <style>
    body {
      background: url("https://bitzquad.com/images/bg/bg-1.jpg") no-repeat;
      @apply bg-center md:bg-cover;
    }
  </style>
</svelte:head>

<main class="main">
  <div class="col-left">
    <div
      class=" bg-gray-900 bg-opacity-10 rounded-lg shadow-xl xl:rounded-2xl"
    />
    ABCD
    <!-- <Countdown /> -->
  </div>
  <div class="col-right">
    <Header />
    <div class="w-3/4 my-10 md:mt-20 md:ml-10 mx-auto ">
      <h3 class="text-gray-100 font-semibold text-4xl md:text-5xl 2xl:text-7xl">
        COMMING SOON
      </h3>
      <p class="text-gray-300 font-light mt-2 2xl:text-2xl">
        Our website is currently undergoing scheduled maintenance. We Should be
        back shortly. Thank you for your patience.
      </p>
      <div class="socialContainer" />
    </div>
    <div class=" w-[275px] mx-auto md:hidden mt-10">
      <!-- <Countdown /> -->
      XYZ
    </div>
  </div>
</main>

<style>
  .main {
    @apply md:table w-screen h-screen;
  }

  .col-left {
    @apply hidden md:flex flex-col items-center justify-center absolute md:w-1/2 md:top-0 md:bottom-0 md:left-0;
  }

  .col-right {
    @apply bg-gray-900 absolute bg-opacity-30  md:w-1/2 top-0 bottom-0 md:right-0 flex-col items-center justify-center;
  }

  .wrapper {
    @apply grid grid-cols-2  justify-items-center h-full p-2;
  }

  .timeLeftContainer {
    @apply bg-gray-900 bg-opacity-90 w-28 h-28    border-4 m-2  border-gray-300 border-opacity-50 rounded-xl  flex flex-col justify-center items-center 
  2xl:w-48 2xl:h-48 2xl:rounded-3xl;
  }

  .timeLeft {
    @apply text-4xl 2xl:text-6xl font-bold text-purple-600;
  }

  .timeLeftTitle {
    @apply text-gray-300 2xl:text-3xl 2xl:mt-1 font-semibold;
  }
</style>
