代发 wailian999

[U81] JS：初始化项目
来源：http://jid.dianchejie.cn

npm init -y;  npm i express
来源：http://suf.ydzc1.top

[U82] JS：package.json 脚本
来源：http://pfr.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://clv.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://xhh.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://jnv.ydjk.org.cn

[U84] JS：CommonJS 写法
来源：http://jkt.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://uni.smart0.xyz

[U85] JS：可选链
来源：http://oyf.cqqwz.cn

a?.b?.c
来源：http://rnk.tian-w.cn

[U86] JS：空值合并
来源：http://buw.mhx1999.top

a ?? b
来源：http://uju.tarul.cn

[U87] JS：解构默认值
来源：http://cfv.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://uvp.mhx1999.top

[U88] JS：对象展开合并
来源：http://gsc.wangdashe.top

{ ...a, ...b }
来源：http://pkf.haohaochexian.top

[U89] JS：数组去重
来源：http://xaq.aizwys.cn

[...new Set(arr)]
来源：http://klh.yueranfly.top

[U90] JS：数字数组排序
来源：http://ppt.fanxiaobao.xyz

[...arr].sort((a, b) => a - b)
来源：http://fer.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://lwv.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://psn.guowangkeji.top

[U92] JS：深拷贝
来源：http://nkq.yanxiufei.cn

structuredClone(obj)
来源：http://frh.hesvh.cn

[U93] JS：模板字符串
来源：http://ffy.zycfv.cn

`共 ${n} 条`
来源：http://nyv.fzhhl.top

[U94] JS：箭头函数
来源：http://wco.yj20258.top

const double = x => x * 2;
来源：http://xxi.yueranfly.top

[U95] JS：Promise 包装
来源：http://xil.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://uap.sysykeji.top

[U96] JS：async/await 与异常
来源：http://wmv.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wcz.tarul.cn

[U97] JS：并发请求
来源：http://evb.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xav.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://bui.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://egx.haohaochexian.top

[U99] JS：事件监听
来源：http://xzm.fehbvm.com

el.addEventListener("click", e => {})
来源：http://quz.gogol.net.cn

[U100] JS：DOM 查询
来源：http://vwl.zhoulong.xyz

document.querySelector(".item")
来源：http://gkf.hfpthk.cn

[U101] JS：classList 操作
来源：http://sjd.zdbjq.cn

el.classList.toggle("active")
来源：http://oec.pycfn.com

[U102] JS：本地存储
来源：http://btu.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wgt.ydzc1.top

[U103] JS：定时器
来源：http://eci.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mpl.haohaochexian.top

[U104] JS：防抖
来源：http://tgh.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qfd.yongpay.top

[U105] JS：节流
来源：http://aok.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://glv.vehdjk.com

[U106] JS：日期格式化
来源：http://iag.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cgt.fehbvm.com

[U107] JS：数字千分位
来源：http://bfh.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mdf.daxiang520.top

[U108] JS：随机整数
来源：http://sxu.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://egy.kuanghao11.cn

[U109] JS：数组分组
来源：http://nwx.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://tbe.yuxming.cn

[U110] JS：数组分块
来源：http://crb.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfz.cheryme.top

[U111] JS：对象转 Map
来源：http://ltz.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://iur.shuidangran.top

[U112] JS：字符串补位
来源：http://nzv.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://tsj.gotoacloud.top

[U113] JS：正则替换全部
来源：http://wcu.yongpay.top

s.replaceAll("a", "b")
来源：http://fwz.hesvh.cn

[U114] JS：JSON 深比较
来源：http://zly.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kze.xuanzx.com

[U115] JS：生成 UUID
来源：http://net.zhixingplan.top

crypto.randomUUID()
来源：http://yiv.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://gsr.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://omj.chenzaomai.com

[U117] JS：单元测试
来源：http://gas.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://dgk.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://cba.epnwcf.com

npm i -D vite;  npx vite
来源：http://uus.andypj.xyz

[U119] JS：生产构建
来源：http://ebg.yuxming.cn

npx vite build
来源：http://ydt.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://yau.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://lfd.chenjidiqi.icu

================================================================================
来源：http://axj.gotoacloud.top

统计汇总
来源：http://mwt.jlsjyb.cn

================================================================================
来源：http://ffw.bjfxy.top

按语言统计（条）：
来源：http://mtm.nwbrower.top

Python ......... 252
来源：http://pug.zhiwuduotai.top

PHP ............ 252
来源：http://kvh.pycfn.com

JavaScript ..... 252
来源：http://mpr.yonumen.top

TypeScript ..... 212
来源：http://mgx.smart0.xyz

Java ........... 212
来源：http://der.jqgfzy.top

Go ............. 212
来源：http://ouk.shuidangran.top

Ruby ........... 212
来源：http://qtt.ehwqpu.com

C# ............. 212
来源：http://csf.xuanzx.com

C .............. 30
来源：http://dpv.aizwys.cn

C++ ............ 30
来源：http://enm.havefunace.top

SQL ............ 90
来源：http://bvx.iojbl.cn

Bash ........... 80
来源：http://xer.yvedp.cn

Kotlin ......... 15
来源：http://zeq.shanyushiyangkeji.top

Swift .......... 15
来源：http://tht.cashguo.top

Lua ............ 10
来源：http://oxo.sweek.top

Perl ........... 10
来源：http://ztu.nanxinkj.top

Scala .......... 10
来源：http://txh.zhongyouzk.top

------------------------------------
来源：http://pfv.aibaodan.cn

合计 ........... 2106 条
来源：http://bbd.meibo888.top

按章节统计：
来源：http://hnx.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dka.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qre.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iva.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://liz.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jyv.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dcv.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://peo.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://neh.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yka.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lpt.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ngc.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lcb.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vnb.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://riq.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vak.jlsjyb.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fns.ivvv.top

Q SQL 专题                              90
来源：http://ifd.aizwys.cn

R Bash 专题                             80
来源：http://thd.0kj1m.cn

S C / C++ 专题                          60
来源：http://ghr.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://ldl.haohaochexian.top

U 高频实用片段                         120
来源：http://xka.yongpay.top

------------------------------------
来源：http://dut.pycfn.com

合计                                  2106 条
来源：http://dia.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ght.birdmap.top

使用提醒
来源：http://hgk.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://rbw.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://whj.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dai.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ble.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lik.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dlu.guowangkeji.top

—— 文件结束 ——
来源：http://qqb.gzhubu.top

================================================================================
来源：http://pxm.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://bfv.zycfv.cn

Common Programming Examples Cheat Book
来源：http://scu.gogol.net.cn

================================================================================
来源：http://yco.yj202588.top

【收录内容】
来源：http://vxg.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xfj.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mbl.andypj.xyz

SQL · Bash · C · C++
来源：http://luh.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jvv.jiagoushi.top

【使用说明】
来源：http://qmh.chenjidiqi.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wnx.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cic.ydzc1.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://piz.daxiang520.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://efq.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hky.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kkh.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ayp.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ftu.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ldy.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qsn.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lty.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xto.yj20258888.top

【文件统计】
来源：http://atx.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cee.epnwcf.com

--------------------------------------------------------------------------------
来源：http://sry.xinyue.icu

目  录
来源：http://mmg.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://eke.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rjw.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ssj.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oqr.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zpb.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ejx.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eql.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nvq.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vrp.zhengqikj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ray.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lqq.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bsj.jyoumei.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://reo.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hru.ppjwa.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ltm.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sev.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://joh.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://scy.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hpp.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mby.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qte.shuidangran.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zhm.jinqigfzy.top

================================================================================
来源：http://bcs.sjlbkw.cn

A. 基础语法与类型
来源：http://gzb.kuanghao11.cn

================================================================================
来源：http://wxg.yuxming.cn

[A01] Hello World
来源：http://ero.guannengcc.top

Py:   print("Hello, World!")
来源：http://nvc.ppjwa.cn

PHP:  echo "Hello, World!";
来源：http://tqb.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://fqn.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jkh.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://jmx.zhixingplan.top

Go:   fmt.Println("Hello, World!")
来源：http://vzj.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://nop.havefunace.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ftd.fehbvm.com

[A02] 变量声明与赋值
来源：http://fsu.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eje.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://crt.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://zpb.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yww.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://npa.yueranfly.top

Go:   name := "Alex"; age := 20
来源：http://wuv.jinqigfzy.top

Ruby: name = "Alex"; age = 20
来源：http://xco.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://jmx.pengpengdd.cyou

[A03] 常量定义
来源：http://csn.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ago.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://keh.jiagoushi.top

JS:   const PI = 3.14159;
来源：http://lmf.redwolf501.top

TS:   const PI: number = 3.14159;
来源：http://dka.quarkkingdee.top

Java: static final double PI = 3.14159;
来源：http://idi.316326.xyz

Go:   const PI = 3.14159
来源：http://lcx.aizwys.cn

Ruby: PI = 3.14159
来源：http://ffp.havefunace.top

C#:   const double PI = 3.14159;
来源：http://gwe.ydzc1.top

[A04] 判断变量类型
来源：http://kmr.bjfxy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://idf.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ddg.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ayr.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://npc.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ufg.yj20258888.top

Go:   reflect.TypeOf(x).Name()
来源：http://vun.hongshengwenyu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ihh.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://vpr.guannengcc.top

[A05] 整数除法与取模
来源：http://jbl.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fjd.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uqf.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kei.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lrf.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://vla.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://all.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://wup.gzhubu.top

C#:   7 / 2; 7 % 2
来源：http://ghr.zhengqikj.top

[A06] 字符串转数字
来源：http://owy.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://ufi.jinghuilouyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nxp.shanyushiyangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kpa.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://qds.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lgs.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kmh.fanxiaobao.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://zpl.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xir.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://ixd.jianghu66.top

Py:   str(42)
来源：http://ujj.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://tem.316326.xyz

JS:   String(42); (42).toString()
来源：http://hxs.yuanzhike.top

TS:   String(42)
来源：http://twp.guannengcc.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jil.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://ith.jqgufenzy.top

Ruby: 42.to_s
来源：http://yxd.tanke756.top

C#:   42.ToString()
来源：http://gzg.ehwqpu.com

[A08] 取整与四舍五入
来源：http://vbj.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ekm.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mpy.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mjt.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://anr.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wem.quarkkingdee.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xlz.cqqwz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://etb.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rui.fanxiaobao.xyz

[A09] 绝对值与最大最小值
来源：http://rpe.ppjwa.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://afn.shuidangran.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jde.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vie.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zgl.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tyb.xuetiantiany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://efb.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hny.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://css.ppjwa.cn

[A10] 生成随机数
来源：http://beu.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://ajy.cucudq.cn

PHP:  random_int(1, 100);
来源：http://tzi.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://obu.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wyb.316326.xyz

Java: new Random().nextInt(100) + 1
来源：http://sbu.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xsg.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://auy.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://qpe.tanke756.top

[A11] 条件表达式（三元）
来源：http://ijc.xylfe.cn

Py:   "yes" if x > 0 else "no"
来源：http://oan.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ocr.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oft.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://llh.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://azu.xuetiantiany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jag.yvedp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hjw.pycfn.com

C#:   x > 0 ? "yes" : "no"
来源：http://yvg.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://alo.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wiu.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zcs.hnqzz.top

JS:   `Hello, ${name}!`
来源：http://ubc.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://dwn.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://lom.jqgfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xtb.xuanzx.com

Ruby: "Hello, #{name}!"
来源：http://hjj.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://bgr.vehdjk.com

[A13] 多行字符串（练习 \n 转义）
来源：http://ywu.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://hdy.tarul.cn

PHP:  "第一行\n第二行"
来源：http://gmk.havefunace.top

JS:   "第一行\n第二行"
来源：http://ugn.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://dgk.shanyushiyangkeji.top


<!-- 参考信息 -->