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
<center>
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
    <br>Kay or Josh Harmon, 141 S. 6th Ave, Unit 42, Tucson, Az 85702 </h5><br><br>
    <a href="https://64f686283e38133f8e1183ea--wonderful-swan-0c6557.netlify.app/" class="link_button2">links</a><br><br>
    <a href="https://form.jotform.com/232398357846168" class="link_button2">apply</a><br><br>
    <a href="https://us21.list-manage.com/contact-form?u=c2c0f20a2043f1dd6472ffd6c&form_id=0bd25ece95a2940d5a4ca8ac7ed827c7" class="link_button2">send message</a><br>
</center>
  </div>
</body>
</template>
<style>

.link_button2 {
  -webkit-border-radius: 4px;
  -moz-border-radius: 4px;
  border-radius: 4px;
  border: solid 1px #1A4575;
  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.4);
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.4), 0 1px 1px rgba(0, 0, 0, 0.2);
  -moz-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.4), 0 1px 1px rgba(0, 0, 0, 0.2);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.4), 0 1px 1px rgba(0, 0, 0, 0.2);
  background: #3A68A1;
  color: #fee1cc;
  text-decoration: none;
  padding: 8px 12px;
  text-decoration: none;
  font-size: larger;
}
a.link_button2:hover {
  text-decoration: underline;
  background: #4479BA;
  border: solid 1px #20538D;
  /*
  text-shadow: 0 -1px 0 rgba(0, 0, 0, 0.7);
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.7), 0 1px 1px rgba(0, 0, 0, 0.4);
  -moz-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.7), 0 1px 1px rgba(0, 0, 0, 0.4);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.7), 0 1px 1px rgba(0, 0, 0, 0.4);
  */
}
</style>
