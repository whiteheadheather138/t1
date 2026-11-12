代发 wailian999

[U105] JS：节流
来源：http://wcz.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ziw.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://tqo.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://frs.jlsjyb.cn

[U107] JS：数字千分位
来源：http://boc.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sjr.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://yzj.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rrh.shuidangran.top

[U109] JS：数组分组
来源：http://zvq.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://azi.jinyuanbaomall.cn

[U110] JS：数组分块
来源：http://tfh.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tbs.xinyue.icu

[U111] JS：对象转 Map
来源：http://xjw.sysykeji.top

new Map(Object.entries(obj))
来源：http://qid.zhijiandao.cn

[U112] JS：字符串补位
来源：http://elk.yangfankeji.com

"7".padStart(3, "0")
来源：http://jte.havefunace.top

[U113] JS：正则替换全部
来源：http://ela.ivvv.top

s.replaceAll("a", "b")
来源：http://ujz.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://zbn.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://jjw.fengsongda.top

[U115] JS：生成 UUID
来源：http://moj.yj20258888.top

crypto.randomUUID()
来源：http://crh.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://fqu.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://zny.yuxming.cn

[U117] JS：单元测试
来源：http://dom.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://mgr.guannengcc.top

[U118] JS：开发服务器
来源：http://iil.fktsv.cn

npm i -D vite;  npx vite
来源：http://rpm.vehdjk.com

[U119] JS：生产构建
来源：http://ntd.yangfankeji.com

npx vite build
来源：http://cul.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://mio.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://fmi.jqgufenzy.top

================================================================================
来源：http://hbs.xziqi.cn

统计汇总
来源：http://imc.sysykeji.top

================================================================================
来源：http://ztw.zdbjq.cn

按语言统计（条）：
来源：http://ejq.jinyuanbaomall.cn

Python ......... 252
来源：http://ugj.dashuyun.cn

PHP ............ 252
来源：http://ajx.fanxiaobao.xyz

JavaScript ..... 252
来源：http://sza.tian-w.cn

TypeScript ..... 212
来源：http://uba.guowangkeji.top

Java ........... 212
来源：http://dqu.nanxuanxn.top

Go ............. 212
来源：http://bmn.dashuyun.cn

Ruby ........... 212
来源：http://pis.vqdsnc.cn

C# ............. 212
来源：http://ptz.shuidangran.top

C .............. 30
来源：http://uhg.hammf.cn

C++ ............ 30
来源：http://rof.cheryme.top

SQL ............ 90
来源：http://gys.quarkkingdee.top

Bash ........... 80
来源：http://edp.zhijiandao.cn

Kotlin ......... 15
来源：http://rwz.dianchejie.cn

Swift .......... 15
来源：http://mxf.birdmap.top

Lua ............ 10
来源：http://ufj.yonumen.top

Perl ........... 10
来源：http://pss.meibo888.top

Scala .......... 10
来源：http://blv.cqqwz.cn

------------------------------------
来源：http://eyw.tian-w.cn

合计 ........... 2106 条
来源：http://jgo.jyoumei.cn

按章节统计：
来源：http://bsk.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://spo.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ycm.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fcl.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tef.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zoy.jlsjyb.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zfq.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hhs.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fce.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://diu.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kbv.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rpz.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://itp.cashguo.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sgm.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://owm.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://shu.jinghuilouyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jta.wangshuangyany.cn

Q SQL 专题                              90
来源：http://kww.fzhhl.top

R Bash 专题                             80
来源：http://jvi.daria6918.cn

S C / C++ 专题                          60
来源：http://jqy.iojbl.cn

T 其他语言补充                          60
来源：http://hea.hnxiangtu.top

U 高频实用片段                         120
来源：http://kwa.xinyue.icu

------------------------------------
来源：http://mvg.pycfn.com

合计                                  2106 条
来源：http://mms.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://byv.shanyushiyangtech.top

使用提醒
来源：http://akv.birdmap.top

--------------------------------------------------------------------------------
来源：http://txg.chenjidiqi.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dme.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cxw.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tgf.hammf.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://swj.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rsv.birdmap.top

—— 文件结束 ——
来源：http://iiu.9152youxi.cn

================================================================================
来源：http://wum.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://ses.jinqigufen.top

Common Programming Examples Cheat Book
来源：http://ben.zdqjudy.top

================================================================================
来源：http://zei.52xcode.cn

【收录内容】
来源：http://wop.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://taq.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kia.yj20258.top

SQL · Bash · C · C++
来源：http://scb.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mqt.shanyushiyangtech.top

【使用说明】
来源：http://pwj.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://adi.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://poq.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qul.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lqv.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bus.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dsw.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://set.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tty.yangfankeji.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kvm.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://udo.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qjv.ydzc1.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qcl.shanyushiyangtech.top

【文件统计】
来源：http://ber.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://auf.xinyue.icu

--------------------------------------------------------------------------------
来源：http://ogn.vehdjk.com

目  录
来源：http://xrc.yfazqb.com

--------------------------------------------------------------------------------
来源：http://fqg.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ugl.cqqwz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aaj.jqgfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uag.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mef.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kyj.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://akf.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xqv.sweek.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eys.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ryg.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nqn.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yfl.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qeb.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kst.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vms.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://htx.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://axx.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lld.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uun.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eei.vqdsnc.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bek.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://chh.hongshengwenyu.top

================================================================================
来源：http://lqt.jinqigfzy.top

A. 基础语法与类型
来源：http://dnc.ydzc1.top

================================================================================
来源：http://ktm.shangyingyoupin.top

[A01] Hello World
来源：http://beb.xylfe.cn

Py:   print("Hello, World!")
来源：http://myb.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://uzn.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://dut.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yfn.gaohongyu789.top

Java: System.out.println("Hello, World!");
来源：http://gnb.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://cyf.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://eon.pycfn.com

C#:   Console.WriteLine("Hello, World!");
来源：http://rls.chenlongwang.top

[A02] 变量声明与赋值
来源：http://eyr.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bmp.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jeg.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://mmi.cdnleiting.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vbh.hysaishi.cn

Java: String name = "Alex"; int age = 20;
来源：http://xsy.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://eto.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://bse.mhx1999.top

C#:   string name = "Alex"; int age = 20;
来源：http://fum.hnxiangtu.top

[A03] 常量定义
来源：http://sen.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://coj.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://gsd.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://wto.vehdjk.com

TS:   const PI: number = 3.14159;
来源：http://sbd.epnwcf.com

Java: static final double PI = 3.14159;
来源：http://bqe.sxryk.cn

Go:   const PI = 3.14159
来源：http://uae.yj202588.top

Ruby: PI = 3.14159
来源：http://jbi.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://uft.ctjpmb.com

[A04] 判断变量类型
来源：http://ieo.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yix.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gya.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qgp.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://qhf.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cvu.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://rxe.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kjt.redwolf501.top

C#:   x.GetType().Name; x is int
来源：http://gnr.sxryk.cn

[A05] 整数除法与取模
来源：http://gqu.zycfv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yes.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xto.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ehd.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nix.chenjidiqi.icu

Java: 7 / 2; 7 % 2
来源：http://lbe.uphjek.com

Go:   7 / 2; 7 % 2
来源：http://utu.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://lef.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://nvb.zdbjq.cn

[A06] 字符串转数字
来源：http://ngj.gogol.net.cn

Py:   int("42"); float("3.14")
来源：http://zwz.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zky.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zkh.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://och.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hyu.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pxk.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ude.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cfm.yuanzhike.top

[A07] 数字转字符串
来源：http://yrk.fehbvm.com

Py:   str(42)
来源：http://xxj.xuanzx.com

PHP:  (string) 42; strval(42)
来源：http://yob.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://qvh.redwolf501.top

TS:   String(42)
来源：http://ohn.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://mvv.tarul.cn

Go:   strconv.Itoa(42)
来源：http://qww.ppjwa.cn

Ruby: 42.to_s
来源：http://xuq.yvedp.cn

C#:   42.ToString()
来源：http://kup.jinqigfzy.top

[A08] 取整与四舍五入
来源：http://ljq.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zza.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xny.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qoz.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rpw.wangshuangyany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fjl.hammf.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://epo.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ohq.9152youxi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://egf.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://jfj.dianchejie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tpk.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ild.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ogr.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gqh.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dkq.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ijt.hysaishi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hkc.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fpv.hywenlv.cn

[A10] 生成随机数
来源：http://ddv.zhengqikj.top

Py:   import random; random.randint(1, 100)
来源：http://gcj.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://eok.fanxiaobao.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vbj.nanxinkj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iwq.shuidangran.top

Java: new Random().nextInt(100) + 1
来源：http://yrp.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kap.zycfv.cn

Ruby: rand(1..100)
来源：http://mee.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://oxl.vqdsnc.cn

[A11] 条件表达式（三元）
来源：http://wcj.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://lkf.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://chl.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://xka.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://tdb.cqqwz.cn

Java: x > 0 ? "yes" : "no"
来源：http://uvl.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xhy.hywenlv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dsi.ppjwa.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sdg.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://rvu.feifeiyinyue.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rll.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fbf.hfpthk.cn

JS:   `Hello, ${name}!`
来源：http://eso.xuanzx.com

TS:   `Hello, ${name}!`
来源：http://nph.aibaodan.cn

Java: "Hello, %s!".formatted(name)
来源：http://mmb.quarkkingdee.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ymx.zhoulong.xyz

Ruby: "Hello, #{name}!"
来源：http://ybg.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://zsb.sjlbkw.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vxn.svipenyu.cn

Py:   "第一行\n第二行"
来源：http://wfb.yfazqb.com

PHP:  "第一行\n第二行"
来源：http://usm.tian-w.cn

JS:   "第一行\n第二行"
来源：http://xfm.yj20258888.top

TS:   "第一行\n第二行"
来源：http://ekh.jqgufenzy.top

Java: "第一行\n第二行"
来源：http://ezg.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://pxd.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://veq.havefunace.top

C#:   "第一行\n第二行"
来源：http://ueg.sysykeji.top

[A14] 注释写法
来源：http://hev.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gzu.pycfn.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://jko.guowangkeji.top

JS:   // 单行；/* 多行 */
来源：http://jso.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://vjp.birdmap.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oen.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://mac.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://cfj.hywenlv.cn

C#:   // 单行；/* 多行 */
来源：http://pjv.haohaochexian.top

[A15] 空值判断与默认值
来源：http://dax.shzxlz.cn

Py:   value = data or "默认值"
来源：http://mqf.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://dwo.hnxiangtu.top

JS:   const value = data ?? "默认值";
来源：http://fmt.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://dym.smart0.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tur.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://ivu.cqqwz.cn

Ruby: value = data || "默认值"
来源：http://kot.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://ims.birdmap.top

[A16] 真假值判断规则
来源：http://vzo.quarkkingdee.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pox.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aex.jianghu66.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jlr.hcnkem.com

TS:   if (!x) {}
来源：http://rlu.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xpr.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ouw.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hbs.sxryk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nhe.guannengcc.top

[A17] 位运算
来源：http://jcb.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fwo.tanke756.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://psl.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://stj.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mea.sjlbkw.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vej.yueranfly.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gnx.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txv.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cne.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://xnd.tanke756.top

Py:   ord("A"); chr(65)
来源：http://vfw.svipenyu.cn

PHP:  ord("A"); chr(65)
来源：http://ego.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://omo.jinyuanbaomall.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xdl.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://uwm.sweek.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jib.havefunace.top

Ruby: "A".ord; 65.chr
来源：http://rzk.gogol.net.cn


<!-- 参考信息 -->