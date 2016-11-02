---
layout: default
title: "People"
---

# People

## PI
<div class="table-responsive">
  <table class="table table-striped table-bordered table-hover table-responsive">
    <thead>
      <tr>
        <th>Name</th>
        <th>Email</th>
        <th>Website</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="name">{{site.data.people.pi.name}}</td>
        <td class="email">{{site.data.people.pi.email | replace: '@', ' åt '}}</td>
        <td class="site"><a target="_blank" href="{{site.data.people.pi.website}}">{{site.data.people.pi.website}}</a></td>
      </tr>
    </tbody>
  </table>
</div>

## Independent Researchers and Visitors
<div class="table-responsive">
  <table class="table table-striped table-bordered table-hover table-responsive">
    <thead>
      <tr>
        <th>Name</th>
        <th>Email</th>
        <th>Website</th>
      </tr>
    </thead>
    <tbody>
      {% for person in site.data.people.indep_visitors %}
        <tr>
          <td class="name">{{person.name}}</td>
          <td class="email">{{person.email | replace: '@', ' åt '}}</td>
          <td class="site"><a target="_blank" href="{{person.website}}">{{person.website}}</a></td>
        </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

## Postdocs
<div class="table-responsive">
  <table class="table table-striped table-bordered table-hover table-responsive">
  <thead>
    <tr>
      <th>Name</th>
      <th>Email</th>
      <th>Website</th>
    </tr>
  </thead>
  <tbody>
    {% for person in site.data.people.postdocs %}
      <tr>
        <td class="name">{{person.name}}</td>
        <td class="email">{{person.email | replace: '@', ' åt '}}</td>
        <td class="site"><a target="_blank" href="{{person.website}}">{{person.website}}</a></td>
      </tr>
    {% endfor %}
  </tbody>
  </table>
</div>

## Graduate Students
<div class="table-responsive">
  <table class="table table-striped table-bordered table-hover table-responsive">
  <thead>
    <tr>
      <th>Name</th>
      <th>Email</th>
      <th>Website</th>
    </tr>
  </thead>
  <tbody>
    {% for person in site.data.people.gradStudents %}
      <tr>
        <td class="name">{{person.name}}</td>
        <td class="email">{{person.email | replace: '@', ' åt '}}</td>
        <td class="site"><a target="_blank" href="{{person.website}}">{{person.website}}</a></td>
      </tr>
    {% endfor %}
  </tbody>
  </table>
</div>
