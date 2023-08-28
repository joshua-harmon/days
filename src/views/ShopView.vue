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

  
         
<template #default='{readonly, submitting, submitted}'>
  <netlify-form name='Contact' :form='form'>


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
