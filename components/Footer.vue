<template>
  <div class="border-t">
    <div class="mx-auto w-5/6">
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
      <div class="text-center">
        <p>Gefördert von:</p>
        <div class="mx-auto flex justify-center text-center">
          <Bund class="w-56" />
          <RlpLogo class="w-48 pt-4" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Bund from "./Bund.vue";
import RlpLogo from "./Rlplogo.vue";

export default {
  data() {
    return {};
  },
  methods: {},
  components: { Bund, RlpLogo },
};
</script>
