---
permalink: /soluciones/
title: "INPER Ingeniería"
sidebar:
  - image: assets/images/imprer_persona_2.png
    text: '<div style="font-size: 16px" id="p0">"Nuestra empresa ofrece un servicio serio, competente y de elevada calidad"<p style="font-style: italic;" class="align-right"><a href="/contacto">Gabriel Gimeno - CEO</a></p></div><p id="p1" class="ocultar-div"></p>'
author_profile: false
classes: wide
call_out:
  - image_path: assets/images/imprer_persona_1.png
    excerpt: "<big class='align-center'>Estamos aquí para <strong>ayudarle</strong>.</big>"
    url: "/contacto"
    btn_label: "Contacte con Nosotros"
    btn_class: "btn--inverse btn--large align--center"
gallery:
  - url: /assets/images/imper_familias.png
    image_path: /assets/images/imper_familias.png
  - url: /assets/images/imper_electricidad.png
    image_path: /assets/images/imper_electricidad.png
---

<style>

@media screen and (max-width: 600px) {
    .ocultar-div{
    display:none;
    }
  }
</style>

<h2>Soluciones {{ site.time | date: '%Y' }}</h2>

INPER  Ingeniería es una empresa formada por la unión de un grupo de Técnicos de Ingeniería y Arquitectura con muchos años de experiencia, que tienen como objetivo principal ofrecer al cliente un servicio serio, competente y de elevada calidad, ofreciendo las mejores soluciones a nuestros clientes..


{% include gallery %}

La alta profesionalidad y experiencia hacen que el cliente se sienta siempre satisfecho tanto a corto como a largo plazo.

Realizamos proyectos para licencias de actividades, planes de autoprotección, certificaciones de eficiencia energética, instalaciones de media y baja tensión, informes de evaluación del edificio (IEE), Infraestructura común de telecomunicaciones (ICT),  etc…

En nuestro gabinete estamos especializados, desde hace décadas, en la peritación general. Llevamos a cabo peritajes de todo tipo. Contamos con un equipo perito de seguros, embarcaciones de recreo, inmobiliarios, etc. 

Si necesita que nuestra empresa lleve a cabo cualquier peritación, contacte con nosotros. Contamos con un equipo altamente cualificado que le ofrecerá un servicio integral y profesional.

Entre nuestros muchos servicios, destacamos los siguientes:

* Peritación de daños
* Defectos constructivos
* Peritos de seguros

Cuente con nosotros y le ayudaremos en todo lo que esté en nuestra mano. 

{% include feature_row id="call_out" type="center" %}

Adicionalmente, ofrecemos a nuestros clientes un asesoramiento y una atención personalizada, prestando unos servicios que permitan al cliente prever y desarrollar sus actividades con garantías de seguridad, eficacia y rentabilidad.

Visión
======
Ser capaces de dar respuesta a las necesidades de nuestros clientes, creando y diseñando soluciones ad hoc a través de nuestros colaboradores.

Valores
=======
Los valores o principios éticos sobre los que se asienta la cultura de nuestra compañía y que nos permite crear nuestras pautas de comportamiento. Son los siguientes Confianza, Compromiso, Experiencia, Integridad e Ilusión.



<div id='pueblos'>
<h3 class="archive__subtitle">Prestamos Servicios a Toda Mallorca:</h3>
<ul>
{% for p in site.data.pueblos %}
  <li>
    <a href="/servicios-mallorca/{{ p.trim }}/">
      {{ p.nombre }}, {{ p.municipio }}
    </a>
  </li>
{% endfor %}
</ul>
</div>

<script>
window.onload = function() {
    let amigo = document.getElementById('pueblos');
    document.getElementById('p1').innerHTML=amigo.innerHTML;
    document.getElementById('pueblos').innerHTML="";
}
</script>