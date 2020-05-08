---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: InstallPython3.com
description: How to install Python 3 on Mac, Windows, Linux, or Chromebook
---

<div class="pricing-header px-3 py-3 pt-md-5 pb-md-4 mx-auto text-center">
  <h1 class="display-4">Install Python 3</h1>
  <p class="lead">A step-by-step guide</p>
</div>

<div class="container">
  <div class="card-deck mb-6 text-center">
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-windows %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Windows</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/windows.svg.png" class="img-fluid">
        </div>
      </a>
    </div>
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-mac %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Mac</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/apple.svg.png" class="img-fluid">
        </div>
      </a>
    </div>
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-linux %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Linux</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/tux.svg.png" class="img-fluid">
        </div>
      </a>
    </div>
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-chromebook %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Chromebook</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/chrome.svg.png" class="img-fluid">
        </div>
      </a>
    </div>
    <!-- <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-docker %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Docker</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/docker.svg.png" class="img-fluid">
        </div>
      </a>
    </div> -->
  </div>
  <br />
  <h2>Why This Guide?</h2>
  <p>There are multiple ways to install Python on a computer. The guides here for each operating system are up-to-date, allow for upgrades, and make it possible to install multiple versions of Python on a computer as needed.</p>

  <p>Unfortunately, many newcomers unsuccessfully try several different approaches, none of which work. Often the culprit is a <a href="https://en.wikipedia.org/wiki/PATH_(variable)">PATH variable</a> improperly configured, so that when you type `python` on the command line, it doesn't refer to the proper Python installation.</p>
</div>
