<template>
<div class="contact max">
    <h1>Contact</h1>
    <form name="contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field">
      <input type="hidden" name="form-name" value="contact" />
        <input type="text" name="name" placeholder="Name"/>   
        <input type="email" name="email" placeholder="Email"/>
        <textarea name="message" placeholder="Message"></textarea>
        <p><button type="submit">Send</button></p>
    </form>
</div>
</template>

<script>
export default {
  name: 'Contact',

}
</script>