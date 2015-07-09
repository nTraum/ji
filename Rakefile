require "bundler/gem_tasks"

require "rspec/core/rake_task"
RSpec::Core::RakeTask.new(:spec)

require "rubocop/rake_task"
RuboCop::RakeTask.new

require "reek/rake/task"
Reek::Rake::Task.new { |task| task.fail_on_error = true }

task default: [:spec, :rubocop, :reek]
