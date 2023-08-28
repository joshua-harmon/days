<template>
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
