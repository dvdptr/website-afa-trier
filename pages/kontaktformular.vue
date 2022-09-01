<template>
  <div>
    <Header />
    <div class="pb-8">
      <p class="pb-8 text-center text-3xl font-bold">Kontaktformular</p>
      <p class="mx-auto text-center sm:w-1/3">
        Kurze Erklärung zum Kontaktformular
      </p>
    </div>
    <!-- Formular -->
    <div class="mx-auto mb-12 rounded-lg p-4 shadow-lg sm:w-1/2">
      <section>
        <div>
          <form
            name="contact-form"
            method="post"
            action="/contact/thankyou/"
            data-netlify="true"
            data-netlify-honeypot="bot-field"
          >
            <div>
              <input type="hidden" name="form-name" value="contact-form" />
              <div>
                <input
                  for="name"
                  type="text"
                  name="name"
                  required
                  placeholder="Name"
                />
              </div>
              <div>
                <input type="email" name="email" required placeholder="Email" />
              </div>
              <div>
                <textarea
                  name="message"
                  required
                  placeholder="Message"
                ></textarea>
              </div>
              <div>
                <button type="submit" value="Send message">Submit</button>
              </div>
            </div>
          </form>
        </div>
      </section>
    </div>
    <Footer />
  </div>
</template>
