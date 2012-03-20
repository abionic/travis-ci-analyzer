namespace :sys do
  namespace :os do
    desc 'nix cmd: uname'
    task :uname do
      puts %x{uname -a}
    end

    task :env do
      puts %x{env}
    end

    task :ifconfig do
      puts %x{ifconfig --all}
    end

    task :ls_svc do
      puts %x{ls /etc/init.d/}
    end

    task :ls_dpkg do
      puts %x{dpkg --get-selections}
    end
  end


end


task :default => ['sys:os:uname', 'sys:os:env', 'sys:os:ifconfig', 'sys:os:ls_svc', 'sys:os:ls_dpkg']
