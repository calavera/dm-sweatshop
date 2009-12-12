require 'rubygems'
require 'rake'

begin
  gem 'jeweler', '~> 1.4'
  require 'jeweler'

  Jeweler::Tasks.new do |gem|
    gem.name        = 'dm-sweatshop'
    gem.summary     = 'DataMapper plugin for building pseudo random models'
    gem.description = gem.summary
    gem.email       = 'ben [a] benburkert [d] com'
    gem.homepage    = 'http://github.com/datamapper/dm-more/tree/master/%s' % gem.name
    gem.authors     = [ 'Ben Burkert' ]

    gem.rubyforge_project = 'datamapper'

    gem.add_dependency 'dm-core', '~> 0.10.2'
    gem.add_dependency 'randexp', '~> 0.1.4'

    gem.add_development_dependency 'rspec', '~> 1.2.9'
    gem.add_development_dependency 'yard',  '~> 0.4.0'
  end

  Jeweler::GemcutterTasks.new

  FileList['tasks/**/*.rake'].each { |task| import task }
rescue LoadError
  puts 'Jeweler (or a dependency) not available. Install it with: gem install jeweler'
end
