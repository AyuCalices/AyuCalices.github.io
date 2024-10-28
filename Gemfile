# frozen_string_literal: true

source "https://rubygems.org"

gem "jekyll", "~> 4.3.2"
gem "jekyll-admin", "~> 0.11.0", group: :jekyll_plugins # specify version if needed
gem "sinatra", "~> 3.0"

# Adding standard libraries that will not be default gems in future Ruby versions
gem "logger"
gem "csv"
gem "ostruct"

group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.16" # updated from 0.6 to latest stable
  gem "jekyll-paginate", "~> 1.1.0" # same version, as no recent updates
end

# macOS specific dependency
require 'rbconfig'
if RbConfig::CONFIG['target_os'] =~ /darwin(1[0-3])/i
  gem "rb-fsevent", "~> 0.11"
end

gem "webrick", "~> 1.8" # kept version for Jekyll's dependency compatibility
