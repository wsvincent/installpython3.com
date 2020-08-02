---
layout: page
title:  "InstallPython3.com | Chromebook"
description: "How to install Python 3 properly on a Chromebook"
date:   2019-08-06 08:53:27 -0500
categories:
sitemap: true
---

# Chromebook

A Chromebook runs [ChromeOS](https://en.wikipedia.org/wiki/Chrome_OS) as its operating system and historically running anything other than a web app--such as Python--was challenging.

However, that is no longer the case! You can now run [Linux apps on ChromeOS](https://support.google.com/chromebook/answer/9145439?hl=en) which opens the door to using [MiniConda](https://docs.conda.io/en/latest/miniconda.html) to install Python 3.

## Step 1: Turn On Linux (Beta)

Make sure you are logged in first. These steps won't work if you're still in Guest mode!

Open your Chromebook's [system settings](chrome://settings) by clicking on the Time in the lower right corner and then the Gear icon for Settings.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/time_icon.png" alt="Time Icon">

Scroll down to "Linux (Beta)" and select **Turn On**.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/linux_beta.png" alt="Linux Beta">

Follow the prompts and at the end a Terminal window will open. You can run Linux commands here. (Tip: pin it to the dock for easy access).

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/terminal.png" alt="Terminal">


## 2. Download Miniconda

[MiniConda](https://docs.conda.io/en/latest/miniconda.html) is a free distribution of Python that works on Linux computers. It provides a basic implementation of Python and the ability to add additional packages manually as needed. Since disk space is at a premium, we will use this as opposed to Anaconda, its full-featured cousin, which includes many Python packages like numpy, scipy, and ipython notebook automatically.

Navigate to the [MiniConda](https://docs.conda.io/en/latest/miniconda.html) site, scroll down to the "Linux installers" section, and click on the link for 64-bit version of Python 3.8.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/64_bit_download.png" alt="64 Bit Download">

Once downloaded, click on the "Confirm download" pop-up and select "Keep".

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/confirm_download_keep.png" alt="Keep Download">

It's **very important** to now move the installer into the "Linux files" section of your computer. Open up your files by clicking on the Launcher button in the lower left corner, then the Up arrow, and then Files under the search bar. The file will be named something like `Miniconda3-latest-Linux-x86_64.sh`.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/downloads.png" alt="Downloads">

Drag it from *Downloads* into the *Linux Files* section.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/linux_files.png" alt="Linux Files">

## 3. Install Miniconda

Open the Terminal app from the Start? area.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/terminal_open.png" alt="Terminal Open">

Confirm that the Miniconda installer is in your current directory by typing `ls`.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/ls.png" alt="ls">

Then to install it run the command `sudo bash Miniconda3-latest-Linux-x86_64.sh`.

```sh
$ sudo bash Miniconda3-latest-Linux-x86_64.sh
```

There will be a prompt to review the license. Click Enter to continue:

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/review_license.png" alt="Review License">

On the final step, you'll be asked: "Do you accept the license terms? [yes|no]". Type in "yes" and press Enter.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/license_terms.png" alt="License Terms">

The next step asks where to install Miniconda. The default suggested is `/root/miniconda3` however I prefer to use `/opt/miniconda3` instead which is a directory commonly used for installing unbundled software packages. So type in `/opt/miniconda3` instead.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/opt_miniconda.png" alt="Opt Miniconda">

When asked, "Do you wish the installer to initialize MiniConda3 by running conda init? [yes|no]" type in `yes`.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/initialize.png" alt="Initialize">

And we're done! The instructions will note that closing and re-opening the Terminal app is required. Do so.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/install_done.png" alt="Install Done">

Set the proper permissions for the directory so that `conda` can add/remove software packages. Make sure to replace my username, `williamsvincent`, with yours which is found at the beginning of the prompt before `@penguin`. Also note that if you did not use the `/opt/miniconda3` path for installing your miniconda, but rather deferred to the default `root/miniconda3`, you will have to replace `opt` with `root` in the command below.

```sh
$ sudo chown -R williamsvincent /opt/miniconda3
```

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/sudo_chown.png" alt="Permissions">


## 4. Using Python

To run Conda--and by extension Python--enter a base environment by typing `source /opt/miniconda3/bin/activate`.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/activate.png" alt="Activate">

The new parentheses at the start of the prompt called `(base)` confirm the environment is active. To confirm the installed Python version, type `python --version`.

```sh
$ python --version
Python 3.8.5
```

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/python_version.png" alt="Python Version">

And then to enter Python itself, simply type `python`.

<img class="img-fluid" src="{{ site.url }}/assets/images/chromebook/python_conda.png" alt="Python Conda">


## Next Steps
To learn more about Python, the books [Python Crash Course](https://amzn.to/2okggMH) and [Automate the Boring Stuff](https://amzn.to/366CebJ) are great resources. For free tutorials on web development with Python check out [Learn Django](https://learndjango.com).
