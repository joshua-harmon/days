<script>
import {setPageTitle, setPageMetaData} from '@/seo';

export default {
  name: "MembershipsView",
  setup() {
    setPageTitle("Membresías - Vue Seo");
    setPageMetaData([
      {
        name: "description",
        content: "Las membresías de la plataforma te ofrecen acceso completo"
      }
    ])
  }
}
</script>
<template>
  <section id="farEast">
  <div class="box">
<ul id="bookmarks">
  <li><a href="#">moreFood</a>
   <ul class= "sites">
    <li><a href="https://www.youtube.com/watch?v=kcSZ22ZY8Qs&feature=youtu.be">eggsBenedict</a></li>
    <li><a href="https://www.youtube.com/watch?v=Zg-89wuPfVc">ramen</a></li>  
    <li><a href="https://www.youtube.com/watch?v=NmH7XzvuaAI">spcyRmen</a></li>  
    <li><a href="https://www.youtube.com/watch?v=_SpkOoN9oiE">mkeRamen</a></li>  
    <li><a href="https://www.youtube.com/watch?v=fT14pV6oxvI">wonton</a></li> 
    <li><a href="https://www.youtube.com/watch?v=zdk0bF20Bj8">veganPho</a></li>  
    <li><a href="https://www.youtube.com/watch?v=MN8Mv63BePs">tofuNdls</a></li>  
    <li><a href="https://www.youtube.com/watch?v=zdk0bF20Bj8">veganPho</a></li>  
    <li><a href="https://www.youtube.com/watch?v=EAp87u65snM">twoKago</a></li> 
    <li><a href="https://www.youtube.com/watch?v=2Lgq3EOfU50">shzSauce</a></li>  
  </ul>
 </li>
  <li><a href="#">sushi</a>
   <ul class= "sites">
    <li><a href="https://www.youtube.com/results?search_query=make+sushi">sushi</a></li> 
    <li><a href="https://www.youtube.com/watch?v=zmljfxmZTrs">moreSushi</a></li>  
  </ul>
 </li>
 </ul>
</div>
</section>
</template>
