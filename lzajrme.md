代发 wailian999

[U75] PHP：依赖注入
来源：https://jb.zhonguo1118.cn

composer require psr/container
来源：https://gr.zhonguo6118.cn

[U76] PHP：简单路由
来源：https://dv.zhonguo8118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://lr.zhonguo8118.cn

[U77] PHP：模板渲染
来源：https://rf.zhonguo3118.cn

composer require twig/twig
来源：https://bq.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://py.zhonguo7118.cn

composer require --dev phpunit/phpunit
来源：https://ov.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://mo.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://qo.zhonguo2118.cn

[U80] PHP：代码规范修复
来源：https://qu.zhonguo4118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://on.zhonguo1118.cn

[U81] JS：初始化项目
来源：https://ze.zhonguo6118.cn

npm init -y;  npm i express
来源：https://iu.zhonguo7118.cn

[U82] JS：package.json 脚本
来源：https://mt.zhonguo5118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://dk.zhonguo1118.cn

[U83] JS：ES Module 导入导出
来源：https://dv.zhonguo8118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://ku.zhonguo1118.cn

[U84] JS：CommonJS 写法
来源：https://lh.zhonguo2118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://rf.zhonguo2118.cn

[U85] JS：可选链
来源：https://xf.zhonguo2118.cn

a?.b?.c
来源：https://fc.zhonguo5118.cn

[U86] JS：空值合并
来源：https://cx.zhonguo6118.cn

a ?? b
来源：https://tc.zhonguo8118.cn

[U87] JS：解构默认值
来源：https://df.zhonguo5118.cn

const { a = 1, b = 2 } = obj;
来源：https://qc.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://pe.zhonguo1118.cn

{ ...a, ...b }
来源：https://fo.zhonguo8118.cn

[U89] JS：数组去重
来源：https://cb.zhonguo1118.cn

[...new Set(arr)]
来源：https://kh.zhonguo8118.cn

[U90] JS：数字数组排序
来源：https://rp.zhonguo8118.cn

[...arr].sort((a, b) => a - b)
来源：https://qx.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://kr.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://ka.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://ic.zhonguo1118.cn

structuredClone(obj)
来源：https://uj.zhonguo7118.cn

[U93] JS：模板字符串
来源：https://em.zhonguo3118.cn

`共 ${n} 条`
来源：https://yi.zhonguo7118.cn

[U94] JS：箭头函数
来源：https://ti.zhonguo6118.cn

const double = x => x * 2;
来源：https://di.zhonguo5118.cn

[U95] JS：Promise 包装
来源：https://kd.zhonguo4118.cn

new Promise((resolve, reject) => {})
来源：https://ee.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://cd.zhonguo8118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://vb.zhonguo3118.cn

[U97] JS：并发请求
来源：https://zv.zhonguo7118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://aa.zhonguo5118.cn

[U98] JS：fetch 带 JSON
来源：https://hs.zhonguo8118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://jg.zhonguo1118.cn

[U99] JS：事件监听
来源：https://ly.zhonguo6118.cn

el.addEventListener("click", e => {})
来源：https://ls.zhonguo1118.cn

[U100] JS：DOM 查询
来源：https://vv.zhonguo4118.cn

document.querySelector(".item")
来源：https://aa.zhonguo6118.cn

[U101] JS：classList 操作
来源：https://xa.zhonguo5118.cn

el.classList.toggle("active")
来源：https://jc.zhonguo7118.cn

[U102] JS：本地存储
来源：https://ab.zhonguo7118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://bn.zhonguo5118.cn

[U103] JS：定时器
来源：https://rp.zhonguo6118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://ob.zhonguo1118.cn

[U104] JS：防抖
来源：https://hw.zhonguo6118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://tn.zhonguo4118.cn

[U105] JS：节流
来源：https://tu.zhonguo1118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://nm.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://xb.zhonguo6118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://hn.zhonguo8118.cn

[U107] JS：数字千分位
来源：https://zw.zhonguo1118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://ze.zhonguo1118.cn

[U108] JS：随机整数
来源：https://ie.zhonguo5118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://ha.zhonguo6118.cn

[U109] JS：数组分组
来源：https://ek.zhonguo1118.cn

Object.groupBy(arr, x => x.type)
来源：https://wg.zhonguo6118.cn

[U110] JS：数组分块
来源：https://pr.zhonguo1118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://jc.zhonguo8118.cn

[U111] JS：对象转 Map
来源：https://uj.zhonguo5118.cn

new Map(Object.entries(obj))
来源：https://rl.zhonguo8118.cn

[U112] JS：字符串补位
来源：https://ot.zhonguo6118.cn

"7".padStart(3, "0")
来源：https://nk.zhonguo5118.cn

[U113] JS：正则替换全部
来源：https://qa.zhonguo7118.cn

s.replaceAll("a", "b")
来源：https://qf.zhonguo3118.cn

[U114] JS：JSON 深比较
来源：https://qt.zhonguo4118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://td.zhonguo8118.cn

[U115] JS：生成 UUID
来源：https://dy.zhonguo2118.cn

crypto.randomUUID()
来源：https://va.zhonguo3118.cn

[U116] JS：类型检查（JSDoc）
来源：https://cv.zhonguo7118.cn

/** @param {string} name */ function f(name) {}
来源：https://ij.zhonguo3118.cn

[U117] JS：单元测试
来源：https://fn.zhonguo6118.cn

npm i -D vitest;  npx vitest
来源：https://ts.zhonguo5118.cn

[U118] JS：开发服务器
来源：https://cm.zhonguo2118.cn

npm i -D vite;  npx vite
来源：https://aq.zhonguo7118.cn

[U119] JS：生产构建
来源：https://py.zhonguo6118.cn

npx vite build
来源：https://cw.zhonguo1118.cn

[U120] JS：读取环境变量（Vite）
来源：https://ir.zhonguo3118.cn

import.meta.env.VITE_API_URL
来源：https://hx.zhonguo4118.cn

================================================================================
来源：https://oa.zhonguo6118.cn

统计汇总
来源：https://nd.zhonguo1118.cn

================================================================================
来源：https://hr.zhonguo7118.cn

按语言统计（条）：
来源：https://nr.zhonguo3118.cn

Python ......... 252
来源：https://qu.zhonguo4118.cn

PHP ............ 252
来源：https://ep.zhonguo6118.cn

JavaScript ..... 252
来源：https://on.zhonguo4118.cn

TypeScript ..... 212
来源：https://ww.zhonguo7118.cn

Java ........... 212
来源：https://ot.zhonguo2118.cn

Go ............. 212
来源：https://iy.zhonguo4118.cn

Ruby ........... 212
来源：https://dh.zhonguo7118.cn

C# ............. 212
来源：https://ua.zhonguo7118.cn

C .............. 30
来源：https://wd.zhonguo8118.cn

C++ ............ 30
来源：https://hu.zhonguo4118.cn

SQL ............ 90
来源：https://wd.zhonguo2118.cn

Bash ........... 80
来源：https://jp.zhonguo5118.cn

Kotlin ......... 15
来源：https://ea.zhonguo2118.cn

Swift .......... 15
来源：https://uy.zhonguo8118.cn

Lua ............ 10
来源：https://jy.zhonguo3118.cn

Perl ........... 10
来源：https://it.zhonguo8118.cn

Scala .......... 10
来源：https://wf.zhonguo6118.cn

------------------------------------
来源：https://uk.zhonguo1118.cn

合计 ........... 2106 条
来源：https://nu.zhonguo4118.cn

按章节统计：
来源：https://ea.zhonguo6118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://ei.zhonguo1118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://zp.zhonguo6118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://gd.zhonguo5118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://vt.zhonguo6118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://sk.zhonguo5118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://qb.zhonguo8118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://ei.zhonguo2118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://kz.zhonguo2118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://mw.zhonguo1118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://uc.zhonguo6118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://os.zhonguo3118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://ex.zhonguo6118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://ya.zhonguo4118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://jj.zhonguo3118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://ks.zhonguo3118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://bq.zhonguo4118.cn

Q SQL 专题                              90
来源：https://zy.zhonguo3118.cn

R Bash 专题                             80
来源：https://oi.zhonguo8118.cn

S C / C++ 专题                          60
来源：https://hq.zhonguo6118.cn

T 其他语言补充                          60
来源：https://my.zhonguo8118.cn

U 高频实用片段                         120
来源：https://cd.zhonguo6118.cn

------------------------------------
来源：https://cd.zhonguo2118.cn

合计                                  2106 条
来源：https://sa.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://vw.zhonguo1118.cn

使用提醒
来源：https://ue.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://ko.zhonguo1118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://xi.zhonguo1118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://wr.zhonguo6118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://hz.zhonguo6118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://xx.zhonguo6118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://jl.zhonguo3118.cn

—— 文件结束 ——
来源：https://sw.zhonguo3118.cn

================================================================================
来源：https://mu.zhonguo7118.cn

程序语言常见例子速查手册（2024 版）
来源：https://qj.zhonguo8118.cn

Common Programming Examples Cheat Book
来源：https://xv.zhonguo3118.cn

================================================================================
来源：https://ct.zhonguo2118.cn

【收录内容】
来源：https://cm.zhonguo8118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://dg.zhonguo8118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://fo.zhonguo8118.cn

SQL · Bash · C · C++
来源：https://ii.zhonguo1118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://jo.zhonguo4118.cn

【使用说明】
来源：https://zn.zhonguo2118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://fq.zhonguo7118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://qj.zhonguo4118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://nk.zhonguo8118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://mh.zhonguo6118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://uy.zhonguo8118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://qo.zhonguo5118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://op.zhonguo1118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://gn.zhonguo4118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://iy.zhonguo4118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://dp.zhonguo3118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://eo.zhonguo5118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://fh.zhonguo4118.cn

【文件统计】
来源：https://th.zhonguo3118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://mb.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://um.zhonguo4118.cn

目  录
来源：https://pv.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://zm.zhonguo8118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://av.zhonguo7118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://bf.zhonguo7118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://xg.zhonguo6118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://wk.zhonguo1118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://xc.zhonguo5118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://tc.zhonguo4118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://hi.zhonguo8118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://hb.zhonguo3118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://hu.zhonguo2118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://dk.zhonguo1118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://um.zhonguo7118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://in.zhonguo3118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://in.zhonguo3118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://tl.zhonguo8118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://el.zhonguo5118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://og.zhonguo6118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://qr.zhonguo1118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://hz.zhonguo1118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://fz.zhonguo7118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://vy.zhonguo7118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://la.zhonguo1118.cn

================================================================================
来源：https://el.zhonguo1118.cn

A. 基础语法与类型
来源：https://vh.zhonguo4118.cn

================================================================================
来源：https://xg.zhonguo2118.cn

[A01] Hello World
来源：https://ej.zhonguo1118.cn

Py:   print("Hello, World!")
来源：https://cn.zhonguo8118.cn

PHP:  echo "Hello, World!";
来源：https://hv.zhonguo5118.cn

JS:   console.log("Hello, World!");
来源：https://yh.zhonguo1118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://oh.zhonguo4118.cn

Java: System.out.println("Hello, World!");
来源：https://wc.zhonguo1118.cn

Go:   fmt.Println("Hello, World!")
来源：https://te.zhonguo6118.cn

Ruby: puts "Hello, World!"
来源：https://lp.zhonguo8118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://bo.zhonguo1118.cn

[A02] 变量声明与赋值
来源：https://af.zhonguo7118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://ox.zhonguo4118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://om.zhonguo7118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://nk.zhonguo6118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://wt.zhonguo1118.cn

Java: String name = "Alex"; int age = 20;
来源：https://jp.zhonguo6118.cn

Go:   name := "Alex"; age := 20
来源：https://me.zhonguo3118.cn

Ruby: name = "Alex"; age = 20
来源：https://ls.zhonguo1118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://kc.zhonguo3118.cn

[A03] 常量定义
来源：https://tb.zhonguo2118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://up.zhonguo8118.cn

PHP:  const PI = 3.14159;
来源：https://ot.zhonguo1118.cn

JS:   const PI = 3.14159;
来源：https://cd.zhonguo3118.cn

TS:   const PI: number = 3.14159;
来源：https://kj.zhonguo1118.cn

Java: static final double PI = 3.14159;
来源：https://yr.zhonguo7118.cn

Go:   const PI = 3.14159
来源：https://jw.zhonguo1118.cn

Ruby: PI = 3.14159
来源：https://pf.zhonguo3118.cn

C#:   const double PI = 3.14159;
来源：https://cl.zhonguo4118.cn

[A04] 判断变量类型
来源：https://pr.zhonguo3118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://vj.zhonguo3118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://px.zhonguo8118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://on.zhonguo6118.cn

TS:   typeof x; x instanceof Date
来源：https://zr.zhonguo5118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://hy.zhonguo8118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://jb.zhonguo4118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://qm.zhonguo4118.cn

C#:   x.GetType().Name; x is int
来源：https://wj.zhonguo7118.cn

[A05] 整数除法与取模
来源：https://tf.zhonguo1118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ej.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://ow.zhonguo7118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://rr.zhonguo1118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://pl.zhonguo6118.cn

Java: 7 / 2; 7 % 2
来源：https://ce.zhonguo7118.cn

Go:   7 / 2; 7 % 2
来源：https://zx.zhonguo4118.cn

Ruby: 7 / 2; 7 % 2
来源：https://up.zhonguo8118.cn

C#:   7 / 2; 7 % 2
来源：https://et.zhonguo1118.cn

[A06] 字符串转数字
来源：https://jc.zhonguo8118.cn

Py:   int("42"); float("3.14")
来源：https://eh.zhonguo2118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://dg.zhonguo4118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://sw.zhonguo7118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://yi.zhonguo6118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://zp.zhonguo1118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://xz.zhonguo7118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://nz.zhonguo8118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://co.zhonguo7118.cn

[A07] 数字转字符串
来源：https://bm.zhonguo8118.cn

Py:   str(42)
来源：https://sv.zhonguo5118.cn

PHP:  (string) 42; strval(42)
来源：https://gn.zhonguo8118.cn

JS:   String(42); (42).toString()
来源：https://cu.zhonguo6118.cn

TS:   String(42)
来源：https://mj.zhonguo3118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://hs.zhonguo2118.cn

Go:   strconv.Itoa(42)
来源：https://hp.zhonguo1118.cn

Ruby: 42.to_s
来源：https://ya.zhonguo4118.cn

C#:   42.ToString()
来源：https://lw.zhonguo5118.cn

[A08] 取整与四舍五入
来源：https://uv.zhonguo6118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://dx.zhonguo1118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://bd.zhonguo6118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://pa.zhonguo2118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://yl.zhonguo4118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://uu.zhonguo1118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://dh.zhonguo8118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://bp.zhonguo5118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://hh.zhonguo8118.cn

[A09] 绝对值与最大最小值
来源：https://oq.zhonguo3118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://bu.zhonguo6118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://al.zhonguo8118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://tn.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://xz.zhonguo5118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://uz.zhonguo6118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://pr.zhonguo2118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://po.zhonguo5118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://gh.zhonguo4118.cn

[A10] 生成随机数
来源：https://ms.zhonguo5118.cn

Py:   import random; random.randint(1, 100)
来源：https://rg.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://ri.zhonguo1118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://jj.zhonguo1118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://sp.zhonguo3118.cn

Java: new Random().nextInt(100) + 1
来源：https://dh.zhonguo5118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://yw.zhonguo2118.cn

Ruby: rand(1..100)
来源：https://jz.zhonguo7118.cn

C#:   new Random().Next(1, 101)
来源：https://uo.zhonguo1118.cn

[A11] 条件表达式（三元）
来源：https://mz.zhonguo3118.cn

Py:   "yes" if x > 0 else "no"
来源：https://gf.zhonguo3118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://sk.zhonguo4118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://ep.zhonguo4118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://ec.zhonguo8118.cn

Java: x > 0 ? "yes" : "no"
来源：https://rq.zhonguo4118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://lw.zhonguo2118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://ha.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://vt.zhonguo1118.cn

[A12] 字符串插值 / 格式化
来源：https://uz.zhonguo1118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://dh.zhonguo8118.cn


<!-- 参考信息 -->