# PHP

## Set `phpenv`

```bash
git clone https://github.com/CHH/phpenv.git
git clone https://github.com/CHH/php-build.git ~/.phpenv/plugins/php-build
cd phpenv/bin
./phpenv-install.sh
```

Set the config at `.bash_profile`

```bash
sudo vi ~/.bash_profile

export PATH="$HOME/.phpenv/bin:$PATH"
eval "$(phpenv init -)"

source ~/.bash_profile
```

It's hard to use PHP and you will install `re2c`, `libmcrypt`, `libxml2`, `autoconf`, and `automake`

```bash
brew search bison
echo 'export PATH="/usr/local/opt/bison@2.7/bin:$PATH"'

brew install libxml2
echo 'export PATH="/usr/local/opt/libxml2/bin:$PATH"'
```

After setting, quit the terminal session

List of `PHP` versions that can be installed

```bash
phpenv install --list
phpenv install 7.2.13
phpenv global 7.2.13
phpenv rehash
php -v
```

## Install `composer`

Create a composer project

```bash
git clone https://github.com/ngyuki/phpenv-composer.git ~/.phpenv/plugins/phpenv-composer
composer --version
```
