<script>
import {setPageTitle, setPageMetaData} from '@/seo';
export default {
  name: "",
  setup() {
    setPageTitle("");
    setPageMetaData([
      {
        name: "",
        content: ""
      }
    ])
  }
}
</script>
<script setup>
import { reactive } from 'vue'

const formData = reactive({
  name: '',
  email: '',
  message: '',
  response: ''
})

const encode = data => {
  return Object.keys(data)
    .map(key => `${encodeURIComponent(key)}=${encodeURIComponent(data[key])}`)
    .join('&')
}

const submitForm = () => {
  fetch('/', {
    method: 'POST',
    headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
    body: encode({
      'form-name': 'feedback',
      ...formData
    })
  })
    .then(() => {
      formData.response = '✅ Your response was successfully submitted!'
    })
    .catch(error => {
      formData.response = `❌ There was an error submitting your response: ${error.message}. Please refresh to try again.`
    })
}
</script>

<template>
  <h1>Vue 3 + Netlify Forms</h1>

  <section v-if="formData.response" class="notification">
    <h2>{{ formData.response }}</h2>
  </section>
  <form v-else class="feedback-form" name="feedback" @submit.prevent>
    <input type="hidden" name="form-name" value="feedback" />

    <div class="input-wrapper">
      <label for="name">Name</label>
      <input
        id="name"
        v-model="formData.name"
        type="text"
        placeholder="Your Name"
      />
    </div>

    <div class="input-wrapper">
      <label for="email">Email</label>
      <input
        id="email"
        v-model="formData.email"
        type="email"
        placeholder="yourname@domain.extension"
      />
    </div>

    <div class="input-wrapper">
      <label for="message">Message</label>
      <textarea
        id="message"
        v-model="formData.message"
        placeholder="What would you like to share?"
      />
    </div>

    <button type="submit" @click="submitForm">Submit</button>
  </form>


        <form name="contact" method="POST" data-netlify="true">
  <p>
    <label>Your Name: <input type="text" name="name" /></label>
  </p>
  <p>
    <label>Your Email: <input type="email" name="email" /></label>
  </p>
  <p>
    <label>Your Role: <select name="role[]" multiple>
      <option value="leader">Leader</option>
      <option value="follower">Follower</option>
    </select></label>
  </p>
  <p>
    <label>Message: <textarea name="message"></textarea></label>
  </p>
  <p>
    <button type="submit">Send</button>
  </p>
</form>
</template>

