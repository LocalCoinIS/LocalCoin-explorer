# Open Source LocalCoin Explorer

http://LLC.is

## Install

clone repo:

```
git clone https://github.com/LocalCoinIS/LocalCoin-explorer
cd localcoin-explorer
```

* change localhost if you want to listen outside at https://github.com/LocalCoinIS/LocalCoin-explorer/blob/master/package.json#L57
* change your hostname in grunt if needed: https://github.com/LocalCoinIS/LocalCoin-explorer/blob/master/Gruntfile.js#L61

Install node dependencies:

`npm install`

Install bower dependencies:

`bower install`

or

`bower install --allow-root`

Install compass:

```
sudo apt install ruby-compass
sudo gem install compass
```

Start by npm:

`npm start`

Point your browser to:

http://localhost:8900

Start by grunt:

`grunt serve`

Point your browser to http://localhost:8900 to have a developer version with auto load of changed code.

Create distribution version and move everything to http server:

```
grunt serve:dist --force
cp -rf dist/* /var/www/llc.is/public_html/
```

Point your browser to domain: http://LLC.is
