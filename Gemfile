source "http://rubygems.org"

<<<<<<< HEAD
# For now use master
# gem 'cocoapods', ">= #{YAML.load_file(File.dirname(__FILE__) + "/CocoaPods-version.yml")['last']}"
gem "cocoapods-core", :git => "git://github.com/CocoaPods/Core.git", :branch => 'master'
gem "cocoapods",      :git => "git://github.com/CocoaPods/CocoaPods.git", :branch => 'master'
gem 'rake'
=======
unless defined?(Pod::VERSION)
  ::BUNDLER_GEMSPEC = true unless defined?(::BUNDLER_GEMSPEC)
end
gemspec

group :development do
  if ENV['COCOA_PODS_DEPENDENCIES'] == 'local'
    gem 'cocoapods-core',       :path => '../Core'
    gem 'xcodeproj',            :path => '../Xcodeproj'
    gem 'cocoapods-downloader', :path => '../cocoapods-downloader'
  else
    gem 'cocoapods-core',       :git => "https://github.com/CocoaPods/Core.git"
    gem 'xcodeproj',            :git => "https://github.com/CocoaPods/Xcodeproj.git"
    gem 'cocoapods-downloader', :git => "https://github.com/CocoaPods/cocoapods-downloader.git"
  end

  gem "mocha"
  gem "bacon"
  gem "mocha-on-bacon"
  gem "rake"
  gem 'coveralls', :require => false
end

group :debugging do
  gem "rb-fsevent"
  gem "kicker", :git => "https://github.com/alloy/kicker.git", :branch => "3.0.0"
  gem "awesome_print"
  gem "pry"
  gem "diffy"
end

group :documentation do
  gem 'yard'
  gem 'redcarpet'
  gem 'github-markup'
  gem 'pygments.rb'
end

>>>>>>> 61ddc073e4b60493b862d2f54c179afc172b9fd2
