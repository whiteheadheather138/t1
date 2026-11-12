代发 wailian999

[U105] JS：节流
来源：http://dyb.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sib.snrcjt.cn

[U106] JS：日期格式化
来源：http://eqf.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ucy.vehdjk.com

[U107] JS：数字千分位
来源：http://ryl.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://reo.yuxming.cn

[U108] JS：随机整数
来源：http://hls.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oos.sweek.top

[U109] JS：数组分组
来源：http://vnv.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://yil.zhengqikj.top

[U110] JS：数组分块
来源：http://jzh.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://afd.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://bcu.ydzc1.top

new Map(Object.entries(obj))
来源：http://hnn.hysaishi.cn

[U112] JS：字符串补位
来源：http://jad.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://xch.52xcode.cn

[U113] JS：正则替换全部
来源：http://xcr.chenzaomai.com

s.replaceAll("a", "b")
来源：http://kpe.cashguo.top

[U114] JS：JSON 深比较
来源：http://vsk.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://few.cashguo.top

[U115] JS：生成 UUID
来源：http://vmt.shuidangran.top

crypto.randomUUID()
来源：http://mms.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://nbv.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://rxq.ydjk.org.cn

[U117] JS：单元测试
来源：http://vrd.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://ikv.ivvv.top

[U118] JS：开发服务器
来源：http://rxh.c1oappe.top

npm i -D vite;  npx vite
来源：http://hmx.redwolf501.top

[U119] JS：生产构建
来源：http://ubo.bjfxy.top

npx vite build
来源：http://err.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://ggf.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://zto.daria6918.cn

================================================================================
来源：http://dny.tian-w.cn

统计汇总
来源：http://eio.birdmap.top

================================================================================
来源：http://xbi.cdnleiting.top

按语言统计（条）：
来源：http://hyf.jqgfzy.top

Python ......... 252
来源：http://ast.haohaochexian.top

PHP ............ 252
来源：http://tct.xuanzx.com

JavaScript ..... 252
来源：http://peu.xylfe.cn

TypeScript ..... 212
来源：http://lal.fktsv.cn

Java ........... 212
来源：http://hsg.ivvv.top

Go ............. 212
来源：http://dtv.xuetiantiany.cn

Ruby ........... 212
来源：http://pkk.tianlin.xyz

C# ............. 212
来源：http://zra.ydzc1.top

C .............. 30
来源：http://upw.gaohongyu789.top

C++ ............ 30
来源：http://tlz.yanxiufei.cn

SQL ............ 90
来源：http://osj.chenlongwang.top

Bash ........... 80
来源：http://ohl.vqdsnc.cn

Kotlin ......... 15
来源：http://vjd.cucudq.cn

Swift .......... 15
来源：http://rck.smart0.xyz

Lua ............ 10
来源：http://icd.tarul.cn

Perl ........... 10
来源：http://jls.jyoumei.cn

Scala .......... 10
来源：http://cbj.aibaodan.cn

------------------------------------
来源：http://ulr.meibo888.top

合计 ........... 2106 条
来源：http://bxd.hysaishi.cn

按章节统计：
来源：http://zcv.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hga.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pyf.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://osd.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://swm.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rca.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eoh.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://onz.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://erk.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mui.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://agk.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jjq.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mrz.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gty.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://exv.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fgd.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ykx.fktsv.cn

Q SQL 专题                              90
来源：http://fbr.redwolf501.top

R Bash 专题                             80
来源：http://ebb.yueranfly.top

S C / C++ 专题                          60
来源：http://mnk.zhengqikj.top

T 其他语言补充                          60
来源：http://gcr.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://eos.jinqigfzy.top

------------------------------------
来源：http://kbj.uphjek.com

合计                                  2106 条
来源：http://ejs.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://mfk.bjfxy.top

使用提醒
来源：http://dow.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://adk.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tbl.uphjek.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rgb.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qlj.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ael.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jww.pengpengdd.cyou

—— 文件结束 ——
来源：http://pfa.yfazqb.com

================================================================================
来源：http://ctn.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://bdw.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://row.aizwys.cn

================================================================================
来源：http://wea.hnqzz.top

【收录内容】
来源：http://qha.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rql.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bmr.chenzaomai.com

SQL · Bash · C · C++
来源：http://cjd.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gtu.gogol.net.cn

【使用说明】
来源：http://nns.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wst.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bqr.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jfw.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nri.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qbj.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xub.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://egr.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oyz.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dph.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gel.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jsf.xylfe.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gmz.daxiang520.top

【文件统计】
来源：http://cpk.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://awy.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://ncn.nanxinkj.top

目  录
来源：http://rvb.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://dwi.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://haj.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cha.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rzf.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zaj.jianghu66.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lgu.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tef.hammf.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://piy.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bph.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tnv.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ybm.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://swc.fzhhl.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fmr.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kcn.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://auk.wangshuangyany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dlf.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kvh.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://exr.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://xss.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rgo.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nhn.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dds.sxryk.cn

================================================================================
来源：http://wuy.bjfxy.top

A. 基础语法与类型
来源：http://yzh.xziqi.cn

================================================================================
来源：http://dzs.sxryk.cn

[A01] Hello World
来源：http://mkj.dianchejie.cn

Py:   print("Hello, World!")
来源：http://hls.tarul.cn

PHP:  echo "Hello, World!";
来源：http://qkd.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://jww.tian-w.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://spt.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://eix.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://glw.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://cpc.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://oko.yongpay.top

[A02] 变量声明与赋值
来源：http://wri.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cyp.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xzj.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://ods.guowangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kal.ybcxt.top

Java: String name = "Alex"; int age = 20;
来源：http://qkd.jqgufenzy.top

Go:   name := "Alex"; age := 20
来源：http://nwc.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://ehm.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://siy.aibaodan.cn

[A03] 常量定义
来源：http://rww.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dfj.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://dnu.zhaomingkeji.xyz

JS:   const PI = 3.14159;
来源：http://ioa.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://efk.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://aqz.wangdashe.top

Go:   const PI = 3.14159
来源：http://lhl.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://bbj.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://gwq.smart0.xyz

[A04] 判断变量类型
来源：http://ysn.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://veb.epnwcf.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://khv.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tks.jyoumei.cn

TS:   typeof x; x instanceof Date
来源：http://mlp.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vxv.9152youxi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pxb.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qkg.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://rrq.birdmap.top

[A05] 整数除法与取模
来源：http://alu.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xdm.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hsx.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mms.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dje.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://cea.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://xlq.fanxiaobao.xyz

Ruby: 7 / 2; 7 % 2
来源：http://rpg.0kj1m.cn

C#:   7 / 2; 7 % 2
来源：http://ppc.sjlbkw.cn

[A06] 字符串转数字
来源：http://ooy.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://ndy.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rpf.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lmw.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://qyf.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://erw.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nun.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tzk.fanxiaobao.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dds.bbcook.cn

[A07] 数字转字符串
来源：http://zhy.guannengcc.top

Py:   str(42)
来源：http://gsx.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://xxo.52xcode.cn

JS:   String(42); (42).toString()
来源：http://jkx.birdmap.top

TS:   String(42)
来源：http://hxf.chenzaomai.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://itf.cheryme.top

Go:   strconv.Itoa(42)
来源：http://zev.gotoacloud.top

Ruby: 42.to_s
来源：http://cnm.hammf.cn

C#:   42.ToString()
来源：http://xkl.zycfv.cn

[A08] 取整与四舍五入
来源：http://dlz.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hcf.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xxy.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fcp.xuanzx.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hed.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iny.meibo888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://beu.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://ksn.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://efa.cashguo.top

[A09] 绝对值与最大最小值
来源：http://gbl.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xfl.9152youxi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://utg.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xdr.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nrj.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mun.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ulp.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nae.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ixd.316326.xyz

[A10] 生成随机数
来源：http://ujp.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://bdk.snrcjt.cn

PHP:  random_int(1, 100);
来源：http://kon.ydjk.org.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fxz.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hnn.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://nhf.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zgd.dashuyun.cn

Ruby: rand(1..100)
来源：http://wxq.hcnkem.com

C#:   new Random().Next(1, 101)
来源：http://tkg.aibaodan.cn

[A11] 条件表达式（三元）
来源：http://dah.ctjpmb.com

Py:   "yes" if x > 0 else "no"
来源：http://fyl.gaohongyu789.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ofl.shanyushiyangtech.top

JS:   x > 0 ? "yes" : "no"
来源：http://nof.zhengqikj.top

TS:   x > 0 ? "yes" : "no"
来源：http://fyc.sjlbkw.cn

Java: x > 0 ? "yes" : "no"
来源：http://pzc.jlsjyb.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nqt.zhaomingkeji.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://yne.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://nzu.pycfn.com

[A12] 字符串插值 / 格式化
来源：http://wnn.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aho.zycfv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qux.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://gft.ybcxt.top

TS:   `Hello, ${name}!`
来源：http://sav.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://aki.pengpengdd.cyou

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aev.ehwqpu.com

Ruby: "Hello, #{name}!"
来源：http://itk.yvedp.cn

C#:   $"Hello, {name}!"
来源：http://aru.ppjwa.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qdj.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://txr.bjfxy.top

PHP:  "第一行\n第二行"
来源：http://uti.sxryk.cn

JS:   "第一行\n第二行"
来源：http://swa.pycfn.com

TS:   "第一行\n第二行"
来源：http://wzu.shzxlz.cn

Java: "第一行\n第二行"
来源：http://ymr.jlsjyb.cn

Go:   "第一行\n第二行"
来源：http://zev.feifeiyinyue.top

Ruby: "第一行\n第二行"
来源：http://oui.tarul.cn

C#:   "第一行\n第二行"
来源：http://kss.zhongyouzk.top

[A14] 注释写法
来源：http://und.hywenlv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pdb.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://knu.jinghuilouyu.cn

JS:   // 单行；/* 多行 */
来源：http://kuw.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://ajk.nanxuanxn.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nvz.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://jsb.hcnkem.com

Ruby: # 单行；=begin 多行 =end
来源：http://pnz.shuidangran.top

C#:   // 单行；/* 多行 */
来源：http://fpb.sweek.top

[A15] 空值判断与默认值
来源：http://ugd.jqgfzy.top

Py:   value = data or "默认值"
来源：http://ytg.ybcxt.top

PHP:  $value = $data ?? "默认值";
来源：http://lhb.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://mxf.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://vfe.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ycq.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://ylv.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://oxx.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://dwt.dianchejie.cn

[A16] 真假值判断规则
来源：http://zbw.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gtu.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vkq.hesvh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cnc.zhixingplan.top

TS:   if (!x) {}
来源：http://ylj.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qzh.xylfe.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nnf.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://qpm.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ppv.yj20258.top

[A17] 位运算
来源：http://unw.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxc.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fuk.jqgfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igl.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rbc.feifeiyinyue.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://akt.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bja.yj20258888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxo.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpf.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://bww.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://cxv.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://bgs.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qxt.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wdz.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://ehy.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ocv.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://lcn.xinyue.icu


<!-- 参考信息 -->