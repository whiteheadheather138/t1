代发 wailian999

[U105] JS：节流
来源：https://iy.zhonguo5118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://vn.zhonguo1118.cn

[U106] JS：日期格式化
来源：https://mw.zhonguo6118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://ta.zhonguo4118.cn

[U107] JS：数字千分位
来源：https://vs.zhonguo3118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://gh.zhonguo5118.cn

[U108] JS：随机整数
来源：https://dn.zhonguo8118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://qv.zhonguo7118.cn

[U109] JS：数组分组
来源：https://jq.zhonguo4118.cn

Object.groupBy(arr, x => x.type)
来源：https://ut.zhonguo5118.cn

[U110] JS：数组分块
来源：https://ok.zhonguo3118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ot.zhonguo5118.cn

[U111] JS：对象转 Map
来源：https://cz.zhonguo3118.cn

new Map(Object.entries(obj))
来源：https://kj.zhonguo4118.cn

[U112] JS：字符串补位
来源：https://ct.zhonguo7118.cn

"7".padStart(3, "0")
来源：https://xc.zhonguo4118.cn

[U113] JS：正则替换全部
来源：https://ck.zhonguo4118.cn

s.replaceAll("a", "b")
来源：https://yd.zhonguo8118.cn

[U114] JS：JSON 深比较
来源：https://tg.zhonguo1118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://ay.zhonguo8118.cn

[U115] JS：生成 UUID
来源：https://ne.zhonguo4118.cn

crypto.randomUUID()
来源：https://tw.zhonguo3118.cn

[U116] JS：类型检查（JSDoc）
来源：https://hj.zhonguo7118.cn

/** @param {string} name */ function f(name) {}
来源：https://lu.zhonguo8118.cn

[U117] JS：单元测试
来源：https://cz.zhonguo5118.cn

npm i -D vitest;  npx vitest
来源：https://he.zhonguo2118.cn

[U118] JS：开发服务器
来源：https://pf.zhonguo5118.cn

npm i -D vite;  npx vite
来源：https://rw.zhonguo7118.cn

[U119] JS：生产构建
来源：https://zu.zhonguo6118.cn

npx vite build
来源：https://jz.zhonguo2118.cn

[U120] JS：读取环境变量（Vite）
来源：https://gn.zhonguo5118.cn

import.meta.env.VITE_API_URL
来源：https://yj.zhonguo7118.cn

================================================================================
来源：https://cq.zhonguo8118.cn

统计汇总
来源：https://bi.zhonguo6118.cn

================================================================================
来源：https://bh.zhonguo7118.cn

按语言统计（条）：
来源：https://mh.zhonguo2118.cn

Python ......... 252
来源：https://zf.zhonguo3118.cn

PHP ............ 252
来源：https://gf.zhonguo3118.cn

JavaScript ..... 252
来源：https://za.zhonguo5118.cn

TypeScript ..... 212
来源：https://za.zhonguo5118.cn

Java ........... 212
来源：https://tv.zhonguo2118.cn

Go ............. 212
来源：https://if.zhonguo4118.cn

Ruby ........... 212
来源：https://ke.zhonguo7118.cn

C# ............. 212
来源：https://sk.zhonguo4118.cn

C .............. 30
来源：https://km.zhonguo3118.cn

C++ ............ 30
来源：https://qs.zhonguo6118.cn

SQL ............ 90
来源：https://ma.zhonguo3118.cn

Bash ........... 80
来源：https://qw.zhonguo7118.cn

Kotlin ......... 15
来源：https://sd.zhonguo3118.cn

Swift .......... 15
来源：https://bb.zhonguo7118.cn

Lua ............ 10
来源：https://ms.zhonguo6118.cn

Perl ........... 10
来源：https://yn.zhonguo2118.cn

Scala .......... 10
来源：https://up.zhonguo8118.cn

------------------------------------
来源：https://bq.zhonguo7118.cn

合计 ........... 2106 条
来源：https://vt.zhonguo1118.cn

按章节统计：
来源：https://qo.zhonguo4118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://zo.zhonguo1118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://mg.zhonguo6118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://dl.zhonguo8118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://ja.zhonguo3118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://bj.zhonguo4118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://ro.zhonguo3118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://cj.zhonguo1118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://wk.zhonguo3118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://jk.zhonguo8118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://cm.zhonguo4118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://es.zhonguo6118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://vx.zhonguo5118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://dd.zhonguo6118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://qx.zhonguo5118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://tx.zhonguo2118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://lz.zhonguo8118.cn

Q SQL 专题                              90
来源：https://xr.zhonguo3118.cn

R Bash 专题                             80
来源：https://vj.zhonguo3118.cn

S C / C++ 专题                          60
来源：https://rt.zhonguo1118.cn

T 其他语言补充                          60
来源：https://rw.zhonguo8118.cn

U 高频实用片段                         120
来源：https://ko.zhonguo8118.cn

------------------------------------
来源：https://kq.zhonguo5118.cn

合计                                  2106 条
来源：https://au.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://kw.zhonguo7118.cn

使用提醒
来源：https://rx.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://de.zhonguo4118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://jb.zhonguo4118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://qh.zhonguo5118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://ob.zhonguo6118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://it.zhonguo1118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://ti.zhonguo5118.cn

—— 文件结束 ——
来源：https://dp.zhonguo2118.cn

================================================================================
来源：https://up.zhonguo3118.cn

程序语言常见例子速查手册（2024 版）
来源：https://ld.zhonguo4118.cn

Common Programming Examples Cheat Book
来源：https://vu.zhonguo3118.cn

================================================================================
来源：https://qg.zhonguo5118.cn

【收录内容】
来源：https://zr.zhonguo3118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://um.zhonguo7118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://yb.zhonguo4118.cn

SQL · Bash · C · C++
来源：https://tw.zhonguo3118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://se.zhonguo6118.cn

【使用说明】
来源：https://zo.zhonguo5118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://bl.zhonguo5118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://jv.zhonguo7118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://lw.zhonguo4118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://oh.zhonguo1118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://od.zhonguo4118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://jm.zhonguo4118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://pl.zhonguo6118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://ed.zhonguo8118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://dx.zhonguo3118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://an.zhonguo7118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://bj.zhonguo7118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://er.zhonguo7118.cn

【文件统计】
来源：https://mh.zhonguo8118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://nc.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://uq.zhonguo5118.cn

目  录
来源：https://iu.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://mi.zhonguo8118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://jb.zhonguo4118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://mq.zhonguo5118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://ys.zhonguo3118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://dj.zhonguo5118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://lg.zhonguo8118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://xk.zhonguo5118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://ca.zhonguo5118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://cd.zhonguo5118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://ic.zhonguo3118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://lo.zhonguo3118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://cp.zhonguo7118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://bz.zhonguo4118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://ra.zhonguo8118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://vu.zhonguo3118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://ap.zhonguo6118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://jh.zhonguo3118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://vu.zhonguo2118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://ma.zhonguo5118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://qn.zhonguo5118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://mb.zhonguo5118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://iu.zhonguo2118.cn

================================================================================
来源：https://gd.zhonguo4118.cn

A. 基础语法与类型
来源：https://ba.zhonguo5118.cn

================================================================================
来源：https://mb.zhonguo6118.cn

[A01] Hello World
来源：https://fk.zhonguo5118.cn

Py:   print("Hello, World!")
来源：https://kt.zhonguo3118.cn

PHP:  echo "Hello, World!";
来源：https://ts.zhonguo5118.cn

JS:   console.log("Hello, World!");
来源：https://ur.zhonguo1118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://ss.zhonguo5118.cn

Java: System.out.println("Hello, World!");
来源：https://rr.zhonguo3118.cn

Go:   fmt.Println("Hello, World!")
来源：https://dv.zhonguo5118.cn

Ruby: puts "Hello, World!"
来源：https://bx.zhonguo1118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://ni.zhonguo6118.cn

[A02] 变量声明与赋值
来源：https://fu.zhonguo5118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://ff.zhonguo7118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ur.zhonguo5118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://nl.zhonguo3118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://hc.zhonguo3118.cn

Java: String name = "Alex"; int age = 20;
来源：https://iw.zhonguo7118.cn

Go:   name := "Alex"; age := 20
来源：https://ba.zhonguo7118.cn

Ruby: name = "Alex"; age = 20
来源：https://yc.zhonguo7118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://ff.zhonguo7118.cn

[A03] 常量定义
来源：https://cq.zhonguo1118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://ys.zhonguo7118.cn

PHP:  const PI = 3.14159;
来源：https://nc.zhonguo2118.cn

JS:   const PI = 3.14159;
来源：https://bx.zhonguo5118.cn

TS:   const PI: number = 3.14159;
来源：https://wm.zhonguo8118.cn

Java: static final double PI = 3.14159;
来源：https://vq.zhonguo6118.cn

Go:   const PI = 3.14159
来源：https://pa.zhonguo1118.cn

Ruby: PI = 3.14159
来源：https://ri.zhonguo5118.cn

C#:   const double PI = 3.14159;
来源：https://ak.zhonguo4118.cn

[A04] 判断变量类型
来源：https://ke.zhonguo1118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://as.zhonguo3118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://ln.zhonguo8118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://nd.zhonguo3118.cn

TS:   typeof x; x instanceof Date
来源：https://pp.zhonguo6118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://kh.zhonguo4118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://nk.zhonguo6118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://zk.zhonguo4118.cn

C#:   x.GetType().Name; x is int
来源：https://cl.zhonguo3118.cn

[A05] 整数除法与取模
来源：https://id.zhonguo7118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://io.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://zn.zhonguo1118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://co.zhonguo6118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://yr.zhonguo8118.cn

Java: 7 / 2; 7 % 2
来源：https://vc.zhonguo6118.cn

Go:   7 / 2; 7 % 2
来源：https://er.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://hl.zhonguo8118.cn

C#:   7 / 2; 7 % 2
来源：https://kl.zhonguo8118.cn

[A06] 字符串转数字
来源：https://gq.zhonguo5118.cn

Py:   int("42"); float("3.14")
来源：https://ed.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://xs.zhonguo5118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://mf.zhonguo5118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://yg.zhonguo4118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://xj.zhonguo3118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://gw.zhonguo7118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://qj.zhonguo1118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://fk.zhonguo4118.cn

[A07] 数字转字符串
来源：https://be.zhonguo2118.cn

Py:   str(42)
来源：https://nv.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://ja.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://oz.zhonguo1118.cn

TS:   String(42)
来源：https://qw.zhonguo6118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://ju.zhonguo8118.cn

Go:   strconv.Itoa(42)
来源：https://te.zhonguo4118.cn

Ruby: 42.to_s
来源：https://tw.zhonguo8118.cn

C#:   42.ToString()
来源：https://vg.zhonguo1118.cn

[A08] 取整与四舍五入
来源：https://za.zhonguo2118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://la.zhonguo1118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://ho.zhonguo4118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://tx.zhonguo5118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://tz.zhonguo7118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://dc.zhonguo5118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://dk.zhonguo4118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://ho.zhonguo7118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://ts.zhonguo6118.cn

[A09] 绝对值与最大最小值
来源：https://ob.zhonguo1118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://jr.zhonguo5118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://fj.zhonguo4118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://si.zhonguo5118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://oc.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://sf.zhonguo6118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://ws.zhonguo5118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://yx.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://vy.zhonguo6118.cn

[A10] 生成随机数
来源：https://tz.zhonguo6118.cn

Py:   import random; random.randint(1, 100)
来源：https://mb.zhonguo8118.cn

PHP:  random_int(1, 100);
来源：https://bg.zhonguo2118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://gj.zhonguo2118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://wn.zhonguo2118.cn

Java: new Random().nextInt(100) + 1
来源：https://vo.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://kc.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://le.zhonguo5118.cn

C#:   new Random().Next(1, 101)
来源：https://fs.zhonguo1118.cn

[A11] 条件表达式（三元）
来源：https://ce.zhonguo5118.cn

Py:   "yes" if x > 0 else "no"
来源：https://fi.zhonguo6118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://yd.zhonguo7118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://yl.zhonguo7118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://me.zhonguo6118.cn

Java: x > 0 ? "yes" : "no"
来源：https://zt.zhonguo3118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://xr.zhonguo7118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://vp.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://nc.zhonguo6118.cn

[A12] 字符串插值 / 格式化
来源：https://sk.zhonguo2118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://kv.zhonguo1118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://nb.zhonguo7118.cn

JS:   `Hello, ${name}!`
来源：https://pe.zhonguo3118.cn

TS:   `Hello, ${name}!`
来源：https://ai.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://op.zhonguo5118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://ue.zhonguo8118.cn

Ruby: "Hello, #{name}!"
来源：https://no.zhonguo6118.cn

C#:   $"Hello, {name}!"
来源：https://rh.zhonguo8118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://jl.zhonguo7118.cn

Py:   "第一行\n第二行"
来源：https://wr.zhonguo6118.cn

PHP:  "第一行\n第二行"
来源：https://fv.zhonguo4118.cn

JS:   "第一行\n第二行"
来源：https://lb.zhonguo4118.cn

TS:   "第一行\n第二行"
来源：https://ki.zhonguo8118.cn

Java: "第一行\n第二行"
来源：https://yn.zhonguo3118.cn

Go:   "第一行\n第二行"
来源：https://tm.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://va.zhonguo5118.cn

C#:   "第一行\n第二行"
来源：https://ph.zhonguo1118.cn

[A14] 注释写法
来源：https://on.zhonguo6118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://nm.zhonguo1118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://pj.zhonguo1118.cn

JS:   // 单行；/* 多行 */
来源：https://wf.zhonguo8118.cn

TS:   // 单行；/* 多行 */
来源：https://xf.zhonguo8118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ys.zhonguo7118.cn

Go:   // 单行；/* 多行 */
来源：https://wo.zhonguo4118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://ax.zhonguo4118.cn

C#:   // 单行；/* 多行 */
来源：https://cp.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://hk.zhonguo6118.cn

Py:   value = data or "默认值"
来源：https://gk.zhonguo6118.cn

PHP:  $value = $data ?? "默认值";
来源：https://zi.zhonguo2118.cn

JS:   const value = data ?? "默认值";
来源：https://uv.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://ou.zhonguo3118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://dl.zhonguo6118.cn

Go:   if data == "" { data = "默认值" }
来源：https://ht.zhonguo3118.cn

Ruby: value = data || "默认值"
来源：https://cd.zhonguo5118.cn

C#:   var value = data ?? "默认值";
来源：https://jr.zhonguo4118.cn

[A16] 真假值判断规则
来源：https://hv.zhonguo4118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://wv.zhonguo5118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://fg.zhonguo2118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://yh.zhonguo4118.cn

TS:   if (!x) {}
来源：https://ip.zhonguo5118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://lx.zhonguo2118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://pg.zhonguo6118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://so.zhonguo4118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://pe.zhonguo4118.cn

[A17] 位运算
来源：https://fq.zhonguo6118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ic.zhonguo1118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://jr.zhonguo6118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ak.zhonguo7118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://cl.zhonguo5118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ju.zhonguo2118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://hk.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sx.zhonguo3118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sq.zhonguo3118.cn

[A18] 字符与 ASCII 码互转
来源：https://yj.zhonguo4118.cn

Py:   ord("A"); chr(65)
来源：https://hm.zhonguo4118.cn

PHP:  ord("A"); chr(65)
来源：https://mx.zhonguo5118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://rb.zhonguo2118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://fa.zhonguo2118.cn

Java: (int) 'A'; (char) 65
来源：https://os.zhonguo2118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://cc.zhonguo4118.cn

Ruby: "A".ord; 65.chr
来源：https://pc.zhonguo7118.cn


<!-- 参考信息 -->