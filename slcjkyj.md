代发 wailian999

[U105] JS：节流
来源：https://mz.zhonguo7118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://fa.zhonguo8118.cn

[U106] JS：日期格式化
来源：https://lw.zhonguo3118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://on.zhonguo1118.cn

[U107] JS：数字千分位
来源：https://le.zhonguo5118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://uo.zhonguo6118.cn

[U108] JS：随机整数
来源：https://um.zhonguo2118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://ej.zhonguo3118.cn

[U109] JS：数组分组
来源：https://fn.zhonguo3118.cn

Object.groupBy(arr, x => x.type)
来源：https://co.zhonguo3118.cn

[U110] JS：数组分块
来源：https://mz.zhonguo5118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://sp.zhonguo4118.cn

[U111] JS：对象转 Map
来源：https://ci.zhonguo1118.cn

new Map(Object.entries(obj))
来源：https://ku.zhonguo5118.cn

[U112] JS：字符串补位
来源：https://gb.zhonguo3118.cn

"7".padStart(3, "0")
来源：https://qj.zhonguo6118.cn

[U113] JS：正则替换全部
来源：https://rk.zhonguo8118.cn

s.replaceAll("a", "b")
来源：https://da.zhonguo6118.cn

[U114] JS：JSON 深比较
来源：https://th.zhonguo2118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://lo.zhonguo6118.cn

[U115] JS：生成 UUID
来源：https://aw.zhonguo8118.cn

crypto.randomUUID()
来源：https://mo.zhonguo1118.cn

[U116] JS：类型检查（JSDoc）
来源：https://zc.zhonguo7118.cn

/** @param {string} name */ function f(name) {}
来源：https://as.zhonguo2118.cn

[U117] JS：单元测试
来源：https://pg.zhonguo2118.cn

npm i -D vitest;  npx vitest
来源：https://gt.zhonguo3118.cn

[U118] JS：开发服务器
来源：https://cn.zhonguo6118.cn

npm i -D vite;  npx vite
来源：https://yq.zhonguo4118.cn

[U119] JS：生产构建
来源：https://jt.zhonguo8118.cn

npx vite build
来源：https://uq.zhonguo1118.cn

[U120] JS：读取环境变量（Vite）
来源：https://ic.zhonguo8118.cn

import.meta.env.VITE_API_URL
来源：https://iq.zhonguo5118.cn

================================================================================
来源：https://qt.zhonguo8118.cn

统计汇总
来源：https://ks.zhonguo4118.cn

================================================================================
来源：https://gq.zhonguo8118.cn

按语言统计（条）：
来源：https://ci.zhonguo8118.cn

Python ......... 252
来源：https://yi.zhonguo4118.cn

PHP ............ 252
来源：https://fm.zhonguo8118.cn

JavaScript ..... 252
来源：https://ke.zhonguo2118.cn

TypeScript ..... 212
来源：https://zh.zhonguo4118.cn

Java ........... 212
来源：https://tv.zhonguo2118.cn

Go ............. 212
来源：https://ge.zhonguo8118.cn

Ruby ........... 212
来源：https://rg.zhonguo6118.cn

C# ............. 212
来源：https://lr.zhonguo5118.cn

C .............. 30
来源：https://em.zhonguo1118.cn

C++ ............ 30
来源：https://yj.zhonguo7118.cn

SQL ............ 90
来源：https://pf.zhonguo1118.cn

Bash ........... 80
来源：https://ki.zhonguo8118.cn

Kotlin ......... 15
来源：https://si.zhonguo7118.cn

Swift .......... 15
来源：https://sy.zhonguo5118.cn

Lua ............ 10
来源：https://nm.zhonguo6118.cn

Perl ........... 10
来源：https://mt.zhonguo7118.cn

Scala .......... 10
来源：https://cu.zhonguo3118.cn

------------------------------------
来源：https://zt.zhonguo2118.cn

合计 ........... 2106 条
来源：https://mu.zhonguo6118.cn

按章节统计：
来源：https://pp.zhonguo4118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://sf.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://te.zhonguo3118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://rl.zhonguo4118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://ea.zhonguo8118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://gi.zhonguo6118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://cl.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://ye.zhonguo6118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://eq.zhonguo1118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://hv.zhonguo1118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://kn.zhonguo2118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://gh.zhonguo6118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://zp.zhonguo2118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://bz.zhonguo5118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://ye.zhonguo4118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://qe.zhonguo5118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://up.zhonguo3118.cn

Q SQL 专题                              90
来源：https://tx.zhonguo1118.cn

R Bash 专题                             80
来源：https://gz.zhonguo4118.cn

S C / C++ 专题                          60
来源：https://mj.zhonguo4118.cn

T 其他语言补充                          60
来源：https://an.zhonguo3118.cn

U 高频实用片段                         120
来源：https://ld.zhonguo7118.cn

------------------------------------
来源：https://ve.zhonguo4118.cn

合计                                  2106 条
来源：https://in.zhonguo2118.cn

--------------------------------------------------------------------------------
来源：https://ad.zhonguo5118.cn

使用提醒
来源：https://bg.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://en.zhonguo5118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://jz.zhonguo4118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://br.zhonguo6118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://yz.zhonguo6118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://la.zhonguo5118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://od.zhonguo4118.cn

—— 文件结束 ——
来源：https://lg.zhonguo1118.cn

================================================================================
来源：https://ck.zhonguo6118.cn

程序语言常见例子速查手册（2024 版）
来源：https://ou.zhonguo2118.cn

Common Programming Examples Cheat Book
来源：https://tv.zhonguo7118.cn

================================================================================
来源：https://ju.zhonguo8118.cn

【收录内容】
来源：https://nq.zhonguo7118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://sk.zhonguo7118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://ch.zhonguo1118.cn

SQL · Bash · C · C++
来源：https://xg.zhonguo1118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://hl.zhonguo7118.cn

【使用说明】
来源：https://uv.zhonguo2118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://rp.zhonguo4118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://dm.zhonguo6118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://se.zhonguo7118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://cc.zhonguo6118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://yd.zhonguo5118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://dd.zhonguo4118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://oe.zhonguo3118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://st.zhonguo2118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://ty.zhonguo1118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://mq.zhonguo5118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://kt.zhonguo7118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://te.zhonguo8118.cn

【文件统计】
来源：https://iz.zhonguo3118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://vx.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://sn.zhonguo7118.cn

目  录
来源：https://cm.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://sy.zhonguo4118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://ju.zhonguo8118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://cc.zhonguo2118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://uv.zhonguo2118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://az.zhonguo8118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://ak.zhonguo1118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://yg.zhonguo3118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://vx.zhonguo1118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://cy.zhonguo4118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://tq.zhonguo5118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://ry.zhonguo8118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://zo.zhonguo6118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://ep.zhonguo8118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://co.zhonguo5118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://zp.zhonguo8118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://zy.zhonguo8118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://ga.zhonguo3118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://yo.zhonguo3118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://ck.zhonguo6118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ov.zhonguo4118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://bl.zhonguo3118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://nx.zhonguo7118.cn

================================================================================
来源：https://vq.zhonguo6118.cn

A. 基础语法与类型
来源：https://xg.zhonguo5118.cn

================================================================================
来源：https://yl.zhonguo2118.cn

[A01] Hello World
来源：https://ak.zhonguo4118.cn

Py:   print("Hello, World!")
来源：https://tb.zhonguo3118.cn

PHP:  echo "Hello, World!";
来源：https://lk.zhonguo8118.cn

JS:   console.log("Hello, World!");
来源：https://xd.zhonguo2118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://ww.zhonguo4118.cn

Java: System.out.println("Hello, World!");
来源：https://fo.zhonguo5118.cn

Go:   fmt.Println("Hello, World!")
来源：https://as.zhonguo8118.cn

Ruby: puts "Hello, World!"
来源：https://gx.zhonguo2118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://tj.zhonguo4118.cn

[A02] 变量声明与赋值
来源：https://oq.zhonguo6118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://mg.zhonguo5118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ji.zhonguo1118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://yv.zhonguo6118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://ul.zhonguo5118.cn

Java: String name = "Alex"; int age = 20;
来源：https://ct.zhonguo1118.cn

Go:   name := "Alex"; age := 20
来源：https://sj.zhonguo7118.cn

Ruby: name = "Alex"; age = 20
来源：https://sd.zhonguo6118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://ek.zhonguo5118.cn

[A03] 常量定义
来源：https://zw.zhonguo7118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://wi.zhonguo4118.cn

PHP:  const PI = 3.14159;
来源：https://mx.zhonguo6118.cn

JS:   const PI = 3.14159;
来源：https://dy.zhonguo1118.cn

TS:   const PI: number = 3.14159;
来源：https://ua.zhonguo6118.cn

Java: static final double PI = 3.14159;
来源：https://am.zhonguo3118.cn

Go:   const PI = 3.14159
来源：https://sw.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://yt.zhonguo2118.cn

C#:   const double PI = 3.14159;
来源：https://gp.zhonguo4118.cn

[A04] 判断变量类型
来源：https://wf.zhonguo7118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://fh.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://fo.zhonguo3118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://uz.zhonguo4118.cn

TS:   typeof x; x instanceof Date
来源：https://ao.zhonguo5118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://ul.zhonguo3118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://dl.zhonguo5118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://dy.zhonguo1118.cn

C#:   x.GetType().Name; x is int
来源：https://xc.zhonguo2118.cn

[A05] 整数除法与取模
来源：https://cp.zhonguo7118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://dq.zhonguo8118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://lf.zhonguo3118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://xn.zhonguo7118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://zh.zhonguo7118.cn

Java: 7 / 2; 7 % 2
来源：https://wi.zhonguo7118.cn

Go:   7 / 2; 7 % 2
来源：https://it.zhonguo5118.cn

Ruby: 7 / 2; 7 % 2
来源：https://vf.zhonguo5118.cn

C#:   7 / 2; 7 % 2
来源：https://qp.zhonguo7118.cn

[A06] 字符串转数字
来源：https://nf.zhonguo3118.cn

Py:   int("42"); float("3.14")
来源：https://iy.zhonguo1118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://cz.zhonguo3118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://eg.zhonguo7118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://yr.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://zq.zhonguo7118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://tj.zhonguo4118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://gu.zhonguo2118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://uo.zhonguo7118.cn

[A07] 数字转字符串
来源：https://kv.zhonguo5118.cn

Py:   str(42)
来源：https://qk.zhonguo5118.cn

PHP:  (string) 42; strval(42)
来源：https://ap.zhonguo5118.cn

JS:   String(42); (42).toString()
来源：https://de.zhonguo4118.cn

TS:   String(42)
来源：https://cm.zhonguo4118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://in.zhonguo5118.cn

Go:   strconv.Itoa(42)
来源：https://pc.zhonguo5118.cn

Ruby: 42.to_s
来源：https://od.zhonguo2118.cn

C#:   42.ToString()
来源：https://vo.zhonguo6118.cn

[A08] 取整与四舍五入
来源：https://rx.zhonguo1118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://uz.zhonguo1118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://qg.zhonguo8118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://tq.zhonguo4118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://vk.zhonguo7118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://no.zhonguo2118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://lw.zhonguo1118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://yn.zhonguo4118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://op.zhonguo4118.cn

[A09] 绝对值与最大最小值
来源：https://ne.zhonguo6118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://xw.zhonguo2118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://wt.zhonguo7118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://xu.zhonguo6118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ov.zhonguo1118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://gy.zhonguo2118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://at.zhonguo2118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://hz.zhonguo5118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://pa.zhonguo7118.cn

[A10] 生成随机数
来源：https://sb.zhonguo2118.cn

Py:   import random; random.randint(1, 100)
来源：https://pl.zhonguo3118.cn

PHP:  random_int(1, 100);
来源：https://ct.zhonguo8118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://gs.zhonguo8118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://ps.zhonguo2118.cn

Java: new Random().nextInt(100) + 1
来源：https://ay.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://dw.zhonguo3118.cn

Ruby: rand(1..100)
来源：https://pa.zhonguo6118.cn

C#:   new Random().Next(1, 101)
来源：https://cf.zhonguo3118.cn

[A11] 条件表达式（三元）
来源：https://hx.zhonguo4118.cn

Py:   "yes" if x > 0 else "no"
来源：https://np.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://qz.zhonguo6118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ru.zhonguo2118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://mg.zhonguo2118.cn

Java: x > 0 ? "yes" : "no"
来源：https://sr.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://lw.zhonguo1118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://cf.zhonguo5118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://in.zhonguo3118.cn

[A12] 字符串插值 / 格式化
来源：https://gp.zhonguo4118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://jq.zhonguo5118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://gw.zhonguo5118.cn

JS:   `Hello, ${name}!`
来源：https://mt.zhonguo2118.cn

TS:   `Hello, ${name}!`
来源：https://ck.zhonguo3118.cn

Java: "Hello, %s!".formatted(name)
来源：https://xr.zhonguo5118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://xe.zhonguo1118.cn

Ruby: "Hello, #{name}!"
来源：https://gu.zhonguo6118.cn

C#:   $"Hello, {name}!"
来源：https://mt.zhonguo1118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://ee.zhonguo8118.cn

Py:   "第一行\n第二行"
来源：https://cv.zhonguo2118.cn

PHP:  "第一行\n第二行"
来源：https://wj.zhonguo3118.cn

JS:   "第一行\n第二行"
来源：https://qu.zhonguo2118.cn

TS:   "第一行\n第二行"
来源：https://wy.zhonguo7118.cn

Java: "第一行\n第二行"
来源：https://bs.zhonguo2118.cn

Go:   "第一行\n第二行"
来源：https://ny.zhonguo5118.cn

Ruby: "第一行\n第二行"
来源：https://yw.zhonguo8118.cn

C#:   "第一行\n第二行"
来源：https://vj.zhonguo7118.cn

[A14] 注释写法
来源：https://hf.zhonguo2118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://dl.zhonguo6118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://oe.zhonguo6118.cn

JS:   // 单行；/* 多行 */
来源：https://yw.zhonguo7118.cn

TS:   // 单行；/* 多行 */
来源：https://ux.zhonguo8118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://ya.zhonguo5118.cn

Go:   // 单行；/* 多行 */
来源：https://yi.zhonguo6118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://mt.zhonguo1118.cn

C#:   // 单行；/* 多行 */
来源：https://dd.zhonguo2118.cn

[A15] 空值判断与默认值
来源：https://do.zhonguo3118.cn

Py:   value = data or "默认值"
来源：https://wc.zhonguo4118.cn

PHP:  $value = $data ?? "默认值";
来源：https://qm.zhonguo1118.cn

JS:   const value = data ?? "默认值";
来源：https://ru.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://mh.zhonguo1118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://un.zhonguo5118.cn

Go:   if data == "" { data = "默认值" }
来源：https://vr.zhonguo2118.cn

Ruby: value = data || "默认值"
来源：https://kw.zhonguo3118.cn

C#:   var value = data ?? "默认值";
来源：https://nc.zhonguo5118.cn

[A16] 真假值判断规则
来源：https://rc.zhonguo7118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://ut.zhonguo3118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://ay.zhonguo7118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://pg.zhonguo1118.cn

TS:   if (!x) {}
来源：https://vz.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://ld.zhonguo6118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://sy.zhonguo2118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://tz.zhonguo6118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://av.zhonguo3118.cn

[A17] 位运算
来源：https://kl.zhonguo1118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://kh.zhonguo3118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://ub.zhonguo3118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://sn.zhonguo3118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://ds.zhonguo3118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ik.zhonguo5118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://fu.zhonguo2118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://mj.zhonguo2118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://jc.zhonguo7118.cn

[A18] 字符与 ASCII 码互转
来源：https://gg.zhonguo2118.cn

Py:   ord("A"); chr(65)
来源：https://ff.zhonguo7118.cn

PHP:  ord("A"); chr(65)
来源：https://kd.zhonguo2118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://kl.zhonguo4118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://sd.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://dy.zhonguo1118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://ew.zhonguo2118.cn

Ruby: "A".ord; 65.chr
来源：https://lf.zhonguo8118.cn


<!-- 参考信息 -->