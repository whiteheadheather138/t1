代发 wailian999

[U93] JS：模板字符串
来源：http://obq.pengpengdd.cyou

`共 ${n} 条`
来源：http://aiq.sjlbkw.cn

[U94] JS：箭头函数
来源：http://dzs.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://xka.shuidangran.top

[U95] JS：Promise 包装
来源：http://wui.uphjek.com

new Promise((resolve, reject) => {})
来源：http://ebp.havefunace.top

[U96] JS：async/await 与异常
来源：http://qhn.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nql.hesvh.cn

[U97] JS：并发请求
来源：http://ygb.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sgi.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://zvq.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nzt.jqgfzy.top

[U99] JS：事件监听
来源：http://jch.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://fuz.nanxinkj.top

[U100] JS：DOM 查询
来源：http://fgl.52xcode.cn

document.querySelector(".item")
来源：http://loh.guowangkeji.top

[U101] JS：classList 操作
来源：http://twp.aibaodan.cn

el.classList.toggle("active")
来源：http://odm.yanxiufei.cn

[U102] JS：本地存储
来源：http://kca.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dku.jqgfzy.top

[U103] JS：定时器
来源：http://gou.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dkr.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://shw.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgw.nwbrower.top

[U105] JS：节流
来源：http://gjz.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dlo.svipenyu.cn

[U106] JS：日期格式化
来源：http://uzn.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ntc.jiagoushi.top

[U107] JS：数字千分位
来源：http://eph.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gsh.pycfn.com

[U108] JS：随机整数
来源：http://jmm.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ytj.nanxinkj.top

[U109] JS：数组分组
来源：http://wxi.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://odz.xuanzx.com

[U110] JS：数组分块
来源：http://gzq.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nwn.snrcjt.cn

[U111] JS：对象转 Map
来源：http://eqp.nwbrower.top

new Map(Object.entries(obj))
来源：http://aax.zdqjudy.top

[U112] JS：字符串补位
来源：http://upb.andypj.xyz

"7".padStart(3, "0")
来源：http://jyr.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://hvx.gotoacloud.top

s.replaceAll("a", "b")
来源：http://ikf.yvedp.cn

[U114] JS：JSON 深比较
来源：http://gof.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ydl.uphjek.com

[U115] JS：生成 UUID
来源：http://mjh.c1oappe.top

crypto.randomUUID()
来源：http://xer.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://xny.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://kyx.sjlbkw.cn

[U117] JS：单元测试
来源：http://bom.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://hsq.aibaodan.cn

[U118] JS：开发服务器
来源：http://cmn.xziqi.cn

npm i -D vite;  npx vite
来源：http://mcs.52xcode.cn

[U119] JS：生产构建
来源：http://dmq.zhiwuduotai.top

npx vite build
来源：http://hqb.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://kbd.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://ahc.yj20258.top

================================================================================
来源：http://nix.zhongyouzk.top

统计汇总
来源：http://xtf.sysykeji.top

================================================================================
来源：http://kyh.wangshuangyany.cn

按语言统计（条）：
来源：http://bfa.vehdjk.com

Python ......... 252
来源：http://qdm.jinghuilouyu.cn

PHP ............ 252
来源：http://ojq.shanyushiyangtech.top

JavaScript ..... 252
来源：http://qwn.zhixingplan.top

TypeScript ..... 212
来源：http://yyo.jianghu66.top

Java ........... 212
来源：http://plp.shanyushiyangkeji.top

Go ............. 212
来源：http://lsk.jlsjyb.cn

Ruby ........... 212
来源：http://xxn.jinghuilouyu.cn

C# ............. 212
来源：http://uqd.sjlbkw.cn

C .............. 30
来源：http://gtx.wangdashe.top

C++ ............ 30
来源：http://gql.zhixingplan.top

SQL ............ 90
来源：http://jpf.chenjidiqi.icu

Bash ........... 80
来源：http://cgr.wangshuangyany.cn

Kotlin ......... 15
来源：http://dxj.tian-w.cn

Swift .......... 15
来源：http://vjz.havefunace.top

Lua ............ 10
来源：http://wtt.cqqwz.cn

Perl ........... 10
来源：http://xhy.yangfankeji.com

Scala .......... 10
来源：http://kvt.pycfn.com

------------------------------------
来源：http://vnz.vqdsnc.cn

合计 ........... 2106 条
来源：http://peg.dashuyun.cn

按章节统计：
来源：http://zzl.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jyw.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://thy.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ltz.epnwcf.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sai.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://umo.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://isv.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dwo.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zzc.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kes.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cmq.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ydh.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gjy.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bfw.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uof.yj20258.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oid.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bja.sweek.top

Q SQL 专题                              90
来源：http://epx.ydzc1.top

R Bash 专题                             80
来源：http://jgv.ybcxt.top

S C / C++ 专题                          60
来源：http://jbh.yueranfly.top

T 其他语言补充                          60
来源：http://gpp.hysaishi.cn

U 高频实用片段                         120
来源：http://wpc.daria6918.cn

------------------------------------
来源：http://uli.yj20258.top

合计                                  2106 条
来源：http://vll.tanke756.top

--------------------------------------------------------------------------------
来源：http://spx.jyoumei.cn

使用提醒
来源：http://ats.yongpay.top

--------------------------------------------------------------------------------
来源：http://gpd.yvedp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://swn.epnwcf.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nzr.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sfn.yongpay.top

在旧版本上使用前请先确认语法支持情况。
来源：http://shy.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fva.guannengcc.top

—— 文件结束 ——
来源：http://cpr.zhongyouzk.top

================================================================================
来源：http://oey.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://urk.fktsv.cn

Common Programming Examples Cheat Book
来源：http://rbt.sxryk.cn

================================================================================
来源：http://odp.jiagoushi.top

【收录内容】
来源：http://plq.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vbn.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uvg.iojbl.cn

SQL · Bash · C · C++
来源：http://xan.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wea.ywan-chungtsiang.top

【使用说明】
来源：http://jkc.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ykh.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nns.jyoumei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qvi.dianchejie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vkc.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wns.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nsa.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tlq.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://obs.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wxq.yj20258.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dab.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rei.iojbl.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kws.svipenyu.cn

【文件统计】
来源：http://pgo.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jky.aizwys.cn

--------------------------------------------------------------------------------
来源：http://scr.0kj1m.cn

目  录
来源：http://xot.gzhubu.top

--------------------------------------------------------------------------------
来源：http://hiy.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://obh.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xlm.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://upn.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://whq.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ozh.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mrn.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ayk.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zxc.hnqzz.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rhd.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bvt.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fej.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fdf.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pjq.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://izr.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hxw.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bks.316326.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lkc.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gcf.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bbz.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqn.ybcxt.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dmm.cqqwz.cn

================================================================================
来源：http://kse.jyoumei.cn

A. 基础语法与类型
来源：http://zgw.fzhhl.top

================================================================================
来源：http://vfw.jianghu66.top

[A01] Hello World
来源：http://hfb.zhixingplan.top

Py:   print("Hello, World!")
来源：http://swe.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://xai.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://glj.chenzaomai.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lwo.hcnkem.com

Java: System.out.println("Hello, World!");
来源：http://hgk.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://khe.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://fxq.mhx1999.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rez.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://wrw.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rxz.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hrf.xinyue.icu

JS:   let name = "Alex"; const age = 20;
来源：http://hee.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gee.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://vfn.ydzc1.top

Go:   name := "Alex"; age := 20
来源：http://odw.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://npa.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://umg.fengsongda.top

[A03] 常量定义
来源：http://ttv.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jtr.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://ncp.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://vud.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://dwn.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://lxa.ivvv.top

Go:   const PI = 3.14159
来源：http://mep.guannengcc.top

Ruby: PI = 3.14159
来源：http://zho.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://awt.pycfn.com

[A04] 判断变量类型
来源：http://iak.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lai.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nod.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://evw.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://vfg.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iqq.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wpc.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://juc.vehdjk.com

C#:   x.GetType().Name; x is int
来源：http://qqg.jlsjyb.cn

[A05] 整数除法与取模
来源：http://qpj.yangfankeji.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bxr.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ier.bjfxy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ysm.shangyingyoupin.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eyr.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://whq.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://vcd.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://nqt.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://rvk.yonumen.top

[A06] 字符串转数字
来源：http://xku.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://crg.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kto.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eor.jlsjyb.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qwh.svipenyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nnq.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cxi.shzxlz.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hwk.zhiwuduotai.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dkr.hesvh.cn

[A07] 数字转字符串
来源：http://npi.zhiwuduotai.top

Py:   str(42)
来源：http://efd.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://vgs.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://qxp.quarkkingdee.top

TS:   String(42)
来源：http://nai.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jwd.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://oik.yonumen.top

Ruby: 42.to_s
来源：http://gfv.xziqi.cn

C#:   42.ToString()
来源：http://ins.daria6918.cn

[A08] 取整与四舍五入
来源：http://udt.yj20258888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oep.sjlbkw.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tim.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hpm.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ukv.zhixingplan.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sdm.ydjk.org.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dwj.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://bjx.andypj.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://klv.hesvh.cn

[A09] 绝对值与最大最小值
来源：http://iyr.snrcjt.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ykd.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wym.zhaomingkeji.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aea.gotoacloud.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aqx.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zzv.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ppz.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aln.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ssc.shangyingyoupin.top

[A10] 生成随机数
来源：http://gfz.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://xxi.redwolf501.top

PHP:  random_int(1, 100);
来源：http://eet.sxryk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zyn.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://srq.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://dzc.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zad.xylfe.cn

Ruby: rand(1..100)
来源：http://bjp.gogol.net.cn

C#:   new Random().Next(1, 101)
来源：http://ypi.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://nbn.yueranfly.top

Py:   "yes" if x > 0 else "no"
来源：http://irx.uphjek.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://zzt.tanke756.top

JS:   x > 0 ? "yes" : "no"
来源：http://qrl.chenjidiqi.icu

TS:   x > 0 ? "yes" : "no"
来源：http://jpv.jyoumei.cn

Java: x > 0 ? "yes" : "no"
来源：http://cpp.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xrb.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rta.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://mcu.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://qfb.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://heq.xylfe.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://stc.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://way.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://fhw.fengsongda.top

Java: "Hello, %s!".formatted(name)
来源：http://xga.sysykeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eof.yj20258888.top

Ruby: "Hello, #{name}!"
来源：http://pcy.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://ymo.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vka.tarul.cn

Py:   "第一行\n第二行"
来源：http://hqo.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://ews.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://txc.aizwys.cn

TS:   "第一行\n第二行"
来源：http://aha.bbcook.cn

Java: "第一行\n第二行"
来源：http://eal.mhx1999.top

Go:   "第一行\n第二行"
来源：http://jgb.ivvv.top

Ruby: "第一行\n第二行"
来源：http://too.zycfv.cn

C#:   "第一行\n第二行"
来源：http://jcv.jianghu66.top

[A14] 注释写法
来源：http://kys.shanyushiyangtech.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://grv.jqgufenzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://khz.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://mfl.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://rkn.smart0.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xsw.jinghuilouyu.cn

Go:   // 单行；/* 多行 */
来源：http://xlx.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://saj.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://mqv.pycfn.com

[A15] 空值判断与默认值
来源：http://sfa.yangfankeji.com

Py:   value = data or "默认值"
来源：http://gfj.ppjwa.cn

PHP:  $value = $data ?? "默认值";
来源：http://uuf.vqdsnc.cn

JS:   const value = data ?? "默认值";
来源：http://whp.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://nnc.haohaochexian.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xyl.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://ifd.redwolf501.top

Ruby: value = data || "默认值"
来源：http://buw.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://qgr.jianghu66.top

[A16] 真假值判断规则
来源：http://nuw.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vrf.birdmap.top


<!-- 参考信息 -->