---
layout: page
title:  "Chromebook"
date:   2019-08-06 08:53:27 -0500
categories:
---

# Chromebook

*Images coming soon...*

A Chromebook runs [ChromeOS](https://en.wikipedia.org/wiki/Chrome_OS) as its operating system and historically running anything other than a web app--such as Python--was challenging.

However, that is no longer the case! You can now run [Linux apps on ChromeOS](https://support.google.com/chromebook/answer/9145439?hl=en) which opens the door to using [MiniConda](https://docs.conda.io/en/latest/miniconda.html) to install Python 3.

Here's how...

## Step 1: Turn On Linux (Beta)

Open your Chromebook's [system settings](chrome://settings) and scroll down to "Linux (Beta)." Select **Turn On**.

<!-- IMAGE -->

Follow the prompts and at the end a Terminal window will open. You can run Linux commands here. (Tip: pin it to the dock for easy access).

<!-- IMAGE -->

## 2. Download Miniconda

[Anaconda](https://www.anaconda.com) is a free distribution of Python that makes installation on a Linux machine, like our Chromebook, much easier to use. It comes out-of-the box with a host of popular 3rd party Python libraries like numpy, scipy, and ipython notebook which means it can be quite large in size.

Fortunately if you just want Python and the ability to manually add additional packages as needed, there is an option called [MiniConda](https://docs.conda.io/en/latest/miniconda.html). Since most Chromebook's have limited disk space that's what we'll use here.

Go to the [MiniConda](https://docs.conda.io/en/latest/miniconda.html) section, scroll down to "Linux installers," and click the link to download the 64-bit version of Python 3.7

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/install_miniconda.png" alt="Install MiniConda">

Once the installer is downloaded move the file (usually something like Miniconda3-latest-Linux-x86_64) into the “Linux Files” section of your device’s storage.

<!-- IMAGE -->
