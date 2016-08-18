# st1s-io
> My home page

Built using [Appfy](https://appfy.org) to generate some web components and use with Jekyll.

# Requirements
- [Appfy](https://appfy.org)
- [Jekyll](https://jekyllrb.com)

# Install

clone this repo and issue `npm run install` on project root folder

# Serve Appfy
run `$ appfy serve` on project root to serve the Appfy environment

# Serve Jekyll
run `$ jekyll serve --watch` on jekyll folder to serve the Jekyll environment

# Build Appfy modules

default
```
$ appfy build <module_name> -b
```

minified
```
$ appfy build <module_name> -b -m
```

# Using in Jekyll
as Appfy doesn't have all Jekyll tasks implemented yet, to use the exported module you'll have to copy into jekyll folder the files generated by build command, then import manually in your template. Like [here](https://github.com/stewones/st1s-io/blob/master/jekyll/_includes/foot.static.html) and [here](https://github.com/stewones/st1s-io/blob/master/jekyll/_includes/head.static.html). 

# Bootstraping Angular
To use components or features of the exported module, you'll need to boot the angular.js manually on Jekyll. You can see how I did it easily [here](https://github.com/stewones/st1s-io/blob/master/jekyll/_layouts/default.html#L2) and [here](https://github.com/stewones/st1s-io/blob/master/jekyll/static/modules/app.module.js#L10).

# License
MIT