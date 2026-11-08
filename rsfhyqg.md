代发 wailian999

[U43] PHP：声明命名空间
来源：https://jk.zhonguo8118.cn

namespace App\Http;
来源：https://yj.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://uu.zhonguo4118.cn

declare(strict_types=1);
来源：https://ud.zhonguo3118.cn

[U45] PHP：类型声明与返回类型
来源：https://ni.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://nk.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://nt.zhonguo3118.cn

?string $name = null
来源：https://fg.zhonguo4118.cn

[U47] PHP：联合类型
来源：https://kv.zhonguo3118.cn

int|string $id
来源：https://hm.zhonguo6118.cn

[U48] PHP：纯枚举
来源：https://jj.zhonguo6118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://hp.zhonguo1118.cn

[U49] PHP：只读属性
来源：https://xb.zhonguo2118.cn

public readonly string $name
来源：https://ml.zhonguo7118.cn

[U50] PHP：构造器属性提升
来源：https://ou.zhonguo2118.cn

public function __construct(private int $id) {}
来源：https://sw.zhonguo4118.cn

[U51] PHP：数组解构
来源：https://uc.zhonguo2118.cn

[$a, $b] = $arr;
来源：https://kx.zhonguo5118.cn

[U52] PHP：箭头函数
来源：https://fs.zhonguo2118.cn

$double = fn($x) => $x * 2;
来源：https://lq.zhonguo7118.cn

[U53] PHP：空合并运算符
来源：https://af.zhonguo2118.cn

$v = $a ?? $b ?? "default";
来源：https://za.zhonguo4118.cn

[U54] PHP：空安全调用
来源：https://ql.zhonguo7118.cn

$obj?->method()
来源：https://gx.zhonguo6118.cn

[U55] PHP：match 表达式
来源：https://ll.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://rd.zhonguo6118.cn

[U56] PHP：命名参数
来源：https://fs.zhonguo6118.cn

f(a: 1, b: 2)
来源：https://ve.zhonguo6118.cn

[U57] PHP：字符串插值
来源：https://wj.zhonguo4118.cn

"值: {$a}"
来源：https://zk.zhonguo4118.cn

[U58] PHP：数组三件套
来源：https://qw.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://gr.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://is.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://vc.zhonguo4118.cn

[U60] PHP：JSON 编解码
来源：https://jx.zhonguo2118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ql.zhonguo2118.cn

[U61] PHP：正则
来源：https://zw.zhonguo4118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://xv.zhonguo5118.cn

[U62] PHP：日期对象
来源：https://ii.zhonguo6118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://dj.zhonguo3118.cn

[U63] PHP：文件读写
来源：https://mp.zhonguo7118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://pm.zhonguo8118.cn

[U64] PHP：目录遍历
来源：https://rp.zhonguo2118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ln.zhonguo1118.cn

[U65] PHP：会话
来源：https://mf.zhonguo4118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://nz.zhonguo5118.cn

[U66] PHP：设置 Cookie
来源：https://nh.zhonguo7118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://ph.zhonguo8118.cn

[U67] PHP：处理文件上传
来源：https://aa.zhonguo1118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://dm.zhonguo4118.cn

[U68] PHP：PDO 连接
来源：https://oz.zhonguo4118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://uv.zhonguo7118.cn

[U69] PHP：PDO 预处理
来源：https://hr.zhonguo5118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://jp.zhonguo3118.cn

[U70] PHP：PDO 事务
来源：https://yu.zhonguo6118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://hr.zhonguo5118.cn

[U71] PHP：抛出异常
来源：https://nd.zhonguo5118.cn

throw new RuntimeException("失败", 500);
来源：https://ft.zhonguo2118.cn

[U72] PHP：写错误日志
来源：https://ck.zhonguo2118.cn

error_log("失败: " . $e->getMessage());
来源：https://rt.zhonguo4118.cn

[U73] PHP：读取 ini 配置
来源：https://tm.zhonguo1118.cn

parse_ini_file("config.ini", true)
来源：https://hr.zhonguo1118.cn

[U74] PHP：读取环境变量
来源：https://yr.zhonguo3118.cn

getenv("APP_ENV") ?: "production"
来源：https://ip.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://od.zhonguo6118.cn

composer require psr/container
来源：https://ab.zhonguo5118.cn

[U76] PHP：简单路由
来源：https://fz.zhonguo2118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://fc.zhonguo5118.cn

[U77] PHP：模板渲染
来源：https://yz.zhonguo4118.cn

composer require twig/twig
来源：https://bk.zhonguo4118.cn

[U78] PHP：单元测试
来源：https://ye.zhonguo4118.cn

composer require --dev phpunit/phpunit
来源：https://uk.zhonguo4118.cn

[U79] PHP：静态分析
来源：https://el.zhonguo1118.cn

composer require --dev phpstan/phpstan
来源：https://em.zhonguo7118.cn

[U80] PHP：代码规范修复
来源：https://kc.zhonguo5118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://ah.zhonguo6118.cn

[U81] JS：初始化项目
来源：https://yy.zhonguo7118.cn

npm init -y;  npm i express
来源：https://vb.zhonguo4118.cn

[U82] JS：package.json 脚本
来源：https://wm.zhonguo6118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://xs.zhonguo7118.cn

[U83] JS：ES Module 导入导出
来源：https://gw.zhonguo1118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://vu.zhonguo7118.cn

[U84] JS：CommonJS 写法
来源：https://bf.zhonguo4118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://au.zhonguo2118.cn

[U85] JS：可选链
来源：https://uy.zhonguo1118.cn

a?.b?.c
来源：https://yz.zhonguo4118.cn

[U86] JS：空值合并
来源：https://dc.zhonguo4118.cn

a ?? b
来源：https://he.zhonguo5118.cn

[U87] JS：解构默认值
来源：https://ti.zhonguo1118.cn

const { a = 1, b = 2 } = obj;
来源：https://dz.zhonguo2118.cn

[U88] JS：对象展开合并
来源：https://qn.zhonguo1118.cn

{ ...a, ...b }
来源：https://yu.zhonguo5118.cn

[U89] JS：数组去重
来源：https://rq.zhonguo6118.cn

[...new Set(arr)]
来源：https://fs.zhonguo7118.cn

[U90] JS：数字数组排序
来源：https://rq.zhonguo1118.cn

[...arr].sort((a, b) => a - b)
来源：https://qb.zhonguo7118.cn

[U91] JS：对象键值遍历
来源：https://sk.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://rv.zhonguo4118.cn

[U92] JS：深拷贝
来源：https://ez.zhonguo6118.cn

structuredClone(obj)
来源：https://dm.zhonguo4118.cn

[U93] JS：模板字符串
来源：https://xo.zhonguo8118.cn

`共 ${n} 条`
来源：https://yv.zhonguo1118.cn

[U94] JS：箭头函数
来源：https://im.zhonguo1118.cn

const double = x => x * 2;
来源：https://yh.zhonguo5118.cn

[U95] JS：Promise 包装
来源：https://ex.zhonguo7118.cn

new Promise((resolve, reject) => {})
来源：https://zl.zhonguo5118.cn

[U96] JS：async/await 与异常
来源：https://ax.zhonguo7118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://zv.zhonguo6118.cn

[U97] JS：并发请求
来源：https://gv.zhonguo8118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://ah.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://qh.zhonguo2118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://jk.zhonguo4118.cn

[U99] JS：事件监听
来源：https://dd.zhonguo5118.cn

el.addEventListener("click", e => {})
来源：https://wo.zhonguo5118.cn

[U100] JS：DOM 查询
来源：https://kt.zhonguo4118.cn

document.querySelector(".item")
来源：https://lw.zhonguo2118.cn

[U101] JS：classList 操作
来源：https://bf.zhonguo3118.cn

el.classList.toggle("active")
来源：https://ug.zhonguo7118.cn

[U102] JS：本地存储
来源：https://wa.zhonguo2118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://kx.zhonguo2118.cn

[U103] JS：定时器
来源：https://ej.zhonguo4118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://yx.zhonguo3118.cn

[U104] JS：防抖
来源：https://rz.zhonguo2118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://at.zhonguo7118.cn

[U105] JS：节流
来源：https://kd.zhonguo4118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://ad.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://rm.zhonguo1118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://xe.zhonguo4118.cn

[U107] JS：数字千分位
来源：https://bb.zhonguo5118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://xl.zhonguo3118.cn

[U108] JS：随机整数
来源：https://tp.zhonguo4118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://ht.zhonguo7118.cn

[U109] JS：数组分组
来源：https://eb.zhonguo6118.cn

Object.groupBy(arr, x => x.type)
来源：https://zt.zhonguo8118.cn

[U110] JS：数组分块
来源：https://xo.zhonguo5118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://gi.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://ad.zhonguo2118.cn

new Map(Object.entries(obj))
来源：https://bi.zhonguo7118.cn

[U112] JS：字符串补位
来源：https://ud.zhonguo1118.cn

"7".padStart(3, "0")
来源：https://jh.zhonguo3118.cn

[U113] JS：正则替换全部
来源：https://jn.zhonguo2118.cn

s.replaceAll("a", "b")
来源：https://se.zhonguo3118.cn

[U114] JS：JSON 深比较
来源：https://hu.zhonguo3118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://xy.zhonguo4118.cn

[U115] JS：生成 UUID
来源：https://su.zhonguo4118.cn

crypto.randomUUID()
来源：https://qx.zhonguo7118.cn

[U116] JS：类型检查（JSDoc）
来源：https://iy.zhonguo4118.cn

/** @param {string} name */ function f(name) {}
来源：https://gp.zhonguo4118.cn

[U117] JS：单元测试
来源：https://xh.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://iq.zhonguo4118.cn

[U118] JS：开发服务器
来源：https://qf.zhonguo6118.cn

npm i -D vite;  npx vite
来源：https://np.zhonguo2118.cn

[U119] JS：生产构建
来源：https://yc.zhonguo7118.cn

npx vite build
来源：https://ss.zhonguo6118.cn

[U120] JS：读取环境变量（Vite）
来源：https://hk.zhonguo3118.cn

import.meta.env.VITE_API_URL
来源：https://xh.zhonguo7118.cn

================================================================================
来源：https://zx.zhonguo8118.cn

统计汇总
来源：https://kj.zhonguo5118.cn

================================================================================
来源：https://za.zhonguo7118.cn

按语言统计（条）：
来源：https://wf.zhonguo7118.cn

Python ......... 252
来源：https://qy.zhonguo2118.cn

PHP ............ 252
来源：https://mn.zhonguo6118.cn

JavaScript ..... 252
来源：https://uc.zhonguo4118.cn

TypeScript ..... 212
来源：https://zw.zhonguo3118.cn

Java ........... 212
来源：https://gu.zhonguo4118.cn

Go ............. 212
来源：https://kw.zhonguo4118.cn

Ruby ........... 212
来源：https://co.zhonguo8118.cn

C# ............. 212
来源：https://bp.zhonguo3118.cn

C .............. 30
来源：https://qh.zhonguo8118.cn

C++ ............ 30
来源：https://la.zhonguo3118.cn

SQL ............ 90
来源：https://wo.zhonguo3118.cn

Bash ........... 80
来源：https://fy.zhonguo7118.cn

Kotlin ......... 15
来源：https://tt.zhonguo1118.cn

Swift .......... 15
来源：https://mh.zhonguo6118.cn

Lua ............ 10
来源：https://bn.zhonguo2118.cn

Perl ........... 10
来源：https://bu.zhonguo1118.cn

Scala .......... 10
来源：https://dr.zhonguo7118.cn

------------------------------------
来源：https://sy.zhonguo4118.cn

合计 ........... 2106 条
来源：https://ou.zhonguo2118.cn

按章节统计：
来源：https://jl.zhonguo2118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://pf.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://qp.zhonguo4118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://wm.zhonguo7118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://sh.zhonguo2118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://na.zhonguo6118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://cl.zhonguo4118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://zw.zhonguo4118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://ha.zhonguo1118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://yb.zhonguo5118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://dk.zhonguo1118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://kf.zhonguo2118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://uc.zhonguo4118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://az.zhonguo6118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://rr.zhonguo5118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://dc.zhonguo6118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://hr.zhonguo5118.cn

Q SQL 专题                              90
来源：https://at.zhonguo1118.cn

R Bash 专题                             80
来源：https://qv.zhonguo2118.cn

S C / C++ 专题                          60
来源：https://fl.zhonguo4118.cn

T 其他语言补充                          60
来源：https://xc.zhonguo3118.cn

U 高频实用片段                         120
来源：https://uv.zhonguo5118.cn

------------------------------------
来源：https://rx.zhonguo6118.cn

合计                                  2106 条
来源：https://cj.zhonguo2118.cn

--------------------------------------------------------------------------------
来源：https://ua.zhonguo6118.cn

使用提醒
来源：https://fu.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://ia.zhonguo6118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://ms.zhonguo4118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://hx.zhonguo1118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://hn.zhonguo4118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://tm.zhonguo4118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://aq.zhonguo6118.cn

—— 文件结束 ——
来源：https://yk.zhonguo8118.cn

================================================================================
来源：https://fq.zhonguo3118.cn

程序语言常见例子速查手册（2024 版）
来源：https://vz.zhonguo1118.cn

Common Programming Examples Cheat Book
来源：https://ss.zhonguo7118.cn

================================================================================
来源：https://wm.zhonguo4118.cn

【收录内容】
来源：https://wu.zhonguo8118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://fv.zhonguo5118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://ge.zhonguo4118.cn

SQL · Bash · C · C++
来源：https://th.zhonguo2118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://uj.zhonguo6118.cn

【使用说明】
来源：https://fi.zhonguo1118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://gi.zhonguo6118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://ju.zhonguo1118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://dg.zhonguo5118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://dc.zhonguo4118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://fu.zhonguo2118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://pw.zhonguo7118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://hc.zhonguo8118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://sd.zhonguo1118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://md.zhonguo5118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://wq.zhonguo2118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://si.zhonguo2118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://gc.zhonguo7118.cn

【文件统计】
来源：https://ce.zhonguo6118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://aw.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://kq.zhonguo4118.cn

目  录
来源：https://ch.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://cb.zhonguo5118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://zm.zhonguo7118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://qy.zhonguo4118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://fd.zhonguo1118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://wf.zhonguo4118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://ul.zhonguo4118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://wp.zhonguo8118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://wc.zhonguo2118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://jy.zhonguo7118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://xi.zhonguo5118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://ye.zhonguo1118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://zb.zhonguo2118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://tk.zhonguo7118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://tk.zhonguo2118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://ka.zhonguo6118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://tg.zhonguo5118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://my.zhonguo5118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://nz.zhonguo3118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://yr.zhonguo5118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ra.zhonguo6118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://pb.zhonguo2118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://ml.zhonguo3118.cn

================================================================================
来源：https://rw.zhonguo8118.cn

A. 基础语法与类型
来源：https://rx.zhonguo5118.cn

================================================================================
来源：https://mj.zhonguo1118.cn

[A01] Hello World
来源：https://nj.zhonguo1118.cn

Py:   print("Hello, World!")
来源：https://qh.zhonguo4118.cn

PHP:  echo "Hello, World!";
来源：https://vq.zhonguo5118.cn

JS:   console.log("Hello, World!");
来源：https://du.zhonguo8118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://yl.zhonguo1118.cn

Java: System.out.println("Hello, World!");
来源：https://zd.zhonguo1118.cn

Go:   fmt.Println("Hello, World!")
来源：https://ua.zhonguo8118.cn

Ruby: puts "Hello, World!"
来源：https://gw.zhonguo3118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://th.zhonguo7118.cn

[A02] 变量声明与赋值
来源：https://vv.zhonguo3118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://me.zhonguo4118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://eg.zhonguo8118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://qj.zhonguo2118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://nk.zhonguo2118.cn

Java: String name = "Alex"; int age = 20;
来源：https://px.zhonguo5118.cn

Go:   name := "Alex"; age := 20
来源：https://zz.zhonguo7118.cn

Ruby: name = "Alex"; age = 20
来源：https://jn.zhonguo6118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://ef.zhonguo6118.cn

[A03] 常量定义
来源：https://rb.zhonguo4118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://pe.zhonguo5118.cn

PHP:  const PI = 3.14159;
来源：https://dt.zhonguo8118.cn

JS:   const PI = 3.14159;
来源：https://oh.zhonguo1118.cn

TS:   const PI: number = 3.14159;
来源：https://sp.zhonguo5118.cn

Java: static final double PI = 3.14159;
来源：https://zu.zhonguo6118.cn

Go:   const PI = 3.14159
来源：https://xr.zhonguo7118.cn

Ruby: PI = 3.14159
来源：https://vh.zhonguo3118.cn

C#:   const double PI = 3.14159;
来源：https://mt.zhonguo4118.cn

[A04] 判断变量类型
来源：https://ad.zhonguo6118.cn

Py:   type(x).__name__; isinstance(x, int)
来源：https://ay.zhonguo2118.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：https://gu.zhonguo3118.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：https://fb.zhonguo3118.cn

TS:   typeof x; x instanceof Date
来源：https://ri.zhonguo5118.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：https://eb.zhonguo5118.cn

Go:   reflect.TypeOf(x).Name()
来源：https://uj.zhonguo4118.cn

Ruby: x.class; x.is_a?(Integer)
来源：https://je.zhonguo4118.cn

C#:   x.GetType().Name; x is int
来源：https://sd.zhonguo1118.cn

[A05] 整数除法与取模
来源：https://cv.zhonguo6118.cn


<!-- 参考信息 -->