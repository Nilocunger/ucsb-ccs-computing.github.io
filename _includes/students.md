<section>
  <h2>Sample Student Profiles</h2>
  <div id="students-container">
    {% for student in site.students %}
      <div class="student-tombstone">
        <div class="student-image">
          <img src="{{ student.url }}/300h.jpg" class="bottom">
          <img src="{{ student.url }}/300h_b.jpg" class="top">
        </div>
        <div class="student-tag">{{ student.name }}</div>
      </div>
    {% endfor %}
  </div>
</section>
