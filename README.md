# README

Wondering what options `rails new --api` and `rails new --minimal` are doing?

You can see the effect by diffing branches of this repository.

* `--api`: https://github.com/claasz/rails8_cli_new/pull/1/files
* `--minimal`: https://github.com/claasz/rails8_cli_new/pull/2/files

Environment: Ruby 3.3.1, Rails 8.0.1

# --api

Looking at the diff, `--api` disables certain browser related things (web-console, selenium, fragment caching). It also disables all JavaScript related stuff.


## --minimal

Looking at `/config/application.rb` and other config files, `--minimal` disables

* active_job
* active_storage
* action_mailer
* action_mailbox
* action_text
* action_cable
* bootsnap
* javascript
