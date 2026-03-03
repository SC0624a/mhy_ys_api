# 保留所有原CURL


# 首页信息获取
<details>
<summary>CURL</summary>

```curl
curl -X GET 'https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/index?avatar_list_type=1&server=cn_gf01&role_id=XXXX' -H 'User-Agent: Mozilla/5.0 (Linux; Android 12; 2211133C Build/V417IR; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/110.0.5481.154 Safari/537.36 miHoYoBBS/2.102.1' -H 'Accept: application/json, text/plain, */*' -H 'Accept-Encoding: gzip, deflate' -H 'DS: 1772518716,165572,1fc88d5574fdd7838b4596864ca30cd9' -H 'x-rpc-app_version: 2.102.1' -H 'x-rpc-tool_verison: v6.4.0-gr-cn' -H 'x-rpc-device_id: 40818f2a-2395-38df-ab11-93371b77324e' -H 'x-rpc-device_name: Xiaomi%202211133C' -H 'x-rpc-page: v6.4.0-gr-cn_#/ys' -H 'x-rpc-device_fp: 38d816239aab3' -H 'x-rpc-sys_version: 12' -H 'x-rpc-client_type: 5' -H 'Origin: https://webstatic.mihoyo.com' -H 'X-Requested-With: com.mihoyo.hyperion' -H 'Sec-Fetch-Site: same-site' -H 'Sec-Fetch-Mode: cors' -H 'Sec-Fetch-Dest: empty' -H 'Referer: https://webstatic.mihoyo.com/' -H 'Accept-Language: zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7' -H 'Cookie: XXXX'
```
</details>

**请求方式：GET**

链接：`https://api-takumi-record.mihoyo.com/game_record/app/genshin/api/index`

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
tips:这里只写必要请求头

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
