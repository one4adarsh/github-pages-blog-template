# me

## Setup and run locally -
- In Visual Studio Code, install two extensions: 
  - Docker (from Microsoft)
  - Dev Containers (from Microsoft)
- Open the repository in `Dev Container -> Open Folder in Container`
- Install the bundle - `bundle install`
- Update the bundle - `bundle update`
- Run using - `bundle exec jekyll serve --livereload`

## Initial setup steps -
- setup `Dockerfile`
- open project in Dev Containers
- check for installed ruby version - `ruby -v`
- check for installed jekyll version - `jekyll -v`
- setup new jekyll project - `jekyll new . --skip-bundle --force`
- add webrick dependency to the bundle - `bundle add webrick`
- install the bundle - `bundle install`
- update the bundle - `bundle update`
- delete `Gemfile.lock` file
- in `Gemfile`, remove auto-configuration -
  ```
    gem "jekyll", "~> 4.3.3"
    gem "minima", "~> 2.0"
  ```
- in `Gemfile`, manually configure -
  ```
    gem "jekyll", "~> 4.2.0"
    gem "minima", github: "jekyll/minima"
    gem "jekyll-feed", "~> 0.12"
    gem "jekyll-seo-tag"
    gem "jekyll-remote-theme"
  ```
- update the bundle - `bundle update`
- run using - `bundle exec jekyll serve --livereload`

- [refer here](https://youtu.be/zijOXpZzdvs?si=D9Bmpqtt1hoF3x6s)
