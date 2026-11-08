代发 wailian999

[U75] PHP：依赖注入
来源：https://bj.zhonguo8118.cn

composer require psr/container
来源：https://br.zhonguo6118.cn

[U76] PHP：简单路由
来源：https://hp.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://jf.zhonguo4118.cn

[U77] PHP：模板渲染
来源：https://yc.zhonguo2118.cn

composer require twig/twig
来源：https://ro.zhonguo1118.cn

[U78] PHP：单元测试
来源：https://kd.zhonguo5118.cn

composer require --dev phpunit/phpunit
来源：https://zv.zhonguo5118.cn

[U79] PHP：静态分析
来源：https://em.zhonguo8118.cn

composer require --dev phpstan/phpstan
来源：https://ru.zhonguo8118.cn

[U80] PHP：代码规范修复
来源：https://bb.zhonguo8118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://mm.zhonguo4118.cn

[U81] JS：初始化项目
来源：https://mo.zhonguo5118.cn

npm init -y;  npm i express
来源：https://jn.zhonguo4118.cn

[U82] JS：package.json 脚本
来源：https://yv.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://ip.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://cg.zhonguo4118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://ky.zhonguo3118.cn

[U84] JS：CommonJS 写法
来源：https://hd.zhonguo3118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://fi.zhonguo8118.cn

[U85] JS：可选链
来源：https://xt.zhonguo8118.cn

a?.b?.c
来源：https://yo.zhonguo7118.cn

[U86] JS：空值合并
来源：https://uz.zhonguo7118.cn

a ?? b
来源：https://un.zhonguo2118.cn

[U87] JS：解构默认值
来源：https://oj.zhonguo1118.cn

const { a = 1, b = 2 } = obj;
来源：https://go.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://rx.zhonguo8118.cn

{ ...a, ...b }
来源：https://fx.zhonguo8118.cn

[U89] JS：数组去重
来源：https://ht.zhonguo3118.cn

[...new Set(arr)]
来源：https://qp.zhonguo4118.cn

[U90] JS：数字数组排序
来源：https://zp.zhonguo8118.cn

[...arr].sort((a, b) => a - b)
来源：https://qa.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://el.zhonguo6118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://bd.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://eg.zhonguo4118.cn

structuredClone(obj)
来源：https://gz.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://gz.zhonguo3118.cn

`共 ${n} 条`
来源：https://sc.zhonguo3118.cn

[U94] JS：箭头函数
来源：https://cq.zhonguo1118.cn

const double = x => x * 2;
来源：https://pi.zhonguo8118.cn

[U95] JS：Promise 包装
来源：https://gm.zhonguo3118.cn

new Promise((resolve, reject) => {})
来源：https://em.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://xf.zhonguo5118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://vh.zhonguo6118.cn

[U97] JS：并发请求
来源：https://ew.zhonguo7118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://yo.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://cs.zhonguo3118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://xo.zhonguo7118.cn

[U99] JS：事件监听
来源：https://hw.zhonguo4118.cn

el.addEventListener("click", e => {})
来源：https://hv.zhonguo8118.cn

[U100] JS：DOM 查询
来源：https://hf.zhonguo3118.cn

document.querySelector(".item")
来源：https://su.zhonguo5118.cn

[U101] JS：classList 操作
来源：https://bd.zhonguo5118.cn

el.classList.toggle("active")
来源：https://gq.zhonguo5118.cn

[U102] JS：本地存储
来源：https://ga.zhonguo8118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://vd.zhonguo7118.cn

[U103] JS：定时器
来源：https://al.zhonguo4118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://lw.zhonguo1118.cn

[U104] JS：防抖
来源：https://sp.zhonguo5118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://pd.zhonguo2118.cn

[U105] JS：节流
来源：https://zd.zhonguo6118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://ja.zhonguo5118.cn

[U106] JS：日期格式化
来源：https://zw.zhonguo3118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://do.zhonguo7118.cn

[U107] JS：数字千分位
来源：https://ks.zhonguo4118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://nd.zhonguo1118.cn

[U108] JS：随机整数
来源：https://lk.zhonguo2118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://ry.zhonguo1118.cn

[U109] JS：数组分组
来源：https://my.zhonguo2118.cn

Object.groupBy(arr, x => x.type)
来源：https://hj.zhonguo8118.cn

[U110] JS：数组分块
来源：https://wf.zhonguo2118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://dm.zhonguo4118.cn

[U111] JS：对象转 Map
来源：https://or.zhonguo5118.cn

new Map(Object.entries(obj))
来源：https://yb.zhonguo6118.cn

[U112] JS：字符串补位
来源：https://cc.zhonguo5118.cn

"7".padStart(3, "0")
来源：https://as.zhonguo3118.cn

[U113] JS：正则替换全部
来源：https://gj.zhonguo6118.cn

s.replaceAll("a", "b")
来源：https://jy.zhonguo2118.cn

[U114] JS：JSON 深比较
来源：https://cg.zhonguo3118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://cd.zhonguo5118.cn

[U115] JS：生成 UUID
来源：https://vs.zhonguo6118.cn

crypto.randomUUID()
来源：https://jc.zhonguo8118.cn

[U116] JS：类型检查（JSDoc）
来源：https://pw.zhonguo6118.cn

/** @param {string} name */ function f(name) {}
来源：https://fh.zhonguo6118.cn

[U117] JS：单元测试
来源：https://lw.zhonguo1118.cn

npm i -D vitest;  npx vitest
来源：https://lq.zhonguo3118.cn

[U118] JS：开发服务器
来源：https://ft.zhonguo3118.cn

npm i -D vite;  npx vite
来源：https://vk.zhonguo4118.cn

[U119] JS：生产构建
来源：https://zc.zhonguo8118.cn

npx vite build
来源：https://am.zhonguo4118.cn

[U120] JS：读取环境变量（Vite）
来源：https://gs.zhonguo7118.cn

import.meta.env.VITE_API_URL
来源：https://lq.zhonguo5118.cn

================================================================================
来源：https://tl.zhonguo8118.cn

统计汇总
来源：https://sk.zhonguo5118.cn

================================================================================
来源：https://zb.zhonguo4118.cn

按语言统计（条）：
来源：https://ms.zhonguo2118.cn

Python ......... 252
来源：https://ig.zhonguo3118.cn

PHP ............ 252
来源：https://rd.zhonguo6118.cn

JavaScript ..... 252
来源：https://jn.zhonguo4118.cn

TypeScript ..... 212
来源：https://rj.zhonguo3118.cn

Java ........... 212
来源：https://uo.zhonguo7118.cn

Go ............. 212
来源：https://my.zhonguo8118.cn

Ruby ........... 212
来源：https://ca.zhonguo8118.cn

C# ............. 212
来源：https://gw.zhonguo1118.cn

C .............. 30
来源：https://az.zhonguo8118.cn

C++ ............ 30
来源：https://xh.zhonguo3118.cn

SQL ............ 90
来源：https://fp.zhonguo4118.cn

Bash ........... 80
来源：https://cy.zhonguo2118.cn

Kotlin ......... 15
来源：https://gm.zhonguo4118.cn

Swift .......... 15
来源：https://ly.zhonguo1118.cn

Lua ............ 10
来源：https://mi.zhonguo2118.cn

Perl ........... 10
来源：https://ke.zhonguo8118.cn

Scala .......... 10
来源：https://uo.zhonguo2118.cn

------------------------------------
来源：https://zu.zhonguo5118.cn

合计 ........... 2106 条
来源：https://tb.zhonguo8118.cn

按章节统计：
来源：https://et.zhonguo8118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://vr.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://fx.zhonguo4118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://ok.zhonguo2118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://yb.zhonguo2118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://um.zhonguo5118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://vr.zhonguo6118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://zv.zhonguo2118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://bh.zhonguo4118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://jo.zhonguo7118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://ad.zhonguo8118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://sq.zhonguo6118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://kj.zhonguo8118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://sd.zhonguo8118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://oy.zhonguo6118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://or.zhonguo5118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://se.zhonguo1118.cn

Q SQL 专题                              90
来源：https://rh.zhonguo3118.cn

R Bash 专题                             80
来源：https://wl.zhonguo5118.cn

S C / C++ 专题                          60
来源：https://ab.zhonguo5118.cn

T 其他语言补充                          60
来源：https://ya.zhonguo8118.cn

U 高频实用片段                         120
来源：https://nw.zhonguo8118.cn

------------------------------------
来源：https://um.zhonguo3118.cn

合计                                  2106 条
来源：https://ev.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://jd.zhonguo6118.cn

使用提醒
来源：https://mw.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://sp.zhonguo6118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://ae.zhonguo6118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://az.zhonguo3118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://zx.zhonguo7118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://bd.zhonguo7118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://ul.zhonguo2118.cn

—— 文件结束 ——
来源：https://un.zhonguo8118.cn

================================================================================
来源：https://ov.zhonguo3118.cn

程序语言常见例子速查手册（2024 版）
来源：https://vr.zhonguo3118.cn

Common Programming Examples Cheat Book
来源：https://qx.zhonguo5118.cn

================================================================================
来源：https://cv.zhonguo2118.cn

【收录内容】
来源：https://ru.zhonguo3118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://yc.zhonguo5118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://xi.zhonguo6118.cn

SQL · Bash · C · C++
来源：https://vm.zhonguo3118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://sc.zhonguo8118.cn

【使用说明】
来源：https://cr.zhonguo5118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://lu.zhonguo4118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://lr.zhonguo8118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://fa.zhonguo7118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://dg.zhonguo4118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://fh.zhonguo2118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://yy.zhonguo8118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://ep.zhonguo1118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://xq.zhonguo2118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://ik.zhonguo1118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://jp.zhonguo4118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://em.zhonguo5118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://uj.zhonguo3118.cn

【文件统计】
来源：https://hv.zhonguo6118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://qs.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://xv.zhonguo7118.cn

目  录
来源：https://be.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://op.zhonguo5118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://fe.zhonguo1118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://ft.zhonguo6118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://mr.zhonguo4118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://eu.zhonguo2118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://db.zhonguo1118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://cv.zhonguo8118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://fi.zhonguo4118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://cl.zhonguo3118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://ze.zhonguo3118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://yv.zhonguo5118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://vl.zhonguo6118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://re.zhonguo4118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://rh.zhonguo8118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://td.zhonguo6118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://gq.zhonguo3118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://pj.zhonguo3118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://lb.zhonguo6118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://qd.zhonguo6118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://sa.zhonguo4118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://nm.zhonguo2118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://yi.zhonguo2118.cn

================================================================================
来源：https://cf.zhonguo8118.cn

A. 基础语法与类型
来源：https://up.zhonguo4118.cn

================================================================================
来源：https://ip.zhonguo8118.cn

[A01] Hello World
来源：https://ph.zhonguo5118.cn

Py:   print("Hello, World!")
来源：https://ha.zhonguo4118.cn

PHP:  echo "Hello, World!";
来源：https://fv.zhonguo6118.cn

JS:   console.log("Hello, World!");
来源：https://vo.zhonguo7118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://mt.zhonguo6118.cn

Java: System.out.println("Hello, World!");
来源：https://av.zhonguo8118.cn

Go:   fmt.Println("Hello, World!")
来源：https://ih.zhonguo8118.cn

Ruby: puts "Hello, World!"
来源：https://hj.zhonguo4118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://ni.zhonguo7118.cn

[A02] 变量声明与赋值
来源：https://bt.zhonguo1118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://bv.zhonguo6118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ib.zhonguo6118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://hy.zhonguo3118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://ye.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://cf.zhonguo8118.cn

Go:   name := "Alex"; age := 20
来源：https://ec.zhonguo7118.cn

Ruby: name = "Alex"; age = 20
来源：https://pb.zhonguo8118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://xl.zhonguo8118.cn

[A03] 常量定义
来源：https://ls.zhonguo5118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://mx.zhonguo8118.cn

PHP:  const PI = 3.14159;
来源：https://go.zhonguo7118.cn

JS:   const PI = 3.14159;
来源：https://jf.zhonguo6118.cn

TS:   const PI: number = 3.14159;
来源：https://ur.zhonguo2118.cn

Java: static final double PI = 3.14159;
来源：https://hn.zhonguo3118.cn

Go:   const PI = 3.14159
来源：https://la.zhonguo4118.cn

Ruby: PI = 3.14159
来源：https://ms.zhonguo7118.cn

C#:   const double PI = 3.14159;
来源：https://og.zhonguo5118.cn

[A04] 判断变量类型
来源：https://vt.zhonguo1118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://rg.zhonguo7118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://xh.zhonguo6118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://hu.zhonguo7118.cn

TS:   typeof x; x instanceof Date
来源：https://kq.zhonguo6118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://oj.zhonguo7118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://xz.zhonguo8118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://wj.zhonguo4118.cn

C#:   x.GetType().Name; x is int
来源：https://va.zhonguo8118.cn

[A05] 整数除法与取模
来源：https://ne.zhonguo4118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://id.zhonguo7118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://dg.zhonguo6118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://an.zhonguo1118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://ty.zhonguo3118.cn

Java: 7 / 2; 7 % 2
来源：https://wa.zhonguo1118.cn

Go:   7 / 2; 7 % 2
来源：https://oi.zhonguo6118.cn

Ruby: 7 / 2; 7 % 2
来源：https://gy.zhonguo8118.cn

C#:   7 / 2; 7 % 2
来源：https://kf.zhonguo6118.cn

[A06] 字符串转数字
来源：https://ps.zhonguo1118.cn

Py:   int("42"); float("3.14")
来源：https://gq.zhonguo3118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://ch.zhonguo7118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://ui.zhonguo7118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://uz.zhonguo2118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://lb.zhonguo7118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://dd.zhonguo6118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://bz.zhonguo8118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://vh.zhonguo6118.cn

[A07] 数字转字符串
来源：https://vm.zhonguo7118.cn

Py:   str(42)
来源：https://el.zhonguo3118.cn

PHP:  (string) 42; strval(42)
来源：https://am.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://yr.zhonguo4118.cn

TS:   String(42)
来源：https://ty.zhonguo8118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://bo.zhonguo2118.cn

Go:   strconv.Itoa(42)
来源：https://rw.zhonguo8118.cn

Ruby: 42.to_s
来源：https://rg.zhonguo4118.cn

C#:   42.ToString()
来源：https://cb.zhonguo2118.cn

[A08] 取整与四舍五入
来源：https://fj.zhonguo1118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://wz.zhonguo2118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://et.zhonguo7118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://wc.zhonguo3118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://qo.zhonguo8118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://wd.zhonguo7118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://qh.zhonguo8118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://ta.zhonguo2118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://ei.zhonguo7118.cn

[A09] 绝对值与最大最小值
来源：https://ta.zhonguo2118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://zj.zhonguo2118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://ti.zhonguo1118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://ki.zhonguo3118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://zo.zhonguo2118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://un.zhonguo5118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://qf.zhonguo8118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://zn.zhonguo5118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://cn.zhonguo4118.cn

[A10] 生成随机数
来源：https://xn.zhonguo6118.cn

Py:   import random; random.randint(1, 100)
来源：https://dj.zhonguo1118.cn

PHP:  random_int(1, 100);
来源：https://uy.zhonguo6118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://iz.zhonguo5118.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：https://vi.zhonguo5118.cn

Java: new Random().nextInt(100) + 1
来源：https://fd.zhonguo4118.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：https://wj.zhonguo4118.cn

Ruby: rand(1..100)
来源：https://sb.zhonguo5118.cn

C#:   new Random().Next(1, 101)
来源：https://xj.zhonguo4118.cn

[A11] 条件表达式（三元）
来源：https://xp.zhonguo4118.cn

Py:   "yes" if x > 0 else "no"
来源：https://zo.zhonguo5118.cn

PHP:  $x > 0 ? "yes" : "no"
来源：https://tu.zhonguo1118.cn

JS:   x > 0 ? "yes" : "no"
来源：https://pg.zhonguo1118.cn

TS:   x > 0 ? "yes" : "no"
来源：https://iz.zhonguo2118.cn

Java: x > 0 ? "yes" : "no"
来源：https://ww.zhonguo2118.cn

Go:   // 无三元运算符，需用 if 语句
来源：https://fl.zhonguo6118.cn

Ruby: x > 0 ? "yes" : "no"
来源：https://be.zhonguo8118.cn

C#:   x > 0 ? "yes" : "no"
来源：https://zx.zhonguo6118.cn

[A12] 字符串插值 / 格式化
来源：https://uq.zhonguo3118.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：https://gz.zhonguo2118.cn


<!-- 参考信息 -->