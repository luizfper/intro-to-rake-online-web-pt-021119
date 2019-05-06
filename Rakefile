desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end


namespace :greeting do
  task :hello do
    puts "hello from Rake!"
  end
  task :hola do
    puts "hola de Rake!"
  end

end

namespace :db do
  task :migrate => :environment do
    desc 'migrate changes to your database'
      Student.create_table
  end

  task :environment do
    require_relative './config/environment.rb'
  end

  task :seed do
    require_relative "./db/seeds.rb"
  end
end

task :console do
  Pry.start
end
