# Snaps

{% hint style="success" %}
**Rocket.Chat 6.0** is our most secure and scalable version yet. It includes 10 security patches, 9 brand-new features, and 25+ overall platform enhancements. Visit our [website](https://www.rocket.chat/six) to learn more about what’s new in this latest version. [Update now](https://docs.rocket.chat/deploy/updating-rocket.chat)!
{% endhint %}

## Installation

Snap is pre-installed in most modern distributions. If it is not, please read snap's [official documentation](https://snapcraft.io/docs/installing-snapd) on how to install snap.

Installing Rocket.Chat with snap on Ubuntu is as easy as executing:

```
sudo snap install rocketchat-server
```

Then browse to `http://localhost:3000` and setup Rocket.Chat.

The above command should install the latest version available. You can also specify install by track.

Snaps are secure. Rocket.Chat and all of its dependencies are isolated from the rest of your system. Snaps also auto-update when we release a new version. So no need for more hassle updating.

To move between different major releases, from 2.x to 3.x or from 3.x to 4.x, take a look at [snap tracks](https://forums.rocket.chat/t/introducing-snap-tracks/5890).

## Configuration

**To configure snap variables for your Rocket.Chat server:**

To see the list of snap variables to configure for your Rocket.Chat server, run:

```shell
snap get rocketchat-server
```

A list of variables is displayed

```
Key                Value
backup-on-refresh  disable
ignore-errors      false
mongo-oplog-url    mongodb://localhost:27017/local
mongo-url          mongodb://localhost:27017/parties
port               3000
siteurl            http://localhost:3000
```

Setting one is done by simply executing

```bash
sudo snap set rocketchat-server <variable-name>=<value>
```
