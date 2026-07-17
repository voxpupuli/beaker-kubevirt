# frozen_string_literal: true

require 'bundler/gem_tasks'
require 'rspec/core/rake_task'

RSpec::Core::RakeTask.new(:spec)

begin
  require 'rubocop/rake_task'
  RuboCop::RakeTask.new
  task default: %i[spec rubocop]
rescue LoadError
  # RuboCop is optional
  task default: [:spec] # rubocop:disable Rake/DuplicateTask
end

desc 'Run acceptance tests (requires KubeVirt cluster)'
task :acceptance do
  puts 'Running acceptance tests...'
  puts 'Note: This requires a KubeVirt-enabled Kubernetes cluster'
  # Add acceptance test commands here
end

desc 'Run examples'
task :examples do
  ruby 'examples/usage.rb'
end

begin
  require 'github_changelog_generator/task'

  GitHubChangelogGenerator::RakeTask.new :changelog do |config|
    config.header = "# Changelog\n\nAll notable changes to this project will be documented in this file."
    config.exclude_labels = %w[duplicate question invalid wontfix wont-fix skip-changelog github_actions]
    config.user = 'voxpupuli'
    config.project = 'beaker-kubevirt'
    config.future_release = Gem::Specification.load("#{config.project}.gemspec").version
  end
rescue LoadError
  # Optional group in bundler
end
