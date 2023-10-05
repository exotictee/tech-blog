<script>
export default {
  data() {
    return {
      email: '',
      showMessage: false,
    };
  },
  methods: {
    submitForm() {
      if (this.isValidEmail(this.email)) {
        this.showMessage = true;
      } else {
        alert("Please enter a valid email address.");
      }
    },
    isValidEmail(email) {
      // Use a regular expression to check if the email is in a valid format
      const emailRegex = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;
      return emailRegex.test(email);
    },
  },
};
</script>

<template>
  <div class="bg-purple min-h-screen object-cover object-center bg-no-repeat">
    <navbar :page="'index'" />

    <div class="px-20 mt-32">
      <h2 class="text-white text-2xl font-bold">What I Do?</h2>
      <div class="w-[85%] mt-12">
        <p class="text-white text-6xl tracking-wide leading-normal font-extrabold">
          I explain and teach tech­nol­o­gy, solve tech prob­lems and help you make gad­get buy­ing decisions.
        </p>
      </div>
      <div class="flex flex-row w-full mt-40 justify-between items-center">
        <h1 class="text-white font-bold text-2xl tracking-wider">SUBSCRIBE TO OUR NEWSLETTER</h1>
        <hr class="w-[300px] text-white">
      </div>
      <div class="flex flex-row w-full mt-5 justify-between items-center">
        <div v-if="!showMessage" class="flex flex-row pb-9 space-x-2">
          <input v-model="email" type="text" placeholder="Email address"
            class="bg-white w-[550px] px-5 rounded text-xl py-4" @keydown.enter="submitForm">
          <button @click="submitForm" class="bg-green-600 text-white px-14 rounded py-1 text-xl">Submit</button>
        </div>
        <div v-else class="flex flex-row pb-9 space-x-2">
          <p class="flex justify-end text-slate-300 font-extrabold text-lg">Thank you for contacting us, we'll get to you
            shortly.</p>
        </div>
        <div class="flex flex-col space-y-2 pb-9">
          <p class="flex justify-end text-green-600 font-extrabold text-4xl">125.000</p>
          <p class="text-white font-bold text-2xl tracking-wider">JOIN THE LIST OF SUBSCRIBERS</p>
        </div>
      </div>
    </div>

  </div>
  <Slidelogo />
  <Imagecard />
  <Logocard />
  <Card />
  <div class="bg-purple min-h-screen object-cover object-center bg-no-repeat">
    <Footer />
  </div>
</template>



<style scoped></style>
