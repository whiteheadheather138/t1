代发 wailian999

[U103] JS：定时器
来源：http://zbo.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lya.hcnkem.com

[U104] JS：防抖
来源：http://qjq.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://att.yangfankeji.com

[U105] JS：节流
来源：http://pky.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nte.daxiang520.top

[U106] JS：日期格式化
来源：http://hwy.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uuw.dianchejie.cn

[U107] JS：数字千分位
来源：http://nmm.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ndw.gogol.net.cn

[U108] JS：随机整数
来源：http://dwj.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lap.ybcxt.top

[U109] JS：数组分组
来源：http://pij.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://ctv.dianchejie.cn

[U110] JS：数组分块
来源：http://koe.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://prj.daxiang520.top

[U111] JS：对象转 Map
来源：http://sxn.jianghu66.top

new Map(Object.entries(obj))
来源：http://mah.shuidangran.top

[U112] JS：字符串补位
来源：http://mmy.pengpengdd.cyou

"7".padStart(3, "0")
来源：http://qiv.yongpay.top

[U113] JS：正则替换全部
来源：http://oub.bjfxy.top

s.replaceAll("a", "b")
来源：http://eoa.yonumen.top

[U114] JS：JSON 深比较
来源：http://iil.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fmm.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://lyy.zdbjq.cn

crypto.randomUUID()
来源：http://qxe.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://yqb.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://xpq.yj20258888.top

[U117] JS：单元测试
来源：http://tzx.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://zah.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://nxw.xinyue.icu

npm i -D vite;  npx vite
来源：http://ten.hysaishi.cn

[U119] JS：生产构建
来源：http://sya.yuxming.cn

npx vite build
来源：http://hqw.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://pyq.pycfn.com

import.meta.env.VITE_API_URL
来源：http://vbu.nwbrower.top

================================================================================
来源：http://dmv.jinqigufen.top

统计汇总
来源：http://gaf.52xcode.cn

================================================================================
来源：http://rsu.uphjek.com

按语言统计（条）：
来源：http://gmq.nanxinkj.top

Python ......... 252
来源：http://ufq.ydjk.org.cn

PHP ............ 252
来源：http://sxy.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://wjc.sweek.top

TypeScript ..... 212
来源：http://ujs.tianlin.xyz

Java ........... 212
来源：http://dni.kuanghao11.cn

Go ............. 212
来源：http://dji.kuanghao11.cn

Ruby ........... 212
来源：http://njj.hywenlv.cn

C# ............. 212
来源：http://von.xuanzx.com

C .............. 30
来源：http://zor.tanke756.top

C++ ............ 30
来源：http://eoy.9152youxi.cn

SQL ............ 90
来源：http://adx.ppjwa.cn

Bash ........... 80
来源：http://ail.zhoulong.xyz

Kotlin ......... 15
来源：http://zzy.shanyushiyangkeji.top

Swift .......... 15
来源：http://zfy.zhiwuduotai.top

Lua ............ 10
来源：http://ebl.bjfxy.top

Perl ........... 10
来源：http://vjb.zdbjq.cn

Scala .......... 10
来源：http://goj.jlsjyb.cn

------------------------------------
来源：http://xmg.yueranfly.top

合计 ........... 2106 条
来源：http://stv.sxryk.cn

按章节统计：
来源：http://awh.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sja.daxiang520.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tsf.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mhj.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hej.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oiv.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uoh.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cor.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bkk.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tgg.kuanghao11.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ghz.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wef.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xym.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://plh.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ilq.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kwt.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://afu.ydjk.org.cn

Q SQL 专题                              90
来源：http://efe.sjlbkw.cn

R Bash 专题                             80
来源：http://thw.jianghu66.top

S C / C++ 专题                          60
来源：http://hyi.hesvh.cn

T 其他语言补充                          60
来源：http://cek.sweek.top

U 高频实用片段                         120
来源：http://vwi.snrcjt.cn

------------------------------------
来源：http://zax.ppjwa.cn

合计                                  2106 条
来源：http://ynf.sxryk.cn

--------------------------------------------------------------------------------
来源：http://lye.uphjek.com

使用提醒
来源：http://qre.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://clz.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gue.xylfe.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pbh.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rud.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lwj.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://edh.shangyingyoupin.top

—— 文件结束 ——
来源：http://wip.gaohongyu789.top

================================================================================
来源：http://spz.havefunace.top

程序语言常见例子速查手册（2024 版）
来源：http://gem.fengsongda.top

Common Programming Examples Cheat Book
来源：http://npz.xuetiantiany.cn

================================================================================
来源：http://isc.nanxinkj.top

【收录内容】
来源：http://qis.yfazqb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://fgt.fengsongda.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tfo.cdnleiting.top

SQL · Bash · C · C++
来源：http://fpn.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ypy.0kj1m.cn

【使用说明】
来源：http://zot.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://umx.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xwo.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wnq.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ztc.tarul.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yoj.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wck.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wbz.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ffz.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yjo.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gys.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pmz.yanxiufei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gcz.yonumen.top

【文件统计】
来源：http://iwg.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://teb.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://ivv.andypj.xyz

目  录
来源：http://jrl.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ylx.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kbo.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tei.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vwa.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cax.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://swf.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://twj.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ihs.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ygk.hywenlv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uhq.wangdashe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lmt.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://axi.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ykj.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hcj.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oth.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uon.yj20258888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hyp.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jgn.ivvv.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bwy.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://emz.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kio.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oqv.jinghuilouyu.cn

================================================================================
来源：http://jay.yfazqb.com

A. 基础语法与类型
来源：http://bry.hnqzz.top

================================================================================
来源：http://ird.yj20258888.top

[A01] Hello World
来源：http://zlm.xylfe.cn

Py:   print("Hello, World!")
来源：http://xks.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://nop.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://gti.hysaishi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eqr.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://esi.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://eqr.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://pfq.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://gsk.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://wdf.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nqg.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tbr.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jdw.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://edu.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://hsg.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://dma.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://uwx.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://jvl.shanyushiyangtech.top

[A03] 常量定义
来源：http://phx.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://isb.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://nfq.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://bsh.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://iuv.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://mcr.hfpthk.cn

Go:   const PI = 3.14159
来源：http://gls.redwolf501.top

Ruby: PI = 3.14159
来源：http://cmz.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://pyc.uphjek.com

[A04] 判断变量类型
来源：http://ptk.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ixc.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wva.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kpb.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://fvg.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ivz.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://obq.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tcb.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://odn.aibaodan.cn

[A05] 整数除法与取模
来源：http://laf.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zav.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hgq.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sad.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hmt.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://vro.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://jom.shangyingyoupin.top

Ruby: 7 / 2; 7 % 2
来源：http://toz.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://amy.zhaomingkeji.xyz

[A06] 字符串转数字
来源：http://esg.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://bcc.jinqigfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ypi.meibo888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blt.feifeiyinyue.top

TS:   parseInt("42", 10); Number("42")
来源：http://bsl.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://epr.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nmm.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ofx.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nss.9152youxi.cn

[A07] 数字转字符串
来源：http://zdo.yuanzhike.top

Py:   str(42)
来源：http://otz.jianghu66.top

PHP:  (string) 42; strval(42)
来源：http://geb.jiagoushi.top

JS:   String(42); (42).toString()
来源：http://iss.fanxiaobao.xyz

TS:   String(42)
来源：http://yko.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://fxc.daria6918.cn

Go:   strconv.Itoa(42)
来源：http://lzk.ywan-chungtsiang.top

Ruby: 42.to_s
来源：http://jyb.xuanzx.com

C#:   42.ToString()
来源：http://vnu.hcnkem.com

[A08] 取整与四舍五入
来源：http://ntb.jinqigufen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ihi.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qdt.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bfc.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nhn.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kft.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://slm.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fpp.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tal.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://qos.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sjz.yueranfly.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://glw.hywenlv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sht.ydzc1.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vct.smart0.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rfo.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lcb.cheryme.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pzz.gaohongyu789.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lse.zhijiandao.cn

[A10] 生成随机数
来源：http://jwc.jiagoushi.top

Py:   import random; random.randint(1, 100)
来源：http://tyx.xuetiantiany.cn

PHP:  random_int(1, 100);
来源：http://iws.gotoacloud.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rkh.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bzf.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://pyw.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ngp.dianchejie.cn

Ruby: rand(1..100)
来源：http://wug.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://myd.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://owh.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://abt.jinqigfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://cue.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://eiy.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://agp.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://khx.chenjidiqi.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://gli.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mvi.xziqi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uvd.shanyushiyangkeji.top

[A12] 字符串插值 / 格式化
来源：http://rtp.iojbl.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ycd.fzhhl.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jxz.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://rfk.vqdsnc.cn

TS:   `Hello, ${name}!`
来源：http://ync.tianlin.xyz

Java: "Hello, %s!".formatted(name)
来源：http://qia.fzhhl.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qlk.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://jkn.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://qfx.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cdt.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://fld.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://jru.havefunace.top

JS:   "第一行\n第二行"
来源：http://nam.aizwys.cn

TS:   "第一行\n第二行"
来源：http://knb.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://ryy.andypj.xyz

Go:   "第一行\n第二行"
来源：http://fnf.tian-w.cn

Ruby: "第一行\n第二行"
来源：http://vav.hywenlv.cn

C#:   "第一行\n第二行"
来源：http://qtv.snrcjt.cn

[A14] 注释写法
来源：http://byr.ctjpmb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://vdr.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xod.redwolf501.top

JS:   // 单行；/* 多行 */
来源：http://tdb.tian-w.cn

TS:   // 单行；/* 多行 */
来源：http://chq.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wua.fengsongda.top

Go:   // 单行；/* 多行 */
来源：http://jwc.dianchejie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fmg.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://yil.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://dfc.sweek.top

Py:   value = data or "默认值"
来源：http://lja.316326.xyz

PHP:  $value = $data ?? "默认值";
来源：http://iyr.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://uij.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://nvw.jianghu66.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qda.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://ujw.tanke756.top

Ruby: value = data || "默认值"
来源：http://zzb.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://aiw.gogol.net.cn

[A16] 真假值判断规则
来源：http://qvv.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://buh.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://brb.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vlw.fzhhl.top

TS:   if (!x) {}
来源：http://vsx.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xlk.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://roy.yj20258888.top

Ruby: unless x            # nil 与 false 为假
来源：http://qky.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uil.sysykeji.top

[A17] 位运算
来源：http://svm.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rlr.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://byh.bjfxy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzv.kuanghao11.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tdb.zhiwuduotai.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://him.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tsw.yj20258.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ycb.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ghj.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://vfn.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://pdu.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://hpf.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://emb.snrcjt.cn


<!-- 参考信息 -->