require 'straight_line/tasks'
require 'straight_line' 

StraightLine.configure do |config|
    config.add 'provision', :shell, './scripts/provision.sh'
    config.add 'build', :shell, 'composer install'
    config.add 'deploy', :shell, './scripts/deploy.sh', before: 'build'
end