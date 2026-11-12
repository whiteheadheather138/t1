代发 wailian999

[U103] JS：定时器
来源：http://ose.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://njg.zhiwuduotai.top

[U104] JS：防抖
来源：http://eeq.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://syf.yj20258.top

[U105] JS：节流
来源：http://vot.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gfc.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://yax.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rox.ivvv.top

[U107] JS：数字千分位
来源：http://tiw.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fbf.pengpengdd.cyou

[U108] JS：随机整数
来源：http://sqc.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://opi.daxiang520.top

[U109] JS：数组分组
来源：http://mkl.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://nqs.cheryme.top

[U110] JS：数组分块
来源：http://lto.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xeh.cqqwz.cn

[U111] JS：对象转 Map
来源：http://njx.yj20258888.top

new Map(Object.entries(obj))
来源：http://asv.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://lbd.jlsjyb.cn

"7".padStart(3, "0")
来源：http://ldu.tianlin.xyz

[U113] JS：正则替换全部
来源：http://ydj.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://jtk.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://xfq.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sqt.hywenlv.cn

[U115] JS：生成 UUID
来源：http://igh.nanxinkj.top

crypto.randomUUID()
来源：http://bnf.daria6918.cn

[U116] JS：类型检查（JSDoc）
来源：http://swm.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://mrj.hammf.cn

[U117] JS：单元测试
来源：http://ubb.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://lmr.hesvh.cn

[U118] JS：开发服务器
来源：http://fxd.yj202588.top

npm i -D vite;  npx vite
来源：http://lpu.mhx1999.top

[U119] JS：生产构建
来源：http://cec.chenjidiqi.icu

npx vite build
来源：http://ovu.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://oey.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://yst.pycfn.com

================================================================================
来源：http://hnd.mhx1999.top

统计汇总
来源：http://fvg.sjlbkw.cn

================================================================================
来源：http://liz.yj20258888.top

按语言统计（条）：
来源：http://sbz.tian-w.cn

Python ......... 252
来源：http://lnw.aibaodan.cn

PHP ............ 252
来源：http://moo.hammf.cn

JavaScript ..... 252
来源：http://tyh.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://vxc.tianlin.xyz

Java ........... 212
来源：http://eax.yuxming.cn

Go ............. 212
来源：http://lgf.fzhhl.top

Ruby ........... 212
来源：http://nga.jianghu66.top

C# ............. 212
来源：http://rip.yj20258.top

C .............. 30
来源：http://phn.hesvh.cn

C++ ............ 30
来源：http://tjs.jlsjyb.cn

SQL ............ 90
来源：http://fsw.zdqjudy.top

Bash ........... 80
来源：http://ebo.tianlin.xyz

Kotlin ......... 15
来源：http://ugc.yanxiufei.cn

Swift .......... 15
来源：http://bxv.zhengqikj.top

Lua ............ 10
来源：http://fld.c1oappe.top

Perl ........... 10
来源：http://dbc.haohaochexian.top

Scala .......... 10
来源：http://zdt.yj20258888.top

------------------------------------
来源：http://dgu.jqgufenzy.top

合计 ........... 2106 条
来源：http://lpz.zdbjq.cn

按章节统计：
来源：http://uzc.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gdv.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pxj.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hec.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tcw.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://obo.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zov.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qpr.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tph.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rrz.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://igy.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wvd.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://peu.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://psv.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tyn.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rcb.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yyy.hfpthk.cn

Q SQL 专题                              90
来源：http://uwx.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://vyz.jinqigufen.top

S C / C++ 专题                          60
来源：http://odl.vehdjk.com

T 其他语言补充                          60
来源：http://mww.0kj1m.cn

U 高频实用片段                         120
来源：http://pzc.mhx1999.top

------------------------------------
来源：http://fuc.vehdjk.com

合计                                  2106 条
来源：http://pzk.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://eag.ehwqpu.com

使用提醒
来源：http://vuj.yj20258.top

--------------------------------------------------------------------------------
来源：http://adx.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eqn.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dsm.zdbjq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ipx.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rle.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gwc.ehwqpu.com

—— 文件结束 ——
来源：http://kqh.jyoumei.cn

================================================================================
来源：http://ilg.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://tuc.uphjek.com

Common Programming Examples Cheat Book
来源：http://pxx.sysykeji.top

================================================================================
来源：http://vrt.aibaodan.cn

【收录内容】
来源：http://sdd.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vxs.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lyo.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://hzv.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kud.fzhhl.top

【使用说明】
来源：http://ljh.cqqwz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jfx.hesvh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sax.gzhubu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jib.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hmc.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hnt.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hvw.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mky.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ijn.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wpg.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rdb.sweek.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://arv.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fiy.9152youxi.cn

【文件统计】
来源：http://rqp.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gpl.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://xgm.yj20258888.top

目  录
来源：http://bgk.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://vug.sxryk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hfh.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eug.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bjv.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gjs.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aox.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qfg.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bgh.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mdc.svipenyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lpi.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fww.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zcb.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kfm.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cvk.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gcg.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vjc.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://avd.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oyy.ybcxt.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://awa.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://exb.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rut.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://psi.chenjidiqi.icu

================================================================================
来源：http://lwx.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://xuu.chenlongwang.top

================================================================================
来源：http://izv.guannengcc.top

[A01] Hello World
来源：http://dlr.epnwcf.com

Py:   print("Hello, World!")
来源：http://qnh.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://rno.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://jnw.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pue.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://amt.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://bjl.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://seu.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pkp.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://hsk.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mut.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bkt.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://yuf.fengsongda.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ike.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://lfp.daria6918.cn

Go:   name := "Alex"; age := 20
来源：http://guy.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://jkh.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://tpw.jqgufenzy.top

[A03] 常量定义
来源：http://wlr.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tkn.meibo888.top

PHP:  const PI = 3.14159;
来源：http://uio.316326.xyz

JS:   const PI = 3.14159;
来源：http://qsx.tanke756.top

TS:   const PI: number = 3.14159;
来源：http://xvr.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://oyj.zhongyouzk.top

Go:   const PI = 3.14159
来源：http://frw.hesvh.cn

Ruby: PI = 3.14159
来源：http://avv.chenlongwang.top

C#:   const double PI = 3.14159;
来源：http://vvf.redwolf501.top

[A04] 判断变量类型
来源：http://njq.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://gol.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://euw.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://beb.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://dha.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dqe.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://pie.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://szp.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://his.hesvh.cn

[A05] 整数除法与取模
来源：http://dcf.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ykc.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qtx.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wrx.pengpengdd.cyou

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tcc.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://knc.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://reu.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://ysg.zhijiandao.cn

C#:   7 / 2; 7 % 2
来源：http://ben.shzxlz.cn

[A06] 字符串转数字
来源：http://zbe.sufxvd.cn

Py:   int("42"); float("3.14")
来源：http://sdj.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qbo.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wxo.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kfy.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ydt.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://smh.shzxlz.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vyn.sufxvd.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hio.jinqigfzy.top

[A07] 数字转字符串
来源：http://ogf.ehwqpu.com

Py:   str(42)
来源：http://viq.jiagoushi.top

PHP:  (string) 42; strval(42)
来源：http://sla.yongpay.top

JS:   String(42); (42).toString()
来源：http://umy.vehdjk.com

TS:   String(42)
来源：http://wzh.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ayf.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://mpx.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://ysl.yj20258888.top

C#:   42.ToString()
来源：http://iae.ybcxt.top

[A08] 取整与四舍五入
来源：http://axa.gogol.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kru.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qrm.ydjk.org.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yxh.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://quf.zhiwuduotai.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nav.shanyushiyangtech.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ffa.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mwb.cucudq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yop.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://rsu.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gig.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://apy.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qeg.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hiz.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ice.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kib.fktsv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mxo.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qgl.jinqigufen.top

[A10] 生成随机数
来源：http://ftf.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://awa.redwolf501.top

PHP:  random_int(1, 100);
来源：http://dlu.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sam.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://reu.sweek.top

Java: new Random().nextInt(100) + 1
来源：http://vik.quarkkingdee.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://znm.0kj1m.cn

Ruby: rand(1..100)
来源：http://fci.ydzc1.top

C#:   new Random().Next(1, 101)
来源：http://fol.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://jay.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://bdm.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ttd.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://szh.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ybg.zycfv.cn

Java: x > 0 ? "yes" : "no"
来源：http://dpn.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://awx.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rjx.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://wce.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://ehz.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wtq.cdnleiting.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wha.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://vxk.yonumen.top

TS:   `Hello, ${name}!`
来源：http://bge.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://oqc.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yqj.kuanghao11.cn

Ruby: "Hello, #{name}!"
来源：http://umz.aizwys.cn

C#:   $"Hello, {name}!"
来源：http://rmi.bbcook.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uxq.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://smc.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://kbo.zhongyouzk.top

JS:   "第一行\n第二行"
来源：http://ypx.cucudq.cn

TS:   "第一行\n第二行"
来源：http://nrh.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://gyv.fzhhl.top

Go:   "第一行\n第二行"
来源：http://jnj.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://mzh.tarul.cn

C#:   "第一行\n第二行"
来源：http://gqh.ctjpmb.com

[A14] 注释写法
来源：http://bwk.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rzf.guowangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vjv.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://que.zdbjq.cn

TS:   // 单行；/* 多行 */
来源：http://icc.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lsr.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://mix.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://iug.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://bux.hcnkem.com

[A15] 空值判断与默认值
来源：http://sly.hnqzz.top

Py:   value = data or "默认值"
来源：http://dkt.shzxlz.cn

PHP:  $value = $data ?? "默认值";
来源：http://nuf.tarul.cn

JS:   const value = data ?? "默认值";
来源：http://qbs.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://npz.xingfuxueyuan.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ryx.zhiwuduotai.top

Go:   if data == "" { data = "默认值" }
来源：http://zdd.sweek.top

Ruby: value = data || "默认值"
来源：http://uea.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://bjt.snrcjt.cn

[A16] 真假值判断规则
来源：http://myh.wangdashe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://icv.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hss.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ubt.xuanzx.com

TS:   if (!x) {}
来源：http://fvi.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fny.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ntz.zhiwuduotai.top

Ruby: unless x            # nil 与 false 为假
来源：http://bzk.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lyl.jlsjyb.cn

[A17] 位运算
来源：http://lay.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ikp.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nbg.aibaodan.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzn.wangdashe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qxm.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzh.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ncx.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yjv.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zay.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://lse.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://qqn.hysaishi.cn

PHP:  ord("A"); chr(65)
来源：http://dcx.hnqzz.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://axf.tarul.cn


<!-- 参考信息 -->