# Issues

**1) wepack-dev-server**

```
$ ./bin/webpack-dev-server

yarn run v0.27.5
$ "c:\Users\Jonas\apps\webpacker_test\node_modules\.bin\webpack-dev-server" "--progress" "--color" "--config" "c:/Users/Jonas/apps/webpacker_test/config/webpack/development.js"
The filename, directory name, or volume label syntax is incorrect.
```

**2) rails assets:precompile**

```
$ rails assets:precompile --trace
** Invoke assets:precompile (first_time)
** Invoke assets:environment (first_time)
** Execute assets:environment
** Invoke environment (first_time)
** Execute environment
** Invoke yarn:install (first_time)
** Execute yarn:install
** Execute assets:precompile
** Invoke webpacker:compile (first_time)
** Invoke webpacker:verify_install (first_time)
** Invoke webpacker:check_node (first_time)
** Execute webpacker:check_node
** Invoke webpacker:check_yarn (first_time)
** Execute webpacker:check_yarn
** Invoke webpacker:check_webpack_binstubs (first_time)
** Execute webpacker:check_webpack_binstubs
** Execute webpacker:verify_install
Webpacker is installed 🎉 🍰
Using c:/Users/Jonas/apps/webpacker_test/config/webpacker.yml file for setting up webpack paths
** Invoke environment
** Execute webpacker:compile
[Webpacker] Compiling assets 🎉
rails aborted!
Errno::ENOEXEC: Exec format error - ./bin/webpack
c:/RailsInstaller/Ruby2.3.0/lib/ruby/2.3.0/open3.rb:199:in `spawn'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/2.3.0/open3.rb:199:in `popen_run'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/2.3.0/open3.rb:95:in `popen3'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/2.3.0/open3.rb:258:in `capture3'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/webpacker-2.0/lib/tasks/webpacker/compile.rake:13:in `block (2 levels) in <top (required)>'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:250:in `block in execute'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:250:in `each'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:250:in `execute'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:194:in `block in invoke_with_call_chain'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/2.3.0/monitor.rb:214:in `mon_synchronize'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:187:in `invoke_with_call_chain'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:180:in `invoke'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/webpacker-2.0/lib/tasks/webpacker/compile.rake:34:in `block in <top (required)>'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:250:in `block in execute'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:250:in `each'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:250:in `execute'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:194:in `block in invoke_with_call_chain'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/2.3.0/monitor.rb:214:in `mon_synchronize'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:187:in `invoke_with_call_chain'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/task.rb:180:in `invoke'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:152:in `invoke_task'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:108:in `block (2 levels) in top_level'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:108:in `each'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:108:in `block in top_level'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:117:in `run_with_threads'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:102:in `top_level'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/railties-5.1.3/lib/rails/commands/rake/rake_command.rb:21:in `block in perform'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/rake-12.0.0/lib/rake/application.rb:178:in `standard_exception_handling'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/railties-5.1.3/lib/rails/commands/rake/rake_command.rb:18:in `perform'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/railties-5.1.3/lib/rails/command.rb:46:in `invoke'
c:/RailsInstaller/Ruby2.3.0/lib/ruby/gems/2.3.0/gems/railties-5.1.3/lib/rails/commands.rb:16:in `<top (required)>'
bin/rails:4:in `require'
bin/rails:4:in `<main>'
Tasks: TOP => webpacker:compile
```

**3) Webpacker::FileLoader::NotFoundError in Hello#index**

> Can't find application.js in c:/Users/Jonas/apps/webpacker_test/public/packs/manifest.json. Is webpack still compiling?

```
$ rails s
=> Booting Puma
=> Rails 5.1.3 application starting in development on http://localhost:3000
=> Run `rails server -h` for more startup options
*** SIGUSR2 not implemented, signal based restart unavailable!
*** SIGUSR1 not implemented, signal based restart unavailable!
*** SIGHUP not implemented, signal based logs reopening unavailable!
Puma starting in single mode...
* Version 3.10.0 (ruby 2.3.3-p222), codename: Russell's Teapot
* Min threads: 5, max threads: 5
* Environment: development
* Listening on tcp://0.0.0.0:3000
Use Ctrl-C to stop
Started GET "/" for 127.0.0.1 at 2017-08-22 04:30:07 +0200
Processing by HelloController#index as HTML
  Rendering hello/index.html.erb within layouts/application
  Rendered hello/index.html.erb within layouts/application (2.0ms)
Completed 500 Internal Server Error in 8073ms



ActionView::Template::Error (Can't find application.js in c:/Users/Jonas/apps/webpacker_test/public/packs/manifest.json. Is webpack still compiling?):
     6:
     7:     <%= stylesheet_link_tag    'application', media: 'all', 'data-turbolinks-track': 'reload' %>
     8:     <%= javascript_include_tag 'application', 'data-turbolinks-track': 'reload' %>
     9:     <%= javascript_pack_tag 'application' %>
    10:   </head>
    11:
    12:   <body>

app/views/layouts/application.html.erb:9:in `_app_views_layouts_application_html_erb__814739184_46378296'
Started GET "/" for 127.0.0.1 at 2017-08-22 04:38:42 +0200
Processing by HelloController#index as HTML
  Rendering hello/index.html.erb within layouts/application
  Rendered hello/index.html.erb within layouts/application (0.0ms)
Completed 500 Internal Server Error in 167ms
```
