<template>
    <section id="contact">
      <h2>Contact Me</h2>
      <form action="mailto:savinpark0315@gmail.com" method="post">
        <input type="text" placeholder="Name" />
        <input type="email" placeholder="Email" />
        <textarea placeholder="Message"></textarea>
        <button type="submit">Send</button>
      </form>
    </section>
  </template>
  
  <script>
  export default {
    name: "ContactSection",
  };
  </script>
  
  <style scoped>
  form {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  textarea {
    resize: none;
  }
  </style>
  