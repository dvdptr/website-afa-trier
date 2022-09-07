<template>
  <div>
    <Header />
    <div class="mx-auto w-5/6 pb-8 text-center sm:w-3/5 sm:max-w-screen-xl">
      <p class="pb-8 text-center text-2xl font-bold">So erreichst du uns</p>
      <p class="pb-4">
        Unsere Einrichtung befindet sich auf dem Gelände der Afa Trier in Haus
        1.
      </p>
      <p class="pb-4">
        Gerne kannst du dich persönlich bei uns melden und einen Termin für ein
        Gespräch vereinbaren. Des Weiteren besteht auch die Möglichkeit der
        Kontaktaufnahme durch das unten aufgeführte Kontaktformular.
      </p>

      <div>
        <iframe
          src="https://docs.google.com/forms/d/e/1FAIpQLScjxXIpxp-BVV02lKzArieDxv81y1nw3gK9zckoP-AalX-wiw/viewform?embedded=true"
          height="947"
          frameborder="0"
          marginheight="0"
          marginwidth="0"
          class="mx-auto w-full pt-4 sm:w-3/4"
          >Wird geladen…</iframe
        >
      </div>
    </div>

    <!-- Formular -->
    <!-- <div
      class="mx-auto mb-12 rounded-lg border border-gray-300 p-4 shadow-lg sm:w-1/2"
    >
      <p class="pt-2 pb-4 font-bold">Kontaktformular</p>
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
                  class="mb-4 rounded-sm border border-gray-300 p-1"
                  for="name"
                  type="text"
                  name="name"
                  required
                  placeholder="Name"
                />
              </div>
              <div>
                <input
                  class="mb-4 rounded-sm border border-gray-300 p-1"
                  type="email"
                  name="email"
                  required
                  placeholder="Email"
                />
              </div>
              <div>
                <input
                  class="mb-4 rounded-sm border border-gray-300 p-1"
                  type="text"
                  name="herkunftsland"
                  required
                  placeholder="Herkunftsland"
                />
              </div>
              <div>
                <input
                  class="mb-4 rounded-sm border border-gray-300 p-1"
                  type="text"
                  name="zimmernummer"
                  required
                  placeholder="Zimmernummer"
                />
              </div>
              <div>
                <input
                  class="mb-4 rounded-sm border border-gray-300 p-1"
                  type="text"
                  name="telefonnummer"
                  required
                  placeholder="Telefonnummer"
                />
              </div>
              <div>
                <textarea
                  class="mb-4 h-48 w-full rounded-sm border border-gray-300 p-1"
                  name="message"
                  required
                  placeholder="Message"
                ></textarea>
              </div>
              <div>
                <button
                  class="rounded-lg bg-gray-200 px-3 py-2 hover:bg-gray-600 hover:text-white"
                  type="submit"
                  value="Send message"
                >
                  Submit
                </button>
              </div>
            </div>
          </form>
        </div>
      </section>
    </div> -->
    <Footer />
  </div>
</template>
