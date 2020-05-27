<template>
<div class="contact max">
    <h1>Contact</h1>
    <form name="Contact" method="POST" data-netlify="true" data-netlify-honeypot="bot-field">
      <input type="hidden" name="form-name" value="contact" />
        <input type="text" name="name" placeholder="Name"/>   
        <input type="email" name="email" placeholder="Email"/>
        <textarea name="message" placeholder="Message"></textarea>
        <div class="form-btn"><button type="submit">SUBMIT</button></div>
    </form>
</div>
</template>

<script>
export default {
  name: 'Contact',
}
</script>