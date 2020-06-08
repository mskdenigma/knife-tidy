source "https://rubygems.org"

gemspec

group :debug do
  gem "pry"
  gem "pry-byebug"
  gem "pry-stack_explorer"
end

group :development do
  gem "aruba"

  # make sure we can still test on Ruby 2.4
  if RUBY_VERSION.match?(/2\.4/)
    gem "chef", "~> 14"
  else
    gem "chef"
  end
  if Gem::Version.new(RUBY_VERSION) < Gem::Version.new("2.6")
    gem "chef-zero", "~> 14"
  else
    gem "chef-zero"
  end
  gem "chefstyle", git: "https://github.com/chef/chefstyle.git"
  gem "fakefs"
  gem "rake"
  gem "rspec"
  gem "simplecov"
  gem "simplecov-console"
end

group :docs do
  gem "github-markup"
  gem "redcarpet"
  gem "yard"
end
