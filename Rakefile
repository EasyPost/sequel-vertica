#!/usr/bin/env rake
require "bundler/gem_tasks"

require 'rspec/core/rake_task'

desc 'Default: run specs.'
task :default => :spec

# Override `release` task to prevent publish to RubyGems
Rake::Task['release'].prerequisites.delete('release:rubygem_push')