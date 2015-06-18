# Ember Rails Application Template

This is the basic setup to get an ember application (using ember CLI) and a rails application working together.

## Steps that have been followed to create the template
Ensure that you have rails installed on your laptop. You can utilize either rbenv or rvm.
Ensure that you have bundler installed.

Once you have the latest ruby installed,
```
$ gem install rails
``` 

Create the Rails application:


```
$ rails new app -B -S -T -d postgresql
$ mv app rails
```
* -B will not run bundle install
* -T will Skip Test::Unit files
* -S will disable the asset pipeline by bypassing the sprocket option
* -d will create a database based on the option given

---

Ensure that you have node and npm installed on your laptop:

Ember CLI needs at least node version 0.10.5 and npm 2.1.8, so don't proceed if your install versions are older.

```
$ node -v
$ npm -v
```

Once you have the environment Ember CLI runs in, let's install the ember-clipackage itself:

```
$ npm install -g ember-cli
```

Now you should be able to query the ember version:

```
$ ember -v
```

Create the Ember app

```
$ ember new app --skip-git
$ mv app ember
```

* --skip-git so that a git repo is not initialized within the ember directory 
