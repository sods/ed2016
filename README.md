Confweb
---

This is a repository for easily creating conferences. To create your own conference. Create a repo in your username with your confname then type.

```
$ git clone --bare https://github.com/sods/confweb.git
$ cd confweb.git
$ git push --mirrow https://github.com/username/confname.git
$ cd ..
$ rm -rf confweb.git
```

Then you can clone the new website as normal.

The main settings can be found in the ```_config.yml``` file.

The base site is created with

```
$ jekyll site new .
```

Then a few layout files are added

```
_layouts/program.html
_layouts/single.html
_layouts/multi.html
_layouts/registration.html
_layouts/getting_there.html
_layouts/about.html
```

These dictate how the program is displayed. ```single.html``` and ```multi.html`` are for single and multiple track sessions. 

There are some include files for bits of html which are need about the place.

```
_includes/listperson.html
_includes/map.html
_includes/google_tracking_code.html
_includes/listsponsor.html
_includes/listtalk.html
```
