<script setup>
function sendMessage(e) {
  e.preventDefault();
  const popup = document.querySelector('popup');
  const form = document.querySelector('form');
  popup.style.top = '0px';
  form.reset();
}

function hidePopup(e) {
  e.target.style.top = '-38px';
}
</script>

<template>
  <form>
    <popup @click="hidePopup">Message Sent Successfully!</popup>
    <div class="contacts">
      <input type="text" placeholder="Your name" />
      <input type="text" placeholder="Your email" />
    </div>
    <textarea cols="60" rows="10" placeholder="Your message"></textarea>
    <div class="contacts" style="margin-top: 25px">
      <div>
        <input type="checkbox" />
        <span>Send me a copy</span>
      </div>
      <button @click="sendMessage">Send a Message</button>
    </div>
  </form>
</template>

<style scoped>
popup {
  position: absolute;
  color: #000;
  top: 0;
  background: #acffac;
  padding: 10px;
  border-radius: 18px;
  top: -38px;
  transition: 300ms;
}

form {
  display: flex;
  flex-direction: column;
  max-width: fit-content;
  justify-content: center;
  align-items: center;
  margin: auto;
  color: #fff;
}

input {
  border: 1px solid #fff;
  border-radius: 18px;
  padding: 10px;
  background: none;
  opacity: 0.7;
  color: #fff;
}

textarea,
input:focus {
  outline: none;
}

textarea::placeholder,
input::placeholder {
  color: #fff;
}

textarea {
  margin-top: 25px;
  background: none;
  border: 1px solid #fff;
  opacity: 0.7;
  border-radius: 15px;
  resize: none;
  padding: 10px;
  color: #fff;
}

.contacts {
  display: flex;
  justify-content: space-between;
  width: 100%;
}

button {
  background-color: #ff0077;
  border: none;
  border-radius: 18px;
  padding: 10px;
  color: #fff;
}

button:hover {
  cursor: pointer;
}
</style>
