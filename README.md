# rurema

Collector for rurema/doctree RD files. Parses Ruby library documentation using bitclust-core and emits library/class content records.

## Usage

```ruby
require 'rurema'

collector = Rurema::Collector.new(
  { 'doctree_path' => '/path/to/doctree', 'version' => '3.3.0' }
)
records = collector.collect
# => [{ content: "yaml ライブラリ...", source: "rurema/doctree:ruby3.3/yaml" }, ...]
```

## Development

```bash
bundle config set --local path vendor/bundle
bundle install
bundle exec rake test
```
