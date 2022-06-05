---
layout: splash
#layout: home
header:
  overlay_color: "#001233"
  overlay_filter: "0.2"
  overlay_image: "assets/images/imper_mar.jpg"
  actions:
    - label: "Lea más sobre nosotros"
      url: "/soluciones" 
  caption: "<a href='https://wa.me/34722540848/' target='_blank'><img src='assets/images/wa.png' width='42'> WhatsApp: (+34) 722 00 00 00</a>"
excerpt: "En Mallorca, te ofrecemos las mejores **soluciones** con un servicio serio, **competente** y de elevada **calidad**."
intro: 
  # Esto es un CallOut
  - excerpt: '<big>Nuestras áreas de negocio ofrecen soluciones para usted y su <a href="/soluciones">empresa</a> tanto si necesita presentar <a href="/licencias-de-actividad">documentación</a> para su ayuntamiento, para <a href="/ecoingenieria">obras</a> y <a href="/ecoingenieria">reformas</a> o ha sufrido un <a href="/seguros">siniestro</a> y necesita pasar a la acción. Conozca <a href="/soluciones">INPER Ingeniería</a> y <a href="/contacto">contacte</a> con nosotros sin compromiso.</big>'
frase1: 
  - excerpt: '<div style="font-size: 2em;">¿Sabe usted...?</div><big>La actividad de INPER Ingeniería se focaliza en los <a href="/seguros">Sectores Asegurador</a>, <a href="/licencias-de-actividad">Licencias de Actividad</a>, <a href="/ecoingenieria">Instalaciones de Energías Renovables</a></big><br>'
feature_row:
  - image_path: assets/images/imper_solar.png
    alt: "INPER Eco-ingeniería & Instalaciones"
    title: "INPER Eco-Ingeniería e Instalaciones"
    excerpt: "<a href='ecoingenieria#proyectos-y-anteproyectos'>Proyectos y Anteproyectos</a>
    <br><a href='ecoingenieria#control-de-calidad'>Control de calidad</a>
    <br><a href='ecoingenieria#legalizaci%C3%B3n-de-instalaciones'>**Legalización** de instalaciones</a>
    "
  - image_path: assets/images/imper_sol.png
    image_caption: "Servicios a toda [Mallorca](#top): todos los ayuntamientos."
    alt: "INPER Licencias de Actividad y Autorizaciones"
    title: "INPER Licencias de Actividad y Autorizaciones"
    excerpt: "
     <a href='licencias-de-actividad#autorizaciones-y-permisos'>Licencias de actividad</a><br>
     <a href='licencias-de-actividad#permisos-de-reformas-para-su-vivienda-o-local-comercial'> Permisos de **REFORMAS** para su vivienda o local comercial</a> 
    <br><a href='licencias-de-actividad#memoria-de-actividad'>Proyectos de Actividad y Memorias</a>
    "
  - image_path: assets/images/imper_edificio.png
    alt: "INPER Seguros y Contraperitajes"
    title: "INPER Seguros y Contraperitajes"
    excerpt: "<a href='seguros#sector-asegurador'>Sector Asegurador</a>
    <br><a href='seguros#segunda-opini%C3%B3n-y-peritaje-de-parte'>Segunda opinión y peritaje de parte</a>
    <br><a href='seguros#compromiso-con-nuestros-clientes'>Compromiso con nuestros clientes</a>
    "
guia_1:
  - image_path: assets/images/imper_economia.png
    alt: "GUÍA ELEMENTAL"
    title: "Licencias de Apertura y Actividad: ¿Necesito una?"
    excerpt: 'La Licencia de Actividad es la **autorización** municipal sobre un **PROYECTO** para el inicio de obras e instalaciones en un local. La Licencia de Apertura, o de funcionamiento, la concede su ayuntamiento teniendo en cuenta la Licencia de actividad previamente concedida. <br><br>
    INPER Ingeniería puede ayudarle en el proceso de creación y legalización de su empresa. Consulte <a href="#">aquí</a> y <a href="#">aquí</a> el listado de completo de servicios que le ofrecemos. O siga leyendo nuestra **selección de preguntas y respuestas habituales**: 
'
    url: "/necesito-una-licencia"
    btn_label: "Lea: Licencias y Permisos desde cero"
    btn_class: "btn--primary"
call_out:
  - image_path: assets/images/imprer_persona_1.png
    excerpt: "<big class='align-center'>Estamos aquí para <strong>ayudarle</strong>.</big>"
    url: "/contacto"
    btn_label: "Contacte con Nosotros"
    btn_class: "btn--inverse btn--large align--center"


guia_2:
  - image_path: assets/images/imprer_agua.png
    alt: "GUÍA ELEMENTAL"
    title: "Tengo un conflicto con mi Compañía de Seguros o Comunidad de Vecinos ¿Ahora que hago?"
    excerpt: 'En caso de diferencias entre las partes no es necesario ir a juicio. Existen procesos más **ECONÓMICOS** y con plazos más cortos para lograr un acuerdo entre las partes. <br><br>
    INPER Ingeniería puede proporcionarle asesoramiento y una opinión profesional válida para la resolución de un litigio. Conozca nuestros catálogo de servicios completo (<a href="#">asesoramiento y contraperitajes</a>) o siga leyendo nuestra **guía de preguntas y respuestas habituales**:'
    url: "/seguro-sin-complicaciones"
    btn_label: "Lea: Su Seguro, sin complicaciones"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="frase1" type="center" %}

{% include feature_row %}

{% include feature_row id="guia_1" type="left" %}

{% include feature_row id="guia_2" type="left" %}

{% include feature_row id="call_out" type="center" %}

<h3 class="archive__subtitle">Prestamos Servicios a Toda Mallorca:</h3>
<div id='pueblos'>
<ul>
{% for p in site.data.pueblos %}
  <li>
    <a href="servicios-mallorca/{{ p.trim }}/">
      {{ p.nombre }} ➡ Ayuntamiento de {{ p.municipio }}
    </a>
  </li>
{% endfor %}
</ul>
</div>

<h3 class="archive__subtitle">{{ site.data.ui-text[site.localje].recent_posts | default: "Le puede interesar..." }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

<!--{% include paginator.html %}-->

<!---
Comentarios: 

<div class="notice notice--warning">
Eres un puto
</div>

<div class="notice notice--info">
Eres un puto
</div>

{: .notice--danger}
dsfdsafdasfdsfsdafdsfdsfsd

{% include feature_row id="feature_row4" type="center" %}


<script>
    console.log("hola mundo");
</script>

-->