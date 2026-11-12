代发 wailian999

[U105] JS：节流
来源：http://tfw.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uqn.uphjek.com

[U106] JS：日期格式化
来源：http://txc.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uid.snrcjt.cn

[U107] JS：数字千分位
来源：http://tpo.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yen.hongshengwenyu.top

[U108] JS：随机整数
来源：http://ngi.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oer.chenjidiqi.icu

[U109] JS：数组分组
来源：http://jye.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://wca.guowangkeji.top

[U110] JS：数组分块
来源：http://sld.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hoh.9152youxi.cn

[U111] JS：对象转 Map
来源：http://cok.andypj.xyz

new Map(Object.entries(obj))
来源：http://inx.yonumen.top

[U112] JS：字符串补位
来源：http://esb.jianghu66.top

"7".padStart(3, "0")
来源：http://mze.hesvh.cn

[U113] JS：正则替换全部
来源：http://cji.zhengqikj.top

s.replaceAll("a", "b")
来源：http://pqi.sxryk.cn

[U114] JS：JSON 深比较
来源：http://vul.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rni.xinyue.icu

[U115] JS：生成 UUID
来源：http://boi.cheryme.top

crypto.randomUUID()
来源：http://ail.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://abi.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://obv.dianchejie.cn

[U117] JS：单元测试
来源：http://fgf.pycfn.com

npm i -D vitest;  npx vitest
来源：http://dyb.tian-w.cn

[U118] JS：开发服务器
来源：http://wjq.jiagoushi.top

npm i -D vite;  npx vite
来源：http://equ.quarkkingdee.top

[U119] JS：生产构建
来源：http://uid.52xcode.cn

npx vite build
来源：http://zya.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://sgo.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://dte.shangyingyoupin.top

================================================================================
来源：http://rer.zhoulong.xyz

统计汇总
来源：http://qnl.ydzc1.top

================================================================================
来源：http://plj.ppjwa.cn

按语言统计（条）：
来源：http://oea.wangshuangyany.cn

Python ......... 252
来源：http://odr.iojbl.cn

PHP ............ 252
来源：http://qmj.316326.xyz

JavaScript ..... 252
来源：http://hbm.yj20258888.top

TypeScript ..... 212
来源：http://vci.zdbjq.cn

Java ........... 212
来源：http://mja.daxiang520.top

Go ............. 212
来源：http://jnm.0kj1m.cn

Ruby ........... 212
来源：http://qws.pycfn.com

C# ............. 212
来源：http://tow.mhx1999.top

C .............. 30
来源：http://vls.ydzc1.top

C++ ............ 30
来源：http://utj.zycfv.cn

SQL ............ 90
来源：http://fpw.yj20258.top

Bash ........... 80
来源：http://far.gzhubu.top

Kotlin ......... 15
来源：http://wfw.yuxming.cn

Swift .......... 15
来源：http://qca.dashuyun.cn

Lua ............ 10
来源：http://xlc.cdnleiting.top

Perl ........... 10
来源：http://ydg.pengpengdd.cyou

Scala .......... 10
来源：http://bmj.jqgufenzy.top

------------------------------------
来源：http://tzm.quarkkingdee.top

合计 ........... 2106 条
来源：http://pxu.zhengqikj.top

按章节统计：
来源：http://aqm.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rag.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uih.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gqg.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lph.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rua.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dhu.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qvs.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dzd.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fov.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cmh.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sqt.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://juo.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cnk.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zqg.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nni.andypj.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://asr.xuanzx.com

Q SQL 专题                              90
来源：http://vka.shanyushiyangtech.top

R Bash 专题                             80
来源：http://pid.yj202588.top

S C / C++ 专题                          60
来源：http://vtq.yonumen.top

T 其他语言补充                          60
来源：http://nyt.shuidangran.top

U 高频实用片段                         120
来源：http://olf.shanyushiyangkeji.top

------------------------------------
来源：http://dkg.fktsv.cn

合计                                  2106 条
来源：http://ekh.redwolf501.top

--------------------------------------------------------------------------------
来源：http://zob.xuanzx.com

使用提醒
来源：http://wvv.sysykeji.top

--------------------------------------------------------------------------------
来源：http://vwf.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oez.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rhx.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eqa.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hth.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bxd.tarul.cn

—— 文件结束 ——
来源：http://kso.epnwcf.com

================================================================================
来源：http://nkw.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://pew.yongpay.top

Common Programming Examples Cheat Book
来源：http://npy.ehwqpu.com

================================================================================
来源：http://crm.gogol.net.cn

【收录内容】
来源：http://mtx.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://lij.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ukb.quarkkingdee.top

SQL · Bash · C · C++
来源：http://lup.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jpg.zhoulong.xyz

【使用说明】
来源：http://aix.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ygj.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rvm.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bnx.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vra.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ouh.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://inm.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://whp.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dmu.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dvf.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bue.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jwi.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ckj.redwolf501.top

【文件统计】
来源：http://zzr.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ubw.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://uzx.jinqigfzy.top

目  录
来源：http://jiy.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://tir.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pzf.tian-w.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hqj.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wir.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qfq.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bkz.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ibs.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qoi.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qwp.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://snk.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jue.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qlh.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://owf.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://omi.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dga.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nsf.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ypy.yj202588.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tbj.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://exv.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gxv.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fjn.fehbvm.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cey.guowangkeji.top

================================================================================
来源：http://uas.nanxinkj.top

A. 基础语法与类型
来源：http://dop.kuanghao11.cn

================================================================================
来源：http://cca.yonumen.top

[A01] Hello World
来源：http://ytt.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://phi.zdqjudy.top

PHP:  echo "Hello, World!";
来源：http://hvq.yj20258.top

JS:   console.log("Hello, World!");
来源：http://mtz.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eha.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://heb.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://oor.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://zoo.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hps.fktsv.cn

[A02] 变量声明与赋值
来源：http://ycm.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nsu.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ynx.epnwcf.com

JS:   let name = "Alex"; const age = 20;
来源：http://gcu.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gqg.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://ujb.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://bbz.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://mzv.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://tok.cdnleiting.top

[A03] 常量定义
来源：http://dkl.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jvz.cashguo.top

PHP:  const PI = 3.14159;
来源：http://byz.yj20258.top

JS:   const PI = 3.14159;
来源：http://uvm.316326.xyz

TS:   const PI: number = 3.14159;
来源：http://lpz.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://ssx.tanke756.top

Go:   const PI = 3.14159
来源：http://xvm.yfazqb.com

Ruby: PI = 3.14159
来源：http://zoh.jiagoushi.top

C#:   const double PI = 3.14159;
来源：http://jun.yueranfly.top

[A04] 判断变量类型
来源：http://lpp.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kbs.zdqjudy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iki.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cmz.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://liq.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ayd.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://upl.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sqs.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://jhp.jiagoushi.top

[A05] 整数除法与取模
来源：http://rmk.hfpthk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rmu.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bvn.hysaishi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qqv.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://agi.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://bpx.smart0.xyz

Go:   7 / 2; 7 % 2
来源：http://kjc.yj202588.top

Ruby: 7 / 2; 7 % 2
来源：http://qec.bbcook.cn

C#:   7 / 2; 7 % 2
来源：http://hza.yj202588.top

[A06] 字符串转数字
来源：http://dqp.jyoumei.cn

Py:   int("42"); float("3.14")
来源：http://gjg.fengsongda.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nxg.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hnc.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://jpp.ywan-chungtsiang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aks.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wtt.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tlu.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lkp.havefunace.top

[A07] 数字转字符串
来源：http://lfr.pycfn.com

Py:   str(42)
来源：http://hzu.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://wll.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://vtd.fanxiaobao.xyz

TS:   String(42)
来源：http://vfe.sweek.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nsm.jinyuanbaomall.cn

Go:   strconv.Itoa(42)
来源：http://koh.zhoulong.xyz

Ruby: 42.to_s
来源：http://rqr.shuidangran.top

C#:   42.ToString()
来源：http://pqe.yangfankeji.com

[A08] 取整与四舍五入
来源：http://fal.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tsj.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oxm.nanxuanxn.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lrz.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kwc.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ejj.jqgfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nbh.quarkkingdee.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pzt.yuanzhike.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hht.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://cvg.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rfm.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iyv.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cuz.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kyj.xinyue.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wmb.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nhx.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://flr.ydzc1.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fco.hywenlv.cn

[A10] 生成随机数
来源：http://rag.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://xmr.sxryk.cn

PHP:  random_int(1, 100);
来源：http://xoe.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://idr.guowangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eki.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://bwq.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vbf.svipenyu.cn

Ruby: rand(1..100)
来源：http://szp.uphjek.com

C#:   new Random().Next(1, 101)
来源：http://wgj.tarul.cn

[A11] 条件表达式（三元）
来源：http://odr.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://irc.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://sdq.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://kzj.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://vws.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://mpf.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gsd.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://igr.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qmr.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://upm.yanxiufei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://okh.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://abc.yj20258.top

JS:   `Hello, ${name}!`
来源：http://xhr.hywenlv.cn

TS:   `Hello, ${name}!`
来源：http://nod.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://bec.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pbb.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://cnt.hongshengwenyu.top

C#:   $"Hello, {name}!"
来源：http://epl.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ifw.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://krp.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://gcc.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://zjy.0kj1m.cn

TS:   "第一行\n第二行"
来源：http://nix.jlsjyb.cn

Java: "第一行\n第二行"
来源：http://wsi.ydzc1.top

Go:   "第一行\n第二行"
来源：http://yte.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://ncu.hnqzz.top

C#:   "第一行\n第二行"
来源：http://kzl.fanxiaobao.xyz

[A14] 注释写法
来源：http://lmq.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qhs.hongshengwenyu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://too.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://skv.shanyushiyangkeji.top

TS:   // 单行；/* 多行 */
来源：http://zlj.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ksc.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://pct.chenjidiqi.icu

Ruby: # 单行；=begin 多行 =end
来源：http://ygq.xziqi.cn

C#:   // 单行；/* 多行 */
来源：http://zog.tarul.cn

[A15] 空值判断与默认值
来源：http://wgk.snrcjt.cn

Py:   value = data or "默认值"
来源：http://ugr.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://wvx.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://fdj.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://tzj.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gsr.ppjwa.cn

Go:   if data == "" { data = "默认值" }
来源：http://szy.vehdjk.com

Ruby: value = data || "默认值"
来源：http://agj.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://wfc.svipenyu.cn

[A16] 真假值判断规则
来源：http://gjs.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fif.yanxiufei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jbl.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rnn.daria6918.cn

TS:   if (!x) {}
来源：http://vuy.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hce.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hqj.wangdashe.top

Ruby: unless x            # nil 与 false 为假
来源：http://shz.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pqf.jinyuanbaomall.cn

[A17] 位运算
来源：http://xpl.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oop.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ozt.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwq.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cbl.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://poq.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uju.dianchejie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uft.vqdsnc.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ycz.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://eah.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://ogm.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://ife.aibaodan.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kfv.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ecd.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://rbu.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rmx.daxiang520.top

Ruby: "A".ord; 65.chr
来源：http://uxx.andypj.xyz


<!-- 参考信息 -->