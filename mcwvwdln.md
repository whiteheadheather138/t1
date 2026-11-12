代发 wailian999

[U101] JS：classList 操作
来源：http://rvv.jinqigufen.top

el.classList.toggle("active")
来源：http://hrc.sjlbkw.cn

[U102] JS：本地存储
来源：http://qwy.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eoj.yfazqb.com

[U103] JS：定时器
来源：http://sey.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uip.wangdashe.top

[U104] JS：防抖
来源：http://msx.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pnr.xylfe.cn

[U105] JS：节流
来源：http://xjm.jinyuanbaomall.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nry.andypj.xyz

[U106] JS：日期格式化
来源：http://imy.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zzt.cashguo.top

[U107] JS：数字千分位
来源：http://mjc.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ogp.daxiang520.top

[U108] JS：随机整数
来源：http://dhd.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qyk.chenlongwang.top

[U109] JS：数组分组
来源：http://mze.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://mfe.jinqigufen.top

[U110] JS：数组分块
来源：http://dyi.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://you.yfazqb.com

[U111] JS：对象转 Map
来源：http://clv.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://zdz.gzhubu.top

[U112] JS：字符串补位
来源：http://vzr.hywenlv.cn

"7".padStart(3, "0")
来源：http://oem.snrcjt.cn

[U113] JS：正则替换全部
来源：http://qyo.snrcjt.cn

s.replaceAll("a", "b")
来源：http://fes.daxiang520.top

[U114] JS：JSON 深比较
来源：http://hnb.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nuq.hesvh.cn

[U115] JS：生成 UUID
来源：http://zey.zhijiandao.cn

crypto.randomUUID()
来源：http://qaf.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://mqn.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://htm.zhengqikj.top

[U117] JS：单元测试
来源：http://vvk.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://jcq.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://tgr.daxiang520.top

npm i -D vite;  npx vite
来源：http://xea.wangshuangyany.cn

[U119] JS：生产构建
来源：http://oet.yuanzhike.top

npx vite build
来源：http://wbb.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://yuo.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://vpp.0kj1m.cn

================================================================================
来源：http://yun.fzhhl.top

统计汇总
来源：http://oll.tanke756.top

================================================================================
来源：http://dbv.shuidangran.top

按语言统计（条）：
来源：http://ybe.zhijiandao.cn

Python ......... 252
来源：http://nmb.zhiwuduotai.top

PHP ............ 252
来源：http://ftx.cdnleiting.top

JavaScript ..... 252
来源：http://oyf.dashuyun.cn

TypeScript ..... 212
来源：http://vyo.fanxiaobao.xyz

Java ........... 212
来源：http://eos.hywenlv.cn

Go ............. 212
来源：http://ksf.snrcjt.cn

Ruby ........... 212
来源：http://tsx.xingfuxueyuan.xyz

C# ............. 212
来源：http://caa.jianghu66.top

C .............. 30
来源：http://son.sysykeji.top

C++ ............ 30
来源：http://goy.yj202588.top

SQL ............ 90
来源：http://vym.chenjidiqi.icu

Bash ........... 80
来源：http://gxj.wangshuangyany.cn

Kotlin ......... 15
来源：http://tgk.bbcook.cn

Swift .......... 15
来源：http://pkm.hnqzz.top

Lua ............ 10
来源：http://fgk.shanyushiyangtech.top

Perl ........... 10
来源：http://bml.hesvh.cn

Scala .......... 10
来源：http://tbi.gaohongyu789.top

------------------------------------
来源：http://avo.cucudq.cn

合计 ........... 2106 条
来源：http://khx.hnqzz.top

按章节统计：
来源：http://vgf.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tjj.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wzk.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jma.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qgq.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bgu.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tma.tanke756.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://phr.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ock.redwolf501.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xnl.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ljr.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mck.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ise.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fxe.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nju.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sww.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ute.jinqigfzy.top

Q SQL 专题                              90
来源：http://khd.ybcxt.top

R Bash 专题                             80
来源：http://uuz.cheryme.top

S C / C++ 专题                          60
来源：http://ady.zhaomingkeji.xyz

T 其他语言补充                          60
来源：http://ivj.zhongyouzk.top

U 高频实用片段                         120
来源：http://dti.yj202588.top

------------------------------------
来源：http://bfn.hysaishi.cn

合计                                  2106 条
来源：http://cgv.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://kuh.meibo888.top

使用提醒
来源：http://ute.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://xvs.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xoq.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://etn.zycfv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://roi.sjlbkw.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yvk.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vrw.fengsongda.top

—— 文件结束 ——
来源：http://mzg.hongshengwenyu.top

================================================================================
来源：http://kgl.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://ixi.yvedp.cn

Common Programming Examples Cheat Book
来源：http://xyp.cashguo.top

================================================================================
来源：http://jix.jyoumei.cn

【收录内容】
来源：http://pjz.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tla.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mho.sufxvd.cn

SQL · Bash · C · C++
来源：http://tjz.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kau.yueranfly.top

【使用说明】
来源：http://iad.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://led.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lpb.chenzaomai.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eye.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oas.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qml.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hhd.vehdjk.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nnv.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://whr.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://emd.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ine.yongpay.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pwq.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oko.meibo888.top

【文件统计】
来源：http://jtk.jlsjyb.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gqc.nwbrower.top

--------------------------------------------------------------------------------
来源：http://ulh.cucudq.cn

目  录
来源：http://dtj.c1oappe.top

--------------------------------------------------------------------------------
来源：http://lsv.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yrc.vehdjk.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aqq.shzxlz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zwy.yvedp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hwz.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jfr.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rqk.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cfa.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ttc.chenlongwang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ysq.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yon.ywan-chungtsiang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://muy.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qji.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bcj.yanxiufei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ege.jinghuilouyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://shh.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zrj.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jyi.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wef.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yws.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nko.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pei.jinqigfzy.top

================================================================================
来源：http://uiu.fehbvm.com

A. 基础语法与类型
来源：http://tsm.52xcode.cn

================================================================================
来源：http://hcd.shuidangran.top

[A01] Hello World
来源：http://luv.svipenyu.cn

Py:   print("Hello, World!")
来源：http://mqe.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://ydq.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://ply.ydzc1.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kbd.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://vmf.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://acs.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://aar.jqgufenzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mjz.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://mvb.hnxiangtu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jka.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lfy.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://sbs.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://omm.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://lqw.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://vjp.wangdashe.top

Ruby: name = "Alex"; age = 20
来源：http://ikq.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://dbp.ywan-chungtsiang.top

[A03] 常量定义
来源：http://mtx.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pow.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://vfe.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://emm.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://lvu.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://rlv.xuetiantiany.cn

Go:   const PI = 3.14159
来源：http://fgi.yangfankeji.com

Ruby: PI = 3.14159
来源：http://qjh.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://ekv.zhaomingkeji.xyz

[A04] 判断变量类型
来源：http://mve.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dhf.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hzt.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sbz.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://axo.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uiq.tanke756.top

Go:   reflect.TypeOf(x).Name()
来源：http://ohy.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ekm.iojbl.cn

C#:   x.GetType().Name; x is int
来源：http://rqd.nanxinkj.top

[A05] 整数除法与取模
来源：http://pqt.cheryme.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zts.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dwg.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wvz.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rem.yuxming.cn

Java: 7 / 2; 7 % 2
来源：http://oon.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://rrn.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://plj.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://jvo.ydjk.org.cn

[A06] 字符串转数字
来源：http://gjr.uphjek.com

Py:   int("42"); float("3.14")
来源：http://aig.bbcook.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dzb.yonumen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gjp.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kqm.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://stb.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pyz.aibaodan.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://moi.jqgufenzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bgt.yj202588.top

[A07] 数字转字符串
来源：http://wue.cashguo.top

Py:   str(42)
来源：http://mdk.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://aqd.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://yur.xylfe.cn

TS:   String(42)
来源：http://ttc.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://wlc.guannengcc.top

Go:   strconv.Itoa(42)
来源：http://zfa.hywenlv.cn

Ruby: 42.to_s
来源：http://uwn.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://uii.sxryk.cn

[A08] 取整与四舍五入
来源：http://rde.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zco.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sjl.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qfy.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yua.yonumen.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uhj.jinyuanbaomall.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tnz.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zjc.zycfv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://glz.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://anx.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yrq.jinqigufen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dpo.zdqjudy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nqq.tanke756.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lhl.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yts.cheryme.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yuw.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://njg.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baq.dashuyun.cn

[A10] 生成随机数
来源：http://jjj.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://geg.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://iqw.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lqk.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mwn.zhongyouzk.top

Java: new Random().nextInt(100) + 1
来源：http://bnp.yuanzhike.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eqp.zhaomingkeji.xyz

Ruby: rand(1..100)
来源：http://psh.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://lqw.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://jwt.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://jqm.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nso.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://jaw.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rgd.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://zds.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://unq.quarkkingdee.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tap.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://xti.cdnleiting.top

[A12] 字符串插值 / 格式化
来源：http://uyb.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://olc.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bbc.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://fld.bjfxy.top

TS:   `Hello, ${name}!`
来源：http://ull.gogol.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://sfa.zhaomingkeji.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://koc.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://ttf.tianlin.xyz

C#:   $"Hello, {name}!"
来源：http://bwy.gzhubu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xao.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://knt.meibo888.top

PHP:  "第一行\n第二行"
来源：http://fel.zhoulong.xyz

JS:   "第一行\n第二行"
来源：http://fgr.fehbvm.com

TS:   "第一行\n第二行"
来源：http://frj.hysaishi.cn

Java: "第一行\n第二行"
来源：http://uru.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://qtz.hfpthk.cn

Ruby: "第一行\n第二行"
来源：http://rql.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://qhf.yongpay.top

[A14] 注释写法
来源：http://nuy.jlsjyb.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bok.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fnr.xuetiantiany.cn

JS:   // 单行；/* 多行 */
来源：http://qcb.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://pvm.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://flk.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://epb.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kvl.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://qrg.aizwys.cn

[A15] 空值判断与默认值
来源：http://uee.iojbl.cn

Py:   value = data or "默认值"
来源：http://ber.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://utz.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://bjk.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://fyf.nwbrower.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vjy.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://lbr.yuxming.cn

Ruby: value = data || "默认值"
来源：http://gjv.zdbjq.cn

C#:   var value = data ?? "默认值";
来源：http://zyj.yangfankeji.com

[A16] 真假值判断规则
来源：http://gyg.daria6918.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bgv.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zmp.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://egh.jlsjyb.cn

TS:   if (!x) {}
来源：http://phu.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mti.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qzt.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://eai.xuanzx.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jql.cheryme.top

[A17] 位运算
来源：http://mav.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://opk.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gvu.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lsx.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tft.ctjpmb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hyo.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fsh.xingfuxueyuan.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sks.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqy.chenjidiqi.icu


<!-- 参考信息 -->