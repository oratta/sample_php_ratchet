以下構築手順

oratta-MacBook@oratta:Program $ mkdir websocket_sample
oratta-MacBook@oratta:Program $ cd websocket_sample/
oratta-MacBook@oratta:websocket_sample $ vi composer.json
{
  "require": {
    "cboden/Ratchet": "0.2.*"
  }
}

oratta-MacBook@oratta:websocket_sample $ curl -s http://getcomposer.org/installer | php
#!/usr/bin/env php
All settings correct for using Composer
Downloading...

Composer successfully installed to: /Users/oratta/Dropbox/Program/websocket_sample/composer.phar
Use it: php composer.phar
oratta-MacBook@oratta:websocket_sample $ php composer.phar install
Loading composer repositories with package information
Installing dependencies (including require-dev)
- Installing symfony/routing (v2.6.1)
Downloading: 100%

- Installing symfony/http-foundation (v2.6.1)
Downloading: 100%

- Installing symfony/event-dispatcher (v2.6.1)
Downloading: 100%

- Installing guzzle/common (v3.9.2)
Downloading: 100%

- Installing guzzle/stream (v3.9.2)
Downloading: 100%

- Installing guzzle/parser (v3.9.2)
Downloading: 100%

- Installing guzzle/http (v3.9.2)
Downloading: 100%

- Installing evenement/evenement (v2.0.0)
Downloading: 100%

- Installing react/stream (v0.4.2)
Downloading: 100%

- Installing react/event-loop (v0.4.1)
Downloading: 100%

- Installing react/socket (v0.4.2)
Downloading: 100%

- Installing cboden/ratchet (v0.3.2)
Downloading: 100%

symfony/routing suggests installing symfony/config (For using the all-in-one router or any loader)
symfony/routing suggests installing symfony/yaml (For using the YAML loader)
symfony/routing suggests installing symfony/expression-language (For using expression matching)
symfony/routing suggests installing doctrine/annotations (For using the annotation loader)
symfony/event-dispatcher suggests installing symfony/dependency-injection ()
symfony/event-dispatcher suggests installing symfony/http-kernel ()
react/stream suggests installing react/promise (~2.0)
react/event-loop suggests installing ext-libevent (>=0.1.0)
react/event-loop suggests installing ext-event (~1.0)
react/event-loop suggests installing ext-libev (*)
Writing lock file
Generating autoload files

oratta-MacBook@oratta:Program $ mkdir app
oratta-MacBook@oratta:Program $ cd app
oratta-MacBook@oratta:Program $ vi chat.php
oratta-MacBook@oratta:Program $ vi chat.html
oratta-MacBook@oratta:Program $ php chat.php
