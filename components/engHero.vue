<template>
  <div class="">
    <div class="border-y border-gray-200 bg-gray-100 py-12 px-2 sm:px-4">
      <div class="mx-auto sm:max-w-screen-xl">
        <p class="pb-8 text-center text-2xl font-bold sm:text-3xl">Welcome!</p>
        <p class="mx-auto text-center sm:w-4/6">
          We at the Psychosocial Center for Refugees in Trier are a team on site
          to make your arrival in Germany easier. We know that you have lived
          through difficult times in your home country and possibly also during
          the escape. We are pleased that you have now arrived here and would
          like to help you with your start in Germany. We assist you if you are
          not feeling well and will support you with any questions that arise.
        </p>
        <br />
        <p class="mx-auto text-center sm:w-4/6">We are here for you!</p>
        <div class="mt-8 flex justify-center">
          <nuxt-link
            to="/eng/contactform"
            class="mx-2 rounded-lg bg-lime-600 px-3 py-2 text-white hover:bg-lime-700 hover:text-white"
          >
            Contact us
          </nuxt-link>

          <!-- <button class="mx-2 rounded-lg border-2 border-gray-200 px-3 py-2">
            Sprache wählen
          </button> -->
        </div>
      </div>
    </div>
  </div>
</template>
