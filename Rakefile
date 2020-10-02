desc 'outputs hello to the terminal'
namespace :greeting do
  task :hello do
    puts "hello from Rake!"
  end
  desc 'outputs hola to the terminal'
  task :hola do
    puts "dola de Rake!"
  end
end

task :environment do
  require_relative './config/environment'
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do 
    Student.create_table
  end
  desc 'seed the databse with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end
end

