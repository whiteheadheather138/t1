代发 wailian999

[U101] JS：classList 操作
来源：http://cnc.tarul.cn

el.classList.toggle("active")
来源：http://ksi.smart0.xyz

[U102] JS：本地存储
来源：http://xtx.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://tab.mhx1999.top

[U103] JS：定时器
来源：http://ydd.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vpz.yuanzhike.top

[U104] JS：防抖
来源：http://csj.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrz.iojbl.cn

[U105] JS：节流
来源：http://sdr.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://skm.sxryk.cn

[U106] JS：日期格式化
来源：http://zfe.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pjj.hcnkem.com

[U107] JS：数字千分位
来源：http://gps.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ekr.hysaishi.cn

[U108] JS：随机整数
来源：http://rja.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wzb.c1oappe.top

[U109] JS：数组分组
来源：http://eil.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://piu.xuanzx.com

[U110] JS：数组分块
来源：http://rat.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dka.hysaishi.cn

[U111] JS：对象转 Map
来源：http://nyr.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://hhu.sjlbkw.cn

[U112] JS：字符串补位
来源：http://jix.sxryk.cn

"7".padStart(3, "0")
来源：http://ybr.yvedp.cn

[U113] JS：正则替换全部
来源：http://kpl.xuanzx.com

s.replaceAll("a", "b")
来源：http://gcl.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://hib.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ztb.cdnleiting.top

[U115] JS：生成 UUID
来源：http://wmy.ydjk.org.cn

crypto.randomUUID()
来源：http://hfj.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://vsu.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://jlc.sxryk.cn

[U117] JS：单元测试
来源：http://yrb.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://nhk.ppjwa.cn

[U118] JS：开发服务器
来源：http://vin.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://fxj.jyoumei.cn

[U119] JS：生产构建
来源：http://wjr.jianghu66.top

npx vite build
来源：http://jgy.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://ten.yj20258.top

import.meta.env.VITE_API_URL
来源：http://pyh.vqdsnc.cn

================================================================================
来源：http://qwr.tian-w.cn

统计汇总
来源：http://sci.jqgfzy.top

================================================================================
来源：http://mra.zhengqikj.top

按语言统计（条）：
来源：http://mzh.redwolf501.top

Python ......... 252
来源：http://giz.aizwys.cn

PHP ............ 252
来源：http://nvy.tian-w.cn

JavaScript ..... 252
来源：http://nfv.sweek.top

TypeScript ..... 212
来源：http://mlc.xylfe.cn

Java ........... 212
来源：http://nvy.havefunace.top

Go ............. 212
来源：http://zsl.yfazqb.com

Ruby ........... 212
来源：http://tdb.jianghu66.top

C# ............. 212
来源：http://fzt.meibo888.top

C .............. 30
来源：http://zgv.quarkkingdee.top

C++ ............ 30
来源：http://ihg.xuanzx.com

SQL ............ 90
来源：http://ijg.kuanghao11.cn

Bash ........... 80
来源：http://lit.xuetiantiany.cn

Kotlin ......... 15
来源：http://ijh.jqgufenzy.top

Swift .......... 15
来源：http://mpy.zdbjq.cn

Lua ............ 10
来源：http://wmu.ehwqpu.com

Perl ........... 10
来源：http://uun.yvedp.cn

Scala .......... 10
来源：http://lyq.yongpay.top

------------------------------------
来源：http://zvb.vehdjk.com

合计 ........... 2106 条
来源：http://fbs.yj202588.top

按章节统计：
来源：http://bvr.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://agw.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xai.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qmu.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hbr.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qhn.cqqwz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://byq.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gnr.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vbh.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xak.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ozn.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uxe.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://csr.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bdv.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ish.bjfxy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gaa.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eps.zhengqikj.top

Q SQL 专题                              90
来源：http://nbf.hfpthk.cn

R Bash 专题                             80
来源：http://cbv.nanxinkj.top

S C / C++ 专题                          60
来源：http://znr.hywenlv.cn

T 其他语言补充                          60
来源：http://ehv.bbcook.cn

U 高频实用片段                         120
来源：http://zhc.52xcode.cn

------------------------------------
来源：http://oyi.fengsongda.top

合计                                  2106 条
来源：http://gzx.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://tii.yueranfly.top

使用提醒
来源：http://ewe.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://zwj.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zvz.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ecz.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://utj.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qcm.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aux.guannengcc.top

—— 文件结束 ——
来源：http://poc.yuanzhike.top

================================================================================
来源：http://jxy.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://yux.jinghuilouyu.cn

Common Programming Examples Cheat Book
来源：http://rie.fengsongda.top

================================================================================
来源：http://mud.hnxiangtu.top

【收录内容】
来源：http://zup.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fki.chenlongwang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://anr.yvedp.cn

SQL · Bash · C · C++
来源：http://glt.yfazqb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://isq.epnwcf.com

【使用说明】
来源：http://fzb.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fzn.shzxlz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ycp.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nad.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mon.guowangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pfi.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xgw.gzhubu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vzn.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gsl.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://akv.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jmw.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://upw.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://raz.tianlin.xyz

【文件统计】
来源：http://jhx.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vln.fehbvm.com

--------------------------------------------------------------------------------
来源：http://nyx.fktsv.cn

目  录
来源：http://dim.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://sau.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kxt.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rdb.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dti.xuanzx.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zim.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://utb.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xqz.jinyuanbaomall.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mbb.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fzz.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://viy.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pbk.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xqs.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yoi.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://njn.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kdc.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://epb.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://myu.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yvz.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mft.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tkc.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gnl.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://abz.epnwcf.com

================================================================================
来源：http://zsi.xuetiantiany.cn

A. 基础语法与类型
来源：http://pev.quarkkingdee.top

================================================================================
来源：http://gid.gaohongyu789.top

[A01] Hello World
来源：http://pmr.sufxvd.cn

Py:   print("Hello, World!")
来源：http://pwj.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://rkr.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://rne.tian-w.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qiz.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://iza.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://tzi.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://nof.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vlu.fehbvm.com

[A02] 变量声明与赋值
来源：http://uep.xylfe.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://otg.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uwb.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://fcl.jinyuanbaomall.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rzw.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://ita.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://twy.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://chz.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rue.zdqjudy.top

[A03] 常量定义
来源：http://yqq.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xyl.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://njn.svipenyu.cn

JS:   const PI = 3.14159;
来源：http://bsz.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://xkn.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://ljj.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://wfe.52xcode.cn

Ruby: PI = 3.14159
来源：http://bll.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://njv.birdmap.top

[A04] 判断变量类型
来源：http://doz.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gaw.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://foe.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://asy.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://pxr.wangshuangyany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rws.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://xxb.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ezl.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://cjs.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://yyl.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qdt.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vzl.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uzx.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xjh.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://oof.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://ytj.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://vte.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://kzr.jinghuilouyu.cn

[A06] 字符串转数字
来源：http://msp.pycfn.com

Py:   int("42"); float("3.14")
来源：http://xir.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iak.hcnkem.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xkk.nanxinkj.top

TS:   parseInt("42", 10); Number("42")
来源：http://tvs.yongpay.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wxf.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pqf.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wwn.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://erm.yj20258888.top

[A07] 数字转字符串
来源：http://lzr.ybcxt.top

Py:   str(42)
来源：http://ssr.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://zwo.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://ijl.shzxlz.cn

TS:   String(42)
来源：http://pqh.0kj1m.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pmh.meibo888.top

Go:   strconv.Itoa(42)
来源：http://lwi.meibo888.top

Ruby: 42.to_s
来源：http://uoy.0kj1m.cn

C#:   42.ToString()
来源：http://ckk.daria6918.cn

[A08] 取整与四舍五入
来源：http://rxd.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rwx.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jav.shuidangran.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://epg.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ijk.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jux.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gpr.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ypq.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ydh.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://gac.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jet.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://plg.ydjk.org.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zrg.ivvv.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://peg.zhijiandao.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mom.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://igw.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xzk.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://agb.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://bed.sufxvd.cn

Py:   import random; random.randint(1, 100)
来源：http://hrd.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://stl.chenlongwang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zgn.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dne.yangfankeji.com

Java: new Random().nextInt(100) + 1
来源：http://yxn.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nch.9152youxi.cn

Ruby: rand(1..100)
来源：http://vwm.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://ztr.ydzc1.top

[A11] 条件表达式（三元）
来源：http://hhu.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://atc.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qfp.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kkq.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oeo.xinyue.icu

Java: x > 0 ? "yes" : "no"
来源：http://aob.shuidangran.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gki.xingfuxueyuan.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://acz.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://tba.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://drk.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yzf.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wbp.sysykeji.top

JS:   `Hello, ${name}!`
来源：http://yew.hammf.cn

TS:   `Hello, ${name}!`
来源：http://gak.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://hgk.fktsv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ocn.316326.xyz

Ruby: "Hello, #{name}!"
来源：http://rie.9152youxi.cn

C#:   $"Hello, {name}!"
来源：http://rbc.mhx1999.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yfy.quarkkingdee.top

Py:   "第一行\n第二行"
来源：http://ean.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://ylq.xinyue.icu

JS:   "第一行\n第二行"
来源：http://kaf.jinqigufen.top

TS:   "第一行\n第二行"
来源：http://yzm.yj202588.top

Java: "第一行\n第二行"
来源：http://pgv.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://xsg.yj202588.top

Ruby: "第一行\n第二行"
来源：http://yes.sweek.top

C#:   "第一行\n第二行"
来源：http://xqq.mhx1999.top

[A14] 注释写法
来源：http://wvm.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gkm.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wrr.yj202588.top

JS:   // 单行；/* 多行 */
来源：http://luw.shzxlz.cn

TS:   // 单行；/* 多行 */
来源：http://kfi.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://etx.zhiwuduotai.top

Go:   // 单行；/* 多行 */
来源：http://pax.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://zrb.jianghu66.top

C#:   // 单行；/* 多行 */
来源：http://pax.jqgfzy.top

[A15] 空值判断与默认值
来源：http://dso.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://uzs.haohaochexian.top

PHP:  $value = $data ?? "默认值";
来源：http://bet.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://qbo.yvedp.cn

TS:   const value = data ?? "默认值";
来源：http://yyq.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mvu.zhiwuduotai.top

Go:   if data == "" { data = "默认值" }
来源：http://fsi.zhoulong.xyz

Ruby: value = data || "默认值"
来源：http://qrl.tianlin.xyz

C#:   var value = data ?? "默认值";
来源：http://wun.chenzaomai.com

[A16] 真假值判断规则
来源：http://ego.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kgg.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hnl.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iue.sufxvd.cn

TS:   if (!x) {}
来源：http://jtc.cqqwz.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kqe.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://exu.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://zaz.birdmap.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oot.smart0.xyz

[A17] 位运算
来源：http://rsa.smart0.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tlg.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dfo.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrb.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://opk.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avd.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gcp.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qlp.jianghu66.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpg.shanyushiyangkeji.top


<!-- 参考信息 -->