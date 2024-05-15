<h2 id="experience" style="margin: 2px 0px -15px;">Experience</h2>

<div class="experience">
  <ol class="experiences">

    {% for exp in site.data.experience.main %}

    <li>
      <div class="exp-row">
        <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
          {% if exp.logo %} 
          <img src="{{ exp.logo }}" class="logo img-fluid z-depth-1" style="width=100;height=40%">
          {% endif %}
          {% if exp.company_short %} 
          <abbr class="badge">{{ exp.company_short }}</abbr>
          {% endif %}
        </div>
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="position">{{ exp.position }}</div>
          <div class="company">{{ exp.company }}</div>
          <div class="duration"><em>{{ exp.duration }}</em>
          </div>
          <div class="details">
            <ul>
              {% for detail in exp.details %}
              <li>{{ detail }}</li>
              {% endfor %}
            </ul>
          </div>
        </div>
      </div>
    </li>

    <br>

    {% endfor %}

  </ol>
</div>

