---
title: websocket
type: output
---

<!--
     THIS FILE IS AUTOGENERATED!

     To make changes please edit the contents of:
     lib/output/websocket.go
-->


Sends messages to an HTTP server via a websocket connection.


import Tabs from '@theme/Tabs';

<Tabs defaultValue="common" values={[
  { label: 'Common', value: 'common', },
  { label: 'Advanced', value: 'advanced', },
]}>

import TabItem from '@theme/TabItem';

<TabItem value="common">

```yaml
# Common config fields, showing default values
output:
  websocket:
    url: ws://localhost:4195/post/ws
```

</TabItem>
<TabItem value="advanced">

```yaml
# All config fields, showing default values
output:
  websocket:
    url: ws://localhost:4195/post/ws
    oauth:
      access_token: ""
      access_token_secret: ""
      consumer_key: ""
      consumer_secret: ""
      enabled: false
      request_url: ""
    basic_auth:
      enabled: false
      password: ""
      username: ""
```

</TabItem>
</Tabs>

## Fields

### `url`

The URL to connect to.


Type: `string`  
Default: `"ws://localhost:4195/post/ws"`  

### `oauth`

Allows you to specify open authentication.


Type: `object`  
Default: `{"access_token":"","access_token_secret":"","consumer_key":"","consumer_secret":"","enabled":false,"request_url":""}`  

```yaml
# Examples

oauth:
  access_token: baz
  access_token_secret: bev
  consumer_key: foo
  consumer_secret: bar
  enabled: true
  request_url: http://thisisjustanexample.com/dontactuallyusethis
```

### `basic_auth`

Allows you to specify basic authentication.


Type: `object`  
Default: `{"enabled":false,"password":"","username":""}`  

```yaml
# Examples

basic_auth:
  enabled: true
  password: bar
  username: foo
```


