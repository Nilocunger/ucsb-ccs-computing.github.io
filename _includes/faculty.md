<h1>Faculty Profiles</h1>

<div class="profilecontainer">
{% for faculty in site.faculty %}
  <a href="{{ faculty.url }}">
    <div class="profile">
      <div class="profile-pic">
        <img src="{{ faculty.url }}/300h.jpg">
      </div>
      <div>
        {{faculty.name}}
      </div>
    </div>
  </a>
{% endfor %}
</div>
