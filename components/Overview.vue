<template>
  <div class="mx-auto py-12 sm:max-w-screen-xl">
    <!-- Angebote -->
    <nuxt-link to="/angebote">
      <div
        class="mx-auto mb-8 w-5/6 justify-around rounded-lg bg-gray-100 sm:flex"
      >
        <div class="py-4 sm:w-1/2">
          <p class="pb-2 text-xl font-bold">Angebote</p>
          <p class="pb-4">
            Hier findest du unsere Angebote von Erstangeboten und Vorbereitungen
            bis hin zu gemeinschaftlichen Aktivitäten.
          </p>
          <p class="text-sm font-bold text-lime-600 hover:underline">
            Erfahre mehr ▸
          </p>
        </div>
        <div class="my-4 w-full bg-gray-400 sm:w-1/4">image</div>
      </div>
    </nuxt-link>

    <!-- Angebote -->
    <nuxt-link to="/zielgruppe">
      <div
        class="mx-auto mb-8 w-5/6 justify-around rounded-lg bg-gray-100 sm:flex"
      >
        <div class="py-4 sm:w-1/2">
          <p class="pb-2 text-xl font-bold">Zielgruppe und Informationen</p>
          <p class="pb-4">
            Erfahre mehr über unsere Zielgruppe, für wen unsere Angebote
            geeignet sind und weiterführende Informationen.
          </p>
          <p class="text-sm font-bold text-lime-600 hover:underline">
            Erfahre mehr ▸
          </p>
        </div>
        <div class="my-4 w-full bg-gray-400 sm:w-1/4">image</div>
      </div>
    </nuxt-link>
    <!-- Angebote -->
    <nuxt-link to="/about">
      <div
        class="mx-auto mb-8 w-5/6 justify-around rounded-lg bg-gray-100 sm:flex"
      >
        <div class="py-4 sm:w-1/2">
          <p class="pb-2 text-xl font-bold">Über uns</p>
          <p class="pb-4">
            Wir stellen unsere Einrichtung vor und beschreiben unser Vorgehen
            sowie unsere Partner.
          </p>
          <p class="text-sm font-bold text-lime-600 hover:underline">
            Erfahre mehr ▸
          </p>
        </div>
        <div class="my-4 w-full bg-gray-400 sm:w-1/4">image</div>
      </div>
    </nuxt-link>
  </div>
</template>
