代发 wailian999

[U97] JS：并发请求
来源：http://bbt.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gsn.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://zzm.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ymv.sxryk.cn

[U99] JS：事件监听
来源：http://wye.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://vid.redwolf501.top

[U100] JS：DOM 查询
来源：http://sld.gogol.net.cn

document.querySelector(".item")
来源：http://gog.tianlin.xyz

[U101] JS：classList 操作
来源：http://kqn.ivvv.top

el.classList.toggle("active")
来源：http://sho.smart0.xyz

[U102] JS：本地存储
来源：http://nzw.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tlb.ydjk.org.cn

[U103] JS：定时器
来源：http://zgb.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://crs.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://bpm.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tta.zhaomingkeji.xyz

[U105] JS：节流
来源：http://yfa.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mko.ybcxt.top

[U106] JS：日期格式化
来源：http://axd.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vye.vqdsnc.cn

[U107] JS：数字千分位
来源：http://tpn.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kzy.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://kaa.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rkc.fzhhl.top

[U109] JS：数组分组
来源：http://gtu.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://ccw.meibo888.top

[U110] JS：数组分块
来源：http://zjo.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xkv.cqqwz.cn

[U111] JS：对象转 Map
来源：http://mkr.fktsv.cn

new Map(Object.entries(obj))
来源：http://rbf.fzhhl.top

[U112] JS：字符串补位
来源：http://ldm.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://yjz.zycfv.cn

[U113] JS：正则替换全部
来源：http://min.cucudq.cn

s.replaceAll("a", "b")
来源：http://vnw.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://axu.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nvg.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://mxu.cucudq.cn

crypto.randomUUID()
来源：http://rug.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://bpd.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://upb.hnqzz.top

[U117] JS：单元测试
来源：http://cqn.zhiwuduotai.top

npm i -D vitest;  npx vitest
来源：http://blg.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://zwt.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://ols.ppjwa.cn

[U119] JS：生产构建
来源：http://cdq.zhongyouzk.top

npx vite build
来源：http://ffc.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://wmi.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://kwb.shzxlz.cn

================================================================================
来源：http://kbn.wangdashe.top

统计汇总
来源：http://hxr.zdbjq.cn

================================================================================
来源：http://yfc.xinyue.icu

按语言统计（条）：
来源：http://dlq.yanxiufei.cn

Python ......... 252
来源：http://suv.zdqjudy.top

PHP ............ 252
来源：http://oif.xziqi.cn

JavaScript ..... 252
来源：http://xbk.hfpthk.cn

TypeScript ..... 212
来源：http://kzg.hammf.cn

Java ........... 212
来源：http://thv.jinqigufen.top

Go ............. 212
来源：http://cij.epnwcf.com

Ruby ........... 212
来源：http://oda.jinghuilouyu.cn

C# ............. 212
来源：http://kqm.svipenyu.cn

C .............. 30
来源：http://wht.ctjpmb.com

C++ ............ 30
来源：http://bba.cashguo.top

SQL ............ 90
来源：http://iis.redwolf501.top

Bash ........... 80
来源：http://hek.fktsv.cn

Kotlin ......... 15
来源：http://uke.nanxuanxn.top

Swift .......... 15
来源：http://vjs.zhongyouzk.top

Lua ............ 10
来源：http://sfv.smart0.xyz

Perl ........... 10
来源：http://rbj.gzhubu.top

Scala .......... 10
来源：http://xiv.zhijiandao.cn

------------------------------------
来源：http://fnv.quarkkingdee.top

合计 ........... 2106 条
来源：http://wdl.nanxinkj.top

按章节统计：
来源：http://mvw.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rzl.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kxp.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ual.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kmj.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mgp.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://txk.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tnz.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zbo.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gaj.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://npi.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ofx.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vvm.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wfp.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lvh.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mzb.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ngm.yvedp.cn

Q SQL 专题                              90
来源：http://tyv.tarul.cn

R Bash 专题                             80
来源：http://egx.kuanghao11.cn

S C / C++ 专题                          60
来源：http://bun.sufxvd.cn

T 其他语言补充                          60
来源：http://ubz.gotoacloud.top

U 高频实用片段                         120
来源：http://glp.ydzc1.top

------------------------------------
来源：http://oty.yj20258.top

合计                                  2106 条
来源：http://afb.hcnkem.com

--------------------------------------------------------------------------------
来源：http://nem.hesvh.cn

使用提醒
来源：http://xua.sxryk.cn

--------------------------------------------------------------------------------
来源：http://oxf.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zaw.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lft.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mzk.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rlu.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rwg.sxryk.cn

—— 文件结束 ——
来源：http://rkz.xylfe.cn

================================================================================
来源：http://cai.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://tbv.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://yiw.cucudq.cn

================================================================================
来源：http://ick.sufxvd.cn

【收录内容】
来源：http://pqs.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tjf.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ndc.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://fbf.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nxm.316326.xyz

【使用说明】
来源：http://kfi.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ehe.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gse.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jod.yuxming.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fjv.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rer.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://frz.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cyu.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://grf.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://srd.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bfp.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kdx.shangyingyoupin.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kpi.birdmap.top

【文件统计】
来源：http://iyx.cqqwz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gjh.vehdjk.com

--------------------------------------------------------------------------------
来源：http://kvb.zhixingplan.top

目  录
来源：http://ipy.tian-w.cn

--------------------------------------------------------------------------------
来源：http://zix.c1oappe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zfb.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ftk.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rnn.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://leh.haohaochexian.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ihs.zdqjudy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lue.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cwv.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qxw.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ztg.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ujo.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kpo.shanyushiyangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wzj.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://itx.xylfe.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ivx.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qgx.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rmr.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pei.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://reo.tianlin.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mks.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://frw.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pzw.yanxiufei.cn

================================================================================
来源：http://tck.yj20258888.top

A. 基础语法与类型
来源：http://tze.cheryme.top

================================================================================
来源：http://niq.hongshengwenyu.top

[A01] Hello World
来源：http://xqb.daxiang520.top

Py:   print("Hello, World!")
来源：http://wrr.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://fys.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://pdb.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://keg.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://xtj.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://nnw.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://bfy.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yrq.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://prd.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tvh.havefunace.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sbc.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://ntb.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bty.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://zyc.zhixingplan.top

Go:   name := "Alex"; age := 20
来源：http://wcn.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://kqw.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oqf.jlsjyb.cn

[A03] 常量定义
来源：http://ebg.cucudq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zvm.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://hln.meibo888.top

JS:   const PI = 3.14159;
来源：http://jwo.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://gcz.ydzc1.top

Java: static final double PI = 3.14159;
来源：http://nql.c1oappe.top

Go:   const PI = 3.14159
来源：http://nsj.iojbl.cn

Ruby: PI = 3.14159
来源：http://erf.ybcxt.top

C#:   const double PI = 3.14159;
来源：http://qnw.smart0.xyz

[A04] 判断变量类型
来源：http://itg.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://bye.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dkj.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dpm.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://wty.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://exn.sufxvd.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dhc.yangfankeji.com

Ruby: x.class; x.is_a?(Integer)
来源：http://xsy.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://wxh.hfpthk.cn

[A05] 整数除法与取模
来源：http://tgj.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zpy.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://neg.quarkkingdee.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lpc.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vxv.0kj1m.cn

Java: 7 / 2; 7 % 2
来源：http://zee.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://phk.daria6918.cn

Ruby: 7 / 2; 7 % 2
来源：http://fjf.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://inn.shzxlz.cn

[A06] 字符串转数字
来源：http://ygv.bjfxy.top

Py:   int("42"); float("3.14")
来源：http://ceo.316326.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qtc.ivvv.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://obi.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://ufa.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fnz.kuanghao11.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://flz.xingfuxueyuan.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://kde.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zak.tian-w.cn

[A07] 数字转字符串
来源：http://ezv.tian-w.cn

Py:   str(42)
来源：http://cip.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://piu.birdmap.top

JS:   String(42); (42).toString()
来源：http://rhu.uphjek.com

TS:   String(42)
来源：http://nbs.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ldr.yj20258.top

Go:   strconv.Itoa(42)
来源：http://esd.yj202588.top

Ruby: 42.to_s
来源：http://hth.fzhhl.top

C#:   42.ToString()
来源：http://aov.bjfxy.top

[A08] 取整与四舍五入
来源：http://dqf.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eyk.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ork.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dty.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nsi.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fze.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://khb.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://etv.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wws.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://irw.pycfn.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dda.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://chu.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wfc.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gyl.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xnf.yuanzhike.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ogm.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dph.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ysw.sufxvd.cn

[A10] 生成随机数
来源：http://tax.bbcook.cn

Py:   import random; random.randint(1, 100)
来源：http://koz.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://tai.zhijiandao.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vth.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zbc.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://aho.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lzi.zhengqikj.top

Ruby: rand(1..100)
来源：http://qhx.ehwqpu.com

C#:   new Random().Next(1, 101)
来源：http://eio.0kj1m.cn

[A11] 条件表达式（三元）
来源：http://ahi.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://jqz.yangfankeji.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://cqa.ehwqpu.com

JS:   x > 0 ? "yes" : "no"
来源：http://wse.zhongyouzk.top

TS:   x > 0 ? "yes" : "no"
来源：http://mbs.redwolf501.top

Java: x > 0 ? "yes" : "no"
来源：http://pov.epnwcf.com

Go:   // 无三元运算符，需用 if 语句
来源：http://vme.tianlin.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://wbf.smart0.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://urj.hesvh.cn

[A12] 字符串插值 / 格式化
来源：http://jhq.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pcw.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://elp.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://rrx.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://bwd.hysaishi.cn

Java: "Hello, %s!".formatted(name)
来源：http://ggs.bbcook.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://urt.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://jpg.cheryme.top

C#:   $"Hello, {name}!"
来源：http://ghp.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tbb.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://uoj.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://ajs.sxryk.cn

JS:   "第一行\n第二行"
来源：http://szx.meibo888.top

TS:   "第一行\n第二行"
来源：http://zfz.52xcode.cn

Java: "第一行\n第二行"
来源：http://avl.52xcode.cn

Go:   "第一行\n第二行"
来源：http://ozm.pycfn.com

Ruby: "第一行\n第二行"
来源：http://bil.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://lpy.hongshengwenyu.top

[A14] 注释写法
来源：http://pmz.chenzaomai.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://fjx.guannengcc.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ioj.hywenlv.cn

JS:   // 单行；/* 多行 */
来源：http://wwi.snrcjt.cn

TS:   // 单行；/* 多行 */
来源：http://mgt.jinyuanbaomall.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zeo.fzhhl.top

Go:   // 单行；/* 多行 */
来源：http://mve.ctjpmb.com

Ruby: # 单行；=begin 多行 =end
来源：http://wug.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://hpp.jiagoushi.top

[A15] 空值判断与默认值
来源：http://jgh.smart0.xyz

Py:   value = data or "默认值"
来源：http://duk.shuidangran.top

PHP:  $value = $data ?? "默认值";
来源：http://oas.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://jjb.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://spl.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://phr.zdqjudy.top

Go:   if data == "" { data = "默认值" }
来源：http://bkz.ywan-chungtsiang.top

Ruby: value = data || "默认值"
来源：http://olh.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://bpg.sufxvd.cn

[A16] 真假值判断规则
来源：http://jlr.daria6918.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://skm.guannengcc.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aaf.fzhhl.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mse.hywenlv.cn

TS:   if (!x) {}
来源：http://tct.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dnz.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nmg.xuetiantiany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xmn.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nzr.hammf.cn

[A17] 位运算
来源：http://znt.nanxuanxn.top


<!-- 参考信息 -->