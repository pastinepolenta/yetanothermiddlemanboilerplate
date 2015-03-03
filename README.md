### Yet another boilerplate for Middleman
Just because I wanted to have it my way

## Features

  - Middleman (SASS, HTML)
  - Simple SASS structure (colors, vars...)
  - Bourbon, Normalize, Modular-Scale. As (removable) ruby gems
  - Javascript in partials
  - Middleman-deploy

## How to use (Linux/Unix)

  - Go to an empty folder, which will be your website root folder
  - Clone this repo in there, use option `--depth=1` if you don't need the repo history
  - `rm -rf .git` if you don't need the repo history, you can init your git repo later
  - I assume you alredy have ruby installed
  - Run `bundle install --path vendor/bundle` to install the gems in the current folder (so they are inline with the current config)
  - You might need to adjust `config.rb` to match your exact assets path to `vendor/bundle/something/something...`
  - Run `bundle exec middleman`
  - Go to http://localhost:4567, your website should be ready with all the SASS files compiled

## Then...
 
  - Develop something cool
  - `git init`
  - Commit and push (`.gitignore` will ignore build and vendor folders)
  - Setup your remote repo url in the deploy params of `config.rb`
  - Run `bundle exec middleman deploy`. The static code (build folder) should now be in the `compiled` branch of your remote repo.