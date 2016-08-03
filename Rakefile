#!/usr/bin/env rake
# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

# encoding: utf-8

require File.expand_path('../config/application', __FILE__)
RailsApp::Application.load_tasks

require 'rspec/core'
require 'rspec/core/rake_task'

task :spec do
  RSpec::Core::RakeTask.new(:spec) do |spec|
    spec.rspec_opts = ["-c","-f documentation"]
    spec.pattern = FileList['spec/**/*_spec.rb']
  end
end

require 'rubygems'
