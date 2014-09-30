### Fixturesについて(6)

* YAMLのマージ機能も使える
* "DEFAULTS"というラベルの値は無視される

```yaml
# stores.yml
DEFAULTS: &DEFAULTS
  closed: false

MIYAWAKI_GROUP: &MIYAWAKI_GROUP
  <<: *DEFAULTS
  group_id: 10

iwase:
  <<: *DEFAULTS
  name: 岩瀬書店
  address: どこか

miyawaki_honten:
  <<: *MIYAWAKI_GROUP
  name: 宮脇書店 本店
  address: どこか2
```

上記例の場合、"DEFAULT"のデータは出来ないが、"MIYAWAKI_GROUP"のデータは出来てしまう

