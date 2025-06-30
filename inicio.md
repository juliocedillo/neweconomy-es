---
layout: default
title: Inicio
permalink: /
---

<div style="position: relative; width: 100%; height: 60vh; overflow: hidden;">
  <img src="https://juliocedillo.github.io/neweconomy/assets/images/pediment.png" alt="header" style="width: 100%; height: 100%; object-fit: cover; border: none;">
  <div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); color: white; font-size: 24px; font-weight: bold; text-align: center; max-width: 80%; line-height: 1.4;">
    ¿Qué pasaría si las reglas que definieron los últimos 40 años de la historia económica fueran desarrollos únicos y contingentes históricamente que ahora están llegando rápidamente a su fin?
  </div>
</div>

<p>&nbsp;&nbsp;&nbsp;</p>

Armando Lara-Millán está escribiendo un libro titulado tentativamente The Firm That Predicted the Future and the Birth of a New Global Economy (La empresa que predijo el futuro y el nacimiento de una nueva economía global). El libro argumenta que, durante los últimos cuarenta años, cinco dinámicas político-económicas globales fueron en su mayoría equivocadamente tomadas como las nuevas reglas permanentes de la economía globalizada. En cambio, eran desarrollos únicos y contingentes históricamente que ahora están cambiando rápidamente. Emparejando un estudio cualitativo de una firma de inversión clave con el procesamiento de lenguaje natural de décadas de informes trimestrales corporativos, Lara-Millán detalla el fin de la mano de obra barata en China, la transición de sectores de alto crecimiento a sectores cíclicos beneficiarios de Internet, el paso de la energía barata a las materias primas caras, la imposibilidad de seguir reduciendo los impuestos corporativos y el costo del endeudamiento corporativo, y el papel incierto de la política monetaria performativa. El libro ofrece una forma de entender nuestra supuesta "policrisis" para comprender mejor cómo un nuevo orden está luchando por nacer en el presente.

<p>&nbsp;&nbsp;&nbsp;</p>

---

|Meta|Método|Impacto|
|---|---|---|
|Nuestro proyecto investiga el fin de la mano de obra barata en China y el dinero fácil en Silicon Valley, las exploraciones desesperadas de depósitos de cobre y litio en antiguos campos de petróleo y carbón, hasta los juegos de lenguaje de los banquero centrales en Jackson Hole y el Banco Central Europeo.|Tejiendo etnografías de firmas clave de gestión de activos, entrevistas con empleadores y empleados en sectores clave de todo el mundo, y procesamiento de lenguaje natural de décadas de informes trimestrales de todas las principales corporaciones, el proyecto *El Futuro de la Economía Global* trabaja para entender cómo un nuevo orden global está luchando por nacer en el presente.|Al historicizar los últimos 40 años, se entrelazan argumentos dispares sobre el “neoliberalismo”, la “financiarización” y la “hiperglobalización”. De este modo, esperamos dar sentido a nuestra “policrisis” contemporánea y comprender cómo un nuevo orden global está luchando por nacer en el presente.|

---

<p>&nbsp;&nbsp;&nbsp;</p>

<h1 style="text-align: center;">Dinámicas que estamos investigando</h1>

<!-- HTML for the Carousel -->
<div class="carousel">
  <div class="carousel-container">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy-es/assets/images/q1_es.png" alt="Image 1">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy-es/assets/images/q2_es.png" alt="Image 2">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy-es/assets/images/q3_es.png" alt="Image 3">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy-es/assets/images/q4_es.png" alt="Image 4">
    <img class="carousel-slide" src="https://juliocedillo.github.io/neweconomy-es/assets/images/q5_es.png" alt="Image 5">
  </div>
  <button class="carousel-prev" onclick="moveSlide(-1)">&#10094;</button>
  <button class="carousel-next" onclick="moveSlide(1)">&#10095;</button>
</div>

<!-- CSS for styling the Carousel -->
<style>
  .carousel {
  position: relative;
  max-width: 800px;
  margin: auto;
  overflow: hidden;
  }

  .carousel-container {
    display: flex;
    transition: transform 0.5s ease;
  }

  .carousel-slide {
    width: 800px;
    flex-shrink: 0;
    display: block;
  }

  .carousel-prev, .carousel-next {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba(0, 0, 0, 0.5);
    color: white;
    border: none;
    padding: 16px;
    cursor: pointer;
    z-index: 10;
  }

  .carousel-prev {
    left: 0;
  }

  .carousel-next {
    right: 0;
  }
</style>

<script>
  let currentIndex = 0;

  function moveSlide(direction) {
    const slides = document.querySelectorAll('.carousel-slide');
    const totalSlides = slides.length;

    currentIndex = (currentIndex + direction + totalSlides) % totalSlides;

    updateSlidePosition();
  }

  function updateSlidePosition() {
    const slides = document.querySelectorAll('.carousel-slide');
    if (slides.length === 0) return;
    const slideWidth = slides[0].offsetWidth;
    document.querySelector('.carousel-container').style.transform =
      `translateX(-${currentIndex * slideWidth}px)`;
  }

  // Ensure layout is calculated before applying transform
  window.addEventListener('DOMContentLoaded', () => {
    setTimeout(updateSlidePosition, 100);
  });
</script>
