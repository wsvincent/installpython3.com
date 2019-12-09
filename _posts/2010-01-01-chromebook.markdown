---
layout: page
title:  "InstallPython3.com | Chromebook"
description: "How to install Python 3 on a Chromebook"
date:   2019-08-06 08:53:27 -0500
categories:
---

# Chromebook

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

<!-- <img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/install_miniconda.png" alt="Install MiniConda"> -->

Once the installer is downloaded move the file (usually something like Miniconda3-latest-Linux-x86_64) into the “Linux Files” section of your device’s storage.

<!-- IMAGE -->

## 3. Install Miniconda

With the Terminal open navigate to the location of the Miniconda installer using the `cd` command. Within that directory, install `conda` by running the following command (note the dollar sign, `$`, indicates a new command line prompt; do not type it!).

```
$ sudo bash Miniconda3-latest-Linux-xs86_64.sh
```

Keep pressing Enter to read through the license until the final step where you are asked: "Do you accept the license terms? [yes|no]" Type in "yes" and press Enter.

<!-- IMAGE -->

When asked where to install Miniconda a good location is `/opt/minidconda3`.

<!-- IMAGE -->

And then when asked to initialize Miniconda3 in `/root/.bashrc ? [yes|no]` type "yes" and Enter.

Once installed, the last step is to set the proper permissions so Conda can add or remove packages. Type `sudo chonw -R username /opt/miniconda3` replacing "username" with your actual username. <!-- how tell? -->

```
$ sudo chown -R username /opt/minidconda3
```

## 4. Using Python

Within Terminal confirm the version of Python installed by typicing `python --version`.

```
$ python --version
```

And then to enter Python itself, simply type `python`.

```
$ python
>>>
```

## Next Steps
To learn more about Python, the book [Python Crash Course](https://amzn.to/2okggMH) is a great resource. For web development with Python, check out [Django for Beginners](https://djangoforbeginners.com).
