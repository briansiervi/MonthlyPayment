## Enviroment
### Install Ruby on Ubuntu
```
sudo apt-get install ruby-full
```
font: https://www.ruby-lang.org/pt/documentation/installation/#apt

### Install Rails on Ubuntu
```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev nodejs yarn
```

Install RBenv
```
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 2.5.3
rbenv global 2.5.3
ruby -v
```

Update Gem
```
gem update
```

Install bundler
```
gem install bundler
```

Run Rails
```
rails server
```
font: https://gorails.com/setup/ubuntu/18.04#final-steps

### Install Webpacker
No arquivo Gemfile, adicionar a gem:
```
gem 'webpacker'
```

Rodar os comandos
```
bundle install
```
```
bin/rails webpacker:install
```
```
bin/rails webpacker:install:vue
```
```
bin/yarn install
```
```
yarn add vue-turbolinks vue-resource
```
```
yarn add bulma
```