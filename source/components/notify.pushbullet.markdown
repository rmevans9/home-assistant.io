---
layout: page
title: "PushBullet notification support"
description: "Instructions how to add user notifications to Home Assistant."
date: 2015-01-20 22:36
sidebar: false
comments: false
sharing: true
footer: true
---

<img src='/images/supported_brands/pushbullet.png' class='brand pull-right' />
Home Assistant currently supports the awesome [PushBullet](https://www.pushbullet.com/), a free service to send information between your phones, browsers and friends.

To add PushBullet to your installation, add the following to your `configuration.yaml` file:

```yaml
notify:
  name: NOTIFIER_NAME
  platform: pushbullet
  api_key: YOUR_API_KEY
```

Setting the optional parameter `name` allows multiple notifiers to be created.
The default value is `notify`. The notifier will bind to the service
`notify.NOTIFIER_NAME`.

For more automation examples, see the [getting started with automation page]({{site_root}}/components/automation.html).
