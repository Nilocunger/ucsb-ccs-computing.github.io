<section>
  <h2>Sample Faculty Profiles</h2>
  <div id="students-container">
    {% for person in site.faculty %}
      <div class="student-tombstone">
        <div class="student-image">
          <img src="{{ person.url }}/300h.jpg" class="bottom">
          <img src="{{ person.url }}/300h_b.jpg" class="top">
        </div>
        <div class="student-tag">{{ person.name }}</div>
      </div>
    {% endfor %}
  </div>
</section>
