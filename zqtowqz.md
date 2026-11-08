代发 wailian999

[U37] Py：读写 Excel
来源：https://lk.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://cf.zhonguo6118.cn

[U38] Py：获取脚本所在目录
来源：https://yb.zhonguo2118.cn

Path(__file__).resolve().parent
来源：https://tr.zhonguo8118.cn

[U39] Py：判断是否在交互环境
来源：https://db.zhonguo5118.cn

sys.stdout.isatty()
来源：https://tt.zhonguo6118.cn

[U40] Py：打印到标准错误
来源：https://rf.zhonguo6118.cn

print("err", file=sys.stderr)
来源：https://lv.zhonguo2118.cn

[U41] PHP：初始化 Composer 项目
来源：https://qq.zhonguo3118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://eb.zhonguo4118.cn

[U42] PHP：PSR-4 自动加载
来源：https://kj.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://kg.zhonguo7118.cn

[U43] PHP：声明命名空间
来源：https://vb.zhonguo3118.cn

namespace App\Http;
来源：https://yt.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://ow.zhonguo3118.cn

declare(strict_types=1);
来源：https://an.zhonguo8118.cn

[U45] PHP：类型声明与返回类型
来源：https://kv.zhonguo2118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://zp.zhonguo8118.cn

[U46] PHP：可空类型
来源：https://jj.zhonguo3118.cn

?string $name = null
来源：https://cl.zhonguo7118.cn

[U47] PHP：联合类型
来源：https://eq.zhonguo7118.cn

int|string $id
来源：https://ps.zhonguo8118.cn

[U48] PHP：纯枚举
来源：https://hj.zhonguo4118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://lo.zhonguo2118.cn

[U49] PHP：只读属性
来源：https://vb.zhonguo8118.cn

public readonly string $name
来源：https://ge.zhonguo5118.cn

[U50] PHP：构造器属性提升
来源：https://jz.zhonguo7118.cn

public function __construct(private int $id) {}
来源：https://yq.zhonguo5118.cn

[U51] PHP：数组解构
来源：https://ur.zhonguo4118.cn

[$a, $b] = $arr;
来源：https://ge.zhonguo6118.cn

[U52] PHP：箭头函数
来源：https://un.zhonguo3118.cn

$double = fn($x) => $x * 2;
来源：https://zr.zhonguo4118.cn

[U53] PHP：空合并运算符
来源：https://dr.zhonguo7118.cn

$v = $a ?? $b ?? "default";
来源：https://ra.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://xk.zhonguo8118.cn

$obj?->method()
来源：https://fg.zhonguo2118.cn

[U55] PHP：match 表达式
来源：https://tx.zhonguo5118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://ab.zhonguo3118.cn

[U56] PHP：命名参数
来源：https://zn.zhonguo8118.cn

f(a: 1, b: 2)
来源：https://zi.zhonguo4118.cn

[U57] PHP：字符串插值
来源：https://cm.zhonguo8118.cn

"值: {$a}"
来源：https://os.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://jz.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://ub.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://ew.zhonguo6118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://lv.zhonguo7118.cn

[U60] PHP：JSON 编解码
来源：https://si.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://su.zhonguo4118.cn

[U61] PHP：正则
来源：https://eu.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://yl.zhonguo7118.cn

[U62] PHP：日期对象
来源：https://jw.zhonguo6118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://zl.zhonguo2118.cn

[U63] PHP：文件读写
来源：https://xq.zhonguo1118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://nq.zhonguo5118.cn

[U64] PHP：目录遍历
来源：https://di.zhonguo4118.cn

glob("dir/*.php");  scandir("dir");
来源：https://cn.zhonguo7118.cn

[U65] PHP：会话
来源：https://lo.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://zt.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://oj.zhonguo2118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://oe.zhonguo4118.cn

[U67] PHP：处理文件上传
来源：https://yn.zhonguo3118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://sc.zhonguo6118.cn

[U68] PHP：PDO 连接
来源：https://zb.zhonguo7118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://lz.zhonguo7118.cn

[U69] PHP：PDO 预处理
来源：https://fc.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://fr.zhonguo4118.cn

[U70] PHP：PDO 事务
来源：https://sb.zhonguo5118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://az.zhonguo6118.cn

[U71] PHP：抛出异常
来源：https://yb.zhonguo3118.cn

throw new RuntimeException("失败", 500);
来源：https://ef.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://kf.zhonguo8118.cn

error_log("失败: " . $e->getMessage());
来源：https://vn.zhonguo1118.cn

[U73] PHP：读取 ini 配置
来源：https://wt.zhonguo5118.cn

parse_ini_file("config.ini", true)
来源：https://xa.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://za.zhonguo8118.cn

getenv("APP_ENV") ?: "production"
来源：https://iq.zhonguo3118.cn

[U75] PHP：依赖注入
来源：https://xf.zhonguo5118.cn

composer require psr/container
来源：https://qu.zhonguo3118.cn

[U76] PHP：简单路由
来源：https://yl.zhonguo3118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://wr.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://qq.zhonguo4118.cn

composer require twig/twig
来源：https://bh.zhonguo6118.cn

[U78] PHP：单元测试
来源：https://sq.zhonguo1118.cn

composer require --dev phpunit/phpunit
来源：https://zq.zhonguo1118.cn

[U79] PHP：静态分析
来源：https://gb.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://xl.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://od.zhonguo5118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://oc.zhonguo6118.cn

[U81] JS：初始化项目
来源：https://pk.zhonguo6118.cn

npm init -y;  npm i express
来源：https://er.zhonguo7118.cn

[U82] JS：package.json 脚本
来源：https://bu.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://pf.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://dg.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://jl.zhonguo6118.cn

[U84] JS：CommonJS 写法
来源：https://ta.zhonguo2118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ur.zhonguo3118.cn

[U85] JS：可选链
来源：https://es.zhonguo1118.cn

a?.b?.c
来源：https://ut.zhonguo3118.cn

[U86] JS：空值合并
来源：https://gi.zhonguo4118.cn

a ?? b
来源：https://ws.zhonguo1118.cn

[U87] JS：解构默认值
来源：https://yp.zhonguo2118.cn

const { a = 1, b = 2 } = obj;
来源：https://sq.zhonguo4118.cn

[U88] JS：对象展开合并
来源：https://nn.zhonguo2118.cn

{ ...a, ...b }
来源：https://ai.zhonguo6118.cn

[U89] JS：数组去重
来源：https://zv.zhonguo1118.cn

[...new Set(arr)]
来源：https://jc.zhonguo8118.cn

[U90] JS：数字数组排序
来源：https://ty.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://co.zhonguo4118.cn

[U91] JS：对象键值遍历
来源：https://xd.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://rc.zhonguo1118.cn

[U92] JS：深拷贝
来源：https://pb.zhonguo1118.cn

structuredClone(obj)
来源：https://ai.zhonguo5118.cn

[U93] JS：模板字符串
来源：https://zn.zhonguo1118.cn

`共 ${n} 条`
来源：https://zn.zhonguo4118.cn

[U94] JS：箭头函数
来源：https://ek.zhonguo8118.cn

const double = x => x * 2;
来源：https://ba.zhonguo7118.cn

[U95] JS：Promise 包装
来源：https://vk.zhonguo1118.cn

new Promise((resolve, reject) => {})
来源：https://gk.zhonguo4118.cn

[U96] JS：async/await 与异常
来源：https://ta.zhonguo2118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://zq.zhonguo7118.cn

[U97] JS：并发请求
来源：https://dp.zhonguo6118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://aj.zhonguo1118.cn

[U98] JS：fetch 带 JSON
来源：https://yn.zhonguo1118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ga.zhonguo8118.cn

[U99] JS：事件监听
来源：https://fl.zhonguo5118.cn

el.addEventListener("click", e => {})
来源：https://wq.zhonguo2118.cn

[U100] JS：DOM 查询
来源：https://gy.zhonguo8118.cn

document.querySelector(".item")
来源：https://uk.zhonguo3118.cn

[U101] JS：classList 操作
来源：https://hg.zhonguo3118.cn

el.classList.toggle("active")
来源：https://cr.zhonguo2118.cn

[U102] JS：本地存储
来源：https://yv.zhonguo2118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://pn.zhonguo6118.cn

[U103] JS：定时器
来源：https://kx.zhonguo8118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://gr.zhonguo4118.cn

[U104] JS：防抖
来源：https://zx.zhonguo3118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://qe.zhonguo4118.cn

[U105] JS：节流
来源：https://wg.zhonguo2118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://af.zhonguo7118.cn

[U106] JS：日期格式化
来源：https://vl.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://jq.zhonguo1118.cn

[U107] JS：数字千分位
来源：https://eh.zhonguo3118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://vq.zhonguo2118.cn

[U108] JS：随机整数
来源：https://ms.zhonguo2118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://mh.zhonguo2118.cn

[U109] JS：数组分组
来源：https://uq.zhonguo7118.cn

Object.groupBy(arr, x => x.type)
来源：https://cr.zhonguo7118.cn

[U110] JS：数组分块
来源：https://oi.zhonguo5118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://tn.zhonguo4118.cn

[U111] JS：对象转 Map
来源：https://al.zhonguo4118.cn

new Map(Object.entries(obj))
来源：https://vo.zhonguo2118.cn

[U112] JS：字符串补位
来源：https://qp.zhonguo1118.cn

"7".padStart(3, "0")
来源：https://ty.zhonguo8118.cn

[U113] JS：正则替换全部
来源：https://ov.zhonguo5118.cn

s.replaceAll("a", "b")
来源：https://jw.zhonguo5118.cn

[U114] JS：JSON 深比较
来源：https://pu.zhonguo2118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://iy.zhonguo3118.cn

[U115] JS：生成 UUID
来源：https://su.zhonguo3118.cn

crypto.randomUUID()
来源：https://nm.zhonguo5118.cn

[U116] JS：类型检查（JSDoc）
来源：https://nz.zhonguo1118.cn

/** @param {string} name */ function f(name) {}
来源：https://jx.zhonguo2118.cn

[U117] JS：单元测试
来源：https://gw.zhonguo4118.cn

npm i -D vitest;  npx vitest
来源：https://jb.zhonguo1118.cn

[U118] JS：开发服务器
来源：https://mx.zhonguo1118.cn

npm i -D vite;  npx vite
来源：https://ib.zhonguo3118.cn

[U119] JS：生产构建
来源：https://zq.zhonguo2118.cn

npx vite build
来源：https://ft.zhonguo5118.cn

[U120] JS：读取环境变量（Vite）
来源：https://cl.zhonguo4118.cn

import.meta.env.VITE_API_URL
来源：https://cl.zhonguo3118.cn

================================================================================
来源：https://eu.zhonguo3118.cn

统计汇总
来源：https://kg.zhonguo6118.cn

================================================================================
来源：https://vl.zhonguo1118.cn

按语言统计（条）：
来源：https://ad.zhonguo1118.cn

Python ......... 252
来源：https://fx.zhonguo1118.cn

PHP ............ 252
来源：https://cv.zhonguo7118.cn

JavaScript ..... 252
来源：https://zi.zhonguo2118.cn

TypeScript ..... 212
来源：https://dg.zhonguo6118.cn

Java ........... 212
来源：https://vh.zhonguo5118.cn

Go ............. 212
来源：https://po.zhonguo4118.cn

Ruby ........... 212
来源：https://ao.zhonguo7118.cn

C# ............. 212
来源：https://nv.zhonguo2118.cn

C .............. 30
来源：https://zg.zhonguo6118.cn

C++ ............ 30
来源：https://qb.zhonguo6118.cn

SQL ............ 90
来源：https://jv.zhonguo1118.cn

Bash ........... 80
来源：https://bx.zhonguo8118.cn

Kotlin ......... 15
来源：https://dw.zhonguo5118.cn

Swift .......... 15
来源：https://or.zhonguo8118.cn

Lua ............ 10
来源：https://yg.zhonguo3118.cn

Perl ........... 10
来源：https://bi.zhonguo1118.cn

Scala .......... 10
来源：https://kg.zhonguo5118.cn

------------------------------------
来源：https://dj.zhonguo2118.cn

合计 ........... 2106 条
来源：https://hc.zhonguo4118.cn

按章节统计：
来源：https://ki.zhonguo4118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://cq.zhonguo8118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://ex.zhonguo2118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://ra.zhonguo5118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://vq.zhonguo2118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://gv.zhonguo5118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://zk.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://pk.zhonguo2118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://sp.zhonguo5118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://yn.zhonguo2118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://pl.zhonguo6118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://bn.zhonguo7118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://oq.zhonguo1118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://ka.zhonguo7118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://cb.zhonguo6118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://um.zhonguo3118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://kz.zhonguo1118.cn

Q SQL 专题                              90
来源：https://gs.zhonguo1118.cn

R Bash 专题                             80
来源：https://tq.zhonguo8118.cn

S C / C++ 专题                          60
来源：https://rx.zhonguo3118.cn

T 其他语言补充                          60
来源：https://jc.zhonguo2118.cn

U 高频实用片段                         120
来源：https://to.zhonguo2118.cn

------------------------------------
来源：https://ib.zhonguo8118.cn

合计                                  2106 条
来源：https://pu.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://tp.zhonguo2118.cn

使用提醒
来源：https://oq.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://jp.zhonguo3118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://an.zhonguo4118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://nf.zhonguo6118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://ih.zhonguo2118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://ys.zhonguo5118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://ud.zhonguo4118.cn

—— 文件结束 ——
来源：https://pj.zhonguo7118.cn

================================================================================
来源：https://ey.zhonguo1118.cn

程序语言常见例子速查手册（2024 版）
来源：https://wr.zhonguo6118.cn

Common Programming Examples Cheat Book
来源：https://ny.zhonguo8118.cn

================================================================================
来源：https://mr.zhonguo8118.cn

【收录内容】
来源：https://qh.zhonguo7118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://ox.zhonguo2118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://gy.zhonguo2118.cn

SQL · Bash · C · C++
来源：https://bu.zhonguo5118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://zl.zhonguo7118.cn

【使用说明】
来源：https://pq.zhonguo1118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://lg.zhonguo3118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://vd.zhonguo7118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://ot.zhonguo7118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://vp.zhonguo5118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://bp.zhonguo1118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://yn.zhonguo3118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://wv.zhonguo7118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://dt.zhonguo4118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://ly.zhonguo8118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://oa.zhonguo1118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://cn.zhonguo2118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://uj.zhonguo5118.cn

【文件统计】
来源：https://ra.zhonguo8118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://aw.zhonguo2118.cn

--------------------------------------------------------------------------------
来源：https://cg.zhonguo1118.cn

目  录
来源：https://ry.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://so.zhonguo6118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://rk.zhonguo3118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://aj.zhonguo2118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://hv.zhonguo3118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://bp.zhonguo7118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://cm.zhonguo4118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://xc.zhonguo6118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://pz.zhonguo8118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://tk.zhonguo5118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://wc.zhonguo1118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://xu.zhonguo3118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://wn.zhonguo3118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://zo.zhonguo5118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://wg.zhonguo8118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://pw.zhonguo7118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://uu.zhonguo8118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://re.zhonguo2118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://vg.zhonguo8118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://bn.zhonguo1118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://oc.zhonguo8118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://dd.zhonguo4118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://qy.zhonguo8118.cn

================================================================================
来源：https://zc.zhonguo4118.cn

A. 基础语法与类型
来源：https://je.zhonguo1118.cn

================================================================================
来源：https://dk.zhonguo1118.cn

[A01] Hello World
来源：https://is.zhonguo4118.cn

Py:   print("Hello, World!")
来源：https://ei.zhonguo4118.cn

PHP:  echo "Hello, World!";
来源：https://sx.zhonguo2118.cn

JS:   console.log("Hello, World!");
来源：https://jk.zhonguo6118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://or.zhonguo5118.cn

Java: System.out.println("Hello, World!");
来源：https://zx.zhonguo7118.cn

Go:   fmt.Println("Hello, World!")
来源：https://bi.zhonguo8118.cn

Ruby: puts "Hello, World!"
来源：https://yk.zhonguo3118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://ta.zhonguo7118.cn

[A02] 变量声明与赋值
来源：https://oh.zhonguo5118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://zw.zhonguo8118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://bl.zhonguo1118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://wq.zhonguo1118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://iz.zhonguo7118.cn

Java: String name = "Alex"; int age = 20;
来源：https://dm.zhonguo8118.cn

Go:   name := "Alex"; age := 20
来源：https://qy.zhonguo8118.cn

Ruby: name = "Alex"; age = 20
来源：https://ic.zhonguo1118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://oh.zhonguo8118.cn

[A03] 常量定义
来源：https://fo.zhonguo7118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://lv.zhonguo8118.cn

PHP:  const PI = 3.14159;
来源：https://hw.zhonguo3118.cn

JS:   const PI = 3.14159;
来源：https://to.zhonguo7118.cn

TS:   const PI: number = 3.14159;
来源：https://lq.zhonguo2118.cn

Java: static final double PI = 3.14159;
来源：https://yx.zhonguo8118.cn

Go:   const PI = 3.14159
来源：https://fo.zhonguo3118.cn


<!-- 参考信息 -->