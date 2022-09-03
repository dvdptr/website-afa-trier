<template>
  <div class="border-t">
    <div class="justify-center sm:flex">
      <section class="mx-4">
        <p>Psychosoziales Zentrum Trier</p>
        <p>Dasbachstraße 21</p>
        <p>54292 Trier</p>
      </section>
      <section class="mx-4">
        <p>fluechtlingsberatung@diakoniehilft.de</p>
        <p>Tel.: 0651 9910600</p>
        <p>Fax.: 06519916366</p>
      </section>
      <div>
        <Bund class="w-56" />
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
