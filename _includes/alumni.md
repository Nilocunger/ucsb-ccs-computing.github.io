<section>
  <h2>Sample Alumni Profiles</h2>
  <div id="students-container">
    {% for alum in site.alumni %}
      <div class="student-tombstone">
        <div class="student-image">
          <img src="{{ alum.url }}/300h.jpg" class="bottom">
          <img src="{{ alum.url }}/300h_b.jpg" class="top">
        </div>
        <div class="student-tag">{{ alum.name }}</div>
        <div class="student-tag">{{ alum.affiliation }}</div>
      </div>
    {% endfor %}
  </div>
</section>
