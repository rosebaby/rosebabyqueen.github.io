---
layout: post
title: "Set up Jekyll for Mac OS X Yosemite"
---

-install rbenv for ruby version management

    brew install rbenv ruby-build

-enable shims

    follow the hint from brew install

check usr/local/var/rbenv/shims path is included

    echo $PATH

-see versions

    rbenv versions

-choose a version list above to install

    rbenv install 2.0.0-p645

-set up global ruby version

    rbenv global 2.0.0-p645

-set up local ruby version, it only works under currently directory

    rbenv local 2.0.0-p645

check your enviroment

    gem enviroment
    which -a ruby

-install bunlder

    gem install bundler

-create a file named Gemfile under your site\'s repository with following lines

    source 'https://rubygems.org'
    gem 'github-pages'

please refer [using-jekyll-with-pages](https://help.github.com/articles/using-jekyll-with-pages/) for detailed info about installing Jekyll

call bundle to install

    bundle install

-start up jekyll server

    bundler exec jekyll server

Finally, view your sites from http://localhost:4000/
