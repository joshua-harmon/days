<template>
  <netlify-form name='Contact' :form='form'>
    <template #default='{readonly, submitting, submitted}'>
      <p v-if='submitted'>Thanks for your submission</p>
      <input
        name='Email'
        placeholder='Email'
        v-model='form.Email'
        :readonly='readonly'>
      <button>
        {{ submitting ? 'Submitting' : 'Submit' }}
      </button>
  </netlify-form>
  <form name="fileForm" enctype="multipart/form-data" data-netlify="true">
  <p>
    <label>
      <span>Name:</span>
      <input name="name" type="text"/>
    </label>
  </p>
  <p>
    <label>
      <span>Add file:</span>
      <input name="file" type="file"/>
    </label>
  </p>
  <button>Submit</button>
</form>
<p class="result"></p>
</template>
<script>
export default {
  data: function() {
    form: {
      Email: ''
    }
  }
}
</script>
  
