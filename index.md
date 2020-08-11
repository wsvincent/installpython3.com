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
          <img src="assets/images/windows.svg.png" class="img-fluid" alt="Windows logo">
        </div>
      </a>
    </div>
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-mac %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Mac</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/apple.svg.png" class="img-fluid" alt="Apple logo">
        </div>
      </a>
    </div>
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-linux %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Linux</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/tux.svg.png" class="img-fluid" alt="Linux logo">
        </div>
      </a>
    </div>
    <div class="card mb-4 shadow-sm">
      <a href="{{ site.baseurl }}{% post_url/2010-01-01-chromebook %}">
        <div class="card-header">
          <h4 class="my-0 font-weight-normal">Chromebook</h4>
        </div>
        <div class="card-body">
          <img src="assets/images/chrome.svg.png" class="img-fluid" alt="Chromebook logo">
        </div>
      </a>
    </div>
  </div>
  <br />
  <h2>Why This Guide?</h2>
  <br/>
  <div class="xkcd-img">
    <a href="https://xkcd.com/1987/" target="\_blank">
      <img src="https://imgs.xkcd.com/comics/python_environment.png">
    </a>
  </div>
  <br/>
  <p><a href="https://xkcd.com/1987/" target="\blank">This XKCD comic</a> sums up the issue. In short, installing Python on a computer is a challenge for professional programmers and a nightmare for newcomers. It is easy if not inevitable to have multiple installs on a machine, a messed up PATH, and so on. Unfortunately, the advice on the <a href="https://www.python.org/downloads/">official Python downloads page</a> is, arguably, the wrong approach for most programmers. It does not allow for easy updates to future versions of Python. And it makes switching between multiple versions of Python (for example, 3.5 vs 3.8) more challenging than it needs to be.</p>
  <p>If you are a professional programmer, I highly recommend reading the setup choices of <a href="https://jacobian.org/2019/nov/11/python-environment-2020/" target="\_blank">Jacob Kaplan-Moss, co-creator of Django</a>, which covers more advanced options like pyenv, pipx, Poetry, and so on.</p>
</div>
