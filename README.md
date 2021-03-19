# Dokku Sentry Webhook

Dokku Sentry Webhook is a plugin for [Dokku](https://github.com/dokku/dokku) that notifies
[Sentry](https://sentry.io/) of deployments.

## Installation

```sh
# dokku 0.3.26
$ git clone https://github.com/yalabot/dokku-sentry-webhook /var/lib/dokku/plugins/sentry-webhook

# dokku 0.4+
$ dokku plugin:install https://github.com/yalabot/dokku-sentry-webhook.git
```

## Commands

```sh
$ dokku help
    sentry:set <app> <webhook_url>                   Set Sentry WebHook URL
    sentry:clear <app>                               Clears Sentry WebHook URL
    sentry:get <app>                                 Display Sentry WebHook URL
```

The webhook URL can be found under the "Release Tracking" settings section of
individual Sentry projects. There is a "Webhook" box with a long URL
in the format `https://<sentry-host>/api/hooks/release/builtin/<n>/<long-hash>/`.

## License

The MIT License (MIT)

Copyright (c) 2015 ribot (dokku-slack)
Copyright (c) 2017 Jannis Leidel (dokku-sentry-webhook)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
