# Issues

**1) wepack-dev-server**

```
$ ./bin/webpack-dev-server

yarn run v0.27.5
$ "c:\Users\Jonas\apps\webpacker_test\node_modules\.bin\webpack-dev-server" "--progress" "--color" "--config" "c:/Users/Jonas/apps/webpacker_test/config/webpack/development.js"
The filename, directory name, or volume label syntax is incorrect.
```

**2) Webpacker::FileLoader::NotFoundError in Hello#index**

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
