# Deprecation

This repo is deprecated and no longer maintained. There is an alternative here: https://github.com/gcohen55/dokku-hipchat-plugin.

#dokku-hipchat

dokku-hipchat is a plugin for [dokku](https://github.com/progrium/dokku) that notifies [hipchat](http://www.hipchat.com) of build/deployment stages.

## Installation

```sh
git clone https://github.com/cef/dokku-hipchat.git /var/lib/dokku/plugins/hipchat
```

## Configuration
edit `/home/dokku/dockerrc` or `/etc/hipchat`

E.G:
```
export HIPCHAT_TOKEN=<token>
export HIPCHAT_ROOM_ID=<room_id>
export HIPCHAT_NOTIFY=1
export HIPCHAT_FROM='Dokku' # optional in v2
export HIPCHAT_API=v1       # version should be v1 or v2
```

see <https://github.com/hipchat/hipchat-cli#environment-variables> for more details.

All future deployments will notify hipchat pre/post build/deploy.


## License

The MIT License (MIT)

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

[hipchat-cli]: http://github.com/hipchat/hipchat-cli
