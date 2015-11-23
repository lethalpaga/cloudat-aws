require "bundler/gem_tasks"
require 'rspec/core/rake_task'

task default: 'spec'

spec_task = :spec
begin
  RSpec::Core::RakeTask.new(spec_task)
rescue LoadError
  puts "Warning: RSpec isn't available, #{spec_task} task won't be available"
end
