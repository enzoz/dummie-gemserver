A dummie gemserver
================

The simplest implementation of geminabox gem.  
 ***runs with ruby 1.9.3 and requires bundler***

### Running the server

```
$ bundle && thin start
```


### Uploading a gem
```
$ gem build your-gem.gemspec
$ gem inabox -g http://localhost:3000/ your-gem-x.x.x.gem
```

### Checking the available gems

To see the availables gems in your server open just [http://localhost:3000](http://localhost:3000).   

### Using installed gems
To get gems from your server add following line to your Gemfile

```
source 'http://localhost:3000' 
```
or just run in your terminal

``` 
$  gem source -a http://localhost:3000 
```
