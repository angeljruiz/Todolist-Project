require "rake/testtask"
require "bundler/gem_tasks"

desc 'Say hello'
task :hello do
  puts "Hello there. This is the 'hello' task."
end

desc 'Setup and run tests'
task :default => :test

Rake::TestTask.new(:test) do |t|
  t.libs << 'libs'
  t.libs << 'test'
  t.test_files = FileList['test/**/*_test.rb']
end
