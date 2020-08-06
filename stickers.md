---
layout: default
permalink: /stickers.html
---

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
                <a href="{{ item.src }}" class="card-link">Download</a>
            </div>
        </div>
    </div>
    {% endfor %}

</div>
