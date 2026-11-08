代发 wailian999

[U67] PHP：处理文件上传
来源：https://dq.zhonguo8118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://fb.zhonguo8118.cn

[U68] PHP：PDO 连接
来源：https://cj.zhonguo4118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://rv.zhonguo4118.cn

[U69] PHP：PDO 预处理
来源：https://xm.zhonguo7118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://ni.zhonguo6118.cn

[U70] PHP：PDO 事务
来源：https://di.zhonguo4118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://mu.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://ka.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://fb.zhonguo5118.cn

[U72] PHP：写错误日志
来源：https://mg.zhonguo4118.cn

error_log("失败: " . $e->getMessage());
来源：https://rg.zhonguo5118.cn

[U73] PHP：读取 ini 配置
来源：https://ad.zhonguo5118.cn

parse_ini_file("config.ini", true)
来源：https://fd.zhonguo8118.cn

[U74] PHP：读取环境变量
来源：https://xr.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://um.zhonguo4118.cn

[U75] PHP：依赖注入
来源：https://hx.zhonguo8118.cn

composer require psr/container
来源：https://bw.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://zc.zhonguo6118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://fs.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://qe.zhonguo1118.cn

composer require twig/twig
来源：https://wx.zhonguo3118.cn

[U78] PHP：单元测试
来源：https://vc.zhonguo7118.cn

composer require --dev phpunit/phpunit
来源：https://kh.zhonguo3118.cn

[U79] PHP：静态分析
来源：https://yr.zhonguo7118.cn

composer require --dev phpstan/phpstan
来源：https://xx.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://ti.zhonguo2118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://pl.zhonguo5118.cn

[U81] JS：初始化项目
来源：https://vf.zhonguo6118.cn

npm init -y;  npm i express
来源：https://ax.zhonguo5118.cn

[U82] JS：package.json 脚本
来源：https://mq.zhonguo7118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://dm.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://zl.zhonguo3118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://bs.zhonguo1118.cn

[U84] JS：CommonJS 写法
来源：https://uf.zhonguo8118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://of.zhonguo4118.cn

[U85] JS：可选链
来源：https://hg.zhonguo1118.cn

a?.b?.c
来源：https://na.zhonguo7118.cn

[U86] JS：空值合并
来源：https://mr.zhonguo4118.cn

a ?? b
来源：https://ck.zhonguo3118.cn

[U87] JS：解构默认值
来源：https://wx.zhonguo4118.cn

const { a = 1, b = 2 } = obj;
来源：https://lm.zhonguo2118.cn

[U88] JS：对象展开合并
来源：https://co.zhonguo6118.cn

{ ...a, ...b }
来源：https://dw.zhonguo7118.cn

[U89] JS：数组去重
来源：https://ie.zhonguo2118.cn

[...new Set(arr)]
来源：https://tr.zhonguo4118.cn

[U90] JS：数字数组排序
来源：https://lg.zhonguo8118.cn

[...arr].sort((a, b) => a - b)
来源：https://bf.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://cl.zhonguo6118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://lz.zhonguo2118.cn

[U92] JS：深拷贝
来源：https://kb.zhonguo6118.cn

structuredClone(obj)
来源：https://bj.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://ye.zhonguo5118.cn

`共 ${n} 条`
来源：https://xv.zhonguo8118.cn

[U94] JS：箭头函数
来源：https://qa.zhonguo2118.cn

const double = x => x * 2;
来源：https://ai.zhonguo7118.cn

[U95] JS：Promise 包装
来源：https://kf.zhonguo4118.cn

new Promise((resolve, reject) => {})
来源：https://ne.zhonguo4118.cn

[U96] JS：async/await 与异常
来源：https://er.zhonguo4118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://xl.zhonguo6118.cn

[U97] JS：并发请求
来源：https://el.zhonguo6118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://yw.zhonguo1118.cn

[U98] JS：fetch 带 JSON
来源：https://qp.zhonguo8118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ru.zhonguo3118.cn

[U99] JS：事件监听
来源：https://ur.zhonguo5118.cn

el.addEventListener("click", e => {})
来源：https://ex.zhonguo5118.cn

[U100] JS：DOM 查询
来源：https://rf.zhonguo8118.cn

document.querySelector(".item")
来源：https://jm.zhonguo2118.cn

[U101] JS：classList 操作
来源：https://ih.zhonguo1118.cn

el.classList.toggle("active")
来源：https://fs.zhonguo4118.cn

[U102] JS：本地存储
来源：https://fm.zhonguo4118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://zp.zhonguo3118.cn

[U103] JS：定时器
来源：https://rr.zhonguo5118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://cp.zhonguo3118.cn

[U104] JS：防抖
来源：https://ht.zhonguo4118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://gh.zhonguo4118.cn

[U105] JS：节流
来源：https://pz.zhonguo6118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://gz.zhonguo8118.cn

[U106] JS：日期格式化
来源：https://kr.zhonguo3118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://th.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://xr.zhonguo2118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://gh.zhonguo1118.cn

[U108] JS：随机整数
来源：https://lg.zhonguo7118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://hw.zhonguo6118.cn

[U109] JS：数组分组
来源：https://vm.zhonguo4118.cn

Object.groupBy(arr, x => x.type)
来源：https://lg.zhonguo3118.cn

[U110] JS：数组分块
来源：https://po.zhonguo2118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ai.zhonguo1118.cn

[U111] JS：对象转 Map
来源：https://fb.zhonguo3118.cn

new Map(Object.entries(obj))
来源：https://ln.zhonguo4118.cn

[U112] JS：字符串补位
来源：https://ej.zhonguo7118.cn

"7".padStart(3, "0")
来源：https://ow.zhonguo4118.cn

[U113] JS：正则替换全部
来源：https://ko.zhonguo2118.cn

s.replaceAll("a", "b")
来源：https://nb.zhonguo4118.cn

[U114] JS：JSON 深比较
来源：https://pc.zhonguo1118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://ek.zhonguo7118.cn

[U115] JS：生成 UUID
来源：https://dp.zhonguo1118.cn

crypto.randomUUID()
来源：https://su.zhonguo4118.cn

[U116] JS：类型检查（JSDoc）
来源：https://ir.zhonguo4118.cn

/** @param {string} name */ function f(name) {}
来源：https://so.zhonguo1118.cn

[U117] JS：单元测试
来源：https://zi.zhonguo7118.cn

npm i -D vitest;  npx vitest
来源：https://xi.zhonguo7118.cn

[U118] JS：开发服务器
来源：https://sl.zhonguo7118.cn

npm i -D vite;  npx vite
来源：https://mf.zhonguo2118.cn

[U119] JS：生产构建
来源：https://oe.zhonguo6118.cn

npx vite build
来源：https://ko.zhonguo8118.cn

[U120] JS：读取环境变量（Vite）
来源：https://gq.zhonguo1118.cn

import.meta.env.VITE_API_URL
来源：https://ea.zhonguo8118.cn

================================================================================
来源：https://ng.zhonguo2118.cn

统计汇总
来源：https://kt.zhonguo6118.cn

================================================================================
来源：https://gw.zhonguo8118.cn

按语言统计（条）：
来源：https://wt.zhonguo1118.cn

Python ......... 252
来源：https://ey.zhonguo6118.cn

PHP ............ 252
来源：https://xk.zhonguo7118.cn

JavaScript ..... 252
来源：https://ud.zhonguo3118.cn

TypeScript ..... 212
来源：https://gj.zhonguo2118.cn

Java ........... 212
来源：https://fi.zhonguo8118.cn

Go ............. 212
来源：https://je.zhonguo3118.cn

Ruby ........... 212
来源：https://mb.zhonguo5118.cn

C# ............. 212
来源：https://tg.zhonguo6118.cn

C .............. 30
来源：https://om.zhonguo3118.cn

C++ ............ 30
来源：https://ht.zhonguo5118.cn

SQL ............ 90
来源：https://hp.zhonguo5118.cn

Bash ........... 80
来源：https://ra.zhonguo4118.cn

Kotlin ......... 15
来源：https://sq.zhonguo2118.cn

Swift .......... 15
来源：https://cy.zhonguo1118.cn

Lua ............ 10
来源：https://ew.zhonguo8118.cn

Perl ........... 10
来源：https://fo.zhonguo5118.cn

Scala .......... 10
来源：https://yr.zhonguo7118.cn

------------------------------------
来源：https://bl.zhonguo5118.cn

合计 ........... 2106 条
来源：https://sy.zhonguo2118.cn

按章节统计：
来源：https://js.zhonguo5118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://hp.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://vt.zhonguo3118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://it.zhonguo4118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://hx.zhonguo2118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://fx.zhonguo7118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://yz.zhonguo6118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://eq.zhonguo4118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://zu.zhonguo3118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://vx.zhonguo3118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://qk.zhonguo8118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://sa.zhonguo7118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://tp.zhonguo6118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://wt.zhonguo4118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://xc.zhonguo6118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://xk.zhonguo2118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://hx.zhonguo4118.cn

Q SQL 专题                              90
来源：https://cx.zhonguo6118.cn

R Bash 专题                             80
来源：https://rj.zhonguo7118.cn

S C / C++ 专题                          60
来源：https://vl.zhonguo5118.cn

T 其他语言补充                          60
来源：https://he.zhonguo6118.cn

U 高频实用片段                         120
来源：https://yk.zhonguo1118.cn

------------------------------------
来源：https://qr.zhonguo1118.cn

合计                                  2106 条
来源：https://vn.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://bk.zhonguo5118.cn

使用提醒
来源：https://qr.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://ap.zhonguo1118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://ez.zhonguo4118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://ao.zhonguo8118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://yi.zhonguo1118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://fu.zhonguo6118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://fp.zhonguo5118.cn

—— 文件结束 ——
来源：https://zz.zhonguo4118.cn

================================================================================
来源：https://pp.zhonguo8118.cn

程序语言常见例子速查手册（2024 版）
来源：https://rg.zhonguo5118.cn

Common Programming Examples Cheat Book
来源：https://ho.zhonguo1118.cn

================================================================================
来源：https://hz.zhonguo7118.cn

【收录内容】
来源：https://jh.zhonguo6118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://dj.zhonguo2118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://tw.zhonguo6118.cn

SQL · Bash · C · C++
来源：https://ub.zhonguo4118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://xa.zhonguo7118.cn

【使用说明】
来源：https://ff.zhonguo2118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://rt.zhonguo5118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://ej.zhonguo7118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://ju.zhonguo1118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://xo.zhonguo4118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://ot.zhonguo2118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://ql.zhonguo6118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://rq.zhonguo8118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://iy.zhonguo7118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://by.zhonguo8118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://ri.zhonguo2118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://eo.zhonguo3118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://us.zhonguo1118.cn

【文件统计】
来源：https://tz.zhonguo2118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://vy.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://xk.zhonguo5118.cn

目  录
来源：https://ga.zhonguo2118.cn

--------------------------------------------------------------------------------
来源：https://lg.zhonguo4118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://az.zhonguo5118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://ts.zhonguo4118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://ca.zhonguo5118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://ei.zhonguo5118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://yu.zhonguo3118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://fx.zhonguo7118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://ey.zhonguo6118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://jn.zhonguo5118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://rb.zhonguo8118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://pv.zhonguo4118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://sa.zhonguo8118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://bp.zhonguo5118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://op.zhonguo5118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://kd.zhonguo1118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://dz.zhonguo5118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://bv.zhonguo5118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://rq.zhonguo4118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://za.zhonguo8118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://jn.zhonguo5118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://ik.zhonguo5118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://rf.zhonguo5118.cn

================================================================================
来源：https://hv.zhonguo3118.cn

A. 基础语法与类型
来源：https://ep.zhonguo8118.cn

================================================================================
来源：https://qi.zhonguo3118.cn

[A01] Hello World
来源：https://kb.zhonguo4118.cn

Py:   print("Hello, World!")
来源：https://tx.zhonguo8118.cn

PHP:  echo "Hello, World!";
来源：https://pt.zhonguo3118.cn

JS:   console.log("Hello, World!");
来源：https://bz.zhonguo5118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://wq.zhonguo1118.cn

Java: System.out.println("Hello, World!");
来源：https://ps.zhonguo8118.cn

Go:   fmt.Println("Hello, World!")
来源：https://wq.zhonguo5118.cn

Ruby: puts "Hello, World!"
来源：https://fl.zhonguo5118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://xc.zhonguo1118.cn

[A02] 变量声明与赋值
来源：https://fy.zhonguo4118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://ku.zhonguo1118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ts.zhonguo8118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://hb.zhonguo6118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://bm.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://jj.zhonguo5118.cn

Go:   name := "Alex"; age := 20
来源：https://ie.zhonguo8118.cn

Ruby: name = "Alex"; age = 20
来源：https://at.zhonguo6118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://gs.zhonguo6118.cn

[A03] 常量定义
来源：https://jj.zhonguo6118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://ky.zhonguo4118.cn

PHP:  const PI = 3.14159;
来源：https://ve.zhonguo1118.cn

JS:   const PI = 3.14159;
来源：https://wi.zhonguo7118.cn

TS:   const PI: number = 3.14159;
来源：https://yc.zhonguo8118.cn

Java: static final double PI = 3.14159;
来源：https://gp.zhonguo2118.cn

Go:   const PI = 3.14159
来源：https://cu.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://uw.zhonguo8118.cn

C#:   const double PI = 3.14159;
来源：https://ce.zhonguo8118.cn

[A04] 判断变量类型
来源：https://ih.zhonguo5118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://qg.zhonguo5118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://qs.zhonguo3118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://bl.zhonguo8118.cn

TS:   typeof x; x instanceof Date
来源：https://st.zhonguo8118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://bl.zhonguo7118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://gb.zhonguo3118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://lr.zhonguo3118.cn

C#:   x.GetType().Name; x is int
来源：https://zs.zhonguo4118.cn

[A05] 整数除法与取模
来源：https://bh.zhonguo6118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://wu.zhonguo2118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://wa.zhonguo8118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://ry.zhonguo5118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://yx.zhonguo1118.cn

Java: 7 / 2; 7 % 2
来源：https://pt.zhonguo3118.cn

Go:   7 / 2; 7 % 2
来源：https://jf.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://wp.zhonguo7118.cn

C#:   7 / 2; 7 % 2
来源：https://xf.zhonguo8118.cn

[A06] 字符串转数字
来源：https://ej.zhonguo1118.cn

Py:   int("42"); float("3.14")
来源：https://kz.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://we.zhonguo3118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://iw.zhonguo5118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://bn.zhonguo8118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://mj.zhonguo4118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://ck.zhonguo1118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://wz.zhonguo2118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://ez.zhonguo7118.cn

[A07] 数字转字符串
来源：https://yk.zhonguo2118.cn

Py:   str(42)
来源：https://tn.zhonguo8118.cn

PHP:  (string) 42; strval(42)
来源：https://ym.zhonguo1118.cn

JS:   String(42); (42).toString()
来源：https://ig.zhonguo3118.cn

TS:   String(42)
来源：https://ks.zhonguo2118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://rx.zhonguo4118.cn

Go:   strconv.Itoa(42)
来源：https://ch.zhonguo3118.cn

Ruby: 42.to_s
来源：https://av.zhonguo5118.cn

C#:   42.ToString()
来源：https://wa.zhonguo4118.cn

[A08] 取整与四舍五入
来源：https://id.zhonguo7118.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：https://hk.zhonguo1118.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：https://rs.zhonguo8118.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：https://jw.zhonguo2118.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：https://ha.zhonguo5118.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：https://cg.zhonguo5118.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：https://ge.zhonguo7118.cn

Ruby: 3.567.round(2); 3.9.floor
来源：https://oi.zhonguo3118.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：https://ld.zhonguo6118.cn

[A09] 绝对值与最大最小值
来源：https://ye.zhonguo8118.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：https://jn.zhonguo8118.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：https://vn.zhonguo8118.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：https://sk.zhonguo1118.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：https://ae.zhonguo2118.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：https://jw.zhonguo6118.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：https://gf.zhonguo7118.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：https://mj.zhonguo5118.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：https://tr.zhonguo5118.cn

[A10] 生成随机数
来源：https://me.zhonguo3118.cn

Py:   import random; random.randint(1, 100)
来源：https://ut.zhonguo4118.cn

PHP:  random_int(1, 100);
来源：https://lh.zhonguo1118.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：https://pm.zhonguo2118.cn


<!-- 参考信息 -->