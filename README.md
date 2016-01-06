#vim-refills

This is a vim plugin for adding vim commands to utilize
[thoughtbot's refills gem](http://github.com/thoughtbot/refills).

For example, if you want to generate the hero refill you would run
the following command in vim:

```
:RefillHero
```

This will run the following command in your shell:

```
rails generate refills:import hero
```

If you deleted stylesheet sprocket directives you will have to either
require the entire refills directory:

``` sass
@import 'refills/*'
```

or list each component one by one:

``` sass
@import 'refills/hero'
```

You can now use the refill as a partial.

``` erb
<%= render "refills/hero" %>
```
