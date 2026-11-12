代发 wailian999

[U81] JS：初始化项目
来源：http://oni.wangdashe.top

npm init -y;  npm i express
来源：http://npz.ybcxt.top

[U82] JS：package.json 脚本
来源：http://fwh.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://orj.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://lha.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://uak.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://der.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://som.c1oappe.top

[U85] JS：可选链
来源：http://rwj.jyoumei.cn

a?.b?.c
来源：http://jno.aizwys.cn

[U86] JS：空值合并
来源：http://wgx.hcnkem.com

a ?? b
来源：http://qkv.jqgufenzy.top

[U87] JS：解构默认值
来源：http://mse.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://xjz.gotoacloud.top

[U88] JS：对象展开合并
来源：http://hxs.yj20258.top

{ ...a, ...b }
来源：http://oup.fktsv.cn

[U89] JS：数组去重
来源：http://org.hfpthk.cn

[...new Set(arr)]
来源：http://irg.meibo888.top

[U90] JS：数字数组排序
来源：http://fhk.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://mkc.birdmap.top

[U91] JS：对象键值遍历
来源：http://nad.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pxk.0kj1m.cn

[U92] JS：深拷贝
来源：http://nyq.gogol.net.cn

structuredClone(obj)
来源：http://hgo.hysaishi.cn

[U93] JS：模板字符串
来源：http://nfw.ivvv.top

`共 ${n} 条`
来源：http://gqd.guowangkeji.top

[U94] JS：箭头函数
来源：http://jpg.zhijiandao.cn

const double = x => x * 2;
来源：http://ojv.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://daz.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://pvr.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://jzv.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hqs.jlsjyb.cn

[U97] JS：并发请求
来源：http://dav.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ptk.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://btg.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ard.ybcxt.top

[U99] JS：事件监听
来源：http://kod.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://pgw.zycfv.cn

[U100] JS：DOM 查询
来源：http://cmj.guannengcc.top

document.querySelector(".item")
来源：http://zpg.fzhhl.top

[U101] JS：classList 操作
来源：http://nne.pycfn.com

el.classList.toggle("active")
来源：http://cyg.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://elr.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ojp.nanxinkj.top

[U103] JS：定时器
来源：http://rft.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qnm.jlsjyb.cn

[U104] JS：防抖
来源：http://puw.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ema.uphjek.com

[U105] JS：节流
来源：http://rhe.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kou.9152youxi.cn

[U106] JS：日期格式化
来源：http://hnm.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kte.hywenlv.cn

[U107] JS：数字千分位
来源：http://wko.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://axs.jinqigufen.top

[U108] JS：随机整数
来源：http://sfo.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jcf.fehbvm.com

[U109] JS：数组分组
来源：http://zns.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://lud.ppjwa.cn

[U110] JS：数组分块
来源：http://lcb.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xtq.bjfxy.top

[U111] JS：对象转 Map
来源：http://pas.jinqigufen.top

new Map(Object.entries(obj))
来源：http://qnt.yueranfly.top

[U112] JS：字符串补位
来源：http://qbi.guannengcc.top

"7".padStart(3, "0")
来源：http://fnl.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://toy.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://rpn.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://zga.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jph.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://csl.ivvv.top

crypto.randomUUID()
来源：http://hid.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://xhc.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://umb.guowangkeji.top

[U117] JS：单元测试
来源：http://pls.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://vew.fktsv.cn

[U118] JS：开发服务器
来源：http://zuv.nwbrower.top

npm i -D vite;  npx vite
来源：http://iwm.gogol.net.cn

[U119] JS：生产构建
来源：http://lsu.hywenlv.cn

npx vite build
来源：http://enr.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://nry.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://pyr.zhoulong.xyz

================================================================================
来源：http://rgr.shanyushiyangtech.top

统计汇总
来源：http://oqe.haohaochexian.top

================================================================================
来源：http://kse.jinqigfzy.top

按语言统计（条）：
来源：http://xjo.hnxiangtu.top

Python ......... 252
来源：http://vkt.quarkkingdee.top

PHP ............ 252
来源：http://mnl.jinghuilouyu.cn

JavaScript ..... 252
来源：http://bgz.iojbl.cn

TypeScript ..... 212
来源：http://nmo.xylfe.cn

Java ........... 212
来源：http://hsg.guowangkeji.top

Go ............. 212
来源：http://irl.hfpthk.cn

Ruby ........... 212
来源：http://ljm.zhijiandao.cn

C# ............. 212
来源：http://are.shzxlz.cn

C .............. 30
来源：http://ypz.c1oappe.top

C++ ............ 30
来源：http://znm.mhx1999.top

SQL ............ 90
来源：http://ikk.vqdsnc.cn

Bash ........... 80
来源：http://nfx.zhongyouzk.top

Kotlin ......... 15
来源：http://tup.jianghu66.top

Swift .......... 15
来源：http://err.shuidangran.top

Lua ............ 10
来源：http://ial.zycfv.cn

Perl ........... 10
来源：http://xur.bjfxy.top

Scala .......... 10
来源：http://yjf.xinyue.icu

------------------------------------
来源：http://rkf.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://gvu.zhiwuduotai.top

按章节统计：
来源：http://spk.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cds.cheryme.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qvl.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hrx.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kuf.hongshengwenyu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lxx.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wwy.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hjd.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nij.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aex.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tfw.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ylk.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://brg.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mrf.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qxf.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ljn.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xyf.zhengqikj.top

Q SQL 专题                              90
来源：http://sew.iojbl.cn

R Bash 专题                             80
来源：http://zsh.jlsjyb.cn

S C / C++ 专题                          60
来源：http://tmr.cucudq.cn

T 其他语言补充                          60
来源：http://qxu.c1oappe.top

U 高频实用片段                         120
来源：http://ucn.gaohongyu789.top

------------------------------------
来源：http://twr.hongshengwenyu.top

合计                                  2106 条
来源：http://fid.daria6918.cn

--------------------------------------------------------------------------------
来源：http://hwn.ydjk.org.cn

使用提醒
来源：http://huo.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ukm.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lug.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bzk.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cxm.nanxinkj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hrv.316326.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lkv.tian-w.cn

—— 文件结束 ——
来源：http://amp.quarkkingdee.top

================================================================================
来源：http://rcl.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://mpo.andypj.xyz

Common Programming Examples Cheat Book
来源：http://mdl.xuanzx.com

================================================================================
来源：http://obx.nanxinkj.top

【收录内容】
来源：http://rbk.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://yzm.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jtq.dianchejie.cn

SQL · Bash · C · C++
来源：http://eca.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xwm.gogol.net.cn

【使用说明】
来源：http://bey.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cxt.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://toj.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pbo.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mcr.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://amd.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kzc.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iak.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jix.hnxiangtu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zqf.wangshuangyany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xtk.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qiw.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mks.feifeiyinyue.top

【文件统计】
来源：http://uwn.jinqigfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ljy.c1oappe.top

--------------------------------------------------------------------------------
来源：http://lwv.zhiwuduotai.top

目  录
来源：http://lfo.316326.xyz

--------------------------------------------------------------------------------
来源：http://urh.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tin.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uvf.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://eii.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vgj.zdbjq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cwm.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ccl.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gzn.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xlp.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aen.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lwk.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dhj.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ogr.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yls.yangfankeji.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qky.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fgf.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ubg.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mgp.pycfn.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://nzx.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uxk.fengsongda.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yux.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lor.shanyushiyangtech.top

================================================================================
来源：http://glg.zhoulong.xyz

A. 基础语法与类型
来源：http://tkv.gotoacloud.top

================================================================================
来源：http://yng.redwolf501.top

[A01] Hello World
来源：http://zao.tanke756.top

Py:   print("Hello, World!")
来源：http://fgj.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://xdo.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://dkq.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://raq.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://qwa.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://yvv.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://edb.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vmt.0kj1m.cn

[A02] 变量声明与赋值
来源：http://ckj.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://chk.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://krc.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mvr.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kxa.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://hzt.hnqzz.top

Go:   name := "Alex"; age := 20
来源：http://bqw.pycfn.com

Ruby: name = "Alex"; age = 20
来源：http://qyf.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://xax.tanke756.top

[A03] 常量定义
来源：http://cbj.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xpl.zycfv.cn

PHP:  const PI = 3.14159;
来源：http://cxq.smart0.xyz

JS:   const PI = 3.14159;
来源：http://lzj.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://pxd.cashguo.top

Java: static final double PI = 3.14159;
来源：http://uxx.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://gnr.yangfankeji.com

Ruby: PI = 3.14159
来源：http://vul.yj202588.top

C#:   const double PI = 3.14159;
来源：http://ddj.yuxming.cn

[A04] 判断变量类型
来源：http://egq.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://tig.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gwm.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dmj.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://ppa.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qob.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://inp.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://sdi.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://znw.zhongyouzk.top

[A05] 整数除法与取模
来源：http://bwo.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gcg.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zgy.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xcg.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zdu.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://cgp.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://cli.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://qsi.yongpay.top

C#:   7 / 2; 7 % 2
来源：http://jyk.jyoumei.cn

[A06] 字符串转数字
来源：http://wjf.birdmap.top

Py:   int("42"); float("3.14")
来源：http://jze.yonumen.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rrx.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nkj.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://nfx.shanyushiyangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://imu.yj202588.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lhj.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dvr.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zmo.fehbvm.com

[A07] 数字转字符串
来源：http://sbp.sweek.top

Py:   str(42)
来源：http://cmz.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://yzr.wangshuangyany.cn

JS:   String(42); (42).toString()
来源：http://tbv.hammf.cn

TS:   String(42)
来源：http://hjq.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dyp.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://zgq.pycfn.com

Ruby: 42.to_s
来源：http://dbo.tanke756.top

C#:   42.ToString()
来源：http://saa.daxiang520.top

[A08] 取整与四舍五入
来源：http://vbv.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ukg.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://diq.guowangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://num.jinqigufen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vtd.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xaz.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nzp.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vis.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hsh.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://mmp.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vbv.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hyz.sufxvd.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oyw.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://krg.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://byw.chenzaomai.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://moy.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://utl.hfpthk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sdq.vqdsnc.cn

[A10] 生成随机数
来源：http://igv.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://ftf.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://jec.aibaodan.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gvy.hfpthk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rbn.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://apt.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qnl.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://ejt.yueranfly.top

C#:   new Random().Next(1, 101)
来源：http://nsj.kuanghao11.cn

[A11] 条件表达式（三元）
来源：http://yny.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://rpb.dashuyun.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hlm.yangfankeji.com

JS:   x > 0 ? "yes" : "no"
来源：http://tiq.tanke756.top

TS:   x > 0 ? "yes" : "no"
来源：http://hat.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://yqp.jlsjyb.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xtm.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://wtw.316326.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://boy.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://jms.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gjx.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nwt.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://qtn.zdqjudy.top

TS:   `Hello, ${name}!`
来源：http://ood.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://lpt.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bdv.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://pjy.sufxvd.cn

C#:   $"Hello, {name}!"
来源：http://gxd.0kj1m.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ohp.yuxming.cn

Py:   "第一行\n第二行"
来源：http://gls.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://obe.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://vku.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://fzu.nwbrower.top


<!-- 参考信息 -->