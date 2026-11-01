代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://mobile.bbcook.cn/Article/details/gzrtzspcc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/guribwcic.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/grsiniclm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gqishabun.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gwiwdunkz.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gnvllvxfd.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gckbcsmlv.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/geiidchng.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/ghvflnjsd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fktsv.cn/Article/details/gaiohejdv.sHtML

[U88] JS：对象展开合并
来源：http://baike.epnwcf.com/Article/details/gcawuxiiv.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/gspxjkxwg.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/gyyuuxara.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gpguizpla.sHtML

[U90] JS：数字数组排序
来源：http://blog.vehdjk.com/Article/details/geewoxboo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/giwzayhsh.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gdgkxegee.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.bbcook.cn/Article/details/geknhglcf.sHtML

[U92] JS：深拷贝
来源：http://read.share.fktsv.cn/Article/details/gjekpvgap.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gmaburqnk.sHtML

[U93] JS：模板字符串
来源：http://3g.bbcook.cn/Article/details/gmyskdsnz.sHtML

`共 ${n} 条`
来源：http://www.m.share.sjlbkw.cn/Article/details/glxewrekh.sHtML

[U94] JS：箭头函数
来源：http://m.share.yfazqb.com/Article/details/ghgcithbh.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/gizsiiuan.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gqiisdvlu.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/ggnljxfil.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.bbcook.cn/Article/details/gkuwqgqaw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gxiqwxvjg.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gugljnibi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gfmcrwhqh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gahentgcl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gbtpknfsz.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gqagezefq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.tarul.cn/Article/details/gzfwdnxxf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.yfazqb.com/Article/details/galvvafzf.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gwzdreres.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gwbjbecgs.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/ggwcuxeog.sHtML

[U102] JS：本地存储
来源：http://blog.bbcook.cn/Article/details/gnpkecwef.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gftmuelwh.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gnkluvkwa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/gddvxgvqz.sHtML

[U104] JS：防抖
来源：http://blog.yfazqb.com/Article/details/giywobfsz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/grjvsfxro.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gurtyuccb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gktdrolkx.sHtML

[U106] JS：日期格式化
来源：http://m.share.fktsv.cn/Article/details/gnzzhldty.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.vehdjk.com/Article/details/gacwiyqkv.sHtML

[U107] JS：数字千分位
来源：http://blog.vehdjk.com/Article/details/gmdfiepqp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gpsqdaofa.sHtML

[U108] JS：随机整数
来源：http://read.share.yfazqb.com/Article/details/gipjvpcwh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.vehdjk.com/Article/details/gvquczukt.sHtML

[U109] JS：数组分组
来源：http://wap.fktsv.cn/Article/details/gjfdjhagg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gadofvffm.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/grfekuqtj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/ggopgoqfb.sHtML

[U111] JS：对象转 Map
来源：http://wap.bbcook.cn/Article/details/gibjxraxn.sHtML

new Map(Object.entries(obj))
来源：http://wap.tarul.cn/Article/details/gzwrrdnhp.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.vehdjk.com/Article/details/gdvgasang.sHtML

"7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/guaamsfyk.sHtML

[U113] JS：正则替换全部
来源：http://3g.fktsv.cn/Article/details/glernpeoi.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gikutyqkj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.tarul.cn/Article/details/gnifzpybm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gfjgdhynw.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gzlxmgpbk.sHtML

crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gmwyjsnmu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/gzrwvztpy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gitbczeam.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gecljgxmw.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.epnwcf.com/Article/details/gefarggcl.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gjovbfxyr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/goghrnlkv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.yfazqb.com/Article/details/ggnyiwtdb.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/gldpfcyfn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.tarul.cn/Article/details/ggbtqjray.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/gemdezilm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gehzuxgdm.sHtML

统计汇总
来源：http://read.share.epnwcf.com/Article/details/geibebnul.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/giopfdmdx.sHtML

按语言统计（条）：
来源：http://read.share.bbcook.cn/Article/details/gxzfarsnb.sHtML

Python ......... 252
来源：http://www.m.share.tarul.cn/Article/details/gkjrovcmb.sHtML

PHP ............ 252
来源：http://read.share.vehdjk.com/Article/details/gymdxrcod.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gdhxwokwi.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/gqwrfqmca.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gmfgqmtpf.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/gmgaakapw.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/glcldygcn.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/gqjafeckd.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/gubelftxy.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gwrcmlpsr.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/glohfgwew.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gbislftff.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gjfgchdou.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gcxhhfoin.sHtML

Lua ............ 10
来源：http://baike.yfazqb.com/Article/details/gyfinpuxe.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/gpmwjtaap.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gizqmkmya.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gzyrnrrnr.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/gdypklpjh.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gebfbpgmz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gkqnhmmcm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gmlijfbri.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gnhgestdu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gsdmskgbb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.tarul.cn/Article/details/ggfotuzod.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/goplgiyye.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gzpsfoysp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/grejhrzva.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gxtpuqucn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gfsnlnucl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gswojtmmk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gujiwvbnf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gutprnrrc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gvrtwuiba.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/gtfebzsuh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gazhtabqy.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/gzbgfjqqt.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gtcxwrfxa.sHtML

S C / C++ 专题                          60
来源：http://wap.sjlbkw.cn/Article/details/gjcdhaygi.sHtML

T 其他语言补充                          60
来源：http://m.share.yfazqb.com/Article/details/gxlhxpkis.sHtML

U 高频实用片段                         120
来源：http://baike.epnwcf.com/Article/details/gotaugola.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gxhmanpbx.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gosrqjacp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gmjmkdofu.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/gjfthbvsy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gxpximaug.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.sjlbkw.cn/Article/details/gsvbdwcdo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvwoozsb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.tarul.cn/Article/details/gpmcnctlz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.yfazqb.com/Article/details/gqeousasj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.sjlbkw.cn/Article/details/goaxwwxgr.sHtML

—— 文件结束 ——
来源：http://www.m.share.fktsv.cn/Article/details/gdugekmvr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gefcmdcrh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gzwndpjtc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.yfazqb.com/Article/details/gbojmhcle.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvjcerjeg.sHtML

【收录内容】
来源：http://blog.yfazqb.com/Article/details/gwuhkbbwk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/guvwetkvk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/gugilvvqy.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gldjtdzdt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.epnwcf.com/Article/details/gpfazuqwu.sHtML

【使用说明】
来源：http://baike.tarul.cn/Article/details/gaeshzmzn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.vehdjk.com/Article/details/gwphopyrl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.yfazqb.com/Article/details/gtmxcevoo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.epnwcf.com/Article/details/gffcmtgkl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.sjlbkw.cn/Article/details/grzjltrlo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fktsv.cn/Article/details/gfrcshmjk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.vehdjk.com/Article/details/gdointrlr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fktsv.cn/Article/details/gucmsixye.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.vehdjk.com/Article/details/gpjuylkhv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.tarul.cn/Article/details/gbsdyafch.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.sjlbkw.cn/Article/details/gfrxzilfb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.epnwcf.com/Article/details/gfkinexvr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.epnwcf.com/Article/details/gyigifyca.sHtML

【文件统计】
来源：http://wap.fktsv.cn/Article/details/glzjezldr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.yfazqb.com/Article/details/gbebynvjx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gatbmhizr.sHtML

目  录
来源：http://m.share.epnwcf.com/Article/details/gxztopxbi.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gpkviaqge.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gegrwvkkm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/grfjhfkaz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsmekaurc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/garjwnvqc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.vehdjk.com/Article/details/gahytjbxp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gmczchjjd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/ghwigjryz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/gxchpishz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/giooqrpak.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/guacsxdfp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gpuytcnve.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gguivrlts.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gsduadxbo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gvpxidtks.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.epnwcf.com/Article/details/gtekktqph.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gvgafbjfu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/ggvlrvaxe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.bbcook.cn/Article/details/gvqychaha.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fktsv.cn/Article/details/goqbmsafe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gfvexjlfd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/geeeyukef.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsfzqhrhq.sHtML

A. 基础语法与类型
来源：http://blog.epnwcf.com/Article/details/geflsccgk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gafmkxwfm.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/glkoihwpg.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/guuuiwvpu.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.vehdjk.com/Article/details/ghdagscsn.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gurjtfnfb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.vehdjk.com/Article/details/gpynpvngp.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/ggjxhjoom.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.tarul.cn/Article/details/gorlqblxa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.bbcook.cn/Article/details/gozgprdnr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gkbfmppka.sHtML

[A02] 变量声明与赋值
来源：http://baike.epnwcf.com/Article/details/gaqegrqvi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.epnwcf.com/Article/details/glvbtewjv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/ghmytthgf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.tarul.cn/Article/details/grbcehlsv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.vehdjk.com/Article/details/gijqlwtji.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gabdfvwwq.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/givyewlsb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gadbtektf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gcaaxayzq.sHtML

[A03] 常量定义
来源：http://mobile.tarul.cn/Article/details/gaotexbwq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.bbcook.cn/Article/details/ggpffgfgu.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gmvyaguel.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gnbbwhumb.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.tarul.cn/Article/details/govwxohod.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gztuudnmf.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gqqpvdlrx.sHtML

Ruby: PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gcwwefmvv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gofquible.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gbsedkzvc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.vehdjk.com/Article/details/gjdgptlyp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fktsv.cn/Article/details/gyuealkvc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/gguywlfdz.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gvuvtcsas.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.sjlbkw.cn/Article/details/gfnenhsps.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/gkajwzvjf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.sjlbkw.cn/Article/details/gyjatogji.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.epnwcf.com/Article/details/gdbeednvq.sHtML

[A05] 整数除法与取模
来源：http://www.share.epnwcf.com/Article/details/geejdyxnn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.epnwcf.com/Article/details/gbhwlntqa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/guvnhuorn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gmlplqqih.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gpzatpzxz.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gvkskbzcl.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gjzxsnlzb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/garctmqbh.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gtdfwlgdr.sHtML

[A06] 字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gqzidcjuj.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.vehdjk.com/Article/details/gmamihoyf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.epnwcf.com/Article/details/glvaftlce.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gebihvadh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gzjwxqwhp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.epnwcf.com/Article/details/geswilqym.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.bbcook.cn/Article/details/gncugcbte.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.bbcook.cn/Article/details/gpuwbbhsc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.tarul.cn/Article/details/gkhzvypfx.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/gehpyokaz.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/gbxmjjsbo.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.tarul.cn/Article/details/gpoebnbsm.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.yfazqb.com/Article/details/ggbfdzhqv.sHtML

TS:   String(42)
来源：http://www.share.tarul.cn/Article/details/gpohekski.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.vehdjk.com/Article/details/gjdicstrr.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.epnwcf.com/Article/details/groxlsgqq.sHtML

Ruby: 42.to_s
来源：http://www.share.vehdjk.com/Article/details/glclogseh.sHtML

C#:   42.ToString()
来源：http://wap.yfazqb.com/Article/details/gkwsrpysa.sHtML

[A08] 取整与四舍五入
来源：http://read.share.epnwcf.com/Article/details/gldncnrnq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gofhwqywi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.tarul.cn/Article/details/gkuohoqvi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/glvtggiqm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.tarul.cn/Article/details/graouffzs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gxwwazekg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gxhvjpdio.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.bbcook.cn/Article/details/gcnnzycnb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gcstcupbb.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.tarul.cn/Article/details/gjvcifsuf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.bbcook.cn/Article/details/gonskushh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gxsgdjuxp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gadibqabx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gvonpiaig.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gvqvatdlu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fktsv.cn/Article/details/gzfzidmut.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.epnwcf.com/Article/details/gbandmgaw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/grfwnjhqk.sHtML

[A10] 生成随机数
来源：http://blog.epnwcf.com/Article/details/gkgkqsjwm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.vehdjk.com/Article/details/gemcevfgw.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fktsv.cn/Article/details/gekicouua.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gwetgcgwv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/gfofddvet.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.tarul.cn/Article/details/gvuxelgfp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.vehdjk.com/Article/details/gwfhiinas.sHtML

Ruby: rand(1..100)
来源：http://wap.yfazqb.com/Article/details/gaosmuimu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fktsv.cn/Article/details/gfnxjjxio.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.yfazqb.com/Article/details/ghzvrnwnr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fktsv.cn/Article/details/gbypbhlob.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gddvuqixz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gnhzrhjbt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/givmihude.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gbcljjgcv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.tarul.cn/Article/details/gmfwimzkw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gmswrftyq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/grfoxtuzf.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fktsv.cn/Article/details/gnkjxaaco.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.yfazqb.com/Article/details/gfbytzwyh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.epnwcf.com/Article/details/gwhztfjli.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/gjblmklab.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gooridxtc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.epnwcf.com/Article/details/gzdyaueip.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.bbcook.cn/Article/details/gwlvnvssu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.vehdjk.com/Article/details/gmrojdakq.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.yfazqb.com/Article/details/gftewuwqr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.tarul.cn/Article/details/gbybdqozs.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/ggsiiopqy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gjucbcejz.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/ghgpnaqjf.sHtML

TS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gkxvyybnc.sHtML

Java: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/goaofultc.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gzdnclcay.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gaumjehbk.sHtML

C#:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/ginrzlbid.sHtML


<!-- 参考信息 -->