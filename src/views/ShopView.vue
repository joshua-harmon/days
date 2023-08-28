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

    </template>
  </netlify-form>

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
