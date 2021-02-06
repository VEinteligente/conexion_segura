---
layout: default
permalink: /signal
---

<main class="container">
 <div class="row my-5">
  <div class="col-auto">
    <section class="mb-4">
      <h2 class="cs-h2 text-center">Stickers para Signal</h2>
    </section>

    <section class="text-justify">
      <p class="cs-text-indent">
        Signal es nuestra principal recomendación para chats seguros, y para
        darte la bienvenida a Signal estamos creando estos geniales paquetes de
        stickers. ¡Puedes <a href="https://signal.org/en/download/">descargar signal</a>
        para Android, iPhone y tu computadora!
      </p>

      <p class="cs-text-indent">
        Recuerda que la seguridad de una app no es suficiente, tienes que poder
        confiar en las personas con quién tienes conversaciones sensibles.
      </p>
    </section>
  </div>
 </div>

 <div class="row my-5">
  {% for item in site.data.stickers %}
  <div class="col-lg-4 col-md-3 col-sm-6 mt-4">
    <div class="card h-100">
      <img
        src="{{ item.src-img }}"
        class="card-img-top"
        alt="{{ item.title }}"
      />
      <div class="card-body">
        <h5 class="card-title">{{ item.title }}</h5>
        <p class="card-text">{{ item.description }}</p>
        {% if item.src %}
        <a
          href="{{ item.src }}"
          target="_blank"
          class="card-link btn btn-primary"
          ><svg
            width="1em"
            height="1em"
            viewBox="0 0 16 16"
            class="bi bi-cloud-download"
            fill="currentColor"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M4.406 1.342A5.53 5.53 0 0 1 8 0c2.69 0 4.923 2 5.166 4.579C14.758 4.804 16 6.137 16 7.773 16 9.569 14.502 11 12.687 11H10a.5.5 0 0 1 0-1h2.688C13.979 10 15 8.988 15 7.773c0-1.216-1.02-2.228-2.313-2.228h-.5v-.5C12.188 2.825 10.328 1 8 1a4.53 4.53 0 0 0-2.941 1.1c-.757.652-1.153 1.438-1.153 2.055v.448l-.445.049C2.064 4.805 1 5.952 1 7.318 1 8.785 2.23 10 3.781 10H6a.5.5 0 0 1 0 1H3.781C1.708 11 0 9.366 0 7.318c0-1.763 1.266-3.223 2.942-3.593.143-.863.698-1.723 1.464-2.383z"
            />
            <path
              fill-rule="evenodd"
              d="M7.646 15.854a.5.5 0 0 0 .708 0l3-3a.5.5 0 0 0-.708-.708L8.5 14.293V5.5a.5.5 0 0 0-1 0v8.793l-2.146-2.147a.5.5 0 0 0-.708.708l3 3z"
            />
          </svg>
          &nbsp; Instalar</a
        >
        {% endif %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>
</main>
