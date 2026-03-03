# 保留所有原CURL


# 首页信息获取
<details>
<summary>CURL</summary>

```curl
curl -X GET 'https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/index?avatar_list_type=1&server=cn_gf01&role_id=XXXX' -H 'User-Agent: Mozilla/5.0 (Linux; Android 12; 2211133C Build/V417IR; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/110.0.5481.154 Safari/537.36 miHoYoBBS/2.102.1' -H 'Accept: application/json, text/plain, */*' -H 'Accept-Encoding: gzip, deflate' -H 'DS: 1772518716,165572,1fc88d5574fdd7838b4596864ca30cd9' -H 'x-rpc-app_version: 2.102.1' -H 'x-rpc-tool_verison: v6.4.0-gr-cn' -H 'x-rpc-device_id: 40818f2a-2395-38df-ab11-93371b77324e' -H 'x-rpc-device_name: Xiaomi%202211133C' -H 'x-rpc-page: v6.4.0-gr-cn_#/ys' -H 'x-rpc-device_fp: 38d816239aab3' -H 'x-rpc-sys_version: 12' -H 'x-rpc-client_type: 5' -H 'Origin: https://webstatic.mihoyo.com' -H 'X-Requested-With: com.mihoyo.hyperion' -H 'Sec-Fetch-Site: same-site' -H 'Sec-Fetch-Mode: cors' -H 'Sec-Fetch-Dest: empty' -H 'Referer: https://webstatic.mihoyo.com/' -H 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7' -H 'Cookie: XXXX'
```
</details>

**请求方式：GET**

> 链接：`https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/index`

参数：
| 字段 | 类型 | 内容 | 备注 |
| ---- | ---- | ---- | ---- |
| avatar_list_type | int | 1 | 未知 |
| server | str | cn_gf01 | 服务器 |
| role_id | int | ~ | 角色id |

<details>
<summary>json格式的参数</summary>

```json
{
  "avatar_list_type": "1",
  "server": "cn_gf01",
  "role_id": "XXXX"
}
```
</details>

**请求头**

> tips:这里只写必要请求头

| 字段 | 类型 | 内容 | 是否必填 |
| ---- | ---- | ---- | ---- |
| User-Agent | str | miHoYoBBS/2.102.1 | 是 |
| x-rpc-device_id | str | 40818f2a-2395-38df-ab11-93371b77324e | x-rpc-device_fp二选一 |
| x-rpc-device_fp | str | 38d816239aab3 | x-rpc-device_id二选一 |
| Origin | str | https://webstatic.mihoyo.com | 是 |
| Referer | str | https://webstatic.mihoyo.com/ | 是 |
| Cookie | str | account_mid_v2 | 是 |
| Cookie | str | cookie_token_v2 | 是 |

<details>
<summary>json格式的请求头</summary>

```json
{
  "User-Agent": "Mozilla/5.0 (Linux; Android 12; 2211133C Build/V417IR; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/110.0.5481.154 Safari/537.36 miHoYoBBS/2.102.1",
  "x-rpc-device_fp": "38d816239aab3",
  "Origin": "https://webstatic.mihoyo.com",
  "Referer": "https://webstatic.mihoyo.com/",
  "Cookie": "cookie_token_v2=XX;account_mid_v2=XX"
}
```
</details>

**响应体**

> tips：这里只留返回示例，不对返回进行拆解

<details>
<summary>json格式的响应体</summary>

```json
{
  "retcode": 0,
  "message": "OK",
  "data": {
    "role": {
      "AvatarUrl": "",
      "nickname": "苏辞",
      "region": "天空岛",
      "level": 56,
      "game_head_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/6966dc8c/23699df26cdbcabbddca5ac3830ebd43.png"
    },
    "avatars": [
      {
        "id": 10000052,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/23aa979c8e86b7006a62039b9dd81c5b.png",
        "name": "雷电将军",
        "element": "Electro",
        "fetter": 10,
        "level": 90,
        "rarity": 5,
        "actived_constellation_num": 0,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/46a9bec95f302341ab00637840aa4e5d.png",
        "is_chosen": false,
        "weapon": {
          "id": 13415,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/643071ffc7526446b48101f159ee0437.png",
          "type": 13,
          "rarity": 4,
          "level": 80,
          "affix_level": 5,
          "name": "「渔获」"
        },
        "relics": [
          {
            "id": 29543,
            "name": "旅途中的鲜花",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/17dfffacc89923b85f3fa406f041208e.png",
            "pos": 1,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150291,
              "name": "水仙之梦",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%水元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "普通攻击、重击、下落攻击、元素战技或元素爆发命中敌人后，将产生1层持续8秒的「镜中水仙」效果。处于1/2/3层及以上「镜中水仙」效果下时，攻击力将提高7%/16%/25%，水元素伤害加成提升4%/9%/15%。由普通攻击、重击、下落攻击、元素战技或元素爆发产生的「镜中水仙」将分别独立存在。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94523,
            "name": "切落之羽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/35a171a3906cf9789f208628f0f28770.png",
            "pos": 2,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94553,
            "name": "雷云之笼",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/30ad4db8661bccad21474d67fad9d908.png",
            "pos": 3,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94513,
            "name": "绯花之壶",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/24b9a122db4e39e9b9e2eb1cbcf5925f.png",
            "pos": 4,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94534,
            "name": "华饰之兜",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/8af0dc3497b273ccdee34d2cc948aa59.png",
            "pos": 5,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000030,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/9dcda1d9e45a4f9e59266480ee2fc0c8.png",
        "name": "钟离",
        "element": "Geo",
        "fetter": 10,
        "level": 90,
        "rarity": 5,
        "actived_constellation_num": 2,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f913c3175bbbd4b87e56fcac393584f1.png",
        "is_chosen": false,
        "weapon": {
          "id": 13303,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/badaa063427a6e3f39d9c031b3dddc24.png",
          "type": 13,
          "rarity": 3,
          "level": 60,
          "affix_level": 5,
          "name": "黑缨枪"
        },
        "relics": [
          {
            "id": 91544,
            "name": "勋绩之花",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e52f0d8928f3982864ecc8ea13165ebf.png",
            "pos": 1,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150171,
              "name": "千岩牢固",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "生命值提升20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "元素战技命中敌人后，使队伍中附近的所有角色攻击力提升20%，护盾强效提升30%，持续3秒。该效果每0.5秒至多触发一次。装备此圣遗物套装的角色处于队伍后台时，依然能触发该效果。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 91523,
            "name": "昭武翎羽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/84ba5a506941c2e7c67eec4fc91f6e6a.png",
            "pos": 2,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150171,
              "name": "千岩牢固",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "生命值提升20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "元素战技命中敌人后，使队伍中附近的所有角色攻击力提升20%，护盾强效提升30%，持续3秒。该效果每0.5秒至多触发一次。装备此圣遗物套装的角色处于队伍后台时，依然能触发该效果。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 91553,
            "name": "金铜时晷",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/5e1fe50f98902ba239b743a552c95288.png",
            "pos": 3,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150171,
              "name": "千岩牢固",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "生命值提升20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "元素战技命中敌人后，使队伍中附近的所有角色攻击力提升20%，护盾强效提升30%，持续3秒。该效果每0.5秒至多触发一次。装备此圣遗物套装的角色处于队伍后台时，依然能触发该效果。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94514,
            "name": "绯花之壶",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/24b9a122db4e39e9b9e2eb1cbcf5925f.png",
            "pos": 4,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 91533,
            "name": "将帅兜鍪",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/dcdf1f408c923028f4565bcb1f2d12ae.png",
            "pos": 5,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150171,
              "name": "千岩牢固",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "生命值提升20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "元素战技命中敌人后，使队伍中附近的所有角色攻击力提升20%，护盾强效提升30%，持续3秒。该效果每0.5秒至多触发一次。装备此圣遗物套装的角色处于队伍后台时，依然能触发该效果。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000032,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/41a97aae8bf579ce350a90bbddc59fdf.png",
        "name": "班尼特",
        "element": "Pyro",
        "fetter": 10,
        "level": 90,
        "rarity": 4,
        "actived_constellation_num": 5,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/697a077514d8ec3820d93d087b57c9a1.png",
        "is_chosen": false,
        "weapon": {
          "id": 11501,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2e40de313b0b488549fde96e553e7fcf.png",
          "type": 1,
          "rarity": 5,
          "level": 80,
          "affix_level": 2,
          "name": "风鹰剑"
        },
        "relics": [
          {
            "id": 94543,
            "name": "明威之镡",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/16879d66028f85addecf5a7208f6bffb.png",
            "pos": 1,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 81523,
            "name": "宗室之翎",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7a7f049517a93e3b317a5c5df8892e60.png",
            "pos": 2,
            "rarity": 5,
            "level": 13,
            "set": {
              "id": 2150071,
              "name": "昔日宗室之仪",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素爆发造成的伤害提升20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，队伍中所有角色攻击力提升20%，持续12秒。该效果不可叠加。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 59453,
            "name": "流放者怀表",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f9dd8d807eaa9ec5997b9c0e6f7cd48c.png",
            "pos": 3,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100091,
              "name": "流放者",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，每2秒为队伍中所有角色（不包括自己）恢复2点元素能量。该效果持续6秒，无法叠加。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 59412,
            "name": "流放者之杯",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7847bfdeab60c072ec09b17462505cdc.png",
            "pos": 4,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100091,
              "name": "流放者",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，每2秒为队伍中所有角色（不包括自己）恢复2点元素能量。该效果持续6秒，无法叠加。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 81534,
            "name": "宗室面具",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2e5e66807c6c65eea1918ce6465cdc74.png",
            "pos": 5,
            "rarity": 5,
            "level": 14,
            "set": {
              "id": 2150071,
              "name": "昔日宗室之仪",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素爆发造成的伤害提升20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，队伍中所有角色攻击力提升20%，持续12秒。该效果不可叠加。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000026,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6dca29648877d9140b67d5ccc3db662e.png",
        "name": "魈",
        "element": "Anemo",
        "fetter": 6,
        "level": 70,
        "rarity": 5,
        "actived_constellation_num": 1,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/06537f8e5fbfcf9f0b2bc8fed3c568c5.png",
        "is_chosen": false,
        "weapon": {
          "id": 13406,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/1117bae36b42e7ace47a411cb4b04ca1.png",
          "type": 13,
          "rarity": 4,
          "level": 50,
          "affix_level": 1,
          "name": "千岩长枪"
        },
        "relics": [
          {
            "id": 97544,
            "name": "生灵之华",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c3b0db3fda0f57be83087e8fa47f248d.png",
            "pos": 1,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150231,
              "name": "辰砂往生录",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，将产生持续16秒的「潜光」效果：攻击力提升8%；并在角色的生命值降低时，攻击力进一步提升10%，至多通过这种方式提升4次，每0.8秒至多触发一次。「潜光」效果将在角色退场时消失；持续期间再次施放元素爆发，将移除原有的「潜光」。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 97422,
            "name": "潜光片羽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0fce49c2072b19b474a29a3ea2300bd8.png",
            "pos": 2,
            "rarity": 4,
            "level": 16,
            "set": {
              "id": 2150231,
              "name": "辰砂往生录",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，将产生持续16秒的「潜光」效果：攻击力提升8%；并在角色的生命值降低时，攻击力进一步提升10%，至多通过这种方式提升4次，每0.8秒至多触发一次。「潜光」效果将在角色退场时消失；持续期间再次施放元素爆发，将移除原有的「潜光」。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 93553,
            "name": "朝露之时",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f8a6ac0223534c936003a96d018d498b.png",
            "pos": 3,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150191,
              "name": "追忆之注连",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技时，如果角色的元素能量高于或等于15点，则会流失15点元素能量，使接下来的10秒内，普通攻击、重击、下落攻击造成的伤害提高50%，持续期间内该效果不会再次触发。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 97412,
            "name": "结契之刻",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/801da1ab1db5f074ca151126b0f8aa73.png",
            "pos": 4,
            "rarity": 4,
            "level": 16,
            "set": {
              "id": 2150231,
              "name": "辰砂往生录",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，将产生持续16秒的「潜光」效果：攻击力提升8%；并在角色的生命值降低时，攻击力进一步提升10%，至多通过这种方式提升4次，每0.8秒至多触发一次。「潜光」效果将在角色退场时消失；持续期间再次施放元素爆发，将移除原有的「潜光」。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 97432,
            "name": "虺雷之姿",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e9c3254cf0f4952b3e55c6b3b66f9e11.png",
            "pos": 5,
            "rarity": 4,
            "level": 16,
            "set": {
              "id": 2150231,
              "name": "辰砂往生录",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，将产生持续16秒的「潜光」效果：攻击力提升8%；并在角色的生命值降低时，攻击力进一步提升10%，至多通过这种方式提升4次，每0.8秒至多触发一次。「潜光」效果将在角色退场时消失；持续期间再次施放元素爆发，将移除原有的「潜光」。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000005,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/static/player/UI_AvatarIcon_PlayerBoy.png",
        "name": "旅行者",
        "element": "Pyro",
        "fetter": 0,
        "level": 70,
        "rarity": 5,
        "actived_constellation_num": 6,
        "card_image": "https://webstatic.mihoyo.com/upload/static-resource/2023/05/08/ec15648be34aa80db3ac32844af3a467_1847677359435043385.png",
        "is_chosen": false,
        "weapon": {
          "id": 11303,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6b735c4a2cc309a44c5c682f81364261.png",
          "type": 1,
          "rarity": 3,
          "level": 50,
          "affix_level": 1,
          "name": "旅行剑"
        },
        "relics": [
          {
            "id": 98543,
            "name": "魂香之花",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/45b3135178fa8e47165f7b2000479f45.png",
            "pos": 1,
            "rarity": 5,
            "level": 9,
            "set": {
              "id": 2150241,
              "name": "来歆余响",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "普通攻击命中敌人时，有36%概率触发「幽谷祝祀」：普通攻击造成的伤害提高，伤害提高值为攻击力的70%，该效果将在普通攻击造成伤害后的0.05秒后清除。普通攻击未触发「幽谷祝祀」时，会使下次触发概率提升20%；0.2秒内至多判定1次触发与否。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 75524,
            "name": "角斗士的归宿",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/5f120cdac0fc7783d0ba6d1452818d5d.png",
            "pos": 2,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150011,
              "name": "角斗士的终幕礼",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "装备该圣遗物套装的角色为单手剑、双手剑、长柄武器角色时，角色普通攻击造成的伤害提高35%。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 75553,
            "name": "角斗士的希冀",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/34b9935fadcb083f8b4db3c4fd915754.png",
            "pos": 3,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150011,
              "name": "角斗士的终幕礼",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "装备该圣遗物套装的角色为单手剑、双手剑、长柄武器角色时，角色普通攻击造成的伤害提高35%。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 75513,
            "name": "角斗士的酣醉",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0c3a5868f5b77bf7bf8ae6c56e016557.png",
            "pos": 4,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150011,
              "name": "角斗士的终幕礼",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "装备该圣遗物套装的角色为单手剑、双手剑、长柄武器角色时，角色普通攻击造成的伤害提高35%。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 75534,
            "name": "角斗士的凯旋",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/69750e95511b6aed7919f73b1d568ccd.png",
            "pos": 5,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150011,
              "name": "角斗士的终幕礼",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "装备该圣遗物套装的角色为单手剑、双手剑、长柄武器角色时，角色普通攻击造成的伤害提高35%。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000125,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/6966dc8c/3e648c232fb84bea351096c3f2129489.png",
        "name": "哥伦比娅",
        "element": "Hydro",
        "fetter": 1,
        "level": 60,
        "rarity": 5,
        "actived_constellation_num": 0,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/6966dc8c/fedee1565c95644de49e69e26376a52f.png",
        "is_chosen": false,
        "weapon": {
          "id": 14509,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/5df4b80100a07922792ac85362ee6af8.png",
          "type": 10,
          "rarity": 5,
          "level": 50,
          "affix_level": 1,
          "name": "神乐之真意"
        },
        "relics": [
          {
            "id": 57443,
            "name": "教官的胸花",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/ab213bb1abd2a5467d680d5ea9890417.png",
            "pos": 1,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100071,
              "name": "教官",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素精通提高80点。"
                },
                {
                  "activation_number": 4,
                  "effect": "触发元素反应后，队伍中所有角色的元素精通提高120点，持续8秒。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 57422,
            "name": "教官的羽饰",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/239b10d2e54e17572a34ac34156f91fa.png",
            "pos": 2,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100071,
              "name": "教官",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素精通提高80点。"
                },
                {
                  "activation_number": 4,
                  "effect": "触发元素反应后，队伍中所有角色的元素精通提高120点，持续8秒。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 59453,
            "name": "流放者怀表",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f9dd8d807eaa9ec5997b9c0e6f7cd48c.png",
            "pos": 3,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100091,
              "name": "流放者",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，每2秒为队伍中所有角色（不包括自己）恢复2点元素能量。该效果持续6秒，无法叠加。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 59413,
            "name": "流放者之杯",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7847bfdeab60c072ec09b17462505cdc.png",
            "pos": 4,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100091,
              "name": "流放者",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，每2秒为队伍中所有角色（不包括自己）恢复2点元素能量。该效果持续6秒，无法叠加。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 44533,
            "name": "哀慕的恋歌",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/6966dc8c/f73208d0551624c45222e1234e0e0946.png",
            "pos": 5,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150441,
              "name": "风起之日",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "普通攻击、重击、元素战技或元素爆发命中敌人后，将获得持续6秒的「风与牧歌的眷怜」：攻击力提高25%。若装备者已经完成了「魔女的课业」，则「风与牧歌的眷怜」将会升级为「风与牧歌的决意」，额外使通过考验的装备者的暴击率提升20%。装备者处于队伍后台时，也能触发上述效果。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000035,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2825ff5127afc078dd1bd3e1b2e39996.png",
        "name": "七七",
        "element": "Cryo",
        "fetter": 4,
        "level": 60,
        "rarity": 5,
        "actived_constellation_num": 0,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d2e43a6abf3a467608fa3243efcdb1d7.png",
        "is_chosen": false,
        "weapon": {
          "id": 11302,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/048119e09a837be4c1a735fd046e3261.png",
          "type": 1,
          "rarity": 3,
          "level": 20,
          "affix_level": 5,
          "name": "黎明神剑"
        },
        "relics": [
          {
            "id": 74543,
            "name": "远方的少女之心",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/4c8a4c6d40add9e2437f556163501b83.png",
            "pos": 1,
            "rarity": 5,
            "level": 8,
            "set": {
              "id": 2140041,
              "name": "被怜爱的少女",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "角色造成的治疗效果提升15%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技或元素爆发后的10秒内，队伍中所有角色受治疗效果加成提高20%。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 74524,
            "name": "少女飘摇的思念",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b5ff9725aa638fdc76d9eaea734d481e.png",
            "pos": 2,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2140041,
              "name": "被怜爱的少女",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "角色造成的治疗效果提升15%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技或元素爆发后的10秒内，队伍中所有角色受治疗效果加成提高20%。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 74553,
            "name": "少女苦短的良辰",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b8dc97d9352fccfe769738e8d9877252.png",
            "pos": 3,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2140041,
              "name": "被怜爱的少女",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "角色造成的治疗效果提升15%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技或元素爆发后的10秒内，队伍中所有角色受治疗效果加成提高20%。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 74513,
            "name": "少女片刻的闲暇",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/979e1957d22f002ffa7d16d1659107d8.png",
            "pos": 4,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2140041,
              "name": "被怜爱的少女",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "角色造成的治疗效果提升15%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技或元素爆发后的10秒内，队伍中所有角色受治疗效果加成提高20%。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 74533,
            "name": "少女易逝的芳颜",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/37fe25ed4ab1c52a54e0c26017b1cf54.png",
            "pos": 5,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2140041,
              "name": "被怜爱的少女",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "角色造成的治疗效果提升15%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技或元素爆发后的10秒内，队伍中所有角色受治疗效果加成提高20%。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000033,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e23dde6e455a2dc62dcebbf2d41f7f72.png",
        "name": "达达利亚",
        "element": "Hydro",
        "fetter": 4,
        "level": 60,
        "rarity": 5,
        "actived_constellation_num": 0,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e09ed0998404365c2027728fa7d58382.png",
        "is_chosen": false,
        "weapon": {
          "id": 15405,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6b682afb95373317a4a965b8974b5d08.png",
          "type": 12,
          "rarity": 4,
          "level": 70,
          "affix_level": 2,
          "name": "弓藏"
        },
        "relics": [
          {
            "id": 90544,
            "name": "饰金胸花",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e3f3ff85477d75c6b073dcb941865249.png",
            "pos": 1,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150161,
              "name": "沉沦之心",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%水元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技后的15秒内，普通攻击与重击造成的伤害提高30%。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 90524,
            "name": "追忆之风",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c57c81c236d88176a653c2b0be80d71d.png",
            "pos": 2,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150161,
              "name": "沉沦之心",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%水元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技后的15秒内，普通攻击与重击造成的伤害提高30%。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 90554,
            "name": "坚铜罗盘",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6c8ad61b731cc2c0c53ddd4f22e6a50d.png",
            "pos": 3,
            "rarity": 5,
            "level": 16,
            "set": {
              "id": 2150161,
              "name": "沉沦之心",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%水元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技后的15秒内，普通攻击与重击造成的伤害提高30%。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 74514,
            "name": "少女片刻的闲暇",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/979e1957d22f002ffa7d16d1659107d8.png",
            "pos": 4,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2140041,
              "name": "被怜爱的少女",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "角色造成的治疗效果提升15%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技或元素爆发后的10秒内，队伍中所有角色受治疗效果加成提高20%。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 90533,
            "name": "酒渍船帽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/a6efed58b340e9aea774bd7d53544bc7.png",
            "pos": 5,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150161,
              "name": "沉沦之心",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%水元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技后的15秒内，普通攻击与重击造成的伤害提高30%。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000025,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/cf352253ba22524007154d6d6fc66b55.png",
        "name": "行秋",
        "element": "Hydro",
        "fetter": 8,
        "level": 60,
        "rarity": 4,
        "actived_constellation_num": 4,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/89be6f2f06f7b49ccc5c051364e79255.png",
        "is_chosen": false,
        "weapon": {
          "id": 11403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/8d40dcb0e8e25ad6c5940095fa6984ab.png",
          "type": 1,
          "rarity": 4,
          "level": 1,
          "affix_level": 1,
          "name": "祭礼剑"
        },
        "relics": [
          {
            "id": 94543,
            "name": "明威之镡",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/16879d66028f85addecf5a7208f6bffb.png",
            "pos": 1,
            "rarity": 5,
            "level": 10,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94523,
            "name": "切落之羽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/35a171a3906cf9789f208628f0f28770.png",
            "pos": 2,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 77554,
            "name": "终幕的时计",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/00cfc809485c04ff1092838901c8c413.png",
            "pos": 3,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150031,
              "name": "流浪大地的乐团",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素精通提高80点。"
                },
                {
                  "activation_number": 4,
                  "effect": "装备该圣遗物套装的角色为法器、弓箭角色时，角色重击造成的伤害提高35%。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 59412,
            "name": "流放者之杯",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7847bfdeab60c072ec09b17462505cdc.png",
            "pos": 4,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100091,
              "name": "流放者",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，每2秒为队伍中所有角色（不包括自己）恢复2点元素能量。该效果持续6秒，无法叠加。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 59433,
            "name": "流放者头冠",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/22faf0f5c42ac3652ea2c4a1ca38ac05.png",
            "pos": 5,
            "rarity": 4,
            "level": 0,
            "set": {
              "id": 2100091,
              "name": "流放者",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素爆发后，每2秒为队伍中所有角色（不包括自己）恢复2点元素能量。该效果持续6秒，无法叠加。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000023,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c836c2dc7d71fe8065ae2798d360167b.png",
        "name": "香菱",
        "element": "Pyro",
        "fetter": 7,
        "level": 60,
        "rarity": 4,
        "actived_constellation_num": 6,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c56e6b7ce9072e548ea8aaef94db3554.png",
        "is_chosen": false,
        "weapon": {
          "id": 13407,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7db45b7a84bb80468aaf0f5f430e9bdc.png",
          "type": 13,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "西风长枪"
        },
        "relics": [
          {
            "id": 93544,
            "name": "羁缠之花",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/85f548425496394e4b812302b3de514a.png",
            "pos": 1,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150191,
              "name": "追忆之注连",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技时，如果角色的元素能量高于或等于15点，则会流失15点元素能量，使接下来的10秒内，普通攻击、重击、下落攻击造成的伤害提高50%，持续期间内该效果不会再次触发。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 93524,
            "name": "思忆之矢",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/afcf2a5cf7f130054dac4f31dd7d6c03.png",
            "pos": 2,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150191,
              "name": "追忆之注连",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技时，如果角色的元素能量高于或等于15点，则会流失15点元素能量，使接下来的10秒内，普通攻击、重击、下落攻击造成的伤害提高50%，持续期间内该效果不会再次触发。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 92553,
            "name": "停摆之刻",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/22be2edca2dccded53c85f524b860631.png",
            "pos": 3,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150181,
              "name": "苍白之火",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "造成的物理伤害提高25%。"
                },
                {
                  "activation_number": 4,
                  "effect": "元素战技命中敌人后，攻击力提升9%。该效果持续7秒，至多叠加2层，每0.3秒至多触发一次。叠满2层时，2件套的效果提升100%。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 92513,
            "name": "超越之盏",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/86f0c7fcf7afe2813a3d463ab1a5848f.png",
            "pos": 4,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150181,
              "name": "苍白之火",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "造成的物理伤害提高25%。"
                },
                {
                  "activation_number": 4,
                  "effect": "元素战技命中敌人后，攻击力提升9%。该效果持续7秒，至多叠加2层，每0.3秒至多触发一次。叠满2层时，2件套的效果提升100%。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 93533,
            "name": "无常之面",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/71e9ec339457ff7e274469ddb97889f4.png",
            "pos": 5,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150191,
              "name": "追忆之注连",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "攻击力提高18%。"
                },
                {
                  "activation_number": 4,
                  "effect": "施放元素战技时，如果角色的元素能量高于或等于15点，则会流失15点元素能量，使接下来的10秒内，普通攻击、重击、下落攻击造成的伤害提高50%，持续期间内该效果不会再次触发。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000015,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/c1d2a8e0948af4942feb5d086500528b.png",
        "name": "凯亚",
        "element": "Cryo",
        "fetter": 2,
        "level": 60,
        "rarity": 4,
        "actived_constellation_num": 0,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/3adac950e5854a16fa2cb30efc4f005e.png",
        "is_chosen": false,
        "weapon": {
          "id": 11402,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e72bdcaaeb4b0a1ea13cfb76c88aa4cb.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "笛剑"
        },
        "relics": [
          {
            "id": 94544,
            "name": "明威之镡",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/16879d66028f85addecf5a7208f6bffb.png",
            "pos": 1,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94524,
            "name": "切落之羽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/35a171a3906cf9789f208628f0f28770.png",
            "pos": 2,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94554,
            "name": "雷云之笼",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/30ad4db8661bccad21474d67fad9d908.png",
            "pos": 3,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 94513,
            "name": "绯花之壶",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/24b9a122db4e39e9b9e2eb1cbcf5925f.png",
            "pos": 4,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150201,
              "name": "绝缘之旗印",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素充能效率提高20%。"
                },
                {
                  "activation_number": 4,
                  "effect": "基于元素充能效率的25%，提高元素爆发造成的伤害。至多通过这种方式获得75%提升。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 77533,
            "name": "指挥的礼帽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/83903a2b1f0da3e6aeab6328089c9595.png",
            "pos": 5,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150031,
              "name": "流浪大地的乐团",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "元素精通提高80点。"
                },
                {
                  "activation_number": 4,
                  "effect": "装备该圣遗物套装的角色为法器、弓箭角色时，角色重击造成的伤害提高35%。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      },
      {
        "id": 10000047,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7d56eb845d4f982757a942a97f88b958.png",
        "name": "枫原万叶",
        "element": "Anemo",
        "fetter": 9,
        "level": 50,
        "rarity": 5,
        "actived_constellation_num": 0,
        "card_image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0c1aa899e2b8ea002a0249ab1e09da8f.png",
        "is_chosen": false,
        "weapon": {
          "id": 11422,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/74ef003a497f24a85e4e1e0af0793530.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "东花坊时雨"
        },
        "relics": [
          {
            "id": 76544,
            "name": "野花记忆的绿野",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/79119f6a441fc37f39b08f225d63034b.png",
            "pos": 1,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150021,
              "name": "翠绿之影",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%风元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "扩散反应造成的伤害提升60%。根据扩散的元素类型，降低受到影响的敌人40%的对应元素抗性，持续10秒。"
                }
              ]
            },
            "pos_name": "生之花",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 76523,
            "name": "猎人青翠的箭羽",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/37134a2511467762e3a085ab1d043965.png",
            "pos": 2,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150021,
              "name": "翠绿之影",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%风元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "扩散反应造成的伤害提升60%。根据扩散的元素类型，降低受到影响的敌人40%的对应元素抗性，持续10秒。"
                }
              ]
            },
            "pos_name": "死之羽",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 76554,
            "name": "翠绿猎人的笃定",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/892c53d0973b06b805a48c8d5054f53c.png",
            "pos": 3,
            "rarity": 5,
            "level": 20,
            "set": {
              "id": 2150021,
              "name": "翠绿之影",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%风元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "扩散反应造成的伤害提升60%。根据扩散的元素类型，降低受到影响的敌人40%的对应元素抗性，持续10秒。"
                }
              ]
            },
            "pos_name": "时之沙",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 76513,
            "name": "翠绿猎人的容器",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/cfd075bca5834faa858d8a6c5d6dc95c.png",
            "pos": 4,
            "rarity": 5,
            "level": 0,
            "set": {
              "id": 2150021,
              "name": "翠绿之影",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%风元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "扩散反应造成的伤害提升60%。根据扩散的元素类型，降低受到影响的敌人40%的对应元素抗性，持续10秒。"
                }
              ]
            },
            "pos_name": "空之杯",
            "main_property": null,
            "sub_property_list": []
          },
          {
            "id": 76533,
            "name": "翠绿的猎人之冠",
            "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f568e5d02b0cfa74365cda3159cfacc8.png",
            "pos": 5,
            "rarity": 5,
            "level": 1,
            "set": {
              "id": 2150021,
              "name": "翠绿之影",
              "affixes": [
                {
                  "activation_number": 2,
                  "effect": "获得15%风元素伤害加成。"
                },
                {
                  "activation_number": 4,
                  "effect": "扩散反应造成的伤害提升60%。根据扩散的元素类型，降低受到影响的敌人40%的对应元素抗性，持续10秒。"
                }
              ]
            },
            "pos_name": "理之冠",
            "main_property": null,
            "sub_property_list": []
          }
        ]
      }
    ],
    "stats": {
      "active_day_number": 580,
      "achievement_number": 553,
      "anemoculus_number": 66,
      "geoculus_number": 131,
      "avatar_number": 63,
      "way_point_number": 544,
      "domain_number": 50,
      "spiral_abyss": "7-3",
      "precious_chest_number": 173,
      "luxurious_chest_number": 71,
      "exquisite_chest_number": 428,
      "common_chest_number": 396,
      "electroculus_number": 181,
      "magic_chest_number": 32,
      "dendroculus_number": 271,
      "hydroculus_number": 152,
      "pyroculus_number": 17,
      "field_ext_map": {
        "role_combat_pc": {
          "link": "",
          "backup_link": ""
        },
        "common_chest_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=17&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "way_point_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=3,2&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "magic_chest_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=269&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "precious_chest_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=45&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "avatar_number": {
          "link": "",
          "backup_link": ""
        },
        "exquisite_chest_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=44&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "spiral_abyss": {
          "link": "",
          "backup_link": ""
        },
        "geoculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=6&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "domain_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=154&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "hard_challenge": {
          "link": "",
          "backup_link": ""
        },
        "hydroculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=508&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "role_combat": {
          "link": "https://webstatic.mihoyo.com/ys/event/lineup-fe/index.html?mhy_presentation_style=fullscreen&utm_source=bbs&utm_medium=mys&utm_campaign=ImaginariumTheater#/m/index?tab=2",
          "backup_link": ""
        },
        "moonoculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=strategy&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=694&center=306.00,-11007.00&zoom=-2.00",
          "backup_link": ""
        },
        "pyroculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=626&&center=4122.97,-9099.99",
          "backup_link": ""
        },
        "anemoculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=5&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "luxurious_chest_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=46&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "electroculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=194&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        },
        "dendroculus_number": {
          "link": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=403&center=2008.50,-1084.00&zoom=-3.00",
          "backup_link": ""
        }
      },
      "role_combat": {
        "is_unlock": true,
        "max_round_id": 0,
        "has_data": false,
        "has_detail_data": false,
        "tarot_finished_cnt": 0,
        "difficulty_id": 0
      },
      "full_fetter_avatar_num": 3,
      "hard_challenge": {
        "difficulty": 0,
        "name": "摧枯之役",
        "has_data": false,
        "is_unlock": true
      },
      "moonoculus_number": 109
    },
    "city_explorations": [],
    "world_explorations": [
      {
        "level": 0,
        "exploration_percentage": 380,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Nordkalei.png",
        "name": "挪德卡莱",
        "type": "Reputation",
        "offerings": [
          {
            "name": "终夜长茔",
            "level": 0,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_NordkaleiLighthouse.png",
            "open_state": "OfferingOpenStateLocked"
          },
          {
            "name": "叮铃哐啷蛋卷工坊",
            "level": 1,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_NordkaleiGarbage.png",
            "open_state": "OfferingOpenStateUnlocked"
          },
          {
            "name": "霜月之坊",
            "level": 4,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_NordkaleiCamp.png",
            "open_state": "OfferingOpenStateUnlocked"
          },
          {
            "name": "魔女的花园",
            "level": 4,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_NordkaleiRoleCombat.png",
            "open_state": "OfferingOpenStateUnlocked"
          },
          {
            "name": "西风戍垒",
            "level": 5,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_NordkaleiTuanZhang.png",
            "open_state": "OfferingOpenStateUnlocked"
          },
          {
            "name": "望崖营壁",
            "level": 4,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_NordkaleiShouYe.png",
            "open_state": "OfferingOpenStateUnlocked"
          }
        ],
        "id": 17,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=strategy&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=-390.00,-10652.50&zoom=-1.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/472?bbs_presentation_style=no_header",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Nordkalei.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Nordkalei.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Nordkalei.png",
        "area_exploration_list": [
          {
            "name": "帕哈岛",
            "exploration_percentage": 77
          },
          {
            "name": "伦波岛",
            "exploration_percentage": 243
          },
          {
            "name": "希汐岛",
            "exploration_percentage": 879
          },
          {
            "name": "虚海望",
            "exploration_percentage": 840
          },
          {
            "name": "逐浪野",
            "exploration_percentage": 962
          },
          {
            "name": "烟硌山峰",
            "exploration_percentage": 877
          }
        ],
        "boss_list": [
          {
            "name": "蕴光月幻蝶",
            "kill_num": 2
          },
          {
            "name": "重拳出击鸭",
            "kill_num": 1
          },
          {
            "name": "霜夜巡天灵主",
            "kill_num": 0
          },
          {
            "name": "超重型陆巡舰·机动战垒",
            "kill_num": 0
          },
          {
            "name": "深黯魇语之主",
            "kill_num": 0
          },
          {
            "name": "蕴光月守宫",
            "kill_num": 0
          }
        ],
        "is_hot": false,
        "index_active": true,
        "detail_active": true,
        "seven_statue_level": 5,
        "natan_reputation": null,
        "world_type": 2
      },
      {
        "level": 0,
        "exploration_percentage": 100,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Nata.png",
        "name": "纳塔",
        "type": "Reputation",
        "offerings": [
          {
            "name": "煅石之火",
            "level": 2,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_PaskTemple.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 15,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?&center=4122.97,-9099.99",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/409?bbs_presentation_style=no_header",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Nata.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Nata.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Nata.png",
        "area_exploration_list": [
          {
            "name": "坚岩隘谷",
            "exploration_percentage": 167
          },
          {
            "name": "万火之瓯",
            "exploration_percentage": 185
          },
          {
            "name": "涌流地",
            "exploration_percentage": 52
          },
          {
            "name": "踞石山",
            "exploration_percentage": 109
          },
          {
            "name": "镜璧山",
            "exploration_percentage": 223
          },
          {
            "name": "奥奇卡纳塔",
            "exploration_percentage": 5
          },
          {
            "name": "翘枝崖",
            "exploration_percentage": 147
          },
          {
            "name": "安饶之野",
            "exploration_percentage": 57
          },
          {
            "name": "悠悠度假村",
            "exploration_percentage": 287
          }
        ],
        "boss_list": [
          {
            "name": "贪食匿叶龙山王",
            "kill_num": 0
          },
          {
            "name": "金焰绒翼龙暴君",
            "kill_num": 0
          },
          {
            "name": "秘源机兵·构型械",
            "kill_num": 0
          },
          {
            "name": "深邃摹结株",
            "kill_num": 0
          },
          {
            "name": "灵觉隐修的迷者",
            "kill_num": 0
          },
          {
            "name": "熔岩辉龙像",
            "kill_num": 0
          },
          {
            "name": "秘源机兵·统御械",
            "kill_num": 0
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 1,
        "natan_reputation": {
          "tribal_list": [
            {
              "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/icon_2.png",
              "image": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/background_2.png",
              "name": "「流泉之众」",
              "id": 2,
              "level": 0
            },
            {
              "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/icon_1.png",
              "image": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/background_1.png",
              "name": "「悬木人」",
              "id": 1,
              "level": 0
            },
            {
              "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/icon_3.png",
              "image": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/background_3.png",
              "name": "「回声之子」",
              "id": 3,
              "level": 0
            },
            {
              "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/icon_4.png",
              "image": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/background_4.png",
              "name": "「花羽会」",
              "id": 4,
              "level": 0
            },
            {
              "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/icon_5.png",
              "image": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/background_5.png",
              "name": "「烟谜主」",
              "id": 5,
              "level": 0
            },
            {
              "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/icon_6.png",
              "image": "https://act-webstatic.mihoyo.com/game_record/genshin/tribal_reputation/background_6.png",
              "name": "「沃陆之邦」",
              "id": 6,
              "level": 0
            }
          ]
        },
        "world_type": 2
      },
      {
        "level": 0,
        "exploration_percentage": 183,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_TheOldSea.png",
        "name": "旧日之海",
        "type": "TypeUnknow",
        "offerings": [],
        "id": 14,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/34",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/384?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_TheOldSea.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_TheOldSea.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_TheOldSea.png",
        "area_exploration_list": [],
        "boss_list": [],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 0,
        "exploration_percentage": 222,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_ChenYuVale.png",
        "name": "沉玉谷·上谷",
        "type": "TypeUnknow",
        "offerings": [],
        "id": 13,
        "parent_id": 10,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=123.63,-2671.88&zoom=0.50",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/373?bbs_presentation_style=no_header&from=COLLECTION_BG&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_ChenYuVale.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_ChenYuVale.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_ChenYuVale.png",
        "area_exploration_list": [],
        "boss_list": [],
        "is_hot": false,
        "index_active": false,
        "detail_active": false,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 0,
        "exploration_percentage": 189,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_ChenYuVale.png",
        "name": "沉玉谷·南陵",
        "type": "TypeUnknow",
        "offerings": [],
        "id": 12,
        "parent_id": 10,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=815.18,-2869.16&zoom=0.50",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/373?bbs_presentation_style=no_header&from=COLLECTION_BG&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_ChenYuVale.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_ChenYuVale.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_ChenYuVale.png",
        "area_exploration_list": [],
        "boss_list": [],
        "is_hot": false,
        "index_active": false,
        "detail_active": false,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 0,
        "exploration_percentage": 302,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_ChenYuVale.png",
        "name": "来歆山",
        "type": "TypeUnknow",
        "offerings": [],
        "id": 11,
        "parent_id": 10,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=856.37,-3574.15&zoom=1.50",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/373?bbs_presentation_style=no_header&from=COLLECTION_BG&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_ChenYuVale.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_ChenYuVale.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_ChenYuVale.png",
        "area_exploration_list": [],
        "boss_list": [],
        "is_hot": false,
        "index_active": false,
        "detail_active": false,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 1,
        "exploration_percentage": 360,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Fengdan.png",
        "name": "枫丹",
        "type": "Reputation",
        "offerings": [
          {
            "name": "露景泉",
            "level": 0,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_DewTemple.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 9,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=-769.00,-5003.00&zoom=-1.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/341?bbs_presentation_style=no_header&from=COLLECTION_BG&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Fengdan.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Fengdan.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Fengdan.png",
        "area_exploration_list": [
          {
            "name": "白露区",
            "exploration_percentage": 659
          },
          {
            "name": "苍晶区",
            "exploration_percentage": 495
          },
          {
            "name": "枫丹廷区",
            "exploration_percentage": 519
          },
          {
            "name": "黎翡区",
            "exploration_percentage": 550
          },
          {
            "name": "枫丹动能工程科学研究院区",
            "exploration_percentage": 513
          },
          {
            "name": "伊黎耶林区",
            "exploration_percentage": 144
          },
          {
            "name": "莫尔泰区",
            "exploration_percentage": 216
          },
          {
            "name": "诺思托伊区",
            "exploration_percentage": 273
          }
        ],
        "boss_list": [
          {
            "name": "铁甲熔火帝皇",
            "kill_num": 2
          },
          {
            "name": "冰风组曲",
            "kill_num": 1
          },
          {
            "name": "实验性场力发生装置",
            "kill_num": 0
          },
          {
            "name": "千年珍珠骏麟",
            "kill_num": 0
          },
          {
            "name": "水形幻人",
            "kill_num": 5
          },
          {
            "name": "魔像督军",
            "kill_num": 0
          }
        ],
        "is_hot": true,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 6,
        "natan_reputation": null,
        "world_type": 2
      },
      {
        "level": 2,
        "exploration_percentage": 390,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Xumi.png",
        "name": "须弥",
        "type": "Reputation",
        "offerings": [
          {
            "name": "梦之树",
            "level": 2,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_DreamTree.png",
            "open_state": "OfferingOpenStateUnknow"
          },
          {
            "name": "甘露池",
            "level": 0,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_Vourukasha.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 8,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=3311.00,-4372.00&zoom=-1.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3592/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Xumi.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Xumi.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Xumi.png",
        "area_exploration_list": [
          {
            "name": "护世森",
            "exploration_percentage": 521
          },
          {
            "name": "阿陀河谷",
            "exploration_percentage": 572
          },
          {
            "name": "二净甸",
            "exploration_percentage": 563
          },
          {
            "name": "善见地",
            "exploration_percentage": 441
          },
          {
            "name": "道成林",
            "exploration_percentage": 519
          },
          {
            "name": "失落的苗圃",
            "exploration_percentage": 766
          },
          {
            "name": "桓那兰那",
            "exploration_percentage": 632
          },
          {
            "name": "下风蚀地",
            "exploration_percentage": 486
          },
          {
            "name": "列柱沙原",
            "exploration_percentage": 425
          },
          {
            "name": "上风蚀地",
            "exploration_percentage": 422
          },
          {
            "name": "千壑沙地",
            "exploration_percentage": 449
          },
          {
            "name": "荒石苍漠",
            "exploration_percentage": 370
          },
          {
            "name": "浮罗囿",
            "exploration_percentage": 323
          }
        ],
        "boss_list": [
          {
            "name": "掣电树",
            "kill_num": 3
          },
          {
            "name": "兆载永劫龙兽",
            "kill_num": 2
          },
          {
            "name": "翠翎恐蕈",
            "kill_num": 11
          },
          {
            "name": "无相之草",
            "kill_num": 2
          },
          {
            "name": "风蚀沙虫",
            "kill_num": 1
          },
          {
            "name": "半永恒统辖矩阵",
            "kill_num": 1
          },
          {
            "name": "深罪浸礼者",
            "kill_num": 1
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 10,
        "natan_reputation": null,
        "world_type": 2
      },
      {
        "level": 10,
        "exploration_percentage": 706,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_ChasmsMaw.png",
        "name": "层岩巨渊·地下矿区",
        "type": "Offering",
        "offerings": [
          {
            "name": "流明石触媒",
            "level": 10,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_Lumenstone.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 7,
        "parent_id": 6,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/9?shown_types=&center=-1.50,-77.00&zoom=0.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3314/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_ChasmsMaw.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_ChasmsMaw.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_ChasmsMaw.png",
        "area_exploration_list": [],
        "boss_list": [],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 10,
        "exploration_percentage": 371,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_ChasmsMaw.png",
        "name": "层岩巨渊",
        "type": "Offering",
        "offerings": [
          {
            "name": "流明石触媒",
            "level": 10,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_Lumenstone.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 6,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=3025.75,-2558.50&zoom=1.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3314/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_ChasmsMaw.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_ChasmsMaw.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_ChasmsMaw.png",
        "area_exploration_list": [],
        "boss_list": [
          {
            "name": "遗迹巨蛇",
            "kill_num": 3
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 0,
        "exploration_percentage": 183,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Enkanomiya.png",
        "name": "渊下宫",
        "type": "Offering",
        "offerings": [],
        "id": 5,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/7?shown_types=&center=117.50,4.00&zoom=0.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3457/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Enkanomiya.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Enkanomiya.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Enkanomiya.png",
        "area_exploration_list": [],
        "boss_list": [
          {
            "name": "深海龙蜥之群",
            "kill_num": 0
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 4,
        "exploration_percentage": 560,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Daoqi.png",
        "name": "稻妻",
        "type": "Reputation",
        "offerings": [
          {
            "name": "神樱眷顾",
            "level": 10,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_Oraionokami.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 4,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=5137.00,2980.00&zoom=-1.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3495/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Daoqi.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Daoqi.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Daoqi.png",
        "area_exploration_list": [
          {
            "name": "鸣神岛",
            "exploration_percentage": 612
          },
          {
            "name": "神无冢",
            "exploration_percentage": 473
          },
          {
            "name": "八酝岛",
            "exploration_percentage": 733
          },
          {
            "name": "清籁岛",
            "exploration_percentage": 639
          },
          {
            "name": "海祇岛",
            "exploration_percentage": 535
          },
          {
            "name": "鹤观",
            "exploration_percentage": 470
          }
        ],
        "boss_list": [
          {
            "name": "无相之火",
            "kill_num": 4
          },
          {
            "name": "恒常机关阵列",
            "kill_num": 1
          },
          {
            "name": "魔偶剑鬼",
            "kill_num": 10
          },
          {
            "name": "无相之水",
            "kill_num": 1
          },
          {
            "name": "雷音权现",
            "kill_num": 21
          },
          {
            "name": "黄金王兽",
            "kill_num": 4
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 10,
        "natan_reputation": null,
        "world_type": 2
      },
      {
        "level": 9,
        "exploration_percentage": 729,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Dragonspine.png",
        "name": "龙脊雪山",
        "type": "Offering",
        "offerings": [
          {
            "name": "忍冬之树",
            "level": 9,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_Eldertree.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 3,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=1215.50,12.00&zoom=0.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3458/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Dragonspine.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Dragonspine.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Dragonspine.png",
        "area_exploration_list": [],
        "boss_list": [
          {
            "name": "无相之冰",
            "kill_num": 2
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      },
      {
        "level": 3,
        "exploration_percentage": 462,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Liyue.png",
        "name": "璃月",
        "type": "Reputation",
        "offerings": [],
        "id": 2,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=2449.00,-1662.00&zoom=-1.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3494/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Liyue.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Liyue.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Liyue.png",
        "area_exploration_list": [
          {
            "name": "碧水原",
            "exploration_percentage": 557
          },
          {
            "name": "珉林",
            "exploration_percentage": 406
          },
          {
            "name": "云来海",
            "exploration_percentage": 507
          },
          {
            "name": "璃沙郊",
            "exploration_percentage": 389
          },
          {
            "name": "琼玑野",
            "exploration_percentage": 426
          }
        ],
        "boss_list": [
          {
            "name": "无相之岩",
            "kill_num": 27
          },
          {
            "name": "纯水精灵",
            "kill_num": 16
          },
          {
            "name": "爆炎树",
            "kill_num": 34
          },
          {
            "name": "古岩龙蜥",
            "kill_num": 11
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 10,
        "natan_reputation": null,
        "world_type": 2
      },
      {
        "level": 6,
        "exploration_percentage": 699,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_Mengde.png",
        "name": "蒙德",
        "type": "Reputation",
        "offerings": [],
        "id": 1,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=15.50,56.00&zoom=0.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/content/3493/detail?bbs_presentation_style=no_header&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_Mengde.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_Mengde.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_Mengde.png",
        "area_exploration_list": [
          {
            "name": "坠星山谷",
            "exploration_percentage": 571
          },
          {
            "name": "风啸山坡",
            "exploration_percentage": 904
          },
          {
            "name": "苍风高地",
            "exploration_percentage": 775
          },
          {
            "name": "明冠山地",
            "exploration_percentage": 644
          }
        ],
        "boss_list": [
          {
            "name": "无相之雷",
            "kill_num": 20
          },
          {
            "name": "无相之风",
            "kill_num": 9
          },
          {
            "name": "急冻树",
            "kill_num": 19
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 10,
        "natan_reputation": null,
        "world_type": 2
      },
      {
        "level": 0,
        "exploration_percentage": 0,
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterIcon_ChenYuVale.png",
        "name": "沉玉谷",
        "type": "Offering",
        "offerings": [
          {
            "name": "祀珑典仪",
            "level": 0,
            "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterOffering_ChenYuVale.png",
            "open_state": "OfferingOpenStateUnknow"
          }
        ],
        "id": 10,
        "parent_id": 0,
        "map_url": "https://act.mihoyo.com/ys/app/interactive-map/index.html?bbs_presentation_style=no_header&lang=zh-cn&utm_source=gamerecord&utm_medium=ys&utm_campaign=icon&_markerFps=24#/map/2?shown_types=&center=585.50,-2999.00&zoom=0.00",
        "strategy_url": "https://baike.mihoyo.com/ys/strategy/channel/map/45/373?bbs_presentation_style=no_header&from=COLLECTION_BG&utm_source=wiki&utm_medium=ys&utm_campaign=guide",
        "background_image": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterBackground_ChenYuVale.png",
        "inner_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterInnerIcon_ChenYuVale.png",
        "cover": "https://act-webstatic.mihoyo.com/game_record/genshin/city_icon/UI_ChapterCover_ChenYuVale.png",
        "area_exploration_list": [],
        "boss_list": [
          {
            "name": "隐山猊兽",
            "kill_num": 0
          }
        ],
        "is_hot": false,
        "index_active": false,
        "detail_active": true,
        "seven_statue_level": 0,
        "natan_reputation": null,
        "world_type": 1
      }
    ],
    "homes": [
      {
        "level": 3,
        "visit_num": 1,
        "comfort_num": 4020,
        "item_num": 292,
        "name": "罗浮洞",
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_HomeworldModule_2_Pic.png",
        "comfort_level_name": "屋舍俨然",
        "comfort_level_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_Homeworld_Comfort_3.png"
      },
      {
        "level": 3,
        "visit_num": 1,
        "comfort_num": 4020,
        "item_num": 292,
        "name": "妙香林",
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_HomeworldModule_5_Pic.png",
        "comfort_level_name": "屋舍俨然",
        "comfort_level_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_Homeworld_Comfort_3.png"
      },
      {
        "level": 3,
        "visit_num": 1,
        "comfort_num": 4020,
        "item_num": 292,
        "name": "旋流屿",
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_HomeworldModule_6_Pic.png",
        "comfort_level_name": "屋舍俨然",
        "comfort_level_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_Homeworld_Comfort_3.png"
      },
      {
        "level": 3,
        "visit_num": 1,
        "comfort_num": 4020,
        "item_num": 292,
        "name": "炽空境",
        "icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_HomeworldModule_7_Pic.png",
        "comfort_level_name": "屋舍俨然",
        "comfort_level_icon": "https://act-webstatic.mihoyo.com/game_record/genshin/home/UI_Homeworld_Comfort_3.png"
      }
    ],
    "query_tool_link": "https://act.mihoyo.com/ys/event/bbs-achievements-search/index.html?mhy_presentation_style=fullscreen&mhy_auth_required=true&utm_medium=mys&utm_campaign=GameRecordTools",
    "query_tool_image": "https://act-webstatic.mihoyo.com/game_record/genshin/query_tool/query_tool_entry.png"
  }
}
```
</details>

# 全部角色获取

<details>
<summary>CURL</summary>

```curl
curl -X POST 'https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/character/list' -H 'User-Agent: Mozilla/5.0 (Linux; Android 12; 2211133C Build/V417IR; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/110.0.5481.154 Safari/537.36 miHoYoBBS/2.102.1' -H 'Accept: application/json, text/plain, */*' -H 'Accept-Encoding: gzip, deflate' -H 'DS: 1772521319,101954,f0a13cd9787475e112675b18691a5f12' -H 'x-rpc-app_version: 2.102.1' -H 'x-rpc-tool_verison: v6.4.0-gr-cn' -H 'Content-Type: application/json;charset=UTF-8' -H 'x-rpc-device_id: 40818f2a-2395-38df-ab11-93371b77324e' -H 'x-rpc-device_name: Xiaomi%202211133C' -H 'x-rpc-page: v6.4.0-gr-cn_#/ys/role/all' -H 'x-rpc-device_fp: 38d816239aab3' -H 'x-rpc-sys_version: 12' -H 'x-rpc-client_type: 5' -H 'Origin: https://webstatic.mihoyo.com' -H 'X-Requested-With: com.mihoyo.hyperion' -H 'Sec-Fetch-Site: same-site' -H 'Sec-Fetch-Mode: cors' -H 'Sec-Fetch-Dest: empty' -H 'Referer: https://webstatic.mihoyo.com/' -H 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7' -H 'Cookie: XXXX' -d '{"server":"cn_gf01","role_id":"XXXX","sort_type":1}'
```
</details>

**请求方式：POST**

> 链接：`https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/character/list`

请求体：
| 字段 | 类型 | 内容 | 备注 |
| ---- | ---- | ---- | ---- |
| sort_type | int | 1 | 未知 |
| server | str | cn_gf01 | 服务器 |
| role_id | int | ~ | 角色id |

<details>
<summary>json格式的请求体</summary>

```json
{"server":"cn_gf01","role_id":"XXX","sort_type":1}
```
</details>

**请求头**

> tips:这里只写必要请求头

| 字段 | 类型 | 内容 | 是否必填 |
| ---- | ---- | ---- | ---- |
| User-Agent | str | miHoYoBBS/2.102.1 | 是 |
| x-rpc-device_id | str | 40818f2a-2395-38df-ab11-93371b77324e | x-rpc-device_fp二选一 |
| x-rpc-device_fp | str | 38d816239aab3 | x-rpc-device_id二选一 |
| Origin | str | https://webstatic.mihoyo.com | 是 |
| Referer | str | https://webstatic.mihoyo.com/ | 是 |
| Cookie | str | account_mid_v2 | 是 |
| Cookie | str | cookie_token_v2 | 是 |

<details>
<summary>json格式的请求头</summary>

```json
{
  "User-Agent": "Mozilla/5.0 (Linux; Android 12; 2211133C Build/V417IR; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/110.0.5481.154 Safari/537.36 miHoYoBBS/2.102.1",
  "x-rpc-device_fp": "38d816239aab3",
  "Origin": "https://webstatic.mihoyo.com",
  "Referer": "https://webstatic.mihoyo.com/",
  "Cookie": "cookie_token_v2=XX;account_mid_v2=XX"
}
```
</details>

**响应体**

> tips：这里只留返回示例，不对返回进行拆解

<details>
<summary>json格式的响应体</summary>

```json
{
  "retcode": 0,
  "message": "OK",
  "data": {
    "list": [
      {
        "id": 10000052,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/23aa979c8e86b7006a62039b9dd81c5b.png",
        "name": "雷电将军",
        "element": "Electro",
        "fetter": 10,
        "level": 90,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/c3b756f915148bf843c835251fdf8175.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/ecc17cb83ca92fc24f7a39d7605364e3.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13415,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/643071ffc7526446b48101f159ee0437.png",
          "type": 13,
          "rarity": 4,
          "level": 80,
          "affix_level": 5,
          "name": "「渔获」"
        }
      },
      {
        "id": 10000030,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/9dcda1d9e45a4f9e59266480ee2fc0c8.png",
        "name": "钟离",
        "element": "Geo",
        "fetter": 10,
        "level": 90,
        "rarity": 5,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/832a2ae9dc2d28fdfa666274840d1247.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/cf93186ac38ea6cc0b2f6beec7a74813.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13303,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/badaa063427a6e3f39d9c031b3dddc24.png",
          "type": 13,
          "rarity": 3,
          "level": 60,
          "affix_level": 5,
          "name": "黑缨枪"
        }
      },
      {
        "id": 10000032,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/41a97aae8bf579ce350a90bbddc59fdf.png",
        "name": "班尼特",
        "element": "Pyro",
        "fetter": 10,
        "level": 90,
        "rarity": 4,
        "actived_constellation_num": 5,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/d1c2339492d4812908c61e1c9579dfd8.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/455ee1e4da29c15282faba8243bccdcc.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11501,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2e40de313b0b488549fde96e553e7fcf.png",
          "type": 1,
          "rarity": 5,
          "level": 80,
          "affix_level": 2,
          "name": "风鹰剑"
        }
      },
      {
        "id": 10000026,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6dca29648877d9140b67d5ccc3db662e.png",
        "name": "魈",
        "element": "Anemo",
        "fetter": 6,
        "level": 70,
        "rarity": 5,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/bf55352860f5b3108eb48c465fccde16.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/3e0dcded148a669083fab4d52f82c831.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13406,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/1117bae36b42e7ace47a411cb4b04ca1.png",
          "type": 13,
          "rarity": 4,
          "level": 50,
          "affix_level": 1,
          "name": "千岩长枪"
        }
      },
      {
        "id": 10000005,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/static/player/UI_AvatarIcon_PlayerBoy.png",
        "name": "旅行者",
        "element": "Pyro",
        "fetter": 0,
        "level": 70,
        "rarity": 5,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/5b215c3fb522b2845905ce5c0c589a19.png",
        "is_chosen": false,
        "side_icon": "https://webstatic.mihoyo.com/upload/static-resource/2023/06/15/7f6d24a0876515fb2be301e283571304_7649038398754126009.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11303,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6b735c4a2cc309a44c5c682f81364261.png",
          "type": 1,
          "rarity": 3,
          "level": 50,
          "affix_level": 1,
          "name": "旅行剑"
        }
      },
      {
        "id": 10000125,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/6966dc8c/3e648c232fb84bea351096c3f2129489.png",
        "name": "哥伦比娅",
        "element": "Hydro",
        "fetter": 1,
        "level": 60,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/27f7394e8eeae7eb31a2444c5e5caddf.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/6966dceb/6a05d2352e225e42e07f423bbafe7833.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14509,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/5df4b80100a07922792ac85362ee6af8.png",
          "type": 10,
          "rarity": 5,
          "level": 50,
          "affix_level": 1,
          "name": "神乐之真意"
        }
      },
      {
        "id": 10000035,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2825ff5127afc078dd1bd3e1b2e39996.png",
        "name": "七七",
        "element": "Cryo",
        "fetter": 4,
        "level": 60,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/3a92a219f25c707f3acb2f3dac2d5ffd.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/fa562739ce3ca2fd49ca3aa15415392a.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11302,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/048119e09a837be4c1a735fd046e3261.png",
          "type": 1,
          "rarity": 3,
          "level": 20,
          "affix_level": 5,
          "name": "黎明神剑"
        }
      },
      {
        "id": 10000033,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e23dde6e455a2dc62dcebbf2d41f7f72.png",
        "name": "达达利亚",
        "element": "Hydro",
        "fetter": 4,
        "level": 60,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/7b84f34f84e0f9348a20d52a86920d41.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/34531047e67ab5d6c27646d7e0973ed1.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15405,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6b682afb95373317a4a965b8974b5d08.png",
          "type": 12,
          "rarity": 4,
          "level": 70,
          "affix_level": 2,
          "name": "弓藏"
        }
      },
      {
        "id": 10000025,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/cf352253ba22524007154d6d6fc66b55.png",
        "name": "行秋",
        "element": "Hydro",
        "fetter": 8,
        "level": 60,
        "rarity": 4,
        "actived_constellation_num": 4,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/86d17ffd272051cdca2527ec47ad5f35.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/0c63018b6beced753116e3d7c9447188.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/8d40dcb0e8e25ad6c5940095fa6984ab.png",
          "type": 1,
          "rarity": 4,
          "level": 1,
          "affix_level": 1,
          "name": "祭礼剑"
        }
      },
      {
        "id": 10000023,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c836c2dc7d71fe8065ae2798d360167b.png",
        "name": "香菱",
        "element": "Pyro",
        "fetter": 7,
        "level": 60,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/9958d58bde859327052bab638b0003d9.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/b5d779f06e660962dff9009eb58a90f8.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13407,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7db45b7a84bb80468aaf0f5f430e9bdc.png",
          "type": 13,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "西风长枪"
        }
      },
      {
        "id": 10000015,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/c1d2a8e0948af4942feb5d086500528b.png",
        "name": "凯亚",
        "element": "Cryo",
        "fetter": 2,
        "level": 60,
        "rarity": 4,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/bb950d15a14b528e4275f52486339ff8.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/2781c4fee00e263195f4c1f8cc7aa337.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11402,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e72bdcaaeb4b0a1ea13cfb76c88aa4cb.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "笛剑"
        }
      },
      {
        "id": 10000047,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7d56eb845d4f982757a942a97f88b958.png",
        "name": "枫原万叶",
        "element": "Anemo",
        "fetter": 9,
        "level": 50,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/26ea3d4cecb403fc5368b9a24dc03ecd.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/cba1d6c6811a1e599725d8f24b6b7458.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11422,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/74ef003a497f24a85e4e1e0af0793530.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "东花坊时雨"
        }
      },
      {
        "id": 10000065,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/caa2e14875915abee78b186b61fd8f3a.png",
        "name": "久岐忍",
        "element": "Electro",
        "fetter": 1,
        "level": 50,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/e569300674cb9899ed4670e826c15043.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/4e729aba062b54ac30a6351664e19ff1.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11406,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d859d175bb85b6add3dc3df1fb8abc5a.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "试作斩岩"
        }
      },
      {
        "id": 10000034,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/1eb5023b8ca517a5fe27316b3771a191.png",
        "name": "诺艾尔",
        "element": "Geo",
        "fetter": 2,
        "level": 50,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/7aca4472b525f6a6f88024510b04ff51.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/a61ccec5064fe90c87ed3257bc194b19.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12407,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b014e2aa23e856e0cf3f802584b26862.png",
          "type": 11,
          "rarity": 4,
          "level": 60,
          "affix_level": 1,
          "name": "白影剑"
        }
      },
      {
        "id": 10000027,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/3ae1f1d40773cd13d361e329a7efd887.png",
        "name": "凝光",
        "element": "Geo",
        "fetter": 1,
        "level": 50,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/d200947a8ca1886e5b3311225b4918f1.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/66f8c282f99f623c9aedad6851367397.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14409,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/811ff594eebe6cc05f12e02662803239.png",
          "type": 10,
          "rarity": 4,
          "level": 20,
          "affix_level": 2,
          "name": "昭心"
        }
      },
      {
        "id": 10000021,
        "icon": "https://uploadstatic.mihoyo.com/hk4e/e20200928calculate/common/ambor_48e38b5882f6f03c35aa39aa34c4736b.png",
        "name": "安柏",
        "element": "Pyro",
        "fetter": 2,
        "level": 50,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/2779686571b96e4b4a9993136379f692.png",
        "is_chosen": false,
        "side_icon": "https://fastcdn.mihoyo.com/static-resource-v2/2023/12/14/a273217a806ee130b0c0f51bc5542483_2404530785826539052.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15401,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f0b8edcc330cd9de1dcf97eccb20cbaf.png",
          "type": 12,
          "rarity": 4,
          "level": 20,
          "affix_level": 4,
          "name": "西风猎弓"
        }
      },
      {
        "id": 10000014,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f55430aba2d84b36d64136958c58c93a.png",
        "name": "芭芭拉",
        "element": "Hydro",
        "fetter": 3,
        "level": 50,
        "rarity": 4,
        "actived_constellation_num": 5,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/936c9bf53f1888bd930c43e33a9dc041.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/a3c31e121de86652d1ff2cfd717b60fd.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14501,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d3f398d9ee417e931b1e273242dd8008.png",
          "type": 10,
          "rarity": 5,
          "level": 1,
          "affix_level": 1,
          "name": "天空之卷"
        }
      },
      {
        "id": 10000089,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0a024f0f2e06e99d67f112cd12eef4af.png",
        "name": "芙宁娜",
        "element": "Hydro",
        "fetter": 2,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/58caba691327772ae49b7b008f1802d4.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/1111b471573254806ab26b00445c887c.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0b590e80914fdb8e348323fff888be0c.png",
          "type": 1,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "无锋剑"
        }
      },
      {
        "id": 10000079,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e7beb9e36337d7f64139ee0c97d1a93a.png",
        "name": "迪希雅",
        "element": "Pyro",
        "fetter": 1,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/c700870019c97c84e640ea51387f2b19.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/62f2e8efde668b7e5faa0fb1dc173ae6.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b1e284917f1ca8330ba929ef8f116aba.png",
          "type": 11,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "训练大剑"
        }
      },
      {
        "id": 10000069,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2747d92218297b5094d4b8fe6d5f6475.png",
        "name": "提纳里",
        "element": "Dendro",
        "fetter": 2,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/ee11fd3c6c84958fd90ff6ba85001460.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/9bbe29f8328d15e49f8e4aaab46bed5e.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/4a03625fdbc739dca379573871a4c2ca.png",
          "type": 12,
          "rarity": 4,
          "level": 50,
          "affix_level": 1,
          "name": "祭礼弓"
        }
      },
      {
        "id": 10000060,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/e76d6bdb8f4aeea019df7856ef9eca3f.png",
        "name": "夜兰",
        "element": "Hydro",
        "fetter": 2,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/9f98e730e2d288250a2ba7ccc9f51756.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/3d8e3a00e4222b8884c20e376877dddd.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15402,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/da3d5e7bbc112c4e1378de554a79c6c3.png",
          "type": 12,
          "rarity": 4,
          "level": 70,
          "affix_level": 1,
          "name": "绝弦"
        }
      },
      {
        "id": 10000042,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/89d47da9c1ed3ade59b3c9f7fd00f1e8.png",
        "name": "刻晴",
        "element": "Electro",
        "fetter": 1,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/e93402cd5088ae56d51de8bcc4e1d5d9.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/d12210590f6ba921bc3dc2a573c2f387.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11405,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/85dbd526e5a6d0f20af4d0253be63ac0.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 2,
          "name": "匣里龙吟"
        }
      },
      {
        "id": 10000041,
        "icon": "https://uploadstatic.mihoyo.com/hk4e/e20200928calculate/common/mona_8aa370eb786178163aeac539e2776ca3.png",
        "name": "莫娜",
        "element": "Hydro",
        "fetter": 1,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/ef3318d9d27494a23f012bc6517dc91e.png",
        "is_chosen": false,
        "side_icon": "https://fastcdn.mihoyo.com/static-resource-v2/2023/12/14/0e7ededb3585dc109e409e2213c21fe2_7600023040076112955.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/852d232e46ddaacdfcb86b3f53413405.png",
          "type": 10,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "学徒笔记"
        }
      },
      {
        "id": 10000003,
        "icon": "https://uploadstatic.mihoyo.com/hk4e/e20200928calculate/common/qin_a66a25719b062d5e0f8a7271649a6be9.png",
        "name": "琴",
        "element": "Anemo",
        "fetter": 1,
        "level": 40,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/909badef56b2f351ec9c9f01bb4bbc81.png",
        "is_chosen": false,
        "side_icon": "https://fastcdn.mihoyo.com/static-resource-v2/2023/12/14/765bfdef7f70dffdb80d789817f60ffb_7349415683405267997.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11302,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/048119e09a837be4c1a735fd046e3261.png",
          "type": 1,
          "rarity": 3,
          "level": 20,
          "affix_level": 5,
          "name": "黎明神剑"
        }
      },
      {
        "id": 10000076,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/58a03d4cded3b6e93af3cc3efb708031.png",
        "name": "珐露珊",
        "element": "Anemo",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 5,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/20b3c2297a405f88513cee20de705986.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/efda18cb3e43ffbbb8355b54417f05b6.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c75ade4a5acb5eb9aaefbed318bf75ff.png",
          "type": 12,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "猎弓"
        }
      },
      {
        "id": 10000074,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/523506069469ad5f09b79daf6ed3a285.png",
        "name": "莱依拉",
        "element": "Cryo",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/7f6d246705ba2a1fd1f4b137d5c92a16.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/dd8bc4f0aaa4688582f2df8e02fe7d5d.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/8d40dcb0e8e25ad6c5940095fa6984ab.png",
          "type": 1,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "祭礼剑"
        }
      },
      {
        "id": 10000072,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/9ef120c399afbf7f136034b68d721d44.png",
        "name": "坎蒂丝",
        "element": "Hydro",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/382344dc8c318305283031611f53412c.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/7e050106377d0f3946fe28b681dc5da4.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13303,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/badaa063427a6e3f39d9c031b3dddc24.png",
          "type": 13,
          "rarity": 3,
          "level": 1,
          "affix_level": 1,
          "name": "黑缨枪"
        }
      },
      {
        "id": 10000068,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d4892796ad70d139c13a6e42d170b877.png",
        "name": "多莉",
        "element": "Electro",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/ce6448d7d2bf3dc034ad698fa60917ef.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/6ad4b9ea1bc906f7ba8fb547ba3215c6.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12405,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/de1e307e1104fbf7c8f7a7ef5cb143e1.png",
          "type": 11,
          "rarity": 4,
          "level": 1,
          "affix_level": 2,
          "name": "雨裁"
        }
      },
      {
        "id": 10000064,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/45fc56fa83f5447d6a61677f514a9131.png",
        "name": "云堇",
        "element": "Geo",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 3,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/e410b63ff1e7e75b6885573509f29b8e.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/8ae1c762015220916b8ae9da0705a133.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b96753e95648a2ddf2ece0cdcd12b758.png",
          "type": 13,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "流月针"
        }
      },
      {
        "id": 10000059,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c4d144d578bf42c6f03ac240a3bf2c3c.png",
        "name": "鹿野院平藏",
        "element": "Anemo",
        "fetter": 2,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 4,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/fb2e6bafd48ee948080feafb368fed79.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/564bcd0543848e0d208b492f0ed4e999.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14409,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/811ff594eebe6cc05f12e02662803239.png",
          "type": 10,
          "rarity": 4,
          "level": 20,
          "affix_level": 2,
          "name": "昭心"
        }
      },
      {
        "id": 10000055,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/a3a8da43e8c4d76986237ab784e49070.png",
        "name": "五郎",
        "element": "Geo",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/bf916ae0f5a292ef46a279bce7ae66ac.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/4da651801389b89fd68d6e2d873f646b.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15419,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/6e37803f70f76be9df083b99a5af8307.png",
          "type": 12,
          "rarity": 4,
          "level": 20,
          "affix_level": 5,
          "name": "鹮穿之喙"
        }
      },
      {
        "id": 10000053,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/1791a03bc18b12a8030a4e16df2ea5f6.png",
        "name": "早柚",
        "element": "Anemo",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/8ec174eeff413551afbb7974d4a8f3c4.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/bb21a39564805055edf92b88cbed4acb.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12306,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/8b59cc85afa53362080a7682e0b2284c.png",
          "type": 11,
          "rarity": 3,
          "level": 20,
          "affix_level": 1,
          "name": "飞天大御剑"
        }
      },
      {
        "id": 10000044,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/b3085c5955360785fc5a1c25ab1a15f4.png",
        "name": "辛焱",
        "element": "Pyro",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/06875a6a45f98628eac5c8056fdb51b2.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/4bd8a9ca7b168bc417236c3e3e508aba.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12401,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7646388f158d62d56f368631a37427c3.png",
          "type": 11,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "西风大剑"
        }
      },
      {
        "id": 10000043,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/27ee1aba588f3e8e42800249fe1047e8.png",
        "name": "砂糖",
        "element": "Anemo",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/d6cfdc6183ec1465fef3261baeba31f0.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/9bc7734e2c50399b56e3ad152d71d159.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14304,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/a46be1d86331fa7075c0a968505857d7.png",
          "type": 10,
          "rarity": 3,
          "level": 20,
          "affix_level": 5,
          "name": "翡玉法球"
        }
      },
      {
        "id": 10000036,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/38b5bd856ea9fff842477a77265da49b.png",
        "name": "重云",
        "element": "Cryo",
        "fetter": 2,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/d8cb92b3a21a45ac20173a276d305656.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/db95c5527a3b0f1a59743180e531be63.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b79312ddc86e05133b8a8d984f9931e1.png",
          "type": 11,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "祭礼大剑"
        }
      },
      {
        "id": 10000020,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0a8a2c7373dcc8f2549b645d0c3374b7.png",
        "name": "雷泽",
        "element": "Electro",
        "fetter": 1,
        "level": 40,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/7f5bb79a8d2626d4fe9866577dba0fa4.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/d805cb25bd31bf5863b75a182a58aaad.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12402,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d7f9ca521e414f63dfe24876b91cc139.png",
          "type": 11,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "钟剑"
        }
      },
      {
        "id": 10000048,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/9d2730b17e4cfdc85b52b163948a8c12.png",
        "name": "烟绯",
        "element": "Pyro",
        "fetter": 1,
        "level": 33,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/f285fb42416942ec71797e5bb14c0a22.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/bde023cad87795c72e0dee19d5461f26.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14401,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/bb4ff947d3649e393b6ca2e117b072d6.png",
          "type": 10,
          "rarity": 4,
          "level": 20,
          "affix_level": 2,
          "name": "西风秘典"
        }
      },
      {
        "id": 10000045,
        "icon": "https://uploadstatic.mihoyo.com/hk4e/e20200928calculate/common/rosaria_623de3bc25a21b6e516ea0489ddd11f8.png",
        "name": "罗莎莉亚",
        "element": "Cryo",
        "fetter": 1,
        "level": 30,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/1e36f82f68276f97b62e2fbe798ecdc4.png",
        "is_chosen": false,
        "side_icon": "https://fastcdn.mihoyo.com/static-resource-v2/2023/12/14/3e370a7bf47e75e36313d2da8cf1dfb6_434876880352973489.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13419,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0ea3522df5405f90d90505f5e36c2008.png",
          "type": 13,
          "rarity": 4,
          "level": 20,
          "affix_level": 5,
          "name": "风信之锋"
        }
      },
      {
        "id": 10000118,
        "icon": "https://fastcdn.mihoyo.com/static-resource-v2/2025/10/16/7328f006a498626b32a1e187c0dba1ea_3540908881493819725.png",
        "name": "奇偶·女性",
        "element": "Pyro",
        "fetter": 0,
        "level": 20,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/cf31bb5bd03ef7b2b7e48d13bc14600f.png",
        "is_chosen": false,
        "side_icon": "https://fastcdn.mihoyo.com/static-resource-v2/2025/10/16/96df141f7d4d44b153a5af52420fd1ce_5783188633499201918.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0b590e80914fdb8e348323fff888be0c.png",
          "type": 1,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "无锋剑"
        }
      },
      {
        "id": 10000117,
        "icon": "https://fastcdn.mihoyo.com/static-resource-v2/2025/10/16/af27ded694227c5c49f0f75730eecbb9_8978606435920695541.png",
        "name": "奇偶·男性",
        "element": "Pyro",
        "fetter": 0,
        "level": 20,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/8adbb56a7dcc47232295a1e568da0ed3.png",
        "is_chosen": false,
        "side_icon": "https://fastcdn.mihoyo.com/static-resource-v2/2025/10/16/d926ba69ae198f3f85bda32257a0a2a3_6965405552643353185.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0b590e80914fdb8e348323fff888be0c.png",
          "type": 1,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "无锋剑"
        }
      },
      {
        "id": 10000109,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/1cebf43ac944ad3ff2a0581bebe309d8.png",
        "name": "梦见月瑞希",
        "element": "Anemo",
        "fetter": 1,
        "level": 20,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/782c43fb80b91b9633f797c89940f3c1.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/cc0940bba3cbd136124438cbb113f457.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/852d232e46ddaacdfcb86b3f53413405.png",
          "type": 10,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "学徒笔记"
        }
      },
      {
        "id": 10000107,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/abe2da348abe64c67d9c2763d2d8c4e7.png",
        "name": "茜特菈莉",
        "element": "Cryo",
        "fetter": 1,
        "level": 20,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/bddc9c00c09e9adb9a8d780d655aa5b9.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/59c16c70d2cfc9e939a7835dff00be7e.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/852d232e46ddaacdfcb86b3f53413405.png",
          "type": 10,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "学徒笔记"
        }
      },
      {
        "id": 10000078,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/a7eb0a9a0805bdecfaccfd450ca61102.png",
        "name": "艾尔海森",
        "element": "Dendro",
        "fetter": 2,
        "level": 20,
        "rarity": 5,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/18879316473d04cd094cf9bb23d0ae35.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/f7f3bc2088d83d7394c1c041073f9f41.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11302,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/048119e09a837be4c1a735fd046e3261.png",
          "type": 1,
          "rarity": 3,
          "level": 1,
          "affix_level": 5,
          "name": "黎明神剑"
        }
      },
      {
        "id": 10000121,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/68c0b17a/cfec735e9e867016be94f500e9dae122.png",
        "name": "爱诺",
        "element": "Hydro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/8c2703ada814233cd8bb76f5bfeda98e.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/68c0b1bb/99fb1fb7374069299b6a37848b6cca9e.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b1e284917f1ca8330ba929ef8f116aba.png",
          "type": 11,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "训练大剑"
        }
      },
      {
        "id": 10000100,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/2c4b6f3e78da44cbe10f9cbc37a50fe1.png",
        "name": "卡齐娜",
        "element": "Geo",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/edfc5dbf65ee36356f9e2f64b5c171f6.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/06daf41434926868981682a72bf6e82f.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/ca0ea04c05d8994f0b7e836012e38563.png",
          "type": 13,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "新手长枪"
        }
      },
      {
        "id": 10000097,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/62ddf4187c2aea2dda21813b9d90f27f.png",
        "name": "赛索斯",
        "element": "Electro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/1012f7f6fc03a5434b6a4d3223b28752.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/d36da4388a1637316f5897818d997214.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c75ade4a5acb5eb9aaefbed318bf75ff.png",
          "type": 12,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "猎弓"
        }
      },
      {
        "id": 10000067,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/eaf61637b76953695940fe1ceedb18a0.png",
        "name": "柯莱",
        "element": "Dendro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/6743b943e6a55d1f7a2327292a72bd36.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/54213a15451315dcfc47c040cb46abf4.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/c75ade4a5acb5eb9aaefbed318bf75ff.png",
          "type": 12,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "猎弓"
        }
      },
      {
        "id": 10000056,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/3dc3a368e5c3be42a05afb7a9fdc9c41.png",
        "name": "九条裟罗",
        "element": "Electro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/718dcc3cf7b98010060c5e04964f1ca6.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/29021fd200fb4074bcb857668b406307.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/4a03625fdbc739dca379573871a4c2ca.png",
          "type": 12,
          "rarity": 4,
          "level": 1,
          "affix_level": 1,
          "name": "祭礼弓"
        }
      },
      {
        "id": 10000050,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/57ede6ce84e7030b58af29520198119b.png",
        "name": "托马",
        "element": "Pyro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 6,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/ae0fbc54c69f2fc97e8daaba430acffa.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/49841a48595e474cea1e360acd1d2638.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13303,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/badaa063427a6e3f39d9c031b3dddc24.png",
          "type": 13,
          "rarity": 3,
          "level": 20,
          "affix_level": 5,
          "name": "黑缨枪"
        }
      },
      {
        "id": 10000039,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/699e3449/3de7b18fbecffbb57a73fe5032d24950.png",
        "name": "迪奥娜",
        "element": "Cryo",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/afb458c644664272704592885d789945.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/da4ae4bdb927ab20bf6905fdc61eef44.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/4a03625fdbc739dca379573871a4c2ca.png",
          "type": 12,
          "rarity": 4,
          "level": 1,
          "affix_level": 1,
          "name": "祭礼弓"
        }
      },
      {
        "id": 10000031,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/207a0e35e0637a2bcb0a28fdfa61f7a4.png",
        "name": "菲谢尔",
        "element": "Electro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 5,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/a07343a21aecb509e849a541c9d72901.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/2ad457efe47f31a54bd683286fd03144.png",
        "weapon_type": 12,
        "weapon": {
          "id": 15401,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f0b8edcc330cd9de1dcf97eccb20cbaf.png",
          "type": 12,
          "rarity": 4,
          "level": 1,
          "affix_level": 1,
          "name": "西风猎弓"
        }
      },
      {
        "id": 10000024,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/bc2903d1a46616c871d5108d033a463d.png",
        "name": "北斗",
        "element": "Electro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 3,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/f6389d7277894b1cc1677402a3c64d90.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/d0d7146418af643964a4bc7f8cf9671f.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12305,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/7c806b2d328c89e3f7c6d70b01214af7.png",
          "type": 11,
          "rarity": 3,
          "level": 20,
          "affix_level": 5,
          "name": "以理服人"
        }
      },
      {
        "id": 10000006,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/415cb4af1a402f97aebfcf8edc2ca235.png",
        "name": "丽莎",
        "element": "Electro",
        "fetter": 1,
        "level": 20,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/c57fd813ced89f1f01b5bc68ab78c53b.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/8120c3760d0ef7553024fc402d3d7a2f.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14403,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/807ae55311a3a8382194a656e214e7b1.png",
          "type": 10,
          "rarity": 4,
          "level": 20,
          "affix_level": 1,
          "name": "祭礼残章"
        }
      },
      {
        "id": 10000083,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/5dad272ce992b32d3aa7a708869d1a4a.png",
        "name": "琳妮特",
        "element": "Anemo",
        "fetter": 2,
        "level": 3,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/9e7589a86900298f2f5fca7f7684af0a.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/40653a8bca56c6e205d2a01b2f6f9a00.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11407,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d6627a35dc10a7c7f9d5db832e271cce.png",
          "type": 1,
          "rarity": 4,
          "level": 1,
          "affix_level": 1,
          "name": "铁蜂刺"
        }
      },
      {
        "id": 10000081,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/a34ebd3dba93cda6fba3cc97a995822e.png",
        "name": "卡维",
        "element": "Dendro",
        "fetter": 1,
        "level": 2,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/55160d4a2ef33ff9db735be32c64b158.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/92507726de789bf9b2bb18cb2d6e5e21.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b1e284917f1ca8330ba929ef8f116aba.png",
          "type": 11,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "训练大剑"
        }
      },
      {
        "id": 10000108,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/eba829f8ca4b38367c4a2551d0e228ae.png",
        "name": "蓝砚",
        "element": "Anemo",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/ec405681b4d5e20223a14638789fca44.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/11ee069d5e9ba93fb4325eabd5f16ef1.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/852d232e46ddaacdfcb86b3f53413405.png",
          "type": 10,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "学徒笔记"
        }
      },
      {
        "id": 10000092,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/1238a7679cc90e138ec793b08aa853c7.png",
        "name": "嘉明",
        "element": "Pyro",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/4b7edd0bc705272a16237e88048886f2.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/2e728e093d16c8b7f73c5e962011ac2f.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b1e284917f1ca8330ba929ef8f116aba.png",
          "type": 11,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "训练大剑"
        }
      },
      {
        "id": 10000090,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/817f1d6da2a3ff6e6bfedeb39104ad71.png",
        "name": "夏沃蕾",
        "element": "Pyro",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/1c1c928d7a9757932c6bdbda89073f46.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/e0186b49ed0d791ee6b1dc0b125f6613.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/ca0ea04c05d8994f0b7e836012e38563.png",
          "type": 13,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "新手长枪"
        }
      },
      {
        "id": 10000088,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f4e68e94225fa95112ae03c0a6d10938.png",
        "name": "夏洛蒂",
        "element": "Cryo",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 0,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/1d3fd45b4793e3ac84b71f5495249332.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/bee59717b62a91c6863009a394ca7e4c.png",
        "weapon_type": 10,
        "weapon": {
          "id": 14101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/852d232e46ddaacdfcb86b3f53413405.png",
          "type": 10,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "学徒笔记"
        }
      },
      {
        "id": 10000085,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/34ef1ba51a4893d9df4be717e56891ae.png",
        "name": "菲米尼",
        "element": "Cryo",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/463a5aac4d9004a95f60004a9add9539.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/12d2c7cb8629bea9b1c003026a07ea55.png",
        "weapon_type": 11,
        "weapon": {
          "id": 12101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/b1e284917f1ca8330ba929ef8f116aba.png",
          "type": 11,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "训练大剑"
        }
      },
      {
        "id": 10000080,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/f239b3032e85ebb64554e69a58eec91b.png",
        "name": "米卡",
        "element": "Cryo",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/6ea984ba64a30d66f357f2c1855c1549.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/1e0d82ae5e6314615b3ead8709fff691.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/ca0ea04c05d8994f0b7e836012e38563.png",
          "type": 13,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "新手长枪"
        }
      },
      {
        "id": 10000077,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/d7ec9b285faccd804b54fa026dde96e8.png",
        "name": "瑶瑶",
        "element": "Dendro",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 2,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/f94480f1f92837f11b9cae611e132e8d.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/819994f51843b91ff6ec7f71cfa76293.png",
        "weapon_type": 13,
        "weapon": {
          "id": 13101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/ca0ea04c05d8994f0b7e836012e38563.png",
          "type": 13,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "新手长枪"
        }
      },
      {
        "id": 10000061,
        "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/49767b6d7070afddae937e417253bb3f.png",
        "name": "绮良良",
        "element": "Dendro",
        "fetter": 1,
        "level": 1,
        "rarity": 4,
        "actived_constellation_num": 1,
        "image": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/image_7/f58159762fd8ed196d6ccbe7484aef45.png",
        "is_chosen": false,
        "side_icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f727/d3bc7e170b28a1645e222d9378bdbfc1.png",
        "weapon_type": 1,
        "weapon": {
          "id": 11101,
          "icon": "https://act-webstatic.mihoyo.com/hk4e/e20200928calculate/item_icon/67c7f6c8/0b590e80914fdb8e348323fff888be0c.png",
          "type": 1,
          "rarity": 1,
          "level": 1,
          "affix_level": 1,
          "name": "无锋剑"
        }
      }
    ]
  }
}
```
</details>
