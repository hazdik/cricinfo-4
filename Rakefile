require 'rubygems'
gem 'hoe', '>= 2.1.0'
require 'hoe'
require 'fileutils'
require './lib/cricinfo'

Hoe.plugin :newgem
# Hoe.plugin :website
# Hoe.plugin :cucumberfeatures

# Generate all the Rake tasks
# Run 'rake -T' to see list of generated tasks (from gem root directory)
$hoe = Hoe.spec 'cricinfo' do
  self.developer 'Andrew S Williams', 'sobakasu@gmail.com'
  self.rubyforge_name       = self.name
#  self.excludes = []
end

require 'newgem/tasks'
Dir['tasks/**/*.rake'].each { |t| load t }
