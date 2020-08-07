---
layout: default
permalink: /signal
---

# Stickers para Signal

Signal es nuestra principal recomendación para chats seguros, y para darte la bienvenida a Signal estamos creando estos geniales paquetes de stickers.
¡Puedes descargar signal para Android, iPhone y tu computadora!

Recuerda que la seguridad de una app no es suficente, tienes que pdoer confiar en las personas con quién tienes conversaciones sensibles.

<div class="row">
    {% for item in site.data.stickers %}
    <div class="col-lg-3 col-md-4 col-sm-2 mt-4">
        <div class="card">
            <img src="{{ item.src-img }}" class="card-img-top" alt="{{ item.title }}" />
            <div class="card-body">
                <h5 class="card-title">{{ item.title }}</h5>
                <p class="card-text">
                {{ item.description }}
                </p>
                {% if item.src %}
                  <a href="{{ item.src }}" class="card-link">Descarga</a>
                {% endif %}
            </div>
        </div>
    </div>
    {% endfor %}

</div>
