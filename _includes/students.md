
<h1>Student Profiles</h1>

<div class="profilecontainer">
{% for student in site.students %}
  <a href="{{student.url}}">
    <div class="profile">
      <div class="profile-pic">
        <img src="{{ student.url }}/300h.jpg">
      </div>
      <div>
        {{student.name}}
        <br/>
        {{student.year}}
      </div>
    </div>
  </a>
{% endfor %}
</div>
