# frozen_string_literal: true

source "https://rubygems.org"

gemspec

# Agregar la gema jekyll-sass-converter para manejar SCSS
gem "jekyll-sass-converter", "~> 2.0"

# Agregar la gema bootstrap si deseas usarla en tu proyecto
gem "bootstrap", "~> 5.1"

gem "html-proofer", "~> 5.0", group: :test

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.2.0", :platforms => [:mingw, :x64_mingw, :mswin]
