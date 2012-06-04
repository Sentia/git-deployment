require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "sentia-capistrano-gitflow"
    gem.summary = %Q{Capistrano recipe for a deployment workflow based on git tags. This gem was originally created by Joshua Nichols and modified by Mario Visic at Sentia Australia. }
    gem.description = %Q{Capistrano recipe for a deployment workflow based on git tags. This gem was originally created by Joshua Nichols and modified by Mario Visic at Sentia Australia.}
    gem.email = "mario.visic@sentia.com.au"
    gem.homepage = "https://github.com/Sentia/git-deployment"
    gem.authors = ["Joshua Nichols", "Mario Visic"]
    gem.add_dependency "capistrano"
    gem.add_dependency "stringex"
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

require 'rake/rdoctask'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

  rdoc.rdoc_dir = 'rdoc'
  rdoc.title = "gitflow #{version}"
  rdoc.rdoc_files.include('README*')
  rdoc.rdoc_files.include('lib/**/*.rb')
end
