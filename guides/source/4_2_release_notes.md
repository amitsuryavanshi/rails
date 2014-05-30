Ruby on Rails 4.2 Release Notes
===============================

Highlights in Rails 4.2:

* ...
* ...

These release notes cover only the major changes. To know about various bug
fixes and changes, please refer to the change logs or check out the
[list of commits](https://github.com/rails/rails/commits/master) in the main
Rails repository on GitHub.

--------------------------------------------------------------------------------

Upgrading to Rails 4.2
----------------------

If you're upgrading an existing application, it's a great idea to have good test
coverage before going in. You should also first upgrade to Rails 4.1 in case you
haven't and make sure your application still runs as expected before attempting
an update to Rails 4.2. A list of things to watch out for when upgrading is
available in the
[Upgrading Ruby on Rails](upgrading_ruby_on_rails.html#upgrading-from-rails-4-1-to-rails-4-2)
guide.


Major Features
--------------



Railties
--------

Please refer to the
[Changelog](https://github.com/rails/rails/blob/4-2-stable/railties/CHANGELOG.md)
for detailed changes.

### Notable changes

* ...
* ...


Action Pack
-----------

Please refer to the
[Changelog](https://github.com/rails/rails/blob/4-2-stable/actionpack/CHANGELOG.md)
for detailed changes.

### Notable changes

* ...
* ...


Action Mailer
-------------

Please refer to the
[Changelog](https://github.com/rails/rails/blob/4-2-stable/actionmailer/CHANGELOG.md)
for detailed changes.

### Notable changes

* ...
* ...


Active Record
-------------

Please refer to the
[Changelog](https://github.com/rails/rails/blob/4-2-stable/activerecord/CHANGELOG.md)
for detailed changes.

### Notable changes

* ...
* ...


Active Model
------------

Please refer to the
[Changelog](https://github.com/rails/rails/blob/4-2-stable/activemodel/CHANGELOG.md)
for detailed changes.

### Notable changes

* ...
* ...


Active Support
--------------

Please refer to the
[Changelog](https://github.com/rails/rails/blob/4-2-stable/activesupport/CHANGELOG.md)
for detailed changes.

### Removals

* Removed deprecated `Numeric#ago`, `Numeric#until`, `Numeric#since`,
  `Numeric#from_now`. ([Commit](https://github.com/rails/rails/commit/f1eddea1e3f6faf93581c43651348f48b2b7d8bb))

* Removed deprecated string based terminators for `ActiveSupport::Callbacks`.
  ([Pull Request](https://github.com/rails/rails/pull/15100))

### Deprecations

* Deprecated `Class#superclass_delegating_accessor`, use `Class#class_attribute`
  instead. ([Pull Request](https://github.com/rails/rails/pull/14271))

* Deprecated `ActiveSupport::SafeBuffer#prepend!` as `ActiveSupport::SafeBuffer#prepend`
  now performs the same function. ([Pull Request](https://github.com/rails/rails/pull/14529))

### Notable changes

* The `humanize` inflector helper now strips any leading underscores.
  ([Commit](https://github.com/rails/rails/commit/daaa21bc7d20f2e4ff451637423a25ff2d5e75c7))

* Added `SecureRandom::uuid_v3` and `SecureRandom::uuid_v5`.
  ([Pull Request](https://github.com/rails/rails/pull/12016))

* Introduce `Concern#class_methods` as an alternative to `module ClassMethods`,
  as well as `Kernel#concern` to avoid the `module Foo; extend ActiveSupport::Concern; end`
  boilerplate. ([Commit](https://github.com/rails/rails/commit/b16c36e688970df2f96f793a759365b248b582ad))

Credits
-------

See the
[full list of contributors to Rails](http://contributors.rubyonrails.org/) for
the many people who spent many hours making Rails, the stable and robust
framework it is. Kudos to all of them.
