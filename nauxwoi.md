代发 wailian999

[U77] PHP：模板渲染
来源：https://hg.zhonguo2118.cn

composer require twig/twig
来源：https://aj.zhonguo3118.cn

[U78] PHP：单元测试
来源：https://rq.zhonguo8118.cn

composer require --dev phpunit/phpunit
来源：https://gp.zhonguo7118.cn

[U79] PHP：静态分析
来源：https://wx.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://sf.zhonguo1118.cn

[U80] PHP：代码规范修复
来源：https://sr.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://hj.zhonguo5118.cn

[U81] JS：初始化项目
来源：https://we.zhonguo6118.cn

npm init -y;  npm i express
来源：https://nw.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://cg.zhonguo4118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://gr.zhonguo7118.cn

[U83] JS：ES Module 导入导出
来源：https://rr.zhonguo5118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://te.zhonguo3118.cn

[U84] JS：CommonJS 写法
来源：https://hb.zhonguo7118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ci.zhonguo3118.cn

[U85] JS：可选链
来源：https://wh.zhonguo3118.cn

a?.b?.c
来源：https://zk.zhonguo7118.cn

[U86] JS：空值合并
来源：https://jo.zhonguo2118.cn

a ?? b
来源：https://dq.zhonguo8118.cn

[U87] JS：解构默认值
来源：https://fl.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://zd.zhonguo3118.cn

[U88] JS：对象展开合并
来源：https://vc.zhonguo1118.cn

{ ...a, ...b }
来源：https://tq.zhonguo1118.cn

[U89] JS：数组去重
来源：https://fa.zhonguo1118.cn

[...new Set(arr)]
来源：https://eq.zhonguo1118.cn

[U90] JS：数字数组排序
来源：https://af.zhonguo8118.cn

[...arr].sort((a, b) => a - b)
来源：https://qg.zhonguo8118.cn

[U91] JS：对象键值遍历
来源：https://bc.zhonguo6118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://ly.zhonguo5118.cn

[U92] JS：深拷贝
来源：https://hj.zhonguo3118.cn

structuredClone(obj)
来源：https://fe.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://ug.zhonguo5118.cn

`共 ${n} 条`
来源：https://aa.zhonguo8118.cn

[U94] JS：箭头函数
来源：https://by.zhonguo8118.cn

const double = x => x * 2;
来源：https://yc.zhonguo2118.cn

[U95] JS：Promise 包装
来源：https://gp.zhonguo3118.cn

new Promise((resolve, reject) => {})
来源：https://nm.zhonguo1118.cn

[U96] JS：async/await 与异常
来源：https://yp.zhonguo8118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://sl.zhonguo4118.cn

[U97] JS：并发请求
来源：https://dv.zhonguo5118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://jg.zhonguo3118.cn

[U98] JS：fetch 带 JSON
来源：https://wm.zhonguo4118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://xa.zhonguo4118.cn

[U99] JS：事件监听
来源：https://he.zhonguo3118.cn

el.addEventListener("click", e => {})
来源：https://ah.zhonguo3118.cn

[U100] JS：DOM 查询
来源：https://du.zhonguo6118.cn

document.querySelector(".item")
来源：https://ob.zhonguo8118.cn

[U101] JS：classList 操作
来源：https://fc.zhonguo8118.cn

el.classList.toggle("active")
来源：https://ny.zhonguo3118.cn

[U102] JS：本地存储
来源：https://zm.zhonguo1118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://ue.zhonguo4118.cn

[U103] JS：定时器
来源：https://hz.zhonguo4118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://pu.zhonguo2118.cn

[U104] JS：防抖
来源：https://li.zhonguo7118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://uc.zhonguo7118.cn

[U105] JS：节流
来源：https://qh.zhonguo8118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://ej.zhonguo1118.cn

[U106] JS：日期格式化
来源：https://uq.zhonguo3118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://gt.zhonguo4118.cn

[U107] JS：数字千分位
来源：https://tv.zhonguo2118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://rm.zhonguo7118.cn

[U108] JS：随机整数
来源：https://sw.zhonguo7118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://nl.zhonguo8118.cn

[U109] JS：数组分组
来源：https://ag.zhonguo3118.cn

Object.groupBy(arr, x => x.type)
来源：https://gd.zhonguo6118.cn

[U110] JS：数组分块
来源：https://na.zhonguo1118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://tr.zhonguo6118.cn

[U111] JS：对象转 Map
来源：https://xr.zhonguo7118.cn

new Map(Object.entries(obj))
来源：https://kk.zhonguo3118.cn

[U112] JS：字符串补位
来源：https://bj.zhonguo4118.cn

"7".padStart(3, "0")
来源：https://qa.zhonguo8118.cn

[U113] JS：正则替换全部
来源：https://zt.zhonguo5118.cn

s.replaceAll("a", "b")
来源：https://xo.zhonguo6118.cn

[U114] JS：JSON 深比较
来源：https://hf.zhonguo8118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://mr.zhonguo4118.cn

[U115] JS：生成 UUID
来源：https://ml.zhonguo5118.cn

crypto.randomUUID()
来源：https://hz.zhonguo3118.cn

[U116] JS：类型检查（JSDoc）
来源：https://ah.zhonguo6118.cn

/** @param {string} name */ function f(name) {}
来源：https://uh.zhonguo3118.cn

[U117] JS：单元测试
来源：https://zc.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://jr.zhonguo4118.cn

[U118] JS：开发服务器
来源：https://ah.zhonguo2118.cn

npm i -D vite;  npx vite
来源：https://vu.zhonguo4118.cn

[U119] JS：生产构建
来源：https://wm.zhonguo4118.cn

npx vite build
来源：https://pa.zhonguo3118.cn

[U120] JS：读取环境变量（Vite）
来源：https://bq.zhonguo4118.cn

import.meta.env.VITE_API_URL
来源：https://dl.zhonguo1118.cn

================================================================================
来源：https://wq.zhonguo1118.cn

统计汇总
来源：https://ri.zhonguo1118.cn

================================================================================
来源：https://dn.zhonguo8118.cn

按语言统计（条）：
来源：https://qo.zhonguo3118.cn

Python ......... 252
来源：https://zo.zhonguo5118.cn

PHP ............ 252
来源：https://he.zhonguo5118.cn

JavaScript ..... 252
来源：https://hd.zhonguo4118.cn

TypeScript ..... 212
来源：https://fp.zhonguo4118.cn

Java ........... 212
来源：https://lr.zhonguo4118.cn

Go ............. 212
来源：https://mk.zhonguo8118.cn

Ruby ........... 212
来源：https://vr.zhonguo1118.cn

C# ............. 212
来源：https://nm.zhonguo8118.cn

C .............. 30
来源：https://jf.zhonguo8118.cn

C++ ............ 30
来源：https://zw.zhonguo7118.cn

SQL ............ 90
来源：https://kq.zhonguo4118.cn

Bash ........... 80
来源：https://xu.zhonguo7118.cn

Kotlin ......... 15
来源：https://kf.zhonguo8118.cn

Swift .......... 15
来源：https://zv.zhonguo6118.cn

Lua ............ 10
来源：https://on.zhonguo3118.cn

Perl ........... 10
来源：https://vp.zhonguo5118.cn

Scala .......... 10
来源：https://mu.zhonguo7118.cn

------------------------------------
来源：https://pe.zhonguo3118.cn

合计 ........... 2106 条
来源：https://pm.zhonguo8118.cn

按章节统计：
来源：https://yv.zhonguo6118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://ha.zhonguo3118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://eg.zhonguo7118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://xb.zhonguo3118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://ok.zhonguo5118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://mt.zhonguo5118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://bm.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://kg.zhonguo8118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://xj.zhonguo2118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://pm.zhonguo7118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://wb.zhonguo1118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://tk.zhonguo1118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://oq.zhonguo6118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://up.zhonguo8118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://xv.zhonguo7118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://sa.zhonguo5118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://fx.zhonguo8118.cn

Q SQL 专题                              90
来源：https://hf.zhonguo3118.cn

R Bash 专题                             80
来源：https://dl.zhonguo2118.cn

S C / C++ 专题                          60
来源：https://gn.zhonguo6118.cn

T 其他语言补充                          60
来源：https://od.zhonguo5118.cn

U 高频实用片段                         120
来源：https://vp.zhonguo7118.cn

------------------------------------
来源：https://he.zhonguo1118.cn

合计                                  2106 条
来源：https://cr.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://al.zhonguo5118.cn

使用提醒
来源：https://gt.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://qo.zhonguo8118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://cc.zhonguo8118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://ca.zhonguo6118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://th.zhonguo7118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://lf.zhonguo2118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://zs.zhonguo3118.cn

—— 文件结束 ——
来源：https://qk.zhonguo1118.cn

================================================================================
来源：https://bc.zhonguo2118.cn

程序语言常见例子速查手册（2024 版）
来源：https://fj.zhonguo1118.cn

Common Programming Examples Cheat Book
来源：https://ic.zhonguo1118.cn

================================================================================
来源：https://yb.zhonguo3118.cn

【收录内容】
来源：https://yr.zhonguo8118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://zr.zhonguo6118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://ur.zhonguo8118.cn

SQL · Bash · C · C++
来源：https://la.zhonguo5118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://bx.zhonguo1118.cn

【使用说明】
来源：https://ks.zhonguo5118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://ru.zhonguo7118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://oe.zhonguo1118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://dz.zhonguo3118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://gx.zhonguo6118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://sr.zhonguo1118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://pn.zhonguo1118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://fc.zhonguo7118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://zl.zhonguo6118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://ko.zhonguo4118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://qk.zhonguo1118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://ml.zhonguo1118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://vj.zhonguo4118.cn

【文件统计】
来源：https://qq.zhonguo4118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://fc.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://jr.zhonguo4118.cn

目  录
来源：https://et.zhonguo1118.cn

--------------------------------------------------------------------------------
来源：https://yo.zhonguo1118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://hn.zhonguo3118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://dy.zhonguo3118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://mz.zhonguo6118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://yy.zhonguo2118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://nh.zhonguo2118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://yr.zhonguo8118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://dq.zhonguo6118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://kb.zhonguo1118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://mq.zhonguo4118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://pk.zhonguo6118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://ok.zhonguo7118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://ra.zhonguo2118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://rp.zhonguo3118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://az.zhonguo2118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://wz.zhonguo8118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://rg.zhonguo8118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://ms.zhonguo3118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://ef.zhonguo6118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://gd.zhonguo8118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://pz.zhonguo3118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://pf.zhonguo3118.cn

================================================================================
来源：https://fx.zhonguo3118.cn

A. 基础语法与类型
来源：https://rb.zhonguo2118.cn

================================================================================
来源：https://co.zhonguo4118.cn

[A01] Hello World
来源：https://mq.zhonguo8118.cn

Py:   print("Hello, World!")
来源：https://sv.zhonguo3118.cn

PHP:  echo "Hello, World!";
来源：https://bv.zhonguo2118.cn

JS:   console.log("Hello, World!");
来源：https://bp.zhonguo5118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://os.zhonguo3118.cn

Java: System.out.println("Hello, World!");
来源：https://af.zhonguo6118.cn

Go:   fmt.Println("Hello, World!")
来源：https://zo.zhonguo4118.cn

Ruby: puts "Hello, World!"
来源：https://qn.zhonguo7118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://jx.zhonguo6118.cn

[A02] 变量声明与赋值
来源：https://du.zhonguo1118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://zz.zhonguo2118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://mg.zhonguo6118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://ok.zhonguo8118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://rx.zhonguo6118.cn

Java: String name = "Alex"; int age = 20;
来源：https://ti.zhonguo4118.cn

Go:   name := "Alex"; age := 20
来源：https://vu.zhonguo5118.cn

Ruby: name = "Alex"; age = 20
来源：https://qs.zhonguo7118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://dy.zhonguo3118.cn

[A03] 常量定义
来源：https://yj.zhonguo3118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://hl.zhonguo7118.cn

PHP:  const PI = 3.14159;
来源：https://sv.zhonguo4118.cn

JS:   const PI = 3.14159;
来源：https://yz.zhonguo4118.cn

TS:   const PI: number = 3.14159;
来源：https://oq.zhonguo3118.cn

Java: static final double PI = 3.14159;
来源：https://of.zhonguo8118.cn

Go:   const PI = 3.14159
来源：https://ro.zhonguo3118.cn

Ruby: PI = 3.14159
来源：https://or.zhonguo1118.cn

C#:   const double PI = 3.14159;
来源：https://qj.zhonguo4118.cn

[A04] 判断变量类型
来源：https://yd.zhonguo1118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://gb.zhonguo7118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://ih.zhonguo4118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://in.zhonguo8118.cn

TS:   typeof x; x instanceof Date
来源：https://ne.zhonguo8118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://ui.zhonguo6118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://je.zhonguo3118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://is.zhonguo3118.cn

C#:   x.GetType().Name; x is int
来源：https://ho.zhonguo2118.cn

[A05] 整数除法与取模
来源：https://cq.zhonguo2118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://kp.zhonguo2118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://tv.zhonguo8118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://qy.zhonguo2118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://tm.zhonguo4118.cn

Java: 7 / 2; 7 % 2
来源：https://ic.zhonguo4118.cn

Go:   7 / 2; 7 % 2
来源：https://qj.zhonguo6118.cn

Ruby: 7 / 2; 7 % 2
来源：https://ut.zhonguo8118.cn

C#:   7 / 2; 7 % 2
来源：https://nj.zhonguo8118.cn

[A06] 字符串转数字
来源：https://kk.zhonguo6118.cn

Py:   int("42"); float("3.14")
来源：https://ww.zhonguo8118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://jw.zhonguo5118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://qr.zhonguo3118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://vt.zhonguo4118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://uj.zhonguo6118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://wo.zhonguo7118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://rl.zhonguo3118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://en.zhonguo5118.cn

[A07] 数字转字符串
来源：https://ur.zhonguo3118.cn

Py:   str(42)
来源：https://is.zhonguo6118.cn

PHP:  (string) 42; strval(42)
来源：https://ne.zhonguo8118.cn

JS:   String(42); (42).toString()
来源：https://li.zhonguo1118.cn

TS:   String(42)
来源：https://zt.zhonguo1118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://ps.zhonguo1118.cn

Go:   strconv.Itoa(42)
来源：https://qh.zhonguo5118.cn

Ruby: 42.to_s
来源：https://bw.zhonguo7118.cn

C#:   42.ToString()
来源：https://bx.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://ob.zhonguo1118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://ri.zhonguo2118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://eg.zhonguo8118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://ca.zhonguo2118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://xx.zhonguo5118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://pc.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://rw.zhonguo7118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://va.zhonguo5118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://ol.zhonguo3118.cn

[A09] 绝对值与最大最小值
来源：https://et.zhonguo7118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://ir.zhonguo2118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://lv.zhonguo4118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://je.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ie.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://aq.zhonguo6118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://be.zhonguo2118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://ls.zhonguo2118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://ao.zhonguo6118.cn

[A10] 生成随机数
来源：https://uw.zhonguo5118.cn

Py:   import random; random.randint(1, 100)
来源：https://mn.zhonguo8118.cn

PHP:  random_int(1, 100);
来源：https://qh.zhonguo2118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://gg.zhonguo8118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://ep.zhonguo3118.cn

Java: new Random().nextInt(100) + 1
来源：https://gf.zhonguo7118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://dr.zhonguo3118.cn

Ruby: rand(1..100)
来源：https://fn.zhonguo6118.cn

C#:   new Random().Next(1, 101)
来源：https://kc.zhonguo4118.cn

[A11] 条件表达式（三元）
来源：https://fx.zhonguo1118.cn

Py:   "yes" if x > 0 else "no"
来源：https://ib.zhonguo1118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://vv.zhonguo3118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://kz.zhonguo5118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://xn.zhonguo5118.cn

Java: x > 0 ? "yes" : "no"
来源：https://om.zhonguo2118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://ui.zhonguo2118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://gs.zhonguo1118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://xq.zhonguo6118.cn

[A12] 字符串插值 / 格式化
来源：https://lq.zhonguo7118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://ee.zhonguo5118.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：https://pq.zhonguo1118.cn

JS:   `Hello, ${name}!`
来源：https://qx.zhonguo7118.cn

TS:   `Hello, ${name}!`
来源：https://je.zhonguo5118.cn

Java: "Hello, %s!".formatted(name)
来源：https://cx.zhonguo3118.cn


<!-- 参考信息 -->