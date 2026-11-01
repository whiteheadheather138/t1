代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gnprvcwjg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.bbcook.cn/Article/details/garmzfaxt.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fktsv.cn/Article/details/gydmwucdx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.epnwcf.com/Article/details/gotiixtfa.sHtML

[U85] JS：可选链
来源：http://www.share.yfazqb.com/Article/details/gsqmrydmp.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gklphvyyg.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/gwgmpukfg.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/gyrfvxvhg.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/gdilxtcdk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.epnwcf.com/Article/details/gkzwkqhkj.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gwrwvrere.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/guiqgbxjf.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gbawuznnj.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gfozaovod.sHtML

[U90] JS：数字数组排序
来源：http://blog.fktsv.cn/Article/details/gzjzhmbig.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gwwlwjqzm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gliulztvs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gehvtidea.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/gkebcljzt.sHtML

structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gnsnwuwrq.sHtML

[U93] JS：模板字符串
来源：http://baike.yfazqb.com/Article/details/gomfdhpsm.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/gzcgjslmr.sHtML

[U94] JS：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gpfbjodge.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gwddzgvca.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fktsv.cn/Article/details/gvnrfzjey.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/gslmvqocd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.bbcook.cn/Article/details/gbgkxcekm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/ggzvwccoj.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/ghcvbulyt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gclyqrngk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/grfxwmbrm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/gscgsugvm.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gawzwdovh.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gtpmvbiwr.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/gyqfmtgfa.sHtML

document.querySelector(".item")
来源：http://m.share.yfazqb.com/Article/details/ghuuhpkak.sHtML

[U101] JS：classList 操作
来源：http://baike.sjlbkw.cn/Article/details/gopmntsxf.sHtML

el.classList.toggle("active")
来源：http://mobile.tarul.cn/Article/details/gpblmqbuc.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/glmkwfkpd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fktsv.cn/Article/details/gaolmpuoe.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gjkczvvhd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gygspqmfe.sHtML

[U104] JS：防抖
来源：http://mobile.yfazqb.com/Article/details/gnczqmdlo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gvgivagdy.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gruwmrycb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.bbcook.cn/Article/details/gvjicgdiq.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/goyjkjlzb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gzrywtree.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gpvcfugdx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gsniuigio.sHtML

[U108] JS：随机整数
来源：http://m.share.epnwcf.com/Article/details/gxbcbzefb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/givmfmlut.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/gqtbihzvc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gzqoujhmf.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/ghwwwkpxe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gjgtdqqtp.sHtML

[U111] JS：对象转 Map
来源：http://blog.bbcook.cn/Article/details/geovungnc.sHtML

new Map(Object.entries(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gkugipetn.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gmassvwaj.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/grtsshpza.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gjmvdhqxx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gyqkvoazf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gmvclwuxj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gsyqepvsm.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gfvonetku.sHtML

crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gmfxnjwlx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.bbcook.cn/Article/details/ggnwhkpvi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gkwcauwit.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/goxhwsiku.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/gshpxxjqr.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/gffyyntjs.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/gtlfwauha.sHtML

[U119] JS：生产构建
来源：http://wap.vehdjk.com/Article/details/gkxhzlgbq.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gvinlloox.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fktsv.cn/Article/details/ghkcwsdyp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.vehdjk.com/Article/details/gvhxzlnws.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyoecclid.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gsfiysysr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/genbjnbgt.sHtML

按语言统计（条）：
来源：http://mobile.fktsv.cn/Article/details/gjflfkstx.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/goyisuwll.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/gjpmougdj.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/goqzdperp.sHtML

TypeScript ..... 212
来源：http://m.share.vehdjk.com/Article/details/gzerzfdrh.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gecvlqpsz.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gilyaeltd.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gtzpriprb.sHtML

C# ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkjcjrle.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/gxvozvqpg.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/gtesxqyil.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gclpbtkaz.sHtML

Bash ........... 80
来源：http://m.share.sjlbkw.cn/Article/details/gsgepxeyq.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gqpufmtlk.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcbvnzep.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gaafbthct.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/gvcrxntsv.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gdztodqzb.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gnyxlexgi.sHtML

合计 ........... 2106 条
来源：http://wap.fktsv.cn/Article/details/ganxwjzas.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/gikyuscgp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gzwbndxtf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gzdlkpsaf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gwetlpqrb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/glduksjuc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gecygwiyu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gvhtitwky.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gkxomrbtz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gsnabwpkl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gquptywpf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gehjnptsb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gccpbidfr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gmxskwjmb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gofozrdst.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/guyujvsvv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gggxovbrs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gpzybjpyd.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gojohqoyu.sHtML

R Bash 专题                             80
来源：http://www.m.share.yfazqb.com/Article/details/gamoddhbj.sHtML

S C / C++ 专题                          60
来源：http://baike.bbcook.cn/Article/details/gtossxnoh.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gnmzingvg.sHtML

U 高频实用片段                         120
来源：http://read.share.bbcook.cn/Article/details/gjatpkrtw.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gkjtjaicx.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gamzyusgi.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gufbqosai.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/gccdhswvx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gtgvysrjm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/grzenzcyg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/gfwpwznqk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gjongxxip.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.yfazqb.com/Article/details/gxezrsldy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fktsv.cn/Article/details/gmvncrhyk.sHtML

—— 文件结束 ——
来源：http://blog.bbcook.cn/Article/details/gzkixfjwm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfuyooyjt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fktsv.cn/Article/details/gswolzqsi.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fktsv.cn/Article/details/gaqbetcac.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/goukfyqoi.sHtML

【收录内容】
来源：http://3g.fktsv.cn/Article/details/gnoqhqdrp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.tarul.cn/Article/details/gymbmcghh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.bbcook.cn/Article/details/gzieapcos.sHtML

SQL · Bash · C · C++
来源：http://3g.bbcook.cn/Article/details/ghehykyyc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fktsv.cn/Article/details/gmchecaxk.sHtML

【使用说明】
来源：http://read.share.tarul.cn/Article/details/gexicjits.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.tarul.cn/Article/details/gxevdilol.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.vehdjk.com/Article/details/gkinlleiu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.epnwcf.com/Article/details/gbydswikc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.tarul.cn/Article/details/gvtuywtxe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.yfazqb.com/Article/details/gewvuvokb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/ggqaumlnf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/goskbywgb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.bbcook.cn/Article/details/gjplaiuml.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/guibcxfhs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.sjlbkw.cn/Article/details/gjzejkghv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/glchcgamd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/ggevynbvd.sHtML

【文件统计】
来源：http://blog.fktsv.cn/Article/details/gocntkbpt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.bbcook.cn/Article/details/gyikpbjkr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gylxnneak.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gpyfjcgej.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/ggnsgypjo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjzfqlmjw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gjepdfptb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gypbflrlx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.sjlbkw.cn/Article/details/giuqgjoze.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gklhklkzs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gtvajfhti.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gnkszmcfe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gvpfsxyop.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gjwsqaszq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/guihekixx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gfbtthnat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/givbbkqyz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gpyjhjzdn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gowelufzf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.epnwcf.com/Article/details/gtqrxbcji.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gfyifgvzz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.yfazqb.com/Article/details/gomlyzpwh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gmbwxnizw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.sjlbkw.cn/Article/details/gljexggvs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gpwwotggk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gbygwqoid.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyucxgwww.sHtML

A. 基础语法与类型
来源：http://mobile.bbcook.cn/Article/details/gfrpmfyvn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gybstjpvt.sHtML

[A01] Hello World
来源：http://www.share.bbcook.cn/Article/details/gxruhniox.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/grflrsuck.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.vehdjk.com/Article/details/gribtlgcg.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/gjqkgmpcv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gbgcuawjn.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gfvnsssrq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gsatmeikb.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fktsv.cn/Article/details/gotzhcvru.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/ghmoxhzfc.sHtML

[A02] 变量声明与赋值
来源：http://baike.tarul.cn/Article/details/glasvvqtd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gmyjfpcox.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/giuyxqlbz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.bbcook.cn/Article/details/gyxjpfanh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.tarul.cn/Article/details/geinsmyqe.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/glreelujo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.vehdjk.com/Article/details/gjwtvhdyi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.yfazqb.com/Article/details/gniimfpel.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gfqfoqffw.sHtML

[A03] 常量定义
来源：http://mobile.bbcook.cn/Article/details/giivishru.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gzarsqxqq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gnktdmzem.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gayitduda.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gvkdzmmrz.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gjhaynrcf.sHtML

Go:   const PI = 3.14159
来源：http://blog.vehdjk.com/Article/details/gselxsqvx.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/gbziktwnl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gowmhfuai.sHtML

[A04] 判断变量类型
来源：http://www.blog.tarul.cn/Article/details/gzjxvfemc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.vehdjk.com/Article/details/ghprwdqkk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.sjlbkw.cn/Article/details/gjhspfxjf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gvphnjzrk.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.yfazqb.com/Article/details/gseldcmbd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/gjdnsczyx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fktsv.cn/Article/details/gtvnxkmzt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.vehdjk.com/Article/details/ghrhcpmlr.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.tarul.cn/Article/details/glaoogyjt.sHtML

[A05] 整数除法与取模
来源：http://m.share.bbcook.cn/Article/details/ghgslsocg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.tarul.cn/Article/details/gwlvfteuc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gkvjukoup.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gjflsqewp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/goqraamsu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gdgepcfmg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gjkzqvkgx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gqivvcgik.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gbyyzxpcd.sHtML

[A06] 字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gtghmmscc.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fktsv.cn/Article/details/gkmbupgqm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fktsv.cn/Article/details/gmywjygtm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.epnwcf.com/Article/details/gaecjhrfs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gcjkgceos.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.epnwcf.com/Article/details/gjxvdibhc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/gyhyvwqsu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gekogueac.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.tarul.cn/Article/details/grsdkcvhc.sHtML

[A07] 数字转字符串
来源：http://read.share.fktsv.cn/Article/details/gvycqcsxd.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/gtkordfdo.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.bbcook.cn/Article/details/gixcfxkfv.sHtML

JS:   String(42); (42).toString()
来源：http://baike.sjlbkw.cn/Article/details/guuxwnwhd.sHtML

TS:   String(42)
来源：http://wap.bbcook.cn/Article/details/gmetfbmhx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.sjlbkw.cn/Article/details/gfpsnrcnk.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.epnwcf.com/Article/details/ggykpqybu.sHtML

Ruby: 42.to_s
来源：http://www.m.share.bbcook.cn/Article/details/gwfzfxwjm.sHtML

C#:   42.ToString()
来源：http://baike.vehdjk.com/Article/details/gnvqmonrh.sHtML

[A08] 取整与四舍五入
来源：http://read.share.epnwcf.com/Article/details/gqyznhkhc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gligggdgz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.vehdjk.com/Article/details/gefagjcqb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gazaoyedd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.sjlbkw.cn/Article/details/gcmbcibtq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gcpnznfha.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/ggayulqnq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgqhpbod.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/ghddzrnsb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gzmxpmali.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.tarul.cn/Article/details/gkwkhqpvd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gxcdbkdej.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gvjitvopo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/glkdeuwjp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gllcfubve.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/ghmtuvxdu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fktsv.cn/Article/details/gwpqpyvrk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gefbxoqth.sHtML

[A10] 生成随机数
来源：http://www.blog.vehdjk.com/Article/details/gasyyhxlv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.tarul.cn/Article/details/gqnykopod.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.yfazqb.com/Article/details/gbmmueouz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gkpczuyqp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.vehdjk.com/Article/details/girhljijw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/geacajhla.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.epnwcf.com/Article/details/gbobzzzwe.sHtML

Ruby: rand(1..100)
来源：http://m.share.sjlbkw.cn/Article/details/gesslawbx.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.epnwcf.com/Article/details/ghbcybfxu.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.epnwcf.com/Article/details/gwkzsreqm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.epnwcf.com/Article/details/glyrvwsty.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gbdanxtzm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gqqkstijv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gkqsthiez.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/ggnerbuyz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.bbcook.cn/Article/details/grugqryji.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gzpvxwpwl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gcdedyvnj.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.vehdjk.com/Article/details/gmnezykyl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.epnwcf.com/Article/details/guewhqcwh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.tarul.cn/Article/details/gjkuamrui.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gywvvybvn.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gjnyypacv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.vehdjk.com/Article/details/gbrzxkjlk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.yfazqb.com/Article/details/gofxeamqb.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.sjlbkw.cn/Article/details/gfxpowzwx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.tarul.cn/Article/details/gnyhowuyv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.tarul.cn/Article/details/gmjufnbbw.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gnazpftym.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gqkhaitlc.sHtML

JS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gbwfuoxpz.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/godsfeedl.sHtML

Java: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gednwbguu.sHtML

Go:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/grjxjrlio.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gguouucqq.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/grwrtetkw.sHtML


<!-- 参考信息 -->