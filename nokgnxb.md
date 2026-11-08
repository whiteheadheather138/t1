代发 wailian999

[U55] PHP：match 表达式
来源：https://jz.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://va.zhonguo6118.cn

[U56] PHP：命名参数
来源：https://um.zhonguo1118.cn

f(a: 1, b: 2)
来源：https://hd.zhonguo4118.cn

[U57] PHP：字符串插值
来源：https://po.zhonguo4118.cn

"值: {$a}"
来源：https://ql.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://nr.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://zk.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://kb.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ro.zhonguo3118.cn

[U60] PHP：JSON 编解码
来源：https://sz.zhonguo5118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://mu.zhonguo1118.cn

[U61] PHP：正则
来源：https://pj.zhonguo5118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://xs.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://fu.zhonguo1118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://py.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://lz.zhonguo6118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://cq.zhonguo5118.cn

[U64] PHP：目录遍历
来源：https://nv.zhonguo2118.cn

glob("dir/*.php");  scandir("dir");
来源：https://mw.zhonguo5118.cn

[U65] PHP：会话
来源：https://xa.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://cf.zhonguo4118.cn

[U66] PHP：设置 Cookie
来源：https://aj.zhonguo4118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://et.zhonguo1118.cn

[U67] PHP：处理文件上传
来源：https://tw.zhonguo4118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://en.zhonguo3118.cn

[U68] PHP：PDO 连接
来源：https://we.zhonguo2118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://er.zhonguo5118.cn

[U69] PHP：PDO 预处理
来源：https://np.zhonguo1118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://ib.zhonguo5118.cn

[U70] PHP：PDO 事务
来源：https://xj.zhonguo3118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://jv.zhonguo3118.cn

[U71] PHP：抛出异常
来源：https://eu.zhonguo4118.cn

throw new RuntimeException("失败", 500);
来源：https://uf.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://pn.zhonguo4118.cn

error_log("失败: " . $e->getMessage());
来源：https://mx.zhonguo1118.cn

[U73] PHP：读取 ini 配置
来源：https://ih.zhonguo8118.cn

parse_ini_file("config.ini", true)
来源：https://hw.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://nn.zhonguo7118.cn

getenv("APP_ENV") ?: "production"
来源：https://dk.zhonguo8118.cn

[U75] PHP：依赖注入
来源：https://zy.zhonguo4118.cn

composer require psr/container
来源：https://kc.zhonguo4118.cn

[U76] PHP：简单路由
来源：https://rp.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://po.zhonguo7118.cn

[U77] PHP：模板渲染
来源：https://pv.zhonguo5118.cn

composer require twig/twig
来源：https://bm.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://rn.zhonguo5118.cn

composer require --dev phpunit/phpunit
来源：https://ar.zhonguo3118.cn

[U79] PHP：静态分析
来源：https://sx.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://te.zhonguo5118.cn

[U80] PHP：代码规范修复
来源：https://sp.zhonguo4118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://vg.zhonguo7118.cn

[U81] JS：初始化项目
来源：https://ji.zhonguo4118.cn

npm init -y;  npm i express
来源：https://nf.zhonguo7118.cn

[U82] JS：package.json 脚本
来源：https://rc.zhonguo1118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://aj.zhonguo2118.cn

[U83] JS：ES Module 导入导出
来源：https://tv.zhonguo8118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://gc.zhonguo8118.cn

[U84] JS：CommonJS 写法
来源：https://jh.zhonguo1118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://hv.zhonguo3118.cn

[U85] JS：可选链
来源：https://ov.zhonguo7118.cn

a?.b?.c
来源：https://ta.zhonguo4118.cn

[U86] JS：空值合并
来源：https://tv.zhonguo2118.cn

a ?? b
来源：https://qo.zhonguo8118.cn

[U87] JS：解构默认值
来源：https://ts.zhonguo1118.cn

const { a = 1, b = 2 } = obj;
来源：https://kx.zhonguo1118.cn

[U88] JS：对象展开合并
来源：https://fm.zhonguo1118.cn

{ ...a, ...b }
来源：https://ar.zhonguo2118.cn

[U89] JS：数组去重
来源：https://zs.zhonguo3118.cn

[...new Set(arr)]
来源：https://rh.zhonguo1118.cn

[U90] JS：数字数组排序
来源：https://to.zhonguo8118.cn

[...arr].sort((a, b) => a - b)
来源：https://ge.zhonguo7118.cn

[U91] JS：对象键值遍历
来源：https://oh.zhonguo2118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://be.zhonguo8118.cn

[U92] JS：深拷贝
来源：https://ei.zhonguo3118.cn

structuredClone(obj)
来源：https://zv.zhonguo3118.cn

[U93] JS：模板字符串
来源：https://bo.zhonguo1118.cn

`共 ${n} 条`
来源：https://rv.zhonguo3118.cn

[U94] JS：箭头函数
来源：https://xx.zhonguo4118.cn

const double = x => x * 2;
来源：https://vi.zhonguo6118.cn

[U95] JS：Promise 包装
来源：https://ba.zhonguo3118.cn

new Promise((resolve, reject) => {})
来源：https://nl.zhonguo5118.cn

[U96] JS：async/await 与异常
来源：https://ub.zhonguo3118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://bj.zhonguo1118.cn

[U97] JS：并发请求
来源：https://he.zhonguo8118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://zm.zhonguo6118.cn

[U98] JS：fetch 带 JSON
来源：https://nj.zhonguo4118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ph.zhonguo4118.cn

[U99] JS：事件监听
来源：https://mf.zhonguo2118.cn

el.addEventListener("click", e => {})
来源：https://uv.zhonguo3118.cn

[U100] JS：DOM 查询
来源：https://zi.zhonguo3118.cn

document.querySelector(".item")
来源：https://rt.zhonguo4118.cn

[U101] JS：classList 操作
来源：https://hp.zhonguo7118.cn

el.classList.toggle("active")
来源：https://tj.zhonguo7118.cn

[U102] JS：本地存储
来源：https://cy.zhonguo3118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://sf.zhonguo6118.cn

[U103] JS：定时器
来源：https://ev.zhonguo7118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://sd.zhonguo7118.cn

[U104] JS：防抖
来源：https://mw.zhonguo4118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://yy.zhonguo1118.cn

[U105] JS：节流
来源：https://yk.zhonguo6118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://mz.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://fd.zhonguo1118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://si.zhonguo1118.cn

[U107] JS：数字千分位
来源：https://cq.zhonguo8118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://ho.zhonguo5118.cn

[U108] JS：随机整数
来源：https://yg.zhonguo8118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://kq.zhonguo2118.cn

[U109] JS：数组分组
来源：https://br.zhonguo6118.cn

Object.groupBy(arr, x => x.type)
来源：https://en.zhonguo6118.cn

[U110] JS：数组分块
来源：https://lk.zhonguo8118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://et.zhonguo8118.cn

[U111] JS：对象转 Map
来源：https://ut.zhonguo8118.cn

new Map(Object.entries(obj))
来源：https://nt.zhonguo7118.cn

[U112] JS：字符串补位
来源：https://rf.zhonguo2118.cn

"7".padStart(3, "0")
来源：https://yg.zhonguo3118.cn

[U113] JS：正则替换全部
来源：https://vu.zhonguo5118.cn

s.replaceAll("a", "b")
来源：https://jd.zhonguo3118.cn

[U114] JS：JSON 深比较
来源：https://mk.zhonguo7118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://os.zhonguo5118.cn

[U115] JS：生成 UUID
来源：https://um.zhonguo8118.cn

crypto.randomUUID()
来源：https://uk.zhonguo1118.cn

[U116] JS：类型检查（JSDoc）
来源：https://cl.zhonguo3118.cn

/** @param {string} name */ function f(name) {}
来源：https://lm.zhonguo7118.cn

[U117] JS：单元测试
来源：https://fy.zhonguo1118.cn

npm i -D vitest;  npx vitest
来源：https://nj.zhonguo3118.cn

[U118] JS：开发服务器
来源：https://zg.zhonguo5118.cn

npm i -D vite;  npx vite
来源：https://bs.zhonguo6118.cn

[U119] JS：生产构建
来源：https://xw.zhonguo7118.cn

npx vite build
来源：https://bj.zhonguo5118.cn

[U120] JS：读取环境变量（Vite）
来源：https://lj.zhonguo8118.cn

import.meta.env.VITE_API_URL
来源：https://hc.zhonguo5118.cn

================================================================================
来源：https://mq.zhonguo1118.cn

统计汇总
来源：https://ze.zhonguo8118.cn

================================================================================
来源：https://tz.zhonguo3118.cn

按语言统计（条）：
来源：https://ys.zhonguo2118.cn

Python ......... 252
来源：https://fc.zhonguo8118.cn

PHP ............ 252
来源：https://wa.zhonguo2118.cn

JavaScript ..... 252
来源：https://zl.zhonguo5118.cn

TypeScript ..... 212
来源：https://fu.zhonguo6118.cn

Java ........... 212
来源：https://oc.zhonguo4118.cn

Go ............. 212
来源：https://rs.zhonguo5118.cn

Ruby ........... 212
来源：https://ov.zhonguo1118.cn

C# ............. 212
来源：https://gc.zhonguo3118.cn

C .............. 30
来源：https://ph.zhonguo1118.cn

C++ ............ 30
来源：https://pk.zhonguo6118.cn

SQL ............ 90
来源：https://mv.zhonguo2118.cn

Bash ........... 80
来源：https://cr.zhonguo1118.cn

Kotlin ......... 15
来源：https://bu.zhonguo1118.cn

Swift .......... 15
来源：https://jo.zhonguo5118.cn

Lua ............ 10
来源：https://rq.zhonguo5118.cn

Perl ........... 10
来源：https://rk.zhonguo6118.cn

Scala .......... 10
来源：https://nx.zhonguo1118.cn

------------------------------------
来源：https://vx.zhonguo6118.cn

合计 ........... 2106 条
来源：https://sc.zhonguo6118.cn

按章节统计：
来源：https://xz.zhonguo3118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://jj.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://bh.zhonguo2118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://ln.zhonguo1118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://ga.zhonguo1118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://kk.zhonguo4118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://zt.zhonguo6118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://nl.zhonguo6118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://xg.zhonguo2118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://tz.zhonguo1118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://sz.zhonguo4118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://wl.zhonguo5118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://or.zhonguo1118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://sx.zhonguo2118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://ov.zhonguo6118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://mt.zhonguo2118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://aw.zhonguo5118.cn

Q SQL 专题                              90
来源：https://pb.zhonguo5118.cn

R Bash 专题                             80
来源：https://xz.zhonguo2118.cn

S C / C++ 专题                          60
来源：https://qj.zhonguo4118.cn

T 其他语言补充                          60
来源：https://fv.zhonguo7118.cn

U 高频实用片段                         120
来源：https://kg.zhonguo6118.cn

------------------------------------
来源：https://cy.zhonguo3118.cn

合计                                  2106 条
来源：https://rr.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://an.zhonguo7118.cn

使用提醒
来源：https://wh.zhonguo1118.cn

--------------------------------------------------------------------------------
来源：https://gx.zhonguo1118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://sg.zhonguo2118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://do.zhonguo4118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://jh.zhonguo7118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://nv.zhonguo8118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://zg.zhonguo1118.cn

—— 文件结束 ——
来源：https://ha.zhonguo4118.cn

================================================================================
来源：https://fs.zhonguo4118.cn

程序语言常见例子速查手册（2024 版）
来源：https://ch.zhonguo2118.cn

Common Programming Examples Cheat Book
来源：https://go.zhonguo1118.cn

================================================================================
来源：https://oq.zhonguo6118.cn

【收录内容】
来源：https://ep.zhonguo2118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://ij.zhonguo3118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://cj.zhonguo8118.cn

SQL · Bash · C · C++
来源：https://vb.zhonguo1118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://lb.zhonguo3118.cn

【使用说明】
来源：https://mu.zhonguo3118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://ma.zhonguo6118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://zk.zhonguo5118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://wc.zhonguo6118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://tw.zhonguo6118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://zm.zhonguo4118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://da.zhonguo4118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://am.zhonguo1118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://xx.zhonguo7118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://dw.zhonguo6118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://bf.zhonguo3118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://yc.zhonguo5118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://um.zhonguo7118.cn

【文件统计】
来源：https://mw.zhonguo2118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://gh.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://ur.zhonguo3118.cn

目  录
来源：https://tg.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://pv.zhonguo8118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://zk.zhonguo6118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://cc.zhonguo3118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://uj.zhonguo1118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://hk.zhonguo3118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://zx.zhonguo2118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://qq.zhonguo6118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://na.zhonguo8118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://bn.zhonguo4118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://ye.zhonguo7118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://li.zhonguo3118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://oo.zhonguo3118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://br.zhonguo1118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://nf.zhonguo2118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://jm.zhonguo4118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://gb.zhonguo2118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://gw.zhonguo5118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://ut.zhonguo8118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://on.zhonguo7118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://jc.zhonguo5118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://wb.zhonguo6118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://pz.zhonguo3118.cn

================================================================================
来源：https://pz.zhonguo1118.cn

A. 基础语法与类型
来源：https://jh.zhonguo5118.cn

================================================================================
来源：https://id.zhonguo1118.cn

[A01] Hello World
来源：https://hq.zhonguo7118.cn

Py:   print("Hello, World!")
来源：https://az.zhonguo7118.cn

PHP:  echo "Hello, World!";
来源：https://qb.zhonguo5118.cn

JS:   console.log("Hello, World!");
来源：https://kb.zhonguo1118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://wm.zhonguo4118.cn

Java: System.out.println("Hello, World!");
来源：https://vc.zhonguo1118.cn

Go:   fmt.Println("Hello, World!")
来源：https://un.zhonguo5118.cn

Ruby: puts "Hello, World!"
来源：https://wo.zhonguo3118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://oz.zhonguo7118.cn

[A02] 变量声明与赋值
来源：https://sh.zhonguo5118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://gx.zhonguo4118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://ck.zhonguo4118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://ng.zhonguo4118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://ex.zhonguo3118.cn

Java: String name = "Alex"; int age = 20;
来源：https://xn.zhonguo5118.cn

Go:   name := "Alex"; age := 20
来源：https://al.zhonguo4118.cn

Ruby: name = "Alex"; age = 20
来源：https://ze.zhonguo8118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://wi.zhonguo5118.cn

[A03] 常量定义
来源：https://zu.zhonguo3118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://ad.zhonguo1118.cn

PHP:  const PI = 3.14159;
来源：https://gg.zhonguo4118.cn

JS:   const PI = 3.14159;
来源：https://cu.zhonguo8118.cn

TS:   const PI: number = 3.14159;
来源：https://gv.zhonguo6118.cn

Java: static final double PI = 3.14159;
来源：https://gm.zhonguo7118.cn

Go:   const PI = 3.14159
来源：https://yr.zhonguo2118.cn

Ruby: PI = 3.14159
来源：https://gq.zhonguo4118.cn

C#:   const double PI = 3.14159;
来源：https://ub.zhonguo4118.cn

[A04] 判断变量类型
来源：https://vx.zhonguo6118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://dw.zhonguo7118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://co.zhonguo2118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://ze.zhonguo1118.cn

TS:   typeof x; x instanceof Date
来源：https://ma.zhonguo3118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://lp.zhonguo6118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://jh.zhonguo7118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://dm.zhonguo2118.cn

C#:   x.GetType().Name; x is int
来源：https://go.zhonguo5118.cn

[A05] 整数除法与取模
来源：https://pa.zhonguo8118.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：https://ch.zhonguo6118.cn

PHP:  intdiv(7, 2); 7 % 2
来源：https://nd.zhonguo2118.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：https://kv.zhonguo8118.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：https://mw.zhonguo5118.cn

Java: 7 / 2; 7 % 2
来源：https://al.zhonguo6118.cn

Go:   7 / 2; 7 % 2
来源：https://ft.zhonguo8118.cn

Ruby: 7 / 2; 7 % 2
来源：https://ql.zhonguo2118.cn

C#:   7 / 2; 7 % 2
来源：https://hj.zhonguo8118.cn

[A06] 字符串转数字
来源：https://yt.zhonguo2118.cn

Py:   int("42"); float("3.14")
来源：https://fr.zhonguo6118.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：https://pt.zhonguo7118.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：https://kn.zhonguo5118.cn

TS:   parseInt("42", 10); Number("42")
来源：https://aw.zhonguo4118.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：https://jf.zhonguo3118.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：https://fu.zhonguo8118.cn

Ruby: "42".to_i; "3.14".to_f
来源：https://tc.zhonguo8118.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：https://rp.zhonguo2118.cn

[A07] 数字转字符串
来源：https://jz.zhonguo1118.cn

Py:   str(42)
来源：https://oc.zhonguo1118.cn

PHP:  (string) 42; strval(42)
来源：https://eq.zhonguo7118.cn

JS:   String(42); (42).toString()
来源：https://ea.zhonguo6118.cn

TS:   String(42)
来源：https://oz.zhonguo7118.cn

Java: String.valueOf(42); Integer.toString(42)
来源：https://sq.zhonguo8118.cn

Go:   strconv.Itoa(42)
来源：https://es.zhonguo4118.cn


<!-- 参考信息 -->