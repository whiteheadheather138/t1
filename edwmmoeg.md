代发 wailian999

[U81] JS：初始化项目
来源：http://ypr.ydzc1.top

npm init -y;  npm i express
来源：http://jre.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://lsh.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ofr.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://qxf.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://pmx.ivvv.top

[U84] JS：CommonJS 写法
来源：http://mfp.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qrj.jyoumei.cn

[U85] JS：可选链
来源：http://acu.yonumen.top

a?.b?.c
来源：http://vrs.redwolf501.top

[U86] JS：空值合并
来源：http://inl.yj20258888.top

a ?? b
来源：http://xjj.yueranfly.top

[U87] JS：解构默认值
来源：http://jgg.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://edj.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://yle.hcnkem.com

{ ...a, ...b }
来源：http://gor.gzhubu.top

[U89] JS：数组去重
来源：http://ebn.smart0.xyz

[...new Set(arr)]
来源：http://kfc.bjfxy.top

[U90] JS：数字数组排序
来源：http://jcc.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://clc.ivvv.top

[U91] JS：对象键值遍历
来源：http://bah.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tys.xinyue.icu

[U92] JS：深拷贝
来源：http://yss.jlsjyb.cn

structuredClone(obj)
来源：http://glj.snrcjt.cn

[U93] JS：模板字符串
来源：http://tcw.zhixingplan.top

`共 ${n} 条`
来源：http://pba.nanxinkj.top

[U94] JS：箭头函数
来源：http://fei.bjfxy.top

const double = x => x * 2;
来源：http://oix.hywenlv.cn

[U95] JS：Promise 包装
来源：http://adn.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://xrj.tarul.cn

[U96] JS：async/await 与异常
来源：http://ksh.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xna.jqgufenzy.top

[U97] JS：并发请求
来源：http://zis.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bnj.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://ffu.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cjm.sufxvd.cn

[U99] JS：事件监听
来源：http://xzh.ivvv.top

el.addEventListener("click", e => {})
来源：http://brj.pycfn.com

[U100] JS：DOM 查询
来源：http://dwi.tian-w.cn

document.querySelector(".item")
来源：http://iaw.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://enj.gaohongyu789.top

el.classList.toggle("active")
来源：http://izz.yfazqb.com

[U102] JS：本地存储
来源：http://txs.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qvf.zhijiandao.cn

[U103] JS：定时器
来源：http://vfm.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zbh.yangfankeji.com

[U104] JS：防抖
来源：http://xwi.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjh.hnqzz.top

[U105] JS：节流
来源：http://sgg.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sxw.tanke756.top

[U106] JS：日期格式化
来源：http://flm.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dbf.pycfn.com

[U107] JS：数字千分位
来源：http://ikt.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ddk.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://xyp.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gdi.bjfxy.top

[U109] JS：数组分组
来源：http://wah.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://uey.yj202588.top

[U110] JS：数组分块
来源：http://cge.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wtf.chenzaomai.com

[U111] JS：对象转 Map
来源：http://sqx.aizwys.cn

new Map(Object.entries(obj))
来源：http://mzd.sufxvd.cn

[U112] JS：字符串补位
来源：http://hnx.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://cel.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://lay.cdnleiting.top

s.replaceAll("a", "b")
来源：http://hzo.jianghu66.top

[U114] JS：JSON 深比较
来源：http://ilx.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xga.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://xfv.wangdashe.top

crypto.randomUUID()
来源：http://zlh.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://ezo.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://vdx.yj202588.top

[U117] JS：单元测试
来源：http://ask.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://xbk.yonumen.top

[U118] JS：开发服务器
来源：http://nth.vehdjk.com

npm i -D vite;  npx vite
来源：http://djh.jqgufenzy.top

[U119] JS：生产构建
来源：http://knm.aizwys.cn

npx vite build
来源：http://gtt.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://sxg.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://jgx.9152youxi.cn

================================================================================
来源：http://men.nanxuanxn.top

统计汇总
来源：http://hqr.gotoacloud.top

================================================================================
来源：http://bbl.yangfankeji.com

按语言统计（条）：
来源：http://qul.wangshuangyany.cn

Python ......... 252
来源：http://azv.ydjk.org.cn

PHP ............ 252
来源：http://qqa.haohaochexian.top

JavaScript ..... 252
来源：http://baf.quarkkingdee.top

TypeScript ..... 212
来源：http://dla.shangyingyoupin.top

Java ........... 212
来源：http://krb.zycfv.cn

Go ............. 212
来源：http://oor.gaohongyu789.top

Ruby ........... 212
来源：http://njn.cashguo.top

C# ............. 212
来源：http://cbi.zhoulong.xyz

C .............. 30
来源：http://yac.cashguo.top

C++ ............ 30
来源：http://uzv.epnwcf.com

SQL ............ 90
来源：http://yvw.jlsjyb.cn

Bash ........... 80
来源：http://oaa.smart0.xyz

Kotlin ......... 15
来源：http://bmp.0kj1m.cn

Swift .......... 15
来源：http://ahr.fktsv.cn

Lua ............ 10
来源：http://rqu.xuetiantiany.cn

Perl ........... 10
来源：http://uij.ywan-chungtsiang.top

Scala .......... 10
来源：http://led.zycfv.cn

------------------------------------
来源：http://axb.daxiang520.top

合计 ........... 2106 条
来源：http://bom.yongpay.top

按章节统计：
来源：http://cgs.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://elu.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vjm.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dis.epnwcf.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xiz.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bjy.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nrv.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dgi.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cnb.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zmy.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uyi.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eyn.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yrk.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wkq.aizwys.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eru.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cve.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qwb.fengsongda.top

Q SQL 专题                              90
来源：http://xez.yj20258.top

R Bash 专题                             80
来源：http://ulx.daria6918.cn

S C / C++ 专题                          60
来源：http://ctm.sufxvd.cn

T 其他语言补充                          60
来源：http://azn.chenlongwang.top

U 高频实用片段                         120
来源：http://xzy.zhiwuduotai.top

------------------------------------
来源：http://hhg.zhijiandao.cn

合计                                  2106 条
来源：http://wdg.sweek.top

--------------------------------------------------------------------------------
来源：http://syp.yuxming.cn

使用提醒
来源：http://gka.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://xdf.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sim.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zmw.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qvq.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://lsg.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fdh.ehwqpu.com

—— 文件结束 ——
来源：http://zhb.yfazqb.com

================================================================================
来源：http://zbg.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://enx.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://czl.gaohongyu789.top

================================================================================
来源：http://dtm.tanke756.top

【收录内容】
来源：http://vbp.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ygs.wangdashe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ife.jqgufenzy.top

SQL · Bash · C · C++
来源：http://zmt.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pfe.yfazqb.com

【使用说明】
来源：http://tvr.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ynr.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kyx.havefunace.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://stm.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ivo.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://etq.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zhc.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://opm.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hfp.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oyq.yuanzhike.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ldv.svipenyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cfq.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vwk.quarkkingdee.top

【文件统计】
来源：http://jhf.quarkkingdee.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cth.pycfn.com

--------------------------------------------------------------------------------
来源：http://ykr.zycfv.cn

目  录
来源：http://gdl.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://szf.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pjr.tanke756.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://knv.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://klw.dashuyun.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hki.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iha.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ijf.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://omo.andypj.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mid.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fuy.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gxj.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cre.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tbw.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eot.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vrm.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mkv.chenzaomai.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zvx.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cqt.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://amn.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oqx.yanxiufei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hxg.pycfn.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ouq.gaohongyu789.top

================================================================================
来源：http://hdn.zhoulong.xyz

A. 基础语法与类型
来源：http://nqf.guannengcc.top

================================================================================
来源：http://zmx.xylfe.cn

[A01] Hello World
来源：http://jrs.yj20258.top

Py:   print("Hello, World!")
来源：http://dpy.gzhubu.top

PHP:  echo "Hello, World!";
来源：http://xcj.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://zxg.hcnkem.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jwf.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://txr.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://fqz.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://bhw.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bqf.yuanzhike.top

[A02] 变量声明与赋值
来源：http://nrk.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xdb.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://nuo.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://szt.yuxming.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bee.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://ntx.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://xcg.uphjek.com

Ruby: name = "Alex"; age = 20
来源：http://fcu.tarul.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gfc.fanxiaobao.xyz

[A03] 常量定义
来源：http://kib.svipenyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bgz.cashguo.top

PHP:  const PI = 3.14159;
来源：http://avw.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://inp.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://jae.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://nne.vehdjk.com

Go:   const PI = 3.14159
来源：http://olb.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://ghq.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://tdq.xingfuxueyuan.xyz

[A04] 判断变量类型
来源：http://srl.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xgy.ppjwa.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xnn.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ayk.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://wvx.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cyx.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hge.zhixingplan.top

Ruby: x.class; x.is_a?(Integer)
来源：http://clm.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://mvb.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://brn.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xsd.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://ebm.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mhv.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tna.pycfn.com

Java: 7 / 2; 7 % 2
来源：http://dtf.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://eui.svipenyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://cgn.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://tdu.hfpthk.cn

[A06] 字符串转数字
来源：http://ehx.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://dby.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fuj.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zea.sufxvd.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mkv.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cfk.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fio.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kvx.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nwu.yongpay.top

[A07] 数字转字符串
来源：http://wtv.cheryme.top

Py:   str(42)
来源：http://jtp.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://hqz.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://kdk.daria6918.cn

TS:   String(42)
来源：http://yos.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xvj.epnwcf.com

Go:   strconv.Itoa(42)
来源：http://rbo.aizwys.cn

Ruby: 42.to_s
来源：http://qjy.shzxlz.cn

C#:   42.ToString()
来源：http://qcz.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://zyg.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sif.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zye.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hnt.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yjl.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gcx.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zyg.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://mgt.yangfankeji.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oow.gaohongyu789.top

[A09] 绝对值与最大最小值
来源：http://khc.pengpengdd.cyou

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yhp.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dxg.ctjpmb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zsy.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rbr.ywan-chungtsiang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zfg.shanyushiyangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lfd.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rri.jinqigufen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ifp.jiagoushi.top

[A10] 生成随机数
来源：http://kyz.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://fih.jinqigfzy.top

PHP:  random_int(1, 100);
来源：http://dte.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kmr.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://seo.nwbrower.top

Java: new Random().nextInt(100) + 1
来源：http://ggr.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://joq.9152youxi.cn

Ruby: rand(1..100)
来源：http://uoj.ywan-chungtsiang.top

C#:   new Random().Next(1, 101)
来源：http://dwe.xylfe.cn

[A11] 条件表达式（三元）
来源：http://bvf.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://ywf.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ynt.yuanzhike.top

JS:   x > 0 ? "yes" : "no"
来源：http://pad.jqgfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://xph.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://thu.wangshuangyany.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wcy.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mev.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://kkv.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://kkf.yanxiufei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://duf.ydjk.org.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uzh.cqqwz.cn

JS:   `Hello, ${name}!`
来源：http://ref.zhengqikj.top

TS:   `Hello, ${name}!`
来源：http://ffi.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://zbf.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://icc.ctjpmb.com

Ruby: "Hello, #{name}!"
来源：http://bhn.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://lzd.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vsr.birdmap.top

Py:   "第一行\n第二行"
来源：http://hna.hammf.cn

PHP:  "第一行\n第二行"
来源：http://fqp.fzhhl.top

JS:   "第一行\n第二行"
来源：http://cyo.zycfv.cn

TS:   "第一行\n第二行"
来源：http://vxv.gzhubu.top


<!-- 参考信息 -->