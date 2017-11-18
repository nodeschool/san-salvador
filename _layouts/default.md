<!DOCTYPE html>
<html lang="{{ page.lang | default: site.lang | default: " en " }}">

{% include head.html %}

<body>

  <div class="mw8 center pt4">
    <div class="cf ph2">
      <div class="fl w-100 w-30-ns pa2">
        {% include header.html %} 
      </div>
      <div class="fl w-100 w-70-ns pa2">
        {{ content }}
      </div>
    </div>
  </div>
  
  {% include footer.html %}

</body>

</html>