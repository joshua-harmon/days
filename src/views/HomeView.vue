<script>
import {setPageTitle, setPageMetaData} from '@/seo';

export default {
  name: "HomeView",
  setup() {
    setPageTitle('Inicio - Vue Seo');
    setPageMetaData([
      {
        name: "description",
        content: "Bienvenid@ a nuestra plataforma, estamos seguros que el material te va a ayudar mucho"
      }
    ]);
  }
}
</script>

<template>
  <body>
  <div class="hello">
    <h2>{{ msg }}</h2>

<h3 style = "color:green">    <br>Working with employment opportunities in: </h3>
<h4 style = "color:magenta">   
    <br>Sales
    <br>Engineering (all disciplines)<br> Management (all categories) 
    <br>Construction Management 
    <br>Entry level employment
    <br>Merit advancement </h4>
<h3 style = "color:green">
    <br>Professional positions based upon experience and education
    <br>Self-employment by becoming a working COOP member </h3>
    <h5 style = "color:brown">
    <br>CALL (520) 300-6340, nk@World-of-work-services-coop.com
    <br>Kay or Josh Harmon, 141 S. 6th Ave, Unit 42, Tucson, Az 85702 </h5>
    <form action="https://formsubmit.co/joshua.harmon1960@gmail.com" method="POST">
     <input type="text" name="name" required>
     <input type="email" name="email" required>
     <button type="submit">Send</button>
</form>
    <li><a href="https://64f686283e38133f8e1183ea--wonderful-swan-0c6557.netlify.app/">links</a></li>
  </div>
</body>
</template>
