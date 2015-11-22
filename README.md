# Ruby Setup on OSX
Setting up and installing rbenv, ruby-build, bundler, rbenv-gemset on OS X

Download XCode from Mac App Store

Install command line tools
`xcode-select --install`

Install Homebrew
`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

Install rbenv using Homebrew
'brew install rbenv'

Modify bash_profile or profile to enable rbenv
`echo 'eval "$(rbenv init -)"' >> ~/.profile`<br>
`source ~/.profile`

Install ruby-build
`brew install ruby-build`

Check for the latest stable ruby versions
`ruby-build --definitions`

Install latest ruby version
`rbenv install 2.2.3`<br>
`rbenv rehash`

Set global ruby version to the installed one
`rbenv global 2.2.3`

Show current ruby version
`ruby -v`

Show all installed ruby versions
`rbenv versions`

Install bundler
`gem install bundler`<br>
`rbenv rehash`

Install rbenv-gemset
`brew install rbenv-gemset`

create a new gemset for your ruby project
`rbenv gemset create {ruby version} {gemset-name}`
###### Example
`rbenv gemset create 2.2.3 project1`

create .rbenv-gemset
`echo '{gemset-name}'> .rbenv-gemset`
###### Example
`echo 'project1'> .rbenv-gemset`
`
