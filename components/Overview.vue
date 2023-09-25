<template>
  <div class="mx-auto w-5/6 py-12 sm:max-w-screen-xl">
    <!-- Angebote -->
    <nuxt-link to="/angebote">
      <div
        class="mx-auto mb-8 justify-around rounded-lg bg-gray-100 px-4 sm:flex sm:w-4/6 sm:px-0"
      >
        <div class="py-4 sm:w-1/2">
          <p class="pb-2 text-xl font-bold">Angebote in der AfA Trier</p>
          <p class="pb-4">
            Hier findest du unsere Angebote von Erstangeboten und Vorbereitungen
            bis hin zu gemeinschaftlichen Aktivitäten.
          </p>
          <p class="text-sm font-bold text-lime-600 hover:underline">
            Erfahre mehr ▸
          </p>
        </div>
      </div>
    </nuxt-link>

    <!-- Zielgruppe -->
    <nuxt-link to="/angeboteKommune">
      <div
        class="mx-auto mb-8 justify-around rounded-lg bg-gray-100 px-4 sm:flex sm:w-4/6 sm:px-0"
      >
        <div class="py-4 sm:w-1/2">
          <p class="pb-2 text-xl font-bold">Angebote in der Kommune</p>
          <p class="pb-4">
            Diese Angebote richten sich an alle Geflüchtete die
            Traumatherapeutische und oder psychosoziale Hilfe brauchen.
          </p>
          <p class="text-sm font-bold text-lime-600 hover:underline">
            Erfahre mehr ▸
          </p>
        </div>
      </div>
    </nuxt-link>

    <!-- Über uns -->
    <nuxt-link to="/about">
      <div
        class="mx-auto mb-8 justify-around rounded-lg bg-gray-100 px-4 sm:flex sm:w-4/6 sm:px-0"
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
      </div>
    </nuxt-link>
  </div>
</template>
