---
layout: default
---

<h1 class="f2 fw7 nunito blue ma0">{{ site.title }}</h1>
<p>NodeSchool San Salvador es un evento gratuito dedicado a ayudar a que más personas aprendan programación a través de JavaScript. Ayudamos a personas de todos los niveles, desde principiantes hasta expertos, a descubrir lo que es posible con JavaScript.</p>
<p>¡Acércate, trae tu computadora y el deseo de aprender a nuestro próximo evento!</p>

<section class="mv5">
  
  {% for event in site.data.events limit:1 %}
  {% if event.status %}
  <h3 class="f4 nunito mb1">Próximo evento:</h3>
    <div class="bg-blue ph4 pv3">
    <p class="f3 mv2 white">Fecha: {{ event.date }}</p>
    <p class="f3 mv2 white">Lugar: <a class="white" href="{{ event.venue_link }}">{{ event.venue_label }}</a></p>
    <div class="db mv3">
      <a class="event-link dib f4 blue bg-white mr2 ph3 pv2" href="{{ event.attendant_link }}">Registrarme como estudiante</a>
      <a class="event-link dib f4 white bg-blue ph3 pv2" href="{{ event.mentor_link }}">Registrarme como mentor</a>
    </div>
  </div>
  {% else %}
    <p>No hay eventos próximamente.</p>
  {% endif %}
  {% endfor %}
  
</section>

<section class="mv5">
  <h2 class="f2 nunito mv0">Preguntas frecuentes</h2>
  <div class="pb3 bb b--light-gray">
    <h3 class="fw6">¿Qué debo traer?</h3>
    <p>Necesitas tu laptop y ganas de aprender junto a otras personas.</p>
  </div>
  <div class="pb3 bb b--light-gray">
    <h3 class="fw6">¿Cuál es el costo de la entrada?</h3>
    <p>¡NodeSchool San Salvador es gratis!</p>
  </div>
  <div class="pb3 bb b--light-gray">
    <h3 class="fw6">¿Quiénes son los organizadores?</h3>
    <p>Ricardo Ramírez (<a href="https://twitter.com/ricardoerl">@ricardoerl</a>), Daniel Reyes (<a href="https://twitter.com/drmartinix">@drmartinix</a>), Gary Torres (<a href="https://twitter.com/GaryTorres_">@GaryTorres_</a>) y gran parte de la comunidad de <a href="https://www.facebook.com/groups/horchatajs/">HorchataJS</a>.</p>
  </div>
  <div class="pb3 bb b--light-gray">
    <h3 class="fw6">¿Qué sucede en un evento de NodeSchool San Salvador?</h3>
    <p>En general, los eventos de NodeSchool San Salvador son una oportunidad para reunirse con otros estudiantes y mentores en un entorno amigable y de aprendizaje. Así se ve normalmente el calendario de nuestro evento:</p>
    <ul>
      <li>3:00 - Puertas abiertas</li>
      <li>3:30 - Introducción / Indicaciones</li>
      <li>3:40 - Desarrollo de talleres / Tutoría</li>
      <li>4:30 - ¡Refrigerio!</li>
      <li>5:25 - Foto grupal</li>
      <li>5:30 - Fin del evento</li>
    </ul>
  </div>
  <div class="pb3 bb b--light-gray" id="mentores">
    <h3 class="fw6">¿Como puedo participar como mentor?</h3>
    <p>Los requisitos son los siguientes:</p>
    <ol>
      <li>Completar el <a href="https://www.github.com/sethvincent/javascripting">workshopper de javascripting</a> (cualquier <a href="https://nodeschool.io/#workshopper-list">otro workshopper</a> adicional es un plus)</li>
      <li>Leer <a href="https://github.com/nodeschool/organizers/wiki/Event-Mentor-Best-Practices">Mentor Best Practices</a></li>
      <li>Leer nuestro <a href="https://github.com/devs-sv/codigo-de-conducta">código de conducta</a></li>
      <li>Notificar a algunos organizadores del evento</li>
      <li>Presentarse media hora antes del evento para una reunion de mentores</li>
    </ol>
  </div>
</section>

<section class="mv5">
  <p>Agradecimientos a <a href="https://www.behance.net/leae10">Lea</a> por su ayuda con el logo de NodeSchool San Salvador.</p>
</section>