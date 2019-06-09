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
        <td class="email">
          <SCRIPT type='text/javascript'>
            a='{{site.data.people.pi.email | split: '@' | first}}';
            b='{{site.data.people.pi.email | split: '@' | last}}';
            document.write('<A hre'+'f="mai'+'lto:'+a+'@'+b+'">');
            document.write(a+'@'+b+'</a>');
          </SCRIPT>
        </td>
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
          <td class="email">
            <SCRIPT type='text/javascript'>
              a='{{person.email | split: '@' | first}}';
              b='{{person.email | split: '@' | last}}';
              document.write('<A hre'+'f="mai'+'lto:'+a+'@'+b+'">');
              document.write(a+'@'+b+'</a>');
            </SCRIPT>
          </td>
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
        <td class="email">
          <SCRIPT type='text/javascript'>
            a='{{person.email | split: '@' | first}}';
            b='{{person.email | split: '@' | last}}';
            document.write('<A hre'+'f="mai'+'lto:'+a+'@'+b+'">');
            document.write(a+'@'+b+'</a>');
          </SCRIPT>
        </td>
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
        <td class="email">
          <SCRIPT type='text/javascript'>
            a='{{person.email | split: '@' | first}}';
            b='{{person.email | split: '@' | last}}';
            document.write('<A hre'+'f="mai'+'lto:'+a+'@'+b+'">');
            document.write(a+'@'+b+'</a>');
          </SCRIPT>
        </td>
        <td class="site"><a target="_blank" href="{{person.website}}">{{person.website}}</a></td>
      </tr>
    {% endfor %}
  </tbody>
  </table>
</div>

## Alumni
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
    {% for person in site.data.people.alumni %}
      <tr>
        <td class="name">{{person.name}}</td>
        <td class="email">
          <SCRIPT type='text/javascript'>
            a='{{person.email | split: '@' | first}}';
            b='{{person.email | split: '@' | last}}';
            document.write('<A hre'+'f="mai'+'lto:'+a+'@'+b+'">');
            document.write(a+'@'+b+'</a>');
          </SCRIPT>
        </td>
        <td class="site"><a target="_blank" href="{{person.website}}">{{person.website}}</a></td>
      </tr>
    {% endfor %}
  </tbody>
  </table>
</div>
