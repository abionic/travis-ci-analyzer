namespace :sys do
  namespace :os do
    desc 'nix cmd: uname'
    task :uname do
      puts %x{uname -a}
    end

    task :env do
      puts %{env}
    end

    task :ls_svc do
      puts %{ls /etc/init.d/}
    end
  end


end


task :default => ['sys:os:uname', 'sys:os:env', 'sys:os:ls_svc']
