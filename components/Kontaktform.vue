<template>
  <!-- Kontakt Form -->
  <form
    name="contactform"
    @submit.prevent="handleSubmit"
    method="post"
    netlify
    netlify-honeypot="bot-field"
  >
    <!-- Hidden input to check for bots -->
    <input type="hidden" name="form-name" value="contactform" />
    <div>
      <label for="name" class="block">Name:</label>
      <input
        type="text"
        name="name"
        v-model="name"
        required
        class="title mb-4 w-full border border-gray-300 bg-gray-100 p-2 outline-none"
        placeholder="Ihr Name"
      />
    </div>
    <div>
      <label for="email" class="block">Email:</label>

      <input
        type="email"
        name="email"
        v-model="email"
        required
        class="title mb-4 w-full border border-gray-300 bg-gray-100 p-2 outline-none"
        placeholder="Ihre e-Mail"
      />
    </div>
    <div>
      <label for="message" class="block">Nachricht:</label>
      <textarea
        name="message"
        v-model="message"
        required
        class="title mb-4 w-full border border-gray-300 bg-gray-100 p-2 outline-none"
        placeholder="Ihre Nachricht"
      ></textarea>
    </div>
    <button
      type="submit"
      value="Send message"
      class="btn cursor-pointer rounded border bg-lime-600 p-1 px-4 font-bold text-white hover:bg-lime-700"
    >
      Absenden
    </button>
  </form>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      name: "",
      email: "",
      message: "",
    };
  },
  methods: {
    // This function puts all the form fields into a FormData constructor, which we later encode with the URLSearchParams constructor
    createFormDataObj(data) {
      const formData = new FormData();
      for (const key of Object.keys(data)) {
        formData.append(key, data[key]);
      }
      return formData;
    },
    // This is our custom onSubmit function; don't forget to add `@submit.prevent="handleSubmit"` inside your <form> tag
    handleSubmit() {
      // This `data` object is what's passed to the createFormDataObj function. It needs all of your form fields, where the key is the name= attribute and the value is the computed value.
      const data = {
        "form-name": "contactform",
        name: this.name,
        email: this.email,
        message: this.message,
      };
      // This POSTs your encoded form to Netlify with the required headers (for text; headers will be different for POSTing a file) and, on success, redirects to the custom success page located at pages/thanks.vue
      fetch("/", {
        method: "POST",
        headers: { "Content-Type": "application/x-www-form-urlencoded" },
        body: new URLSearchParams(this.createFormDataObj(data)).toString(),
      })
        // This is how we route to /thanks on successful form submission
        // More on $router.push function: https://router.vuejs.org/guide/essentials/navigation.html
        .then(() => this.$router.push("/bestaetigung"))
        .catch((error) => alert(error));
    },
  },
};
</script>
