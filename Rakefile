require "bundler/gem_tasks"

task :console do
  require 'pry'
  require 'test_gem'

  def reload!
    # Change 'gem_name' here too:
    files = $LOADED_FEATURES.select { |feat| feat =~ /\/test_gem\// }
    files.each { |file| load file }
  end

  ARGV.clear
  Pry.start
end
