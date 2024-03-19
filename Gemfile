# frozen_string_literal: true

source "https://rubygems.org"

# Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem 'tzinfo', '>= 1', '< 3'
  gem 'tzinfo-data'
end

gem 'wdm', '~> 0.1.1', :install_if => Gem.win_platform?
gem 'jekyll-paginate'
gem 'public_suffix', '~> 5.0.3'
gem 'addressable', '~>  2.8.5'
gem 'diff-lcs', '~> 1.5.0'
gem 'ffi', '~> 1.16.3'
gem 'google-protobuf', '~> 3.24.4'
gem 'sass-embedded', '~> 1.69.3'
gem 'jekyll-sass-converter', '~> 3.0.0'
gem 'kramdown', '~> 2.4.0'
gem 'mercenary', '~> 0.4.0'
gem 'rouge', '~> 4.1.3'
gem 'unicode-display_width', '~> 2.5.0'
gem 'terminal-table', '~> 3.0.2'
gem 'webrick', '~> 1.8.1'
gem 'jekyll', '~> 4.3.2'
gem 'nokogiri', '~> 1.15.6'
gem 'rack', '~> 2.2.8'
gem 'rspec-support', '~> 3.12.1'
gem 'rspec-core', '~> 3.12.2'
gem 'rspec-expectations', '~> 3.12.3'
gem 'rspec-mocks', '~> 3.12.6'
gem 'rspec', '~> 3.12.0'

# gem "rails"