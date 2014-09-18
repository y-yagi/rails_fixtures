### fixtureについて(6)

* YAMLのマージ機能も使える
  * "DEFAULTS"は無視される

```
DEFAULTS: &DEFAULTS
  closed: false

MIYAWAKI_GROUP: &MIYAWAKI_GROUP
  <<: *DEFAULTS
  group_id: 10

iwase:
  <<: *DEFAULTS
  name: 岩瀬書店
  address: どこか
  tel: xxxx-xxxx-xxx
  email: shoten@exmaple.com

miyawaki_honten:
  <<: *MIYAWAKI_GROUP
  name: 宮脇書店 本店
  address: どこか2
  tel: xxxx-xxxx-000
  email: miyawaki@exmaple.com
```

上記の場合、"DEFAULT"のデータは出来ないが、"MIYAWAKI_GROUP"のデータは出来てしまう

