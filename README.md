# Middleman::Autoprefixer [![Dependency status](https://gemnasium.com/porada/middleman-autoprefixer.png)](https://gemnasium.com/porada/middleman-autoprefixer)

> [Autoprefixer](https://github.com/ai/autoprefixer) integration with [Middleman](http://middlemanapp.com/)

Automatically add vendor prefixes to CSS rules in the stylesheets served in your Middleman project using values from [Can I Use](http://caniuse.com/).

## Usage

### Installation

Add the following line to your `Gemfile`, and then execute `bundle`.

```ruby
gem 'middleman-autoprefixer'
```

### Configuration

After installation, simply activate the extension in your project’s `config.rb`:

```ruby
activate :autoprefixer
```

#### Browsers

Optionally, you can specify `browsers` as a string or array of strings with accoradance to [Autoprefixer’s documentation](https://github.com/ai/autoprefixer#browsers). There are a few ways to set the option—two examples:

```ruby
activate :autoprefixer, browsers: 'last 1 version'

activate :autoprefixer do |config|
  config.browsers = ['last 2 versions', 'ie 8', 'ie 9']
end
```

## Credits

This gem was created by [Dominik Porada](http://github.com/porada) and makes use of [Autoprefixer Rails](https://github.com/ai/autoprefixer-rails) by [Andrey Sitnik](https://github.com/ai), the author of Autoprefixer.

## License

Middleman Autoprefixer is distributed under the [MIT](http://porada.mit-license.org/) license.
