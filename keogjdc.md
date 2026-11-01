代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.vehdjk.com/Article/details/gxxpdcgce.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.vehdjk.com/Article/details/gpnejuotk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.sjlbkw.cn/Article/details/gytgjajrh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gzmnonkbn.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gplatenkf.sHtML

npm init -y;  npm i express
来源：http://blog.epnwcf.com/Article/details/glqyxxhtf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.yfazqb.com/Article/details/ghdqznyfo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gcfljkvnv.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gjoonaqvn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gdzekosup.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.tarul.cn/Article/details/gggrdarsq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/grzwtxczl.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/gbsecsgzr.sHtML

a?.b?.c
来源：http://www.m.share.vehdjk.com/Article/details/gdsaslvqh.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gocstrwll.sHtML

a ?? b
来源：http://m.share.tarul.cn/Article/details/gaiwfbwwf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/gocjtvmcn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.vehdjk.com/Article/details/gplphmlmu.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/gxfojttlm.sHtML

{ ...a, ...b }
来源：http://3g.fktsv.cn/Article/details/gvyyzciur.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/gjustugus.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gikreuwan.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/gwpuqrjdz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gvxzyigjz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gnsmzhmde.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.tarul.cn/Article/details/gtfjlhuhi.sHtML

[U92] JS：深拷贝
来源：http://www.blog.yfazqb.com/Article/details/ghzkaorgc.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gldccvglg.sHtML

[U93] JS：模板字符串
来源：http://mobile.tarul.cn/Article/details/gypyuaeug.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gwznacxpo.sHtML

[U94] JS：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gcbzeiiwk.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/ghkvnrqbp.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/gfdsxtqfj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.epnwcf.com/Article/details/gaiznicjw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gxgaoknlw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gnifknetr.sHtML

[U97] JS：并发请求
来源：http://mobile.tarul.cn/Article/details/grifsmfdo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gzbmpqjhf.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/gtdcviauf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/gjeqgogvk.sHtML

[U99] JS：事件监听
来源：http://baike.yfazqb.com/Article/details/gtqrtklnj.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.bbcook.cn/Article/details/gnmavlucj.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.epnwcf.com/Article/details/gofbivtmi.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/gfnwyaevl.sHtML

[U101] JS：classList 操作
来源：http://blog.yfazqb.com/Article/details/gajbclfjv.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gvhhvdqqq.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gddczfohk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gbtaoreun.sHtML

[U103] JS：定时器
来源：http://www.share.bbcook.cn/Article/details/gxwnjgsrx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fktsv.cn/Article/details/gmbnjvjhl.sHtML

[U104] JS：防抖
来源：http://wap.yfazqb.com/Article/details/gycmnujal.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gybogjqqu.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gfdbbilaf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.epnwcf.com/Article/details/gklfbowmh.sHtML

[U106] JS：日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gynogcxnm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.bbcook.cn/Article/details/gfvwayghf.sHtML

[U107] JS：数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gykwbmhtj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gddatihlf.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gunzwaaty.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gzhwuikzk.sHtML

[U109] JS：数组分组
来源：http://3g.fktsv.cn/Article/details/gzgiaazzy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gdwrgznia.sHtML

[U110] JS：数组分块
来源：http://3g.bbcook.cn/Article/details/gklcooqde.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fktsv.cn/Article/details/gdnvmcaoq.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gmxdicqwn.sHtML

new Map(Object.entries(obj))
来源：http://baike.bbcook.cn/Article/details/gwswmiwdj.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/ghwvqmqpf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/ggzytgyrr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.sjlbkw.cn/Article/details/gttjshpsn.sHtML

s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gdlswnjaw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gdhrbodzj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gkhxtdnmd.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gtularfoo.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gvnksjcxw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.sjlbkw.cn/Article/details/gfxsywquo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.epnwcf.com/Article/details/ggsmuacwb.sHtML

[U117] JS：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/garazbcdq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fktsv.cn/Article/details/gnvyvbxrt.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/ghzhxynbv.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.sjlbkw.cn/Article/details/gldhhbkgv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/gbbpqhhrs.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gvrjnhxkn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/gyrxersvu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.vehdjk.com/Article/details/gmwpuurdw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqocpwrwy.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/glktenfrk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghrdwnvqq.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gtikpedgj.sHtML

Python ......... 252
来源：http://blog.bbcook.cn/Article/details/gntgrdzeo.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gmqnkutql.sHtML

JavaScript ..... 252
来源：http://mobile.yfazqb.com/Article/details/gtfpxspyr.sHtML

TypeScript ..... 212
来源：http://3g.vehdjk.com/Article/details/geyjtzsdg.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/gvxrfdeai.sHtML

Go ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gqqojhjrn.sHtML

Ruby ........... 212
来源：http://3g.vehdjk.com/Article/details/gzwfmvrhg.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gqdtynxpf.sHtML

C .............. 30
来源：http://3g.epnwcf.com/Article/details/gcxqwfasf.sHtML

C++ ............ 30
来源：http://m.share.tarul.cn/Article/details/ghiucobcj.sHtML

SQL ............ 90
来源：http://www.m.share.yfazqb.com/Article/details/gjgtsfinc.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gnhomutdx.sHtML

Kotlin ......... 15
来源：http://mobile.vehdjk.com/Article/details/ghyjkdsdh.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/gcezeinzk.sHtML

Lua ............ 10
来源：http://read.share.tarul.cn/Article/details/ghkccfwby.sHtML

Perl ........... 10
来源：http://www.m.share.tarul.cn/Article/details/gemyqhlnp.sHtML

Scala .......... 10
来源：http://www.m.share.vehdjk.com/Article/details/gvxlaoxzv.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gbqjegeai.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/gbmmrldme.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/gipbdthrx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gfymtztla.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gueaucafy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gajaxfxgk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gulfhvbsp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/gkfcomgdx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/glxctwvqi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gbxnrutve.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/geuipqxhb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/giwuyvyuu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gcifnzlpz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/govujlseg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gfvoxocmv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gobovehcb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gymudlcsz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.bbcook.cn/Article/details/gafoqijaa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gtxvakhsu.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fktsv.cn/Article/details/grdcwtiru.sHtML

R Bash 专题                             80
来源：http://3g.epnwcf.com/Article/details/ghnobnlyf.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.tarul.cn/Article/details/gxsbwhbmp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/gtlaujrir.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/ghejaydzi.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gqqzmmrad.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/gotqkzbal.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gerammncl.sHtML

使用提醒
来源：http://wap.tarul.cn/Article/details/gputjcsqa.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gvqprvgkq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/grcsnsdce.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.bbcook.cn/Article/details/gjwthhpcp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.bbcook.cn/Article/details/gzztjtfxy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.bbcook.cn/Article/details/gdbluyipp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.vehdjk.com/Article/details/gidvfrjps.sHtML

—— 文件结束 ——
来源：http://read.share.yfazqb.com/Article/details/gxpszbfob.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggjqpcrqs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.tarul.cn/Article/details/gothsqicn.sHtML

Common Programming Examples Cheat Book
来源：http://baike.tarul.cn/Article/details/gysakzwgt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyjfgpvvo.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gkfszfcft.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.yfazqb.com/Article/details/gjlneicdx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.sjlbkw.cn/Article/details/gnmxkaahx.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gcafptnxn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.tarul.cn/Article/details/gaevgdehg.sHtML

【使用说明】
来源：http://www.blog.epnwcf.com/Article/details/gxojearhn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/gjgyhkquh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.vehdjk.com/Article/details/gdyepowxg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fktsv.cn/Article/details/ghuraguyv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.tarul.cn/Article/details/gegotcbqw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.yfazqb.com/Article/details/grrwbeohh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.vehdjk.com/Article/details/gqagwvxom.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/gknzxkvwt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.sjlbkw.cn/Article/details/gbtosecol.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.epnwcf.com/Article/details/ghtmmqmrj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.sjlbkw.cn/Article/details/gmcdhumsv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.epnwcf.com/Article/details/gemjltqla.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gnomxyuwi.sHtML

【文件统计】
来源：http://www.m.share.fktsv.cn/Article/details/gykrgalmo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.vehdjk.com/Article/details/ggdmxhlcp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gtyemknmn.sHtML

目  录
来源：http://read.share.yfazqb.com/Article/details/gyxfvgabw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/grsiyuysn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/grpzpmdzp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/ghkqegycu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gbxirolcz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gqtuteybk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.tarul.cn/Article/details/gmappjguc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/ggazfyxti.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gciphhvfd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/ghxlmfhok.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gbxmwmfqf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gwqwtwlvh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gxtsqfnjm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/ggwbkgsbt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gwmlmlkxb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/gzrthlduy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/geycliqtb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gmgqrsfrh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.yfazqb.com/Article/details/gjgjrvkgf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.bbcook.cn/Article/details/gswvbivmy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.vehdjk.com/Article/details/gzlkrvhxh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gaqkziqan.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/gdfbgnegw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxohizjgy.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gtriqcpwt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxcdrxjpu.sHtML

[A01] Hello World
来源：http://blog.yfazqb.com/Article/details/griwrpduw.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/ghmgmrjhm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.yfazqb.com/Article/details/ghqtnhkex.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gikuhzxgn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.epnwcf.com/Article/details/ghykbekos.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gqbzzntrv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gockashxv.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.epnwcf.com/Article/details/gycjjkqln.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/geqbhohvy.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/gtlsdfmxa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.bbcook.cn/Article/details/gclfovauo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gajgvtbbr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gewxkmfbv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gvrrgayme.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/grpylycqt.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.sjlbkw.cn/Article/details/gdhszlmbh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.yfazqb.com/Article/details/gtknhnibe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/ghekdfxld.sHtML

[A03] 常量定义
来源：http://read.share.yfazqb.com/Article/details/gmzlhpaxk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.tarul.cn/Article/details/gjfucywdj.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gaqxcjgqn.sHtML

JS:   const PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/guqnfxpzc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcgvqkny.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/guvnxgtsh.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gfuugxnge.sHtML

Ruby: PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/grimfsxae.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gfsusxldh.sHtML

[A04] 判断变量类型
来源：http://read.share.bbcook.cn/Article/details/gcnodehcp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.tarul.cn/Article/details/gjpkfydao.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.tarul.cn/Article/details/gyojvdkgw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.tarul.cn/Article/details/gklkfpxhh.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.epnwcf.com/Article/details/gydjhueyk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.tarul.cn/Article/details/gdjehjlas.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.sjlbkw.cn/Article/details/gcmagdjio.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/giilgmzwv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fktsv.cn/Article/details/gbujyjhjn.sHtML

[A05] 整数除法与取模
来源：http://m.share.fktsv.cn/Article/details/gfvwlrhho.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.sjlbkw.cn/Article/details/gdglatigf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/gjbopfbpi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/guqslnfug.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/giakhzvya.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/grzapwuow.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gaphlpnij.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gpctearxt.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gjnuoaxxk.sHtML

[A06] 字符串转数字
来源：http://baike.bbcook.cn/Article/details/gcerprdtv.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gimzlvqom.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.epnwcf.com/Article/details/gndyxegpu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gpaalrmbl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/gusxavvua.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.tarul.cn/Article/details/gnjvisgnt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.vehdjk.com/Article/details/giiympkjo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.yfazqb.com/Article/details/glwvbkunc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fktsv.cn/Article/details/gaixtaigi.sHtML

[A07] 数字转字符串
来源：http://www.share.epnwcf.com/Article/details/gfkkbttdx.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gxsnyggoc.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.sjlbkw.cn/Article/details/ghxyiqvhk.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.yfazqb.com/Article/details/guxynnnpe.sHtML

TS:   String(42)
来源：http://mobile.bbcook.cn/Article/details/gohaiinqi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.yfazqb.com/Article/details/gblqtrvtx.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.tarul.cn/Article/details/gzkrvugqn.sHtML

Ruby: 42.to_s
来源：http://read.share.yfazqb.com/Article/details/gydfkuvml.sHtML

C#:   42.ToString()
来源：http://read.share.fktsv.cn/Article/details/ghdexkjek.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fktsv.cn/Article/details/gjdrkbdzy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gznwyygxg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.tarul.cn/Article/details/ggakehkpk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gnjqndmnk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.epnwcf.com/Article/details/gswzpcjhe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gwrdourdz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gxnvxrybe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.vehdjk.com/Article/details/gffbmdtal.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gdckbyhux.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.tarul.cn/Article/details/gxxsluqnt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gtngjlusw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gwwdnbgyx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gmiutxqng.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gumzwjngw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/ghgbduvat.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.tarul.cn/Article/details/gjgdvyyuw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.epnwcf.com/Article/details/glshcheqf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.bbcook.cn/Article/details/gjsagnytw.sHtML

[A10] 生成随机数
来源：http://read.share.sjlbkw.cn/Article/details/grtxarwvp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.vehdjk.com/Article/details/ggspjftcl.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.yfazqb.com/Article/details/gsxqshjsh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fktsv.cn/Article/details/gibdwkzso.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.sjlbkw.cn/Article/details/gjyvoubcr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.tarul.cn/Article/details/gldvkbduz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/gvalkedpl.sHtML

Ruby: rand(1..100)
来源：http://mobile.tarul.cn/Article/details/gsbvnqtuj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.bbcook.cn/Article/details/ghymkgawr.sHtML

[A11] 条件表达式（三元）
来源：http://3g.epnwcf.com/Article/details/gxwdcfgwi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.vehdjk.com/Article/details/guvrzurbx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/guseztncc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/ghxjmpfvl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gpenlfteh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gtmfdvkph.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.yfazqb.com/Article/details/gobhuwdgi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gqgfoahsb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/grrzhzdil.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/gukzlclpp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.bbcook.cn/Article/details/gklnszrfe.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.vehdjk.com/Article/details/gzwlagpwq.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gpmyqruhc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/guwooabjp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.sjlbkw.cn/Article/details/gaamfyaiv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.sjlbkw.cn/Article/details/gepfnavga.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.epnwcf.com/Article/details/ggmttdpge.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fktsv.cn/Article/details/gaiqkdlfv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.vehdjk.com/Article/details/gozusowox.sHtML


<!-- 参考信息 -->