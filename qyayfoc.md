代发 wailian999

[U105] JS：节流
来源：https://sp.zhonguo5118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://nf.zhonguo7118.cn

[U106] JS：日期格式化
来源：https://bh.zhonguo6118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://yq.zhonguo8118.cn

[U107] JS：数字千分位
来源：https://et.zhonguo4118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://hb.zhonguo5118.cn

[U108] JS：随机整数
来源：https://wj.zhonguo4118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://sv.zhonguo3118.cn

[U109] JS：数组分组
来源：https://zu.zhonguo8118.cn

Object.groupBy(arr, x => x.type)
来源：https://yw.zhonguo4118.cn

[U110] JS：数组分块
来源：https://vc.zhonguo2118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://vz.zhonguo6118.cn

[U111] JS：对象转 Map
来源：https://le.zhonguo2118.cn

new Map(Object.entries(obj))
来源：https://zd.zhonguo1118.cn

[U112] JS：字符串补位
来源：https://sj.zhonguo7118.cn

"7".padStart(3, "0")
来源：https://jt.zhonguo2118.cn

[U113] JS：正则替换全部
来源：https://pn.zhonguo8118.cn

s.replaceAll("a", "b")
来源：https://zz.zhonguo4118.cn

[U114] JS：JSON 深比较
来源：https://yd.zhonguo4118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://af.zhonguo1118.cn

[U115] JS：生成 UUID
来源：https://kn.zhonguo3118.cn

crypto.randomUUID()
来源：https://hj.zhonguo3118.cn

[U116] JS：类型检查（JSDoc）
来源：https://rc.zhonguo7118.cn

/** @param {string} name */ function f(name) {}
来源：https://jz.zhonguo4118.cn

[U117] JS：单元测试
来源：https://zq.zhonguo7118.cn

npm i -D vitest;  npx vitest
来源：https://mh.zhonguo1118.cn

[U118] JS：开发服务器
来源：https://fc.zhonguo4118.cn

npm i -D vite;  npx vite
来源：https://gd.zhonguo6118.cn

[U119] JS：生产构建
来源：https://db.zhonguo6118.cn

npx vite build
来源：https://vn.zhonguo3118.cn

[U120] JS：读取环境变量（Vite）
来源：https://ee.zhonguo6118.cn

import.meta.env.VITE_API_URL
来源：https://sr.zhonguo4118.cn

================================================================================
来源：https://hr.zhonguo2118.cn

统计汇总
来源：https://lo.zhonguo5118.cn

================================================================================
来源：https://kt.zhonguo4118.cn

按语言统计（条）：
来源：https://hl.zhonguo8118.cn

Python ......... 252
来源：https://wa.zhonguo3118.cn

PHP ............ 252
来源：https://uf.zhonguo2118.cn

JavaScript ..... 252
来源：https://wf.zhonguo5118.cn

TypeScript ..... 212
来源：https://gi.zhonguo4118.cn

Java ........... 212
来源：https://wl.zhonguo3118.cn

Go ............. 212
来源：https://nv.zhonguo1118.cn

Ruby ........... 212
来源：https://wt.zhonguo7118.cn

C# ............. 212
来源：https://sm.zhonguo6118.cn

C .............. 30
来源：https://ve.zhonguo6118.cn

C++ ............ 30
来源：https://cs.zhonguo7118.cn

SQL ............ 90
来源：https://bb.zhonguo3118.cn

Bash ........... 80
来源：https://nn.zhonguo7118.cn

Kotlin ......... 15
来源：https://wq.zhonguo3118.cn

Swift .......... 15
来源：https://va.zhonguo5118.cn

Lua ............ 10
来源：https://kv.zhonguo7118.cn

Perl ........... 10
来源：https://ty.zhonguo7118.cn

Scala .......... 10
来源：https://nz.zhonguo7118.cn

------------------------------------
来源：https://pj.zhonguo2118.cn

合计 ........... 2106 条
来源：https://lm.zhonguo3118.cn

按章节统计：
来源：https://di.zhonguo6118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://lz.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://sk.zhonguo7118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://hx.zhonguo3118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://rg.zhonguo7118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://cq.zhonguo8118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://jt.zhonguo6118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://nr.zhonguo8118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://bo.zhonguo8118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://hx.zhonguo7118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://wx.zhonguo3118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://op.zhonguo7118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://gx.zhonguo1118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://eo.zhonguo5118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://qv.zhonguo7118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://ft.zhonguo2118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://rz.zhonguo4118.cn

Q SQL 专题                              90
来源：https://wd.zhonguo1118.cn

R Bash 专题                             80
来源：https://xi.zhonguo6118.cn

S C / C++ 专题                          60
来源：https://xh.zhonguo5118.cn

T 其他语言补充                          60
来源：https://ga.zhonguo7118.cn

U 高频实用片段                         120
来源：https://ni.zhonguo4118.cn

------------------------------------
来源：https://ne.zhonguo3118.cn

合计                                  2106 条
来源：https://au.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://hu.zhonguo5118.cn

使用提醒
来源：https://zu.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://wm.zhonguo2118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://ro.zhonguo2118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://ul.zhonguo7118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://ef.zhonguo1118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://jy.zhonguo7118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://wn.zhonguo7118.cn

—— 文件结束 ——
来源：https://pd.zhonguo5118.cn

================================================================================
来源：https://it.zhonguo1118.cn

程序语言常见例子速查手册（2024 版）
来源：https://mu.zhonguo3118.cn

Common Programming Examples Cheat Book
来源：https://ms.zhonguo3118.cn

================================================================================
来源：https://lq.zhonguo8118.cn

【收录内容】
来源：https://pn.zhonguo3118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://xx.zhonguo4118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://vo.zhonguo8118.cn

SQL · Bash · C · C++
来源：https://ki.zhonguo6118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://nr.zhonguo4118.cn

【使用说明】
来源：https://ac.zhonguo4118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://wi.zhonguo4118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://zo.zhonguo7118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://mc.zhonguo4118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://fy.zhonguo4118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://xn.zhonguo6118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://mi.zhonguo7118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://eg.zhonguo1118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://wl.zhonguo4118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://qh.zhonguo5118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://yb.zhonguo2118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://lx.zhonguo8118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://pg.zhonguo3118.cn

【文件统计】
来源：https://ko.zhonguo1118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://xw.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://xj.zhonguo1118.cn

目  录
来源：https://xq.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://ch.zhonguo7118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://uh.zhonguo1118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://vo.zhonguo2118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://vh.zhonguo5118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://re.zhonguo8118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://ek.zhonguo5118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://iu.zhonguo4118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://ga.zhonguo7118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://gm.zhonguo6118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://ho.zhonguo8118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://tj.zhonguo8118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://zc.zhonguo5118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://gz.zhonguo6118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://hj.zhonguo5118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://nm.zhonguo5118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://ah.zhonguo4118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://bi.zhonguo8118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://em.zhonguo2118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://sf.zhonguo6118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://at.zhonguo7118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://xq.zhonguo1118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://eh.zhonguo3118.cn

================================================================================
来源：https://it.zhonguo6118.cn

A. 基础语法与类型
来源：https://ne.zhonguo4118.cn

================================================================================
来源：https://nd.zhonguo4118.cn

[A01] Hello World
来源：https://xu.zhonguo8118.cn

Py:   print("Hello, World!")
来源：https://lh.zhonguo5118.cn

PHP:  echo "Hello, World!";
来源：https://dw.zhonguo4118.cn

JS:   console.log("Hello, World!");
来源：https://bj.zhonguo6118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://gp.zhonguo8118.cn

Java: System.out.println("Hello, World!");
来源：https://bx.zhonguo4118.cn

Go:   fmt.Println("Hello, World!")
来源：https://rl.zhonguo4118.cn

Ruby: puts "Hello, World!"
来源：https://bc.zhonguo2118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://jp.zhonguo4118.cn

[A02] 变量声明与赋值
来源：https://lj.zhonguo3118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://cc.zhonguo7118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://jn.zhonguo3118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://qc.zhonguo2118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://yc.zhonguo8118.cn

Java: String name = "Alex"; int age = 20;
来源：https://st.zhonguo6118.cn

Go:   name := "Alex"; age := 20
来源：https://ju.zhonguo3118.cn

Ruby: name = "Alex"; age = 20
来源：https://lo.zhonguo3118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://dj.zhonguo8118.cn

[A03] 常量定义
来源：https://wt.zhonguo2118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://su.zhonguo5118.cn

PHP:  const PI = 3.14159;
来源：https://ic.zhonguo3118.cn

JS:   const PI = 3.14159;
来源：https://tr.zhonguo1118.cn

TS:   const PI: number = 3.14159;
来源：https://if.zhonguo4118.cn

Java: static final double PI = 3.14159;
来源：https://lt.zhonguo4118.cn

Go:   const PI = 3.14159
来源：https://ou.zhonguo4118.cn

Ruby: PI = 3.14159
来源：https://ie.zhonguo7118.cn

C#:   const double PI = 3.14159;
来源：https://zx.zhonguo6118.cn

[A04] 判断变量类型
来源：https://yz.zhonguo3118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://ux.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://px.zhonguo3118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://qa.zhonguo4118.cn

TS:   typeof x; x instanceof Date
来源：https://oj.zhonguo6118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://xc.zhonguo5118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://js.zhonguo6118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://be.zhonguo3118.cn

C#:   x.GetType().Name; x is int
来源：https://pi.zhonguo2118.cn

[A05] 整数除法与取模
来源：https://ww.zhonguo1118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://gg.zhonguo1118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://tk.zhonguo3118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://bo.zhonguo2118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://ao.zhonguo4118.cn

Java: 7 / 2; 7 % 2
来源：https://xy.zhonguo1118.cn

Go:   7 / 2; 7 % 2
来源：https://jg.zhonguo4118.cn

Ruby: 7 / 2; 7 % 2
来源：https://hq.zhonguo6118.cn

C#:   7 / 2; 7 % 2
来源：https://wt.zhonguo3118.cn

[A06] 字符串转数字
来源：https://bb.zhonguo8118.cn

Py:   int("42"); float("3.14")
来源：https://ym.zhonguo5118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://no.zhonguo4118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://jf.zhonguo4118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://ql.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://zp.zhonguo3118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://pn.zhonguo2118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://vs.zhonguo3118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://dh.zhonguo6118.cn

[A07] 数字转字符串
来源：https://tm.zhonguo7118.cn

Py:   str(42)
来源：https://hd.zhonguo7118.cn

PHP:  (string) 42; strval(42)
来源：https://ea.zhonguo5118.cn

JS:   String(42); (42).toString()
来源：https://my.zhonguo4118.cn

TS:   String(42)
来源：https://fr.zhonguo7118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://xa.zhonguo2118.cn

Go:   strconv.Itoa(42)
来源：https://xu.zhonguo4118.cn

Ruby: 42.to_s
来源：https://cr.zhonguo2118.cn

C#:   42.ToString()
来源：https://ci.zhonguo4118.cn

[A08] 取整与四舍五入
来源：https://as.zhonguo3118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://zi.zhonguo7118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://tj.zhonguo4118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://ga.zhonguo6118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://wo.zhonguo2118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://si.zhonguo4118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://iw.zhonguo4118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://ny.zhonguo8118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://hj.zhonguo6118.cn

[A09] 绝对值与最大最小值
来源：https://ir.zhonguo3118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://zh.zhonguo1118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://hv.zhonguo3118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://rh.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://xb.zhonguo3118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://my.zhonguo1118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://cn.zhonguo2118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://gr.zhonguo3118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://na.zhonguo7118.cn

[A10] 生成随机数
来源：https://st.zhonguo2118.cn

Py:   import random; random.randint(1, 100)
来源：https://ri.zhonguo5118.cn

PHP:  random_int(1, 100);
来源：https://oy.zhonguo5118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://wl.zhonguo1118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://cd.zhonguo4118.cn

Java: new Random().nextInt(100) + 1
来源：https://sm.zhonguo4118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://oj.zhonguo7118.cn

Ruby: rand(1..100)
来源：https://lx.zhonguo5118.cn

C#:   new Random().Next(1, 101)
来源：https://pm.zhonguo1118.cn

[A11] 条件表达式（三元）
来源：https://gd.zhonguo4118.cn

Py:   "yes" if x > 0 else "no"
来源：https://yn.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://bi.zhonguo5118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ym.zhonguo1118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://xj.zhonguo1118.cn

Java: x > 0 ? "yes" : "no"
来源：https://qv.zhonguo6118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://vy.zhonguo3118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://on.zhonguo5118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://dm.zhonguo5118.cn

[A12] 字符串插值 / 格式化
来源：https://tm.zhonguo6118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://tv.zhonguo4118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://sl.zhonguo3118.cn

JS:   `Hello, ${name}!`
来源：https://hh.zhonguo1118.cn

TS:   `Hello, ${name}!`
来源：https://xg.zhonguo6118.cn

Java: "Hello, %s!".formatted(name)
来源：https://hu.zhonguo3118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://cu.zhonguo3118.cn

Ruby: "Hello, #{name}!"
来源：https://gr.zhonguo8118.cn

C#:   $"Hello, {name}!"
来源：https://xt.zhonguo4118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://xr.zhonguo1118.cn

Py:   "第一行\n第二行"
来源：https://hp.zhonguo6118.cn

PHP:  "第一行\n第二行"
来源：https://lw.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://md.zhonguo1118.cn

TS:   "第一行\n第二行"
来源：https://df.zhonguo3118.cn

Java: "第一行\n第二行"
来源：https://pj.zhonguo5118.cn

Go:   "第一行\n第二行"
来源：https://wp.zhonguo3118.cn

Ruby: "第一行\n第二行"
来源：https://lp.zhonguo4118.cn

C#:   "第一行\n第二行"
来源：https://wo.zhonguo1118.cn

[A14] 注释写法
来源：https://lm.zhonguo7118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://ce.zhonguo8118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://al.zhonguo5118.cn

JS:   // 单行；/* 多行 */
来源：https://yl.zhonguo1118.cn

TS:   // 单行；/* 多行 */
来源：https://fw.zhonguo8118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://il.zhonguo7118.cn

Go:   // 单行；/* 多行 */
来源：https://ab.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://pp.zhonguo4118.cn

C#:   // 单行；/* 多行 */
来源：https://jm.zhonguo1118.cn

[A15] 空值判断与默认值
来源：https://gp.zhonguo7118.cn

Py:   value = data or "默认值"
来源：https://hd.zhonguo2118.cn

PHP:  $value = $data ?? "默认值";
来源：https://xs.zhonguo4118.cn

JS:   const value = data ?? "默认值";
来源：https://es.zhonguo2118.cn

TS:   const value = data ?? "默认值";
来源：https://jb.zhonguo8118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://zb.zhonguo3118.cn

Go:   if data == "" { data = "默认值" }
来源：https://jc.zhonguo1118.cn

Ruby: value = data || "默认值"
来源：https://pk.zhonguo1118.cn

C#:   var value = data ?? "默认值";
来源：https://kk.zhonguo4118.cn

[A16] 真假值判断规则
来源：https://et.zhonguo3118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://fq.zhonguo8118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://ja.zhonguo1118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://qk.zhonguo8118.cn

TS:   if (!x) {}
来源：https://ds.zhonguo8118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://yy.zhonguo8118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://yb.zhonguo3118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://sc.zhonguo5118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://sr.zhonguo3118.cn

[A17] 位运算
来源：https://wx.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ny.zhonguo2118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://di.zhonguo1118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://kg.zhonguo6118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://tn.zhonguo7118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://nz.zhonguo6118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://tf.zhonguo5118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://ja.zhonguo6118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://is.zhonguo8118.cn

[A18] 字符与 ASCII 码互转
来源：https://sj.zhonguo8118.cn

Py:   ord("A"); chr(65)
来源：https://xm.zhonguo2118.cn

PHP:  ord("A"); chr(65)
来源：https://oj.zhonguo3118.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://fy.zhonguo3118.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：https://qx.zhonguo8118.cn

Java: (int) 'A'; (char) 65
来源：https://tm.zhonguo7118.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：https://ty.zhonguo2118.cn

Ruby: "A".ord; 65.chr
来源：https://pz.zhonguo4118.cn


<!-- 参考信息 -->