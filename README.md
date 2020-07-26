---
layout: default
---

<div class='container'>
  <div class='row'>
    <div class='col col-md-12 catchphrase'>
      Er du kreativ, men mangler værkstedet?
    </div>
  </div>
</div>


<div class='container'>
  <div class='row'>
{% for feature in site.data.features %}
    <a class='col col-4 col-md-3 feature_col' href='{{feature.url}}'>
      <div class=feature>
        <div class='feature_heading'>{{feature.name}}</div>
        {% if feature.resize %}
          <div class='feature_illustration'>
            <img class='feature_img' src='assets/images/features/{{feature.img}}' style='max-width: {{feature.resize}}; max-height: {{feature.resize}};'>
          </div>
        {% else  %}
          <div class='feature_illustration'>
            <img class='feature_img' src='assets/images/features/{{feature.img}}'>
          </div>
        {% endif  %}
        <div class='feature_description'>
        </div>
      </div>
    </a> <!-- end col -->

{% endfor %}
  </div> <!-- end row -->
</div>


<div class='container'>
  <div class='row'>
    <div class='col col-md-12 bliv_medlem'>
      Bliv medlem for 200 kr/md (studerende 100kr/md) og få adgang døgnet rundt, eller deltag gratis i vores åbne arrangementer.
    </div>
  </div>
</div>
