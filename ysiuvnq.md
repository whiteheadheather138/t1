代发 wailian999

[U51] PHP：数组解构
来源：https://tc.zhonguo5118.cn

[$a, $b] = $arr;
来源：https://gs.zhonguo3118.cn

[U52] PHP：箭头函数
来源：https://em.zhonguo7118.cn

$double = fn($x) => $x * 2;
来源：https://ls.zhonguo8118.cn

[U53] PHP：空合并运算符
来源：https://bq.zhonguo5118.cn

$v = $a ?? $b ?? "default";
来源：https://ef.zhonguo6118.cn

[U54] PHP：空安全调用
来源：https://zh.zhonguo7118.cn

$obj?->method()
来源：https://wf.zhonguo5118.cn

[U55] PHP：match 表达式
来源：https://ij.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://fn.zhonguo5118.cn

[U56] PHP：命名参数
来源：https://ek.zhonguo5118.cn

f(a: 1, b: 2)
来源：https://ma.zhonguo6118.cn

[U57] PHP：字符串插值
来源：https://ld.zhonguo8118.cn

"值: {$a}"
来源：https://gz.zhonguo6118.cn

[U58] PHP：数组三件套
来源：https://gf.zhonguo4118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://ev.zhonguo5118.cn

[U59] PHP：自定义排序
来源：https://pl.zhonguo5118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ze.zhonguo5118.cn

[U60] PHP：JSON 编解码
来源：https://ue.zhonguo6118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://gn.zhonguo6118.cn

[U61] PHP：正则
来源：https://ur.zhonguo1118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://gp.zhonguo1118.cn

[U62] PHP：日期对象
来源：https://rk.zhonguo3118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://iz.zhonguo5118.cn

[U63] PHP：文件读写
来源：https://es.zhonguo6118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://th.zhonguo8118.cn

[U64] PHP：目录遍历
来源：https://xg.zhonguo5118.cn

glob("dir/*.php");  scandir("dir");
来源：https://mx.zhonguo7118.cn

[U65] PHP：会话
来源：https://aq.zhonguo3118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://dm.zhonguo4118.cn

[U66] PHP：设置 Cookie
来源：https://vf.zhonguo5118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://iw.zhonguo2118.cn

[U67] PHP：处理文件上传
来源：https://aq.zhonguo6118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://vf.zhonguo7118.cn

[U68] PHP：PDO 连接
来源：https://qi.zhonguo1118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ap.zhonguo4118.cn

[U69] PHP：PDO 预处理
来源：https://dy.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://qj.zhonguo4118.cn

[U70] PHP：PDO 事务
来源：https://ga.zhonguo8118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://in.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://ua.zhonguo4118.cn

throw new RuntimeException("失败", 500);
来源：https://ip.zhonguo7118.cn

[U72] PHP：写错误日志
来源：https://sf.zhonguo6118.cn

error_log("失败: " . $e->getMessage());
来源：https://yo.zhonguo3118.cn

[U73] PHP：读取 ini 配置
来源：https://sy.zhonguo1118.cn

parse_ini_file("config.ini", true)
来源：https://mj.zhonguo6118.cn

[U74] PHP：读取环境变量
来源：https://nx.zhonguo7118.cn

getenv("APP_ENV") ?: "production"
来源：https://zh.zhonguo3118.cn

[U75] PHP：依赖注入
来源：https://bl.zhonguo4118.cn

composer require psr/container
来源：https://kd.zhonguo4118.cn

[U76] PHP：简单路由
来源：https://gl.zhonguo4118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ii.zhonguo8118.cn

[U77] PHP：模板渲染
来源：https://hc.zhonguo4118.cn

composer require twig/twig
来源：https://jd.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://dt.zhonguo5118.cn

composer require --dev phpunit/phpunit
来源：https://rz.zhonguo4118.cn

[U79] PHP：静态分析
来源：https://uz.zhonguo8118.cn

composer require --dev phpstan/phpstan
来源：https://sb.zhonguo7118.cn

[U80] PHP：代码规范修复
来源：https://xu.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://xm.zhonguo2118.cn

[U81] JS：初始化项目
来源：https://yg.zhonguo8118.cn

npm init -y;  npm i express
来源：https://ba.zhonguo5118.cn

[U82] JS：package.json 脚本
来源：https://ug.zhonguo2118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://lm.zhonguo5118.cn

[U83] JS：ES Module 导入导出
来源：https://wr.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://hs.zhonguo1118.cn

[U84] JS：CommonJS 写法
来源：https://wv.zhonguo4118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://cg.zhonguo2118.cn

[U85] JS：可选链
来源：https://cu.zhonguo6118.cn

a?.b?.c
来源：https://sh.zhonguo5118.cn

[U86] JS：空值合并
来源：https://tl.zhonguo3118.cn

a ?? b
来源：https://xu.zhonguo4118.cn

[U87] JS：解构默认值
来源：https://nv.zhonguo3118.cn

const { a = 1, b = 2 } = obj;
来源：https://uj.zhonguo4118.cn

[U88] JS：对象展开合并
来源：https://hc.zhonguo1118.cn

{ ...a, ...b }
来源：https://pw.zhonguo7118.cn

[U89] JS：数组去重
来源：https://kf.zhonguo3118.cn

[...new Set(arr)]
来源：https://zk.zhonguo2118.cn

[U90] JS：数字数组排序
来源：https://wy.zhonguo6118.cn

[...arr].sort((a, b) => a - b)
来源：https://uh.zhonguo8118.cn

[U91] JS：对象键值遍历
来源：https://cw.zhonguo7118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://qy.zhonguo2118.cn

[U92] JS：深拷贝
来源：https://jo.zhonguo1118.cn

structuredClone(obj)
来源：https://of.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://rt.zhonguo1118.cn

`共 ${n} 条`
来源：https://fy.zhonguo5118.cn

[U94] JS：箭头函数
来源：https://rr.zhonguo7118.cn

const double = x => x * 2;
来源：https://no.zhonguo7118.cn

[U95] JS：Promise 包装
来源：https://fy.zhonguo1118.cn

new Promise((resolve, reject) => {})
来源：https://nz.zhonguo7118.cn

[U96] JS：async/await 与异常
来源：https://rc.zhonguo2118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://uz.zhonguo8118.cn

[U97] JS：并发请求
来源：https://dk.zhonguo6118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://bi.zhonguo5118.cn

[U98] JS：fetch 带 JSON
来源：https://sy.zhonguo1118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://zx.zhonguo5118.cn

[U99] JS：事件监听
来源：https://ak.zhonguo1118.cn

el.addEventListener("click", e => {})
来源：https://ul.zhonguo1118.cn

[U100] JS：DOM 查询
来源：https://ch.zhonguo8118.cn

document.querySelector(".item")
来源：https://dl.zhonguo8118.cn

[U101] JS：classList 操作
来源：https://qm.zhonguo6118.cn

el.classList.toggle("active")
来源：https://oh.zhonguo3118.cn

[U102] JS：本地存储
来源：https://zy.zhonguo4118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://fw.zhonguo6118.cn

[U103] JS：定时器
来源：https://bg.zhonguo6118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://ls.zhonguo8118.cn

[U104] JS：防抖
来源：https://gg.zhonguo7118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://cs.zhonguo1118.cn

[U105] JS：节流
来源：https://vu.zhonguo1118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://id.zhonguo4118.cn

[U106] JS：日期格式化
来源：https://bz.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://ox.zhonguo2118.cn

[U107] JS：数字千分位
来源：https://rw.zhonguo6118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://fg.zhonguo3118.cn

[U108] JS：随机整数
来源：https://gs.zhonguo1118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://um.zhonguo1118.cn

[U109] JS：数组分组
来源：https://hv.zhonguo6118.cn

Object.groupBy(arr, x => x.type)
来源：https://xl.zhonguo8118.cn

[U110] JS：数组分块
来源：https://ul.zhonguo5118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ij.zhonguo1118.cn

[U111] JS：对象转 Map
来源：https://qh.zhonguo3118.cn

new Map(Object.entries(obj))
来源：https://og.zhonguo1118.cn

[U112] JS：字符串补位
来源：https://he.zhonguo8118.cn

"7".padStart(3, "0")
来源：https://pz.zhonguo4118.cn

[U113] JS：正则替换全部
来源：https://ml.zhonguo1118.cn

s.replaceAll("a", "b")
来源：https://gh.zhonguo7118.cn

[U114] JS：JSON 深比较
来源：https://gk.zhonguo7118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://kk.zhonguo1118.cn

[U115] JS：生成 UUID
来源：https://ce.zhonguo1118.cn

crypto.randomUUID()
来源：https://vx.zhonguo1118.cn

[U116] JS：类型检查（JSDoc）
来源：https://zb.zhonguo5118.cn

/** @param {string} name */ function f(name) {}
来源：https://bd.zhonguo1118.cn

[U117] JS：单元测试
来源：https://zv.zhonguo8118.cn

npm i -D vitest;  npx vitest
来源：https://gy.zhonguo2118.cn

[U118] JS：开发服务器
来源：https://ic.zhonguo8118.cn

npm i -D vite;  npx vite
来源：https://hw.zhonguo3118.cn

[U119] JS：生产构建
来源：https://vu.zhonguo1118.cn

npx vite build
来源：https://be.zhonguo6118.cn

[U120] JS：读取环境变量（Vite）
来源：https://zs.zhonguo7118.cn

import.meta.env.VITE_API_URL
来源：https://yc.zhonguo1118.cn

================================================================================
来源：https://ba.zhonguo6118.cn

统计汇总
来源：https://ao.zhonguo2118.cn

================================================================================
来源：https://gl.zhonguo5118.cn

按语言统计（条）：
来源：https://dj.zhonguo5118.cn

Python ......... 252
来源：https://qa.zhonguo7118.cn

PHP ............ 252
来源：https://al.zhonguo7118.cn

JavaScript ..... 252
来源：https://af.zhonguo1118.cn

TypeScript ..... 212
来源：https://az.zhonguo7118.cn

Java ........... 212
来源：https://nq.zhonguo6118.cn

Go ............. 212
来源：https://jw.zhonguo4118.cn

Ruby ........... 212
来源：https://xl.zhonguo8118.cn

C# ............. 212
来源：https://wg.zhonguo4118.cn

C .............. 30
来源：https://ob.zhonguo2118.cn

C++ ............ 30
来源：https://ud.zhonguo4118.cn

SQL ............ 90
来源：https://wi.zhonguo3118.cn

Bash ........... 80
来源：https://fn.zhonguo8118.cn

Kotlin ......... 15
来源：https://xy.zhonguo3118.cn

Swift .......... 15
来源：https://he.zhonguo2118.cn

Lua ............ 10
来源：https://jl.zhonguo1118.cn

Perl ........... 10
来源：https://zb.zhonguo6118.cn

Scala .......... 10
来源：https://cf.zhonguo6118.cn

------------------------------------
来源：https://km.zhonguo6118.cn

合计 ........... 2106 条
来源：https://bg.zhonguo5118.cn

按章节统计：
来源：https://ha.zhonguo6118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://hu.zhonguo6118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://vr.zhonguo5118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://jd.zhonguo6118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://wg.zhonguo2118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://yi.zhonguo4118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://ly.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://ph.zhonguo6118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://xd.zhonguo8118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://pw.zhonguo3118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://dn.zhonguo3118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://yv.zhonguo1118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://ob.zhonguo6118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://yg.zhonguo8118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://ia.zhonguo1118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://iu.zhonguo6118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://yn.zhonguo2118.cn

Q SQL 专题                              90
来源：https://fb.zhonguo3118.cn

R Bash 专题                             80
来源：https://xn.zhonguo5118.cn

S C / C++ 专题                          60
来源：https://wt.zhonguo6118.cn

T 其他语言补充                          60
来源：https://tr.zhonguo6118.cn

U 高频实用片段                         120
来源：https://nk.zhonguo2118.cn

------------------------------------
来源：https://xf.zhonguo4118.cn

合计                                  2106 条
来源：https://ny.zhonguo1118.cn

--------------------------------------------------------------------------------
来源：https://rg.zhonguo5118.cn

使用提醒
来源：https://sg.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://am.zhonguo8118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://kk.zhonguo7118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://ds.zhonguo5118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://rm.zhonguo1118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://ck.zhonguo4118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://tr.zhonguo2118.cn

—— 文件结束 ——
来源：https://mc.zhonguo1118.cn

================================================================================
来源：https://qk.zhonguo3118.cn

程序语言常见例子速查手册（2024 版）
来源：https://xj.zhonguo3118.cn

Common Programming Examples Cheat Book
来源：https://ib.zhonguo6118.cn

================================================================================
来源：https://rj.zhonguo3118.cn

【收录内容】
来源：https://vi.zhonguo7118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://iv.zhonguo5118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://ld.zhonguo5118.cn

SQL · Bash · C · C++
来源：https://qb.zhonguo4118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://vh.zhonguo6118.cn

【使用说明】
来源：https://cw.zhonguo3118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://zk.zhonguo4118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://yi.zhonguo3118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://oj.zhonguo1118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://io.zhonguo5118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://hy.zhonguo1118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://tz.zhonguo6118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://qn.zhonguo8118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://iz.zhonguo1118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://rw.zhonguo8118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://tp.zhonguo2118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://mo.zhonguo3118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://es.zhonguo4118.cn

【文件统计】
来源：https://gi.zhonguo1118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://qy.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://qg.zhonguo1118.cn

目  录
来源：https://yt.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://pq.zhonguo5118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://aj.zhonguo6118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://bw.zhonguo5118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://lw.zhonguo2118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://nw.zhonguo6118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://sv.zhonguo2118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://ub.zhonguo4118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://mn.zhonguo8118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://qi.zhonguo6118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://oy.zhonguo5118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://nn.zhonguo3118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://mr.zhonguo2118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://dd.zhonguo6118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://be.zhonguo5118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://hn.zhonguo2118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://hv.zhonguo2118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://vk.zhonguo6118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://uj.zhonguo5118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://hj.zhonguo5118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ah.zhonguo8118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://nc.zhonguo2118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://cz.zhonguo3118.cn

================================================================================
来源：https://ir.zhonguo1118.cn

A. 基础语法与类型
来源：https://vk.zhonguo6118.cn

================================================================================
来源：https://xz.zhonguo4118.cn

[A01] Hello World
来源：https://zn.zhonguo3118.cn

Py:   print("Hello, World!")
来源：https://su.zhonguo1118.cn

PHP:  echo "Hello, World!";
来源：https://zb.zhonguo2118.cn

JS:   console.log("Hello, World!");
来源：https://te.zhonguo3118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://fa.zhonguo7118.cn

Java: System.out.println("Hello, World!");
来源：https://tu.zhonguo2118.cn

Go:   fmt.Println("Hello, World!")
来源：https://hp.zhonguo3118.cn

Ruby: puts "Hello, World!"
来源：https://zy.zhonguo2118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://pv.zhonguo8118.cn

[A02] 变量声明与赋值
来源：https://sf.zhonguo7118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://fp.zhonguo2118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ru.zhonguo6118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://jl.zhonguo6118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://gk.zhonguo6118.cn

Java: String name = "Alex"; int age = 20;
来源：https://gs.zhonguo4118.cn

Go:   name := "Alex"; age := 20
来源：https://dh.zhonguo2118.cn

Ruby: name = "Alex"; age = 20
来源：https://wf.zhonguo8118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://ke.zhonguo5118.cn

[A03] 常量定义
来源：https://kq.zhonguo3118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://nt.zhonguo3118.cn

PHP:  const PI = 3.14159;
来源：https://ws.zhonguo4118.cn

JS:   const PI = 3.14159;
来源：https://zq.zhonguo6118.cn

TS:   const PI: number = 3.14159;
来源：https://ua.zhonguo7118.cn

Java: static final double PI = 3.14159;
来源：https://yo.zhonguo5118.cn

Go:   const PI = 3.14159
来源：https://lp.zhonguo6118.cn

Ruby: PI = 3.14159
来源：https://ym.zhonguo8118.cn

C#:   const double PI = 3.14159;
来源：https://wo.zhonguo1118.cn

[A04] 判断变量类型
来源：https://wk.zhonguo3118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://ft.zhonguo4118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://om.zhonguo7118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://nz.zhonguo2118.cn

TS:   typeof x; x instanceof Date
来源：https://ex.zhonguo7118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://gw.zhonguo7118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://ch.zhonguo7118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://pj.zhonguo8118.cn

C#:   x.GetType().Name; x is int
来源：https://mu.zhonguo5118.cn

[A05] 整数除法与取模
来源：https://bn.zhonguo6118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://tl.zhonguo1118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://fo.zhonguo7118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://rr.zhonguo6118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://vj.zhonguo6118.cn

Java: 7 / 2; 7 % 2
来源：https://pi.zhonguo4118.cn

Go:   7 / 2; 7 % 2
来源：https://xt.zhonguo7118.cn

Ruby: 7 / 2; 7 % 2
来源：https://my.zhonguo4118.cn

C#:   7 / 2; 7 % 2
来源：https://xa.zhonguo3118.cn

[A06] 字符串转数字
来源：https://yq.zhonguo4118.cn

Py:   int("42"); float("3.14")
来源：https://ma.zhonguo1118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://wi.zhonguo4118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://ft.zhonguo4118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://sg.zhonguo2118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://mv.zhonguo5118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://be.zhonguo8118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://my.zhonguo2118.cn


<!-- 参考信息 -->