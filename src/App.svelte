<script>
// @ts-nocheck

  import { onMount } from 'svelte';
  import gsap from 'gsap';

  onMount(() => {
    gsap.from(".fade-in", { opacity: 0, y: 50, duration: 1, stagger: 0.3 });
    gsap.from(".cta-button", { scale: 0.8, opacity: 0, duration: 1, delay: 1 });
  });
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Rockwell&display=swap');

  body {
    font-family: 'Rockwell', serif;
    margin: 0;
    padding: 0;
    background-color: #0A1224;
    color: white;
    text-align: center;
  }
  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    padding: 20px;
  }
  .logo {
    width: 150px;
    margin-bottom: 20px;
  }
  h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
  }
  .cta-button {
    padding: 15px 30px;
    font-size: 1.2rem;
    background-color: #EC1F25;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background 0.3s;
  }
  .cta-button:hover {
    background-color: #C81A1E;
  }
</style>

<div class="container">
  <img src="./assets/logo.svg" alt="La Voz Querétaro" class="logo fade-in" />
  <h1 class="fade-in">🎙️ Bienvenidos a La Voz Querétaro</h1>
  <p class="fade-in">Tu fuente confiable de noticias, política y deportes en Querétaro.</p>
  <button class="cta-button" href="https://www.instagram.com/la_voz_queretaro">Escúchalo ahora</button>
</div>