### YARD
---

https://github.com/lsegal/yard


```
gem install yard
sudo apt-get install rdoc
yard --help
yardoc 'lib/**/*.rb' 'app/**/*.rb'
yardoc 'app/**/*.rb' - README LICENSE FAQ
yardoc - README LICENSE FAQ
--query '@api.text == "public"'
--query 'object.has_tag?(:api) && object.tag(:api).text == "public"'
--query 'has_tag?(:api) && tag(:api).text == "public"'
--query '@return' --query '@param'
--query '@return && @param'

rake yard OPTS='--any --extra --opts'
yri YARD::Handlers::Base
yri File.relative_path
yard gems
yard server
yard server --gems
yard graph --protected --full --dependencies

```

```ruby
def reverse(contents)
  contents = content.read if contents.respond_to? :read
  contents.reverse
end

class List
  cattr_accessor :publisher
end

YARD::Rake::YardocTask.new do |t|
  t.files = ['lib/**/*.rb', OTHER_PATHS]
  t.options = ['--any', '--extra', '--opts']
  t.stats_options = ['--list-undoc']
end



```

```

```
