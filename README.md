本库来源于gys619

用于跑基本任务。

## 青龙拉取链接
``` 
ql repo https://github.com/iiiiqt/jdxyy.git "jd_|jx_" "activity|backUp" "^jd[^_]|USER|utils|ZooFaker_Necklace|JDJRValidator_Pure|sign_graphics_validate|function|ql" "balance"
```
```
推荐定时 0 */4 * * *
```



拉不到库是因为版本号没了，需要删了重新拉一下，运行一下下面命令就好了，库不稳，见谅！

docker exec -it 容器名 bash

cd repo

rm -rf iiiiqt_jdxyy



### 脚本说明


* 加了[Oreomeow大佬](https://raw.githubusercontent.com/Oreomeow/VIP/main/Conf/Qinglong/config.sample.sh)的config模板,名字是jd_config.sample.sh
* 财富岛新手任务开木板
  * 修改青龙配置文件,如下,加个ts
  ```
   #ql repo命令拉取脚本时需要拉取的文件后缀，直接写文件后缀名即可
   RepoFileExtensions="js py ts sh"
   ```

 
 
</details>

### 安装青龙需要一些的依赖
<details>
<summary>查看依赖列表</summary>


* 最新青龙支持安装依赖需要啥依赖，去依赖管理添加即可，简单方便
* 遇到Cannot find module 'xxxxxx'报错就进入青龙容器
* docker exec -it QL(自己容器名) bash
* pnpm install xxxxx(报错中引号里的复制过来)

 

 安装青龙的一些依赖，按需求安装

pnpm add -g pnpm

pnpm install -g

npm install -g npm

npm install -g png-js

npm install -g date-fns

npm install -g axios

npm install -g crypto-js

npm install -g ts-md5

npm install -g tslib

npm install -g @types/node

npm install -g requests

npm install -g tough-cookie

npm install -g jsdom

npm install -g download

npm install -g tunnel

npm install -g fs

npm install -g ws

npm install -g form-data

pnpm install -g js-base64

pnpm install -g qrcode-terminal

pnpm install -g silly-datetime

pip3 install requests

cd /ql/scripts/ && apk add --no-cache build-base g++ cairo-dev pango-dev giflib-dev && npm i && npm i -S ts-node typescript @types/node date-fns axios png-js canvas --build-from-source
cd /ql
apk add --no-cache build-base g++ cairo-dev pango-dev giflib-dev && cd scripts && npm install canvas --build-from-source
cd /ql
apk add python3 zlib-dev gcc jpeg-dev python3-dev musl-dev freetype-dev

</details>



### 青龙拉取常用京东脚本库([Oreomeow大佬](https://github.com/Oreomeow/VIP/blob/main/Tasks/qlrepo/Readme.md)整理的一些仓库)
<details>
<summary>京东脚本库</summary>
 

#### 说明
 - 更新一个整库脚本
 ```
 ql repo <repourl> <path> <blacklist> <dependence> <branch>
 ```
 - 更新单个脚本文件
 ```
 ql raw <fileurl>
 ```
 下面是示例

#### 整库
- `Unknown 备份托管等`
  
  1. `JDHelloWorld`
  ```
  ql repo https://github.com/JDHelloWorld/jd_scripts.git "jd_|jx_|getJDCookie" "activity|backUp|Coupon|enen|update|test" "^jd[^_]|USER|^TS|utils|notify|env|package|ken.js"
  ```
  2. `he1pu`（自动提交助力码-京喜工厂、种豆得豆、东东工厂、东东农场、健康社区、京喜财富岛、东东萌宠、闪购盲盒，随机从数据库中选取助力码互助）
  ```
  ql repo https://github.com/he1pu/JDHelp.git "jd_|jx_|getJDCookie" "Coupon|update" "^jd[^_]|USER|^sign|^ZooFaker|utils"
  ```
  3. `shufflewzc`
  ```
  ql repo https://github.com/shufflewzc/faker2.git "jd_|jx_|gua_|jddj_|getJDCookie" "activity|backUp" "^jd[^_]|USER|utils|^JS|^TS|^JDJRValidator_Pure|^ZooFaker|^sign"
  ```
  4. `Aaron-lv`
  ```
  ql repo https://github.com/Aaron-lv/sync.git "jd_|jx_|getJDCookie" "activity|backUp|Coupon" "^jd[^_]|USER|utils" "jd_scripts"
  ```
  5. `panghu999`（无维护）
  ```
  ql repo https://github.com/panghu999/jd_scripts.git "jd_|jx_|getJDCookie" "activity|backUp|Coupon|jd_try|format_" "^jd[^_]|USER"
  ```
  6. `chinnkarahoi`（无维护）
  ```
  ql repo https://github.com/chinnkarahoi/jd_scripts.git "jd_|jx_|getJDCookie" "activity|backUp|Coupon" "^jd[^_]|USER"
  ```

- `passerby-b`
```
ql repo https://github.com/passerby-b/JDDJ.git "jddj_" "scf_test_event|jddj_fruit_code.js|jddj_getck.js|jd_|jddj_cookie"
```
- `curtinlv`
```
ql repo https://github.com/curtinlv/JD-Script.git "jd_"
```
- `smiek2221`
```
ql repo https://github.com/smiek2221/scripts.git "jd_|gua_" "" "^MovementFaker|^JDJRValidator|^ZooFaker|^sign" 
```
- `cdle`
```
ql repo https://github.com/cdle/xdd.git "jd_" "disposable|expired|jdc"
```
- `ZCY01`
```
ql repo https://github.com/ZCY01/daily_scripts.git "jd_"
```
- `whyour/hundun`
```
ql repo https://github.com/whyour/hundun.git "quanx" "tokens|caiyun|didi|donate|fold|Env"
```
- `moposmall`
```
ql repo https://github.com/moposmall/Script.git "Me"
```
- `Ariszy (Zhiyi-N)`
```
ql repo https://github.com/Ariszy/Private-Script.git "JD"
```
- `photonmang`（宠汪汪及兑换、点点券修复）
```
ql repo https://github.com/photonmang/quantumultX.git "JDscripts"
```
- `jiulan`
```
ql repo https://github.com/jiulan/platypus.git "jd_|jx_" "" "overdue" "main"
```
- `star261`
```
ql repo https://github.com/star261/jd.git "jd_|star" "" "code" "main"
```
- `Wenmoux`
```
ql repo https://github.com/Wenmoux/scripts.git "other|jd" "" "" "wen"
```
- `Tsukasa007`
```
ql repo https://github.com/Tsukasa007/my_script.git "jd_|jx_" "jdCookie|USER_AGENTS|sendNotify|backup" "" "master"
```

#### 单脚本
#### 名称之后标注`﹢`的单脚本，若上面已拉取仓库的可以不拉，否则会重复拉取。这里适用于只拉取部分脚本使用
> `curtinlv`﹢

>> 入会
```
ql raw https://raw.githubusercontent.com/curtinlv/JD-Script/main/OpenCard/jd_OpenCard.py
```
>> 关注
```
ql raw https://raw.githubusercontent.com/curtinlv/JD-Script/main/getFollowGifts/jd_getFollowGift.py
```

> `chiupam`

>> 京喜工厂瓜分电力开团 ID 
```
ql raw https://raw.githubusercontent.com/chiupam/JD_Diy/master/pys/activeId.py
```

> `Aaron-lv`+

>> 财富岛
```
ql raw https://raw.githubusercontent.com/Aaron-lv/sync/jd_scripts/jd_cfd.js
```
or
```
ql repo https://github.com/Aaron-lv/sync.git "jd_cfd" "" "" "jd_scripts"
```

> `Wenmoux`+

>> 口袋书店
```
ql raw https://raw.githubusercontent.com/Wenmoux/scripts/wen/jd/chinnkarahoi_jd_bookshop.js
```
or
```
ql repo https://github.com/Wenmoux/scripts.git "chinnkarahoi_jd_bookshop" "" "" "wen"
```

> `NobyDa`

>> 京东多合一签到脚本

```
ql raw https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js
```
or
```
ql repo https://github.com/NobyDa/Script.git "JD-DailyBonus" "" "JD_DailyBonus" "master"
```

#### 已删库存档
- `monk-coder`
```
ql repo https://github.com/monk-dust/dust.git "i-chenzhe|normal|member|car" "backup"
```
- `hyzaw`
```
ql repo https://github.com/hyzaw/scripts.git "ddo_"
```
- `zooPanda`
```
ql repo https://github.com/zooPanda/zoo.git "zoo"
```
- `longzhuzhu`
```
ql repo https://github.com/longzhuzhu/nianyu.git "qx"
```
- `panghu999/panghu`
```
ql repo https://github.com/panghu999/panghu.git "jd_"
```
</details>
 
 

 
 
 

### 致谢
* [@kangwenhang](https://github.com/kangwenhang)
* [@smiek2221](https://github.com/smiek2221/scripts.git)
* [@yuannian1112](https://github.com/yuannian1112/jd_scripts.git)
*  [@shufflewzc](https://github.com/shufflewzc/faker2.git)
*  [@passerby-b](https://github.com/passerby-b/JDDJ.git)
*  [@he1pu](https://github.com/he1pu/JDHelp.git)
*  [@airacg](https://github.com/airacg/jd_task.git)
*  [@ccwav](https://github.com/ccwav/QLScript2.git)
*  [@Zy143L](https://github.com/Zy143L/wskey.git)
*  [@X1a0He](https://github.com/X1a0He/jd_scripts_fixed)
*  [@AlterGu](https://github.com/AlterGu/qinglong_note)
*  [@KingRan](https://github.com/KingRan/JD-Scripts)
*  [@Aaron-lv](https://github.com/Aaron-lv/sync)
*  [@zzfiu](https://github.com/zzfiu/jd.git)
*  [@zero205](https://github.com/zero205/JD_tencent_scf)
*  [@wuye999](https://github.com/wuye999/myScripts)
