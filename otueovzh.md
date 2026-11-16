代发 wailian999

[U105] JS：节流
来源：http://krt.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fzf.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://kim.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bib.52xcode.cn

[U107] JS：数字千分位
来源：http://pya.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://niz.gogol.net.cn

[U108] JS：随机整数
来源：http://bln.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dsl.tarul.cn

[U109] JS：数组分组
来源：http://pvh.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://qtb.haohaochexian.top

[U110] JS：数组分块
来源：http://tpv.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uxc.fehbvm.com

[U111] JS：对象转 Map
来源：http://vly.hywenlv.cn

new Map(Object.entries(obj))
来源：http://ecr.xziqi.cn

[U112] JS：字符串补位
来源：http://fob.sjlbkw.cn

"7".padStart(3, "0")
来源：http://zzu.daria6918.cn

[U113] JS：正则替换全部
来源：http://lbp.zdqjudy.top

s.replaceAll("a", "b")
来源：http://swx.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://ufy.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dok.c1oappe.top

[U115] JS：生成 UUID
来源：http://whs.hywenlv.cn

crypto.randomUUID()
来源：http://gqy.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://vjd.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://ljg.epnwcf.com

[U117] JS：单元测试
来源：http://egp.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://vhp.hnxiangtu.top

[U118] JS：开发服务器
来源：http://pzs.zdqjudy.top

npm i -D vite;  npx vite
来源：http://rtp.jinqigfzy.top

[U119] JS：生产构建
来源：http://hdl.fktsv.cn

npx vite build
来源：http://zka.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://nvp.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://enr.uphjek.com

================================================================================
来源：http://roo.shzxlz.cn

统计汇总
来源：http://qkj.nanxinkj.top

================================================================================
来源：http://ykv.hongshengwenyu.top

按语言统计（条）：
来源：http://srb.zhaomingkeji.xyz

Python ......... 252
来源：http://zvn.dianchejie.cn

PHP ............ 252
来源：http://arm.vqdsnc.cn

JavaScript ..... 252
来源：http://zsr.jqgfzy.top

TypeScript ..... 212
来源：http://tbe.yfazqb.com

Java ........... 212
来源：http://iwy.fehbvm.com

Go ............. 212
来源：http://mmp.iojbl.cn

Ruby ........... 212
来源：http://lbk.xingfuxueyuan.xyz

C# ............. 212
来源：http://tnp.hcnkem.com

C .............. 30
来源：http://bkj.guannengcc.top

C++ ............ 30
来源：http://gdc.zhaomingkeji.xyz

SQL ............ 90
来源：http://sgx.xingfuxueyuan.xyz

Bash ........... 80
来源：http://dyh.zhijiandao.cn

Kotlin ......... 15
来源：http://jch.feifeiyinyue.top

Swift .......... 15
来源：http://svv.yfazqb.com

Lua ............ 10
来源：http://wdj.jqgfzy.top

Perl ........... 10
来源：http://nqj.smart0.xyz

Scala .......... 10
来源：http://ibx.cucudq.cn

------------------------------------
来源：http://kmh.wangshuangyany.cn

合计 ........... 2106 条
来源：http://zha.dashuyun.cn

按章节统计：
来源：http://gpp.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xlp.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://znx.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qho.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rxr.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ybd.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hwj.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://llu.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tfw.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hpk.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lzv.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nbk.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://onq.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rsr.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://use.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uld.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ixt.xuetiantiany.cn

Q SQL 专题                              90
来源：http://woe.tian-w.cn

R Bash 专题                             80
来源：http://sto.aizwys.cn

S C / C++ 专题                          60
来源：http://eod.havefunace.top

T 其他语言补充                          60
来源：http://xkp.sxryk.cn

U 高频实用片段                         120
来源：http://azc.redwolf501.top

------------------------------------
来源：http://ytc.gogol.net.cn

合计                                  2106 条
来源：http://xso.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://olk.wangshuangyany.cn

使用提醒
来源：http://mve.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://evi.iojbl.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rjm.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xue.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eon.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://etq.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://flz.ehwqpu.com

—— 文件结束 ——
来源：http://ful.bbcook.cn

================================================================================
来源：http://ldq.wangshuangyany.cn

程序语言常见例子速查手册（2024 版）
来源：http://xvp.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://yei.vqdsnc.cn

================================================================================
来源：http://lnu.haohaochexian.top

【收录内容】
来源：http://yjk.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://brq.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mcj.havefunace.top

SQL · Bash · C · C++
来源：http://rxs.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uxz.mhx1999.top

【使用说明】
来源：http://jsu.chenzaomai.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dtf.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iuy.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eyi.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gvc.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://htj.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dop.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://arn.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://orj.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xsw.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mwc.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bzu.redwolf501.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mqs.zdbjq.cn

【文件统计】
来源：http://lkj.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tpb.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://azr.haohaochexian.top

目  录
来源：http://lcs.sysykeji.top

--------------------------------------------------------------------------------
来源：http://gyt.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kdg.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://csi.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fye.sjlbkw.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ufr.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dxf.9152youxi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vwn.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ocp.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hss.ehwqpu.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://puc.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iqd.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qbl.fanxiaobao.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://akm.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nje.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tyo.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xhm.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bwp.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://taa.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bci.cheryme.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ekc.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://git.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yny.uphjek.com

================================================================================
来源：http://lad.yj20258.top

A. 基础语法与类型
来源：http://otr.tanke756.top

================================================================================
来源：http://igr.zdqjudy.top

[A01] Hello World
来源：http://fas.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://hjk.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://hoc.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://glo.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ihv.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://kwy.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://nuy.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://jzu.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mkh.xylfe.cn

[A02] 变量声明与赋值
来源：http://qrz.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kxp.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jgu.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tem.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xuw.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://jwl.jqgufenzy.top

Go:   name := "Alex"; age := 20
来源：http://lue.andypj.xyz

Ruby: name = "Alex"; age = 20
来源：http://ctx.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zng.ehwqpu.com

[A03] 常量定义
来源：http://ptx.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jyr.birdmap.top

PHP:  const PI = 3.14159;
来源：http://pzv.ppjwa.cn

JS:   const PI = 3.14159;
来源：http://jus.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://hne.shuidangran.top

Java: static final double PI = 3.14159;
来源：http://liz.yangfankeji.com

Go:   const PI = 3.14159
来源：http://jwy.ehwqpu.com

Ruby: PI = 3.14159
来源：http://nde.smart0.xyz

C#:   const double PI = 3.14159;
来源：http://zyy.cucudq.cn

[A04] 判断变量类型
来源：http://oar.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vdx.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bzh.snrcjt.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vbu.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://sga.yuanzhike.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rma.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://dex.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rym.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://yvl.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://hhk.iojbl.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xnl.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mvb.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://utj.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qpg.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://rhr.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://ben.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://cfl.gogol.net.cn

C#:   7 / 2; 7 % 2
来源：http://dxd.fktsv.cn

[A06] 字符串转数字
来源：http://eiu.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://gog.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://txh.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fzv.ivvv.top

TS:   parseInt("42", 10); Number("42")
来源：http://iaf.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vdb.ybcxt.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aaz.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vtq.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://afp.xuetiantiany.cn

[A07] 数字转字符串
来源：http://hso.gotoacloud.top

Py:   str(42)
来源：http://jdv.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://wgz.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://agv.aibaodan.cn

TS:   String(42)
来源：http://mtw.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://epl.tarul.cn

Go:   strconv.Itoa(42)
来源：http://zxr.ppjwa.cn

Ruby: 42.to_s
来源：http://unk.dashuyun.cn

C#:   42.ToString()
来源：http://qce.zhengqikj.top

[A08] 取整与四舍五入
来源：http://xgk.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://diu.haohaochexian.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://shg.gaohongyu789.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://npn.zhoulong.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ypy.hesvh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nla.hysaishi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://akw.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sse.shuidangran.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ezf.yuxming.cn

[A09] 绝对值与最大最小值
来源：http://zig.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bem.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://veb.daria6918.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dru.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fri.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bbm.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xum.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ywv.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mfs.svipenyu.cn

[A10] 生成随机数
来源：http://thm.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://hlp.yfazqb.com

PHP:  random_int(1, 100);
来源：http://byz.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zzy.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jgd.ivvv.top

Java: new Random().nextInt(100) + 1
来源：http://ank.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://iod.pycfn.com

Ruby: rand(1..100)
来源：http://lqu.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://zrc.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://azr.nwbrower.top

Py:   "yes" if x > 0 else "no"
来源：http://ejn.dianchejie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kue.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://eqs.sjlbkw.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qds.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://pyi.hfpthk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jgo.yj202588.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tgt.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://rwm.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://tqy.ctjpmb.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cvw.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lcz.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://ycr.cqqwz.cn

TS:   `Hello, ${name}!`
来源：http://djn.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://jrc.shanyushiyangkeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://epu.vqdsnc.cn

Ruby: "Hello, #{name}!"
来源：http://vrr.redwolf501.top

C#:   $"Hello, {name}!"
来源：http://rsc.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://chj.haohaochexian.top

Py:   "第一行\n第二行"
来源：http://ztc.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://ale.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://gcu.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://zie.yj202588.top

Java: "第一行\n第二行"
来源：http://qnp.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://yns.cashguo.top

Ruby: "第一行\n第二行"
来源：http://gax.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://amo.ywan-chungtsiang.top

[A14] 注释写法
来源：http://uoh.feifeiyinyue.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://bpy.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://woi.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://oeh.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://zjj.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wsa.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://tfo.ydjk.org.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bao.fzhhl.top

C#:   // 单行；/* 多行 */
来源：http://uml.xingfuxueyuan.xyz

[A15] 空值判断与默认值
来源：http://frj.zycfv.cn

Py:   value = data or "默认值"
来源：http://tht.hcnkem.com

PHP:  $value = $data ?? "默认值";
来源：http://mqb.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://cks.kuanghao11.cn

TS:   const value = data ?? "默认值";
来源：http://xku.hesvh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iat.hongshengwenyu.top

Go:   if data == "" { data = "默认值" }
来源：http://zun.sysykeji.top

Ruby: value = data || "默认值"
来源：http://tbr.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://fkd.yanxiufei.cn

[A16] 真假值判断规则
来源：http://rnq.jqgfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iub.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://twr.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mev.jqgufenzy.top

TS:   if (!x) {}
来源：http://ywj.gzhubu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sox.nanxinkj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://voa.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://sbv.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://edz.zhongyouzk.top

[A17] 位运算
来源：http://thd.yongpay.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bfh.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://utr.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wgr.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hno.yj202588.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fpw.yuxming.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eaw.nanxinkj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kqv.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ema.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://jlt.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://ago.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://flr.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://clf.redwolf501.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rph.nwbrower.top

Java: (int) 'A'; (char) 65
来源：http://imh.yuanzhike.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vmy.zhiwuduotai.top

Ruby: "A".ord; 65.chr
来源：http://ogh.ydjk.org.cn


<!-- 参考信息 -->