# Base box for the Ubuntu/Xenial64

## What's installed

* Apache
* MySQL
* PHP 7
* Ruby 2.3
* Node.js 6.5

## How to create a box

Install vagrant-vbguest.

```
$ vagrant plugin install vagrant-vbguest
```

Provision.

```
$ vagrant up
```

Run tests.

```
$ bundle install --path=vendor/bundle
$ bundle exec rake spec
```

Create a package.

```
$ vagrant package --vagrantfile Vagrantfile.dist
```
