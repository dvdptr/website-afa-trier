<template>
  <div class="border-t">
    <div class="">
      <div class="justify-center py-8 sm:flex">
        <section class="pb-4 sm:mx-4">
          <p>Psychosoziales Zentrum Trier</p>
          <p>Dasbachstraße 21</p>
          <p>54292 Trier</p>
        </section>
        <section class="sm:mx-4">
          <p>fluechtlingsberatung@diakoniehilft.de</p>
          <p>Tel.: 0651 9910600</p>
          <p>Fax.: 06519916366</p>
        </section>
      </div>
      <div class="">
        <Bund class="w-56 sm:mx-auto" />
      </div>
    </div>
  </div>
</template>

<script>
import Bund from "./Bund.vue";

export default {
  data() {
    return {};
  },
  methods: {},
  components: { Bund },
};
</script>
