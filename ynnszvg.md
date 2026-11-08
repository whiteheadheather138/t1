代发 wailian999

[U101] JS：classList 操作
来源：https://qz.zhonguo8118.cn

el.classList.toggle("active")
来源：https://lu.zhonguo4118.cn

[U102] JS：本地存储
来源：https://tp.zhonguo3118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://xo.zhonguo3118.cn

[U103] JS：定时器
来源：https://bz.zhonguo8118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://zs.zhonguo8118.cn

[U104] JS：防抖
来源：https://kl.zhonguo2118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://np.zhonguo1118.cn

[U105] JS：节流
来源：https://pa.zhonguo8118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://an.zhonguo7118.cn

[U106] JS：日期格式化
来源：https://ih.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://tv.zhonguo8118.cn

[U107] JS：数字千分位
来源：https://vw.zhonguo1118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://mg.zhonguo4118.cn

[U108] JS：随机整数
来源：https://wy.zhonguo1118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://cc.zhonguo1118.cn

[U109] JS：数组分组
来源：https://ve.zhonguo1118.cn

Object.groupBy(arr, x => x.type)
来源：https://qf.zhonguo1118.cn

[U110] JS：数组分块
来源：https://wj.zhonguo4118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://tc.zhonguo6118.cn

[U111] JS：对象转 Map
来源：https://ti.zhonguo8118.cn

new Map(Object.entries(obj))
来源：https://fz.zhonguo4118.cn

[U112] JS：字符串补位
来源：https://kg.zhonguo4118.cn

"7".padStart(3, "0")
来源：https://zx.zhonguo3118.cn

[U113] JS：正则替换全部
来源：https://tu.zhonguo7118.cn

s.replaceAll("a", "b")
来源：https://rs.zhonguo6118.cn

[U114] JS：JSON 深比较
来源：https://jb.zhonguo5118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://wm.zhonguo2118.cn

[U115] JS：生成 UUID
来源：https://ze.zhonguo2118.cn

crypto.randomUUID()
来源：https://fn.zhonguo5118.cn

[U116] JS：类型检查（JSDoc）
来源：https://vp.zhonguo6118.cn

/** @param {string} name */ function f(name) {}
来源：https://sn.zhonguo1118.cn

[U117] JS：单元测试
来源：https://mu.zhonguo7118.cn

npm i -D vitest;  npx vitest
来源：https://yb.zhonguo7118.cn

[U118] JS：开发服务器
来源：https://ts.zhonguo5118.cn

npm i -D vite;  npx vite
来源：https://ih.zhonguo4118.cn

[U119] JS：生产构建
来源：https://qw.zhonguo7118.cn

npx vite build
来源：https://er.zhonguo5118.cn

[U120] JS：读取环境变量（Vite）
来源：https://on.zhonguo1118.cn

import.meta.env.VITE_API_URL
来源：https://mx.zhonguo3118.cn

================================================================================
来源：https://ro.zhonguo2118.cn

统计汇总
来源：https://ji.zhonguo4118.cn

================================================================================
来源：https://nn.zhonguo2118.cn

按语言统计（条）：
来源：https://hp.zhonguo2118.cn

Python ......... 252
来源：https://qf.zhonguo4118.cn

PHP ............ 252
来源：https://xd.zhonguo5118.cn

JavaScript ..... 252
来源：https://ng.zhonguo7118.cn

TypeScript ..... 212
来源：https://ox.zhonguo7118.cn

Java ........... 212
来源：https://je.zhonguo7118.cn

Go ............. 212
来源：https://pi.zhonguo8118.cn

Ruby ........... 212
来源：https://qx.zhonguo7118.cn

C# ............. 212
来源：https://zn.zhonguo4118.cn

C .............. 30
来源：https://yn.zhonguo2118.cn

C++ ............ 30
来源：https://nt.zhonguo6118.cn

SQL ............ 90
来源：https://kw.zhonguo4118.cn

Bash ........... 80
来源：https://vf.zhonguo3118.cn

Kotlin ......... 15
来源：https://th.zhonguo6118.cn

Swift .......... 15
来源：https://xh.zhonguo7118.cn

Lua ............ 10
来源：https://qu.zhonguo1118.cn

Perl ........... 10
来源：https://kt.zhonguo2118.cn

Scala .......... 10
来源：https://db.zhonguo1118.cn

------------------------------------
来源：https://wx.zhonguo8118.cn

合计 ........... 2106 条
来源：https://ac.zhonguo6118.cn

按章节统计：
来源：https://vs.zhonguo4118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://ep.zhonguo6118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://hg.zhonguo1118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://vl.zhonguo5118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://jy.zhonguo6118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://yc.zhonguo8118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://oe.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://ye.zhonguo3118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://ca.zhonguo8118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://ql.zhonguo7118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://nn.zhonguo8118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://qj.zhonguo4118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://ug.zhonguo3118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://yp.zhonguo5118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://lm.zhonguo7118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://zz.zhonguo4118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://nl.zhonguo3118.cn

Q SQL 专题                              90
来源：https://li.zhonguo3118.cn

R Bash 专题                             80
来源：https://am.zhonguo8118.cn

S C / C++ 专题                          60
来源：https://hd.zhonguo8118.cn

T 其他语言补充                          60
来源：https://vr.zhonguo6118.cn

U 高频实用片段                         120
来源：https://uk.zhonguo2118.cn

------------------------------------
来源：https://bz.zhonguo6118.cn

合计                                  2106 条
来源：https://ob.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://rd.zhonguo3118.cn

使用提醒
来源：https://wy.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://dn.zhonguo4118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://hc.zhonguo2118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://xy.zhonguo1118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://cv.zhonguo3118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://gb.zhonguo5118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://hf.zhonguo4118.cn

—— 文件结束 ——
来源：https://ta.zhonguo4118.cn

================================================================================
来源：https://jh.zhonguo1118.cn

程序语言常见例子速查手册（2024 版）
来源：https://nw.zhonguo5118.cn

Common Programming Examples Cheat Book
来源：https://ak.zhonguo6118.cn

================================================================================
来源：https://ug.zhonguo4118.cn

【收录内容】
来源：https://cw.zhonguo1118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://bh.zhonguo6118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://pi.zhonguo4118.cn

SQL · Bash · C · C++
来源：https://uo.zhonguo3118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://go.zhonguo8118.cn

【使用说明】
来源：https://jd.zhonguo7118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://su.zhonguo3118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://vz.zhonguo3118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://uu.zhonguo3118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://mi.zhonguo1118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://dd.zhonguo6118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://vc.zhonguo1118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://vh.zhonguo1118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://oc.zhonguo6118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://bo.zhonguo7118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://ub.zhonguo7118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://cj.zhonguo8118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://zo.zhonguo4118.cn

【文件统计】
来源：https://ul.zhonguo4118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://hu.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://st.zhonguo6118.cn

目  录
来源：https://jp.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://kc.zhonguo2118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://ep.zhonguo2118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://jo.zhonguo3118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://xc.zhonguo8118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://gp.zhonguo3118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://oz.zhonguo3118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://hx.zhonguo2118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://zg.zhonguo3118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://sq.zhonguo6118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://ql.zhonguo1118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://ob.zhonguo6118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://fo.zhonguo8118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://sy.zhonguo5118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://al.zhonguo7118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://gw.zhonguo8118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://rl.zhonguo6118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://gu.zhonguo7118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://yb.zhonguo1118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://ig.zhonguo5118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://zo.zhonguo2118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://wn.zhonguo3118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://jf.zhonguo3118.cn

================================================================================
来源：https://js.zhonguo8118.cn

A. 基础语法与类型
来源：https://jq.zhonguo3118.cn

================================================================================
来源：https://nw.zhonguo4118.cn

[A01] Hello World
来源：https://dk.zhonguo4118.cn

Py:   print("Hello, World!")
来源：https://mf.zhonguo1118.cn

PHP:  echo "Hello, World!";
来源：https://mt.zhonguo1118.cn

JS:   console.log("Hello, World!");
来源：https://ek.zhonguo5118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://pn.zhonguo5118.cn

Java: System.out.println("Hello, World!");
来源：https://oq.zhonguo5118.cn

Go:   fmt.Println("Hello, World!")
来源：https://ne.zhonguo5118.cn

Ruby: puts "Hello, World!"
来源：https://th.zhonguo1118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://mm.zhonguo5118.cn

[A02] 变量声明与赋值
来源：https://vh.zhonguo1118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://rt.zhonguo6118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://fn.zhonguo3118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://gt.zhonguo7118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://qj.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://fm.zhonguo6118.cn

Go:   name := "Alex"; age := 20
来源：https://ix.zhonguo6118.cn

Ruby: name = "Alex"; age = 20
来源：https://ax.zhonguo5118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://hd.zhonguo5118.cn

[A03] 常量定义
来源：https://vh.zhonguo5118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://or.zhonguo4118.cn

PHP:  const PI = 3.14159;
来源：https://sd.zhonguo5118.cn

JS:   const PI = 3.14159;
来源：https://lv.zhonguo4118.cn

TS:   const PI: number = 3.14159;
来源：https://wi.zhonguo1118.cn

Java: static final double PI = 3.14159;
来源：https://pk.zhonguo7118.cn

Go:   const PI = 3.14159
来源：https://ii.zhonguo3118.cn

Ruby: PI = 3.14159
来源：https://xy.zhonguo4118.cn

C#:   const double PI = 3.14159;
来源：https://ht.zhonguo6118.cn

[A04] 判断变量类型
来源：https://un.zhonguo7118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://qv.zhonguo5118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://fw.zhonguo1118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://xy.zhonguo2118.cn

TS:   typeof x; x instanceof Date
来源：https://ra.zhonguo2118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://ed.zhonguo8118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://rv.zhonguo5118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://gw.zhonguo8118.cn

C#:   x.GetType().Name; x is int
来源：https://og.zhonguo4118.cn

[A05] 整数除法与取模
来源：https://kv.zhonguo8118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://bw.zhonguo3118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://ed.zhonguo8118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://dp.zhonguo6118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://tc.zhonguo4118.cn

Java: 7 / 2; 7 % 2
来源：https://wn.zhonguo1118.cn

Go:   7 / 2; 7 % 2
来源：https://sd.zhonguo3118.cn

Ruby: 7 / 2; 7 % 2
来源：https://cg.zhonguo4118.cn

C#:   7 / 2; 7 % 2
来源：https://lw.zhonguo4118.cn

[A06] 字符串转数字
来源：https://dw.zhonguo7118.cn

Py:   int("42"); float("3.14")
来源：https://yj.zhonguo3118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://jz.zhonguo6118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://wf.zhonguo7118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://zu.zhonguo3118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://lm.zhonguo8118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://ds.zhonguo5118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://qz.zhonguo8118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://bc.zhonguo2118.cn

[A07] 数字转字符串
来源：https://fs.zhonguo4118.cn

Py:   str(42)
来源：https://db.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://jm.zhonguo8118.cn

JS:   String(42); (42).toString()
来源：https://rm.zhonguo3118.cn

TS:   String(42)
来源：https://te.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://fh.zhonguo1118.cn

Go:   strconv.Itoa(42)
来源：https://sw.zhonguo8118.cn

Ruby: 42.to_s
来源：https://qj.zhonguo4118.cn

C#:   42.ToString()
来源：https://jo.zhonguo8118.cn

[A08] 取整与四舍五入
来源：https://vy.zhonguo7118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ga.zhonguo3118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://gc.zhonguo1118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://gq.zhonguo4118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://wo.zhonguo7118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://yc.zhonguo8118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://px.zhonguo7118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://ce.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://za.zhonguo4118.cn

[A09] 绝对值与最大最小值
来源：https://nu.zhonguo4118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://zm.zhonguo1118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://rk.zhonguo2118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://cl.zhonguo7118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ui.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://cd.zhonguo3118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://lf.zhonguo1118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://zp.zhonguo4118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://yi.zhonguo4118.cn

[A10] 生成随机数
来源：https://pw.zhonguo4118.cn

Py:   import random; random.randint(1, 100)
来源：https://ny.zhonguo5118.cn

PHP:  random_int(1, 100);
来源：https://jd.zhonguo8118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://pd.zhonguo6118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://pe.zhonguo8118.cn

Java: new Random().nextInt(100) + 1
来源：https://as.zhonguo1118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://hb.zhonguo8118.cn

Ruby: rand(1..100)
来源：https://na.zhonguo8118.cn

C#:   new Random().Next(1, 101)
来源：https://yd.zhonguo8118.cn

[A11] 条件表达式（三元）
来源：https://gf.zhonguo6118.cn

Py:   "yes" if x > 0 else "no"
来源：https://fc.zhonguo4118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://ld.zhonguo8118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://kq.zhonguo3118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://of.zhonguo4118.cn

Java: x > 0 ? "yes" : "no"
来源：https://ez.zhonguo7118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://cy.zhonguo3118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ls.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://cw.zhonguo3118.cn

[A12] 字符串插值 / 格式化
来源：https://vo.zhonguo5118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://iz.zhonguo1118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://cp.zhonguo3118.cn

JS:   `Hello, ${name}!`
来源：https://yx.zhonguo2118.cn

TS:   `Hello, ${name}!`
来源：https://du.zhonguo2118.cn

Java: "Hello, %s!".formatted(name)
来源：https://mn.zhonguo4118.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：https://hf.zhonguo6118.cn

Ruby: "Hello, #{name}!"
来源：https://fo.zhonguo4118.cn

C#:   $"Hello, {name}!"
来源：https://nj.zhonguo7118.cn

[A13] 多行字符串（练习 \n 转义）
来源：https://bt.zhonguo2118.cn

Py:   "第一行\n第二行"
来源：https://ia.zhonguo8118.cn

PHP:  "第一行\n第二行"
来源：https://pf.zhonguo7118.cn

JS:   "第一行\n第二行"
来源：https://ns.zhonguo6118.cn

TS:   "第一行\n第二行"
来源：https://ng.zhonguo6118.cn

Java: "第一行\n第二行"
来源：https://qa.zhonguo4118.cn

Go:   "第一行\n第二行"
来源：https://hr.zhonguo2118.cn

Ruby: "第一行\n第二行"
来源：https://qj.zhonguo1118.cn

C#:   "第一行\n第二行"
来源：https://wu.zhonguo8118.cn

[A14] 注释写法
来源：https://oo.zhonguo6118.cn

Py:   # 单行；三引号字符串可作多行说明
来源：https://gm.zhonguo1118.cn

PHP:  // 或 # 单行；/* 多行 */
来源：https://zh.zhonguo6118.cn

JS:   // 单行；/* 多行 */
来源：https://rd.zhonguo7118.cn

TS:   // 单行；/* 多行 */
来源：https://km.zhonguo1118.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：https://gh.zhonguo3118.cn

Go:   // 单行；/* 多行 */
来源：https://kf.zhonguo8118.cn

Ruby: # 单行；=begin 多行 =end
来源：https://pd.zhonguo3118.cn

C#:   // 单行；/* 多行 */
来源：https://ee.zhonguo7118.cn

[A15] 空值判断与默认值
来源：https://ct.zhonguo3118.cn

Py:   value = data or "默认值"
来源：https://mm.zhonguo2118.cn

PHP:  $value = $data ?? "默认值";
来源：https://wn.zhonguo8118.cn

JS:   const value = data ?? "默认值";
来源：https://fg.zhonguo1118.cn

TS:   const value = data ?? "默认值";
来源：https://rh.zhonguo5118.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：https://zm.zhonguo2118.cn

Go:   if data == "" { data = "默认值" }
来源：https://cc.zhonguo4118.cn

Ruby: value = data || "默认值"
来源：https://sh.zhonguo1118.cn

C#:   var value = data ?? "默认值";
来源：https://ui.zhonguo8118.cn

[A16] 真假值判断规则
来源：https://dc.zhonguo6118.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：https://qt.zhonguo7118.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：https://kt.zhonguo7118.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：https://pu.zhonguo3118.cn

TS:   if (!x) {}
来源：https://fr.zhonguo4118.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：https://bu.zhonguo4118.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：https://zm.zhonguo5118.cn

Ruby: unless x            # nil 与 false 为假
来源：https://oi.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：https://io.zhonguo4118.cn

[A17] 位运算
来源：https://og.zhonguo2118.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://iy.zhonguo4118.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：https://nd.zhonguo7118.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://zw.zhonguo6118.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：https://jy.zhonguo7118.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://vr.zhonguo8118.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：https://rp.zhonguo7118.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://xf.zhonguo3118.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：https://oy.zhonguo8118.cn


<!-- 参考信息 -->