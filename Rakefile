$:.unshift File.dirname(__FILE__) + 'lib' 

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new

task :default => :spec


desc "Ejecutar con documentacion"
task :test do
  sh "rspec -I. spec/fraccion_spec.rb --format documentation"
end 

desc "Ejecutar en formato HTML"
task :thtml do
  sh "rspec -I. spec/fraccion_spec.rb --format html"
end 


desc "Espectativas de la clase fraccion"
task :bin do
  sh "ruby -I. lib/frac_main.rb"

end 

