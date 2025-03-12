<script>
  import { onMount } from 'svelte';
  import gsap from 'gsap';

  onMount(() => {
    gsap.from(".fade-in", { opacity: 0, y: 50, duration: 1, stagger: 0.3 });
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
  h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
  }
  .cta-link {
    display: inline-block;
    padding: 15px 30px;
    font-size: 1.2rem;
    background-color: #EC1F25;
    color: white;
    border-radius: 5px;
    text-decoration: none;
    transition: background 0.3s;
  }
  .cta-link:hover {
    background-color: #C81A1E;
  }
</style>

<div class="container">
  <h1 class="fade-in">🎙️ Bienvenidos a La Voz Querétaro</h1>
  <p class="fade-in">Tu fuente confiable de noticias, política y deportes en Querétaro.</p>
  <a href="https://www.instagram.com/la_voz_queretaro/" class="cta-link fade-in" target="_blank">Escúchalo ahora</a>
</div>