# encoding: UTF-8
require 'rubygems'
begin
  require 'bundler/setup'
rescue LoadError
  puts 'You must `gem install bundler` and `bundle install` to run rake tasks'
end

require 'rake'
require 'bundler/gem_tasks'
require 'rake/testtask'

Rake::TestTask.new(:test) do |t|
  t.libs << 'lib'
  t.libs << 'test'
  t.pattern = 'test/**/*_test.rb'
  t.verbose = false
end

Rake::TestTask.new("test:controllers") do |t|
  t.libs << 'lib'
  t.libs << 'test'
  t.pattern = 'test/controllers/*_test.rb'
  t.verbose = false
end

Rake::TestTask.new("test:generators") do |t|
  t.libs << 'lib'
  t.libs << 'test'
  t.pattern = 'test/generators/*_test.rb'
  t.verbose = false
end

Rake::TestTask.new("test:integration") do |t|
  t.libs << 'lib'
  t.libs << 'test'
  t.pattern = 'test/integration/*_test.rb'
  t.verbose = false
end

Rake::TestTask.new("test:models") do |t|
  t.libs << 'lib'
  t.libs << 'test'
  t.pattern = 'test/models/*_test.rb'
  t.verbose = false
end

Rake::TestTask.new("test:functional") do |t|
  t.libs << 'lib'
  t.libs << 'test'
  t.pattern = 'test/functional/*_test.rb'
  t.verbose = false
end

task :default => :test
