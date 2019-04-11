
<h1>Alumni Profiles</h1>

<div class="profilecontainer">
{% for alum in site.alumni %}
  <a href="{{ alum.url }}">
    <div class="profile">
      <div class="profile-pic">
        <img src="{{ alum.url }}/300h.jpg">
      </div>
      <div>
        {{alum.name}}
        <br/>
        {{alum.affiliation}}
        <br/>
        {{alum.city}}
      </div>
    </div>
  </a>
{% endfor %}
