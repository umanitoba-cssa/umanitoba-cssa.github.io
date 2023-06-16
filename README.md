## Computer Science Students' Association Site

This site runs on gitpages and is compiled with Jekyll.
Jekyll is a Ruby Gem that can be installed on most systems.

Gems are code you can include in Ruby projects. Gems package specific functionality. You can share gems across multiple projects or with other people.
Gems can perform actions like:
* Converting a Ruby object to JSON
* Pagination
* Interacting with APIs such as GitHub


## Features

* List collections
* Modular editing
* RSS/Atom feed
* SEO tags
* Google Analytics

## Setup

[Requirements](https://jekyllrb.com/docs/installation/#requirements)
* [Ruby](https://www.ruby-lang.org/en/downloads/) version `2.5.0` or higher, including all development headers (check your Ruby version using `ruby -v`)
* [RubyGems](https://rubygems.org/pages/download) (check your Gems version using `gem -v`)
* GCC and Make (check versions using `gcc -v`,`g++ -v`, and `make -v`)


Bundler is a gem that installs all gems in your Gemfile.
While you don’t have to use Gemfile and bundler, it is highly recommended as it ensures you’re running the same version of Jekyll and its plugins across different environments.

### Jekyll on Ubuntu
#### Install dependencies
Install Ruby and other prerequisites:

~~~bash
$ sudo apt-get install ruby-full build-essential zlib1g-dev
~~~

Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your `~/.bashrc` file to configure the gem installation path:

~~~bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
~~~

Finally, install Jekyll and Bundler:

~~~bash
gem install jekyll bundler
~~~

## Develop

Project started with [Jekyll](https://jekyllrb.com/) version 4.2.1, but should support newer versions as well.


Install the dependencies with [Bundler](http://bundler.io/):

Bundler manages an application's dependencies through its entire life, across many machines, systematically and repeatably.


~~~bash
$ bundle install
~~~

Run `jekyll` commands through Bundler to ensure you're using the right versions:

~~~bash
$ bundle exec jekyll serve
~~~

alt:

~~~bash
$ bundle exec jekyll s
$ Server address: http://127.0.0.1:4000
~~~


## Editing

This site is already optimised for adding, updating and removing components.

This site follows jekyll's native [layouts](https://jekyllrb.com/docs/layouts/).
All of the content is stored seperately in [Includes](https://jekyllrb.com/docs/includes/).

`Staff` and `resources` are set up as collections to be easily added from marddown files.
You can read more about [Collections](https://jekyllrb.com/docs/collections/)

This is set in the \\*_staff_members* and \\*_resources* directory.

You can add more collections by editing your `_config.yml` and creating a corresponding directory.

### Navigation

* Exposed as a data file.
* Set in the *Data* / *Navigation* section.

### Footer

* Exposed as a data file.
* Set in the *Data* / *Footer* section.