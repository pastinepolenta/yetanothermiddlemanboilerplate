### Yet another boilerplate for Middleman
Just because I wanted to have it my way

## Features

  - Middleman (SASS, HTML)
  - Simple SASS structure (colors, vars...)
  - Bourbon, Normalize, Modular-Scale. As (removable) ruby gems
  - Javascript in partials
  - Middleman-deploy

## How to use (Linux/Unix)

  - Clone this repo under ~/.middleman . It will be available as Middleman theme for any project you want
  - I assume you alredy have ruby installed
  - Run `cd /path/to/your/new/website`
  - Run `middleman init --template=yetanothermiddlemanboilerplate`. During the install provide the sudo password to install the gems globally
    or skip with control-c to install them under vendor/bundle (so they are inline with the current config)
  - You might need to adjust `config.rb` to match your exact assets path to `vendor/bundle/something/something...`
  - Run `bundle exec middleman`
  - Go to http://localhost:4567, your website should be ready with all the SASS files compiled

## Then...
 
  - Develop something cool
  - `git init`
  - Commit and push (`.gitignore` will ignore build and vendor folders)
  - Setup your remote repo url in the deploy params of `config.rb`
  - Run `bundle exec middleman deploy`. The static code (build folder) should now be in the `compiled` branch of your remote repo.