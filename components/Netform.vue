<template>
<v-container>
<form
  action="https://formspree.io/xdokvpao"
  method="POST"
>
  <h2>Contact Us</h2>
  <label>
    <p>Your Name:</p>
    <input type="text" name="name">
  </label>
  <label>
    <p>Email:</p>
    <input type="text" name="_replyto">
  </label>
  <label>
    <p>Message:</p>
    <textarea name="message"></textarea>
  </label>

  <!-- your other form fields go here -->

  <button type="submit">Send</button>
</form>
</v-container>
</template>

<style scoped>
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
    background-color: white;
    height: 45px;
    border: 1px solid #171717;
    font-size: 21px;
}

textarea{
    height: 200px;
}

form textarea, input{
  padding:10px;
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

p {
  font-size: 20px;
  margin-top: 20px;
  margin-bottom: 0;
}
</style>

