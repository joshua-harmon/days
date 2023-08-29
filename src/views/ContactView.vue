<script>
import {setPageTitle, setPageMetaData} from '@/seo';

export default {
  name: "ContactView",
  setup() {
    setPageTitle('Contacto - Vue Seo');
    setPageMetaData([
      {
        name: "description",
        content: "¿Tienes alguna duda? ¡Contacta con nosotros!)"
      }
    ])
  }
}
</script>

<template>

  <li><a href="https://preeminent-selkie-6b43a6.netlify.app">menu</a></li>
</template>
