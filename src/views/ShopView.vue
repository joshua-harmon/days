<script>
import {setPageTitle, setPageMetaData} from '@/seo';

export default {
  name: "ShopView",
  setup() {
    setPageTitle("Tienda - Vue Seo");
    setPageMetaData([
      {
        name: "description",
        content: "En la tienda tenemos cursos offline para que una vez los compres los puedas descargar para ver sin conexión"
      }
    ]);
  }
}
</script>

<template>

</template>
