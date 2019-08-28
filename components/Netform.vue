<template>
<v-container>
<form name="contact" method="POST" data-netlify="true">
  <h1 class="title">
      Contact
  </h1>
  <p>
    <label>Nume: <input type="text" name="name" /></label>   
  </p>
  <p>
    <label>Email: <input type="email" name="email" /></label>
  </p>
  <p>
    <label>Mesaj: <textarea name="message"></textarea></label>
  </p>
  <p>
    <button type="submit">Trimite</button>
  </p>
</form>
</v-container>
</template>

<style scoped>
.title {
  margin-bottom: 20px;
}
form {
  margin-left: auto;
  margin-right: auto;
  justify-content: center;
  
  width:100%;
    max-width: 900px;
    margin:10px auto;
}

input, textarea, text{
    width: 900px;
    max-width: 100%;
    resize: none;
    background-color: #f4f5f8;
    height: 35px;
    border: 1px solid #171717
}

textarea{
    height: 200px;
}

form textarea, input{
  padding:5px;
}

form button{
    background: #0288D1;
    font-weight: bold;
    text-transform: uppercase;
    padding: 10px 20px;
    font-size: 18px;
    border:none;
    color:#fff;
}
</style>