# README

Red Panthers Ruby on Rails project startup template

We have found that we are using and reusing a lot of gem and rails best practices over and over again
in all our rails project. We have compiled them together in a single project so as to improve our
time to get started on a project.

## Setup

run `./bin/setup`

or if you want to run step by step follow the below instruction.

```
cp config/database.yml.example config/database.yml
cp config/secrets.yml.example config/secrets.yml
```

## Run in development

We use foreman to manage all our services. So to start the rails project run the following
command.

```
foreman start -f Procfile.dev
```

## Secruity

We give a lot of importance to security when we build/maintain a rails application. The following
gems are added to our project to detect our vulnerabilities before the hackers do.

| Name     | Command to run |
| ---      | ---       |
| Bundler Audit | `bundle audit`        |
| Ruby Audot     | `bundle exec ruby-audit`       |
| Brakeman | `brakeman ./` |

Read through these articles below if you are begineer or first time Rails developer.

[http://guides.rubyonrails.org/security.html](Ruby on Rails security guide)

[https://www.owasp.org/index.php/Ruby_on_Rails_Cheatsheet](OWASP secruity cheatsheet for Rails)


## Note for maintainers

Always keep the project updated with the latest for version of Rails and Ruby.

When we start a new project it is always better to install the latest version of
all the tools, even if your not familiar with it. Because the chances are you might
not be able to update it for a long, long time once you get started.

https://twitter.com/coderhs/status/966713134294560769
