# InstallPython3.com

This is a free, open-source guide to installing Python 3 on a new computer. The goal is not to be a comprehensive resource on the multiple ways to install both Python and configure virtual environments. It is to provide the simplest, workable way for a beginner to start with Python.

If you disagree with a recommended approach, please submit an **Issue**. I'm very eager to discuss the relative merits of different approaches but the goal is to recommend **one** approach to newbies, not overwhelm them.

PRs are welcome for areas--like Linux or Chromebook--not currently covered.

## Local Setup

This is a [Jekyll](https://jekyllrb.com) site deployed on Netlify. The steps below show how to clone the repo, install Jekyll (if needed), and start the local web server.

```
$ git clone https://github.com/wsvincent/installpython3.com.git
$ cd installpython3.com
$ gem install bundler jekyll
$ bundle exec jekyll serve
```

Then navigate to [http://localhost:4000](http://localhost:4000) to view the site.
