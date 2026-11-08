代发 wailian999

[U35] Py：发送邮件
来源：https://ea.zhonguo4118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://hx.zhonguo6118.cn

[U36] Py：定时任务
来源：https://wf.zhonguo8118.cn

schedule.every(10).minutes.do(job)
来源：https://nl.zhonguo3118.cn

[U37] Py：读写 Excel
来源：https://lz.zhonguo1118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://tn.zhonguo1118.cn

[U38] Py：获取脚本所在目录
来源：https://ui.zhonguo3118.cn

Path(__file__).resolve().parent
来源：https://at.zhonguo8118.cn

[U39] Py：判断是否在交互环境
来源：https://vf.zhonguo1118.cn

sys.stdout.isatty()
来源：https://sa.zhonguo1118.cn

[U40] Py：打印到标准错误
来源：https://rn.zhonguo1118.cn

print("err", file=sys.stderr)
来源：https://ym.zhonguo1118.cn

[U41] PHP：初始化 Composer 项目
来源：https://gv.zhonguo7118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://id.zhonguo5118.cn

[U42] PHP：PSR-4 自动加载
来源：https://mb.zhonguo1118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://yo.zhonguo1118.cn

[U43] PHP：声明命名空间
来源：https://xr.zhonguo1118.cn

namespace App\Http;
来源：https://ja.zhonguo5118.cn

[U44] PHP：开启严格类型
来源：https://zy.zhonguo8118.cn

declare(strict_types=1);
来源：https://pq.zhonguo7118.cn

[U45] PHP：类型声明与返回类型
来源：https://sv.zhonguo5118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ls.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://ug.zhonguo2118.cn

?string $name = null
来源：https://ny.zhonguo4118.cn

[U47] PHP：联合类型
来源：https://ct.zhonguo2118.cn

int|string $id
来源：https://dh.zhonguo8118.cn

[U48] PHP：纯枚举
来源：https://ud.zhonguo4118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://al.zhonguo6118.cn

[U49] PHP：只读属性
来源：https://rq.zhonguo2118.cn

public readonly string $name
来源：https://np.zhonguo5118.cn

[U50] PHP：构造器属性提升
来源：https://sv.zhonguo4118.cn

public function __construct(private int $id) {}
来源：https://sn.zhonguo7118.cn

[U51] PHP：数组解构
来源：https://ht.zhonguo6118.cn

[$a, $b] = $arr;
来源：https://pi.zhonguo4118.cn

[U52] PHP：箭头函数
来源：https://ww.zhonguo4118.cn

$double = fn($x) => $x * 2;
来源：https://ey.zhonguo3118.cn

[U53] PHP：空合并运算符
来源：https://qc.zhonguo8118.cn

$v = $a ?? $b ?? "default";
来源：https://jj.zhonguo3118.cn

[U54] PHP：空安全调用
来源：https://wg.zhonguo6118.cn

$obj?->method()
来源：https://gc.zhonguo5118.cn

[U55] PHP：match 表达式
来源：https://od.zhonguo1118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://xa.zhonguo7118.cn

[U56] PHP：命名参数
来源：https://ot.zhonguo3118.cn

f(a: 1, b: 2)
来源：https://na.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://db.zhonguo7118.cn

"值: {$a}"
来源：https://zb.zhonguo6118.cn

[U58] PHP：数组三件套
来源：https://ju.zhonguo6118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://yb.zhonguo2118.cn

[U59] PHP：自定义排序
来源：https://nw.zhonguo5118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ur.zhonguo3118.cn

[U60] PHP：JSON 编解码
来源：https://ev.zhonguo8118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://td.zhonguo1118.cn

[U61] PHP：正则
来源：https://mi.zhonguo2118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://pw.zhonguo5118.cn

[U62] PHP：日期对象
来源：https://vc.zhonguo2118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://gq.zhonguo2118.cn

[U63] PHP：文件读写
来源：https://gy.zhonguo2118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://pj.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://pg.zhonguo1118.cn

glob("dir/*.php");  scandir("dir");
来源：https://nj.zhonguo7118.cn

[U65] PHP：会话
来源：https://vv.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://io.zhonguo5118.cn

[U66] PHP：设置 Cookie
来源：https://rs.zhonguo3118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://wn.zhonguo5118.cn

[U67] PHP：处理文件上传
来源：https://ib.zhonguo5118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://mk.zhonguo7118.cn

[U68] PHP：PDO 连接
来源：https://gd.zhonguo5118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://av.zhonguo4118.cn

[U69] PHP：PDO 预处理
来源：https://bl.zhonguo8118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://gz.zhonguo3118.cn

[U70] PHP：PDO 事务
来源：https://fe.zhonguo8118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://mg.zhonguo2118.cn

[U71] PHP：抛出异常
来源：https://zy.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://wl.zhonguo7118.cn

[U72] PHP：写错误日志
来源：https://jr.zhonguo3118.cn

error_log("失败: " . $e->getMessage());
来源：https://rv.zhonguo6118.cn

[U73] PHP：读取 ini 配置
来源：https://fl.zhonguo8118.cn

parse_ini_file("config.ini", true)
来源：https://fj.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://wz.zhonguo7118.cn

getenv("APP_ENV") ?: "production"
来源：https://rs.zhonguo4118.cn

[U75] PHP：依赖注入
来源：https://xo.zhonguo6118.cn

composer require psr/container
来源：https://sy.zhonguo2118.cn

[U76] PHP：简单路由
来源：https://jp.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ph.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://xs.zhonguo3118.cn

composer require twig/twig
来源：https://ou.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://lb.zhonguo6118.cn

composer require --dev phpunit/phpunit
来源：https://rr.zhonguo2118.cn

[U79] PHP：静态分析
来源：https://fb.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://um.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://hb.zhonguo2118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://sb.zhonguo3118.cn

[U81] JS：初始化项目
来源：https://nc.zhonguo5118.cn

npm init -y;  npm i express
来源：https://mn.zhonguo6118.cn

[U82] JS：package.json 脚本
来源：https://if.zhonguo6118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://bd.zhonguo7118.cn

[U83] JS：ES Module 导入导出
来源：https://js.zhonguo4118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://zc.zhonguo4118.cn

[U84] JS：CommonJS 写法
来源：https://ui.zhonguo1118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://dy.zhonguo8118.cn

[U85] JS：可选链
来源：https://qr.zhonguo1118.cn

a?.b?.c
来源：https://le.zhonguo2118.cn

[U86] JS：空值合并
来源：https://sp.zhonguo3118.cn

a ?? b
来源：https://dk.zhonguo7118.cn

[U87] JS：解构默认值
来源：https://cp.zhonguo2118.cn

const { a = 1, b = 2 } = obj;
来源：https://zw.zhonguo2118.cn

[U88] JS：对象展开合并
来源：https://ga.zhonguo8118.cn

{ ...a, ...b }
来源：https://it.zhonguo6118.cn

[U89] JS：数组去重
来源：https://ta.zhonguo3118.cn

[...new Set(arr)]
来源：https://og.zhonguo6118.cn

[U90] JS：数字数组排序
来源：https://cj.zhonguo2118.cn

[...arr].sort((a, b) => a - b)
来源：https://aq.zhonguo2118.cn

[U91] JS：对象键值遍历
来源：https://hv.zhonguo2118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://sj.zhonguo7118.cn

[U92] JS：深拷贝
来源：https://ch.zhonguo7118.cn

structuredClone(obj)
来源：https://xc.zhonguo1118.cn

[U93] JS：模板字符串
来源：https://qd.zhonguo3118.cn

`共 ${n} 条`
来源：https://hu.zhonguo5118.cn

[U94] JS：箭头函数
来源：https://hv.zhonguo4118.cn

const double = x => x * 2;
来源：https://mu.zhonguo1118.cn

[U95] JS：Promise 包装
来源：https://sc.zhonguo1118.cn

new Promise((resolve, reject) => {})
来源：https://nw.zhonguo4118.cn

[U96] JS：async/await 与异常
来源：https://xp.zhonguo3118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://ag.zhonguo3118.cn

[U97] JS：并发请求
来源：https://lz.zhonguo2118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://gf.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://kz.zhonguo5118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://bx.zhonguo6118.cn

[U99] JS：事件监听
来源：https://yf.zhonguo2118.cn

el.addEventListener("click", e => {})
来源：https://pu.zhonguo1118.cn

[U100] JS：DOM 查询
来源：https://uu.zhonguo4118.cn

document.querySelector(".item")
来源：https://bk.zhonguo1118.cn

[U101] JS：classList 操作
来源：https://yn.zhonguo3118.cn

el.classList.toggle("active")
来源：https://hr.zhonguo8118.cn

[U102] JS：本地存储
来源：https://go.zhonguo8118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://ir.zhonguo8118.cn

[U103] JS：定时器
来源：https://ay.zhonguo1118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://dk.zhonguo6118.cn

[U104] JS：防抖
来源：https://fv.zhonguo7118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://na.zhonguo1118.cn

[U105] JS：节流
来源：https://ad.zhonguo7118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://oy.zhonguo7118.cn

[U106] JS：日期格式化
来源：https://gl.zhonguo2118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://zu.zhonguo4118.cn

[U107] JS：数字千分位
来源：https://bj.zhonguo6118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://ma.zhonguo1118.cn

[U108] JS：随机整数
来源：https://ww.zhonguo4118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://yl.zhonguo1118.cn

[U109] JS：数组分组
来源：https://sx.zhonguo1118.cn

Object.groupBy(arr, x => x.type)
来源：https://lc.zhonguo1118.cn

[U110] JS：数组分块
来源：https://vc.zhonguo1118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ny.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://mv.zhonguo1118.cn

new Map(Object.entries(obj))
来源：https://ma.zhonguo3118.cn

[U112] JS：字符串补位
来源：https://vw.zhonguo3118.cn

"7".padStart(3, "0")
来源：https://vj.zhonguo5118.cn

[U113] JS：正则替换全部
来源：https://gn.zhonguo2118.cn

s.replaceAll("a", "b")
来源：https://yv.zhonguo7118.cn

[U114] JS：JSON 深比较
来源：https://fk.zhonguo6118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://se.zhonguo1118.cn

[U115] JS：生成 UUID
来源：https://jz.zhonguo4118.cn

crypto.randomUUID()
来源：https://rf.zhonguo7118.cn

[U116] JS：类型检查（JSDoc）
来源：https://wx.zhonguo4118.cn

/** @param {string} name */ function f(name) {}
来源：https://bi.zhonguo8118.cn

[U117] JS：单元测试
来源：https://ti.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://wm.zhonguo2118.cn

[U118] JS：开发服务器
来源：https://gi.zhonguo6118.cn

npm i -D vite;  npx vite
来源：https://qv.zhonguo8118.cn

[U119] JS：生产构建
来源：https://nz.zhonguo4118.cn

npx vite build
来源：https://nf.zhonguo5118.cn

[U120] JS：读取环境变量（Vite）
来源：https://dt.zhonguo6118.cn

import.meta.env.VITE_API_URL
来源：https://mj.zhonguo1118.cn

================================================================================
来源：https://er.zhonguo4118.cn

统计汇总
来源：https://ni.zhonguo7118.cn

================================================================================
来源：https://eh.zhonguo3118.cn

按语言统计（条）：
来源：https://ed.zhonguo4118.cn

Python ......... 252
来源：https://eg.zhonguo3118.cn

PHP ............ 252
来源：https://fj.zhonguo1118.cn

JavaScript ..... 252
来源：https://lf.zhonguo2118.cn

TypeScript ..... 212
来源：https://fj.zhonguo2118.cn

Java ........... 212
来源：https://om.zhonguo8118.cn

Go ............. 212
来源：https://js.zhonguo5118.cn

Ruby ........... 212
来源：https://pv.zhonguo1118.cn

C# ............. 212
来源：https://ru.zhonguo8118.cn

C .............. 30
来源：https://xg.zhonguo3118.cn

C++ ............ 30
来源：https://ih.zhonguo5118.cn

SQL ............ 90
来源：https://rm.zhonguo3118.cn

Bash ........... 80
来源：https://ji.zhonguo3118.cn

Kotlin ......... 15
来源：https://vp.zhonguo4118.cn

Swift .......... 15
来源：https://ns.zhonguo5118.cn

Lua ............ 10
来源：https://ec.zhonguo3118.cn

Perl ........... 10
来源：https://oe.zhonguo4118.cn

Scala .......... 10
来源：https://el.zhonguo1118.cn

------------------------------------
来源：https://mr.zhonguo5118.cn

合计 ........... 2106 条
来源：https://ao.zhonguo7118.cn

按章节统计：
来源：https://hj.zhonguo7118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://cp.zhonguo8118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://sr.zhonguo2118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://jg.zhonguo3118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://zu.zhonguo4118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://sj.zhonguo5118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://jc.zhonguo5118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://uq.zhonguo2118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://tf.zhonguo4118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://wx.zhonguo8118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://aq.zhonguo2118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://au.zhonguo5118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://de.zhonguo3118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://lq.zhonguo3118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://tp.zhonguo4118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://de.zhonguo4118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://im.zhonguo6118.cn

Q SQL 专题                              90
来源：https://bb.zhonguo6118.cn

R Bash 专题                             80
来源：https://lw.zhonguo7118.cn

S C / C++ 专题                          60
来源：https://rk.zhonguo3118.cn

T 其他语言补充                          60
来源：https://xn.zhonguo3118.cn

U 高频实用片段                         120
来源：https://tm.zhonguo1118.cn

------------------------------------
来源：https://hl.zhonguo1118.cn

合计                                  2106 条
来源：https://po.zhonguo1118.cn

--------------------------------------------------------------------------------
来源：https://fu.zhonguo4118.cn

使用提醒
来源：https://zq.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://gh.zhonguo6118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://ir.zhonguo5118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://cr.zhonguo4118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://op.zhonguo2118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://gq.zhonguo1118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://px.zhonguo1118.cn

—— 文件结束 ——
来源：https://pd.zhonguo5118.cn

================================================================================
来源：https://lh.zhonguo5118.cn

程序语言常见例子速查手册（2024 版）
来源：https://mu.zhonguo7118.cn

Common Programming Examples Cheat Book
来源：https://ne.zhonguo1118.cn

================================================================================
来源：https://ps.zhonguo8118.cn

【收录内容】
来源：https://xp.zhonguo8118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://oy.zhonguo8118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://by.zhonguo5118.cn

SQL · Bash · C · C++
来源：https://ry.zhonguo1118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://nm.zhonguo1118.cn

【使用说明】
来源：https://kp.zhonguo5118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://ib.zhonguo4118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://tk.zhonguo8118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://zl.zhonguo2118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://ao.zhonguo6118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://ft.zhonguo5118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://tl.zhonguo3118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://wu.zhonguo2118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://sj.zhonguo4118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://em.zhonguo5118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://xp.zhonguo6118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://kf.zhonguo7118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://mx.zhonguo2118.cn

【文件统计】
来源：https://cm.zhonguo7118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://rc.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://ib.zhonguo7118.cn

目  录
来源：https://vk.zhonguo2118.cn

--------------------------------------------------------------------------------
来源：https://yd.zhonguo1118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://ke.zhonguo8118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://mp.zhonguo3118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://oe.zhonguo8118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://dq.zhonguo7118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://rz.zhonguo3118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://yu.zhonguo7118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://lq.zhonguo1118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://jv.zhonguo4118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://xv.zhonguo7118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://vf.zhonguo4118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://yu.zhonguo4118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://og.zhonguo7118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://be.zhonguo1118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://cc.zhonguo4118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://ai.zhonguo5118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://gf.zhonguo6118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://wx.zhonguo4118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://ps.zhonguo7118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://bs.zhonguo5118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://vy.zhonguo4118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://ep.zhonguo6118.cn

================================================================================
来源：https://ja.zhonguo8118.cn

A. 基础语法与类型
来源：https://xg.zhonguo7118.cn

================================================================================
来源：https://sd.zhonguo1118.cn

[A01] Hello World
来源：https://zi.zhonguo1118.cn

Py:   print("Hello, World!")
来源：https://dw.zhonguo8118.cn

PHP:  echo "Hello, World!";
来源：https://cs.zhonguo6118.cn

JS:   console.log("Hello, World!");
来源：https://dm.zhonguo4118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://mu.zhonguo2118.cn

Java: System.out.println("Hello, World!");
来源：https://ap.zhonguo8118.cn

Go:   fmt.Println("Hello, World!")
来源：https://wd.zhonguo7118.cn

Ruby: puts "Hello, World!"
来源：https://vv.zhonguo4118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://my.zhonguo6118.cn

[A02] 变量声明与赋值
来源：https://ks.zhonguo2118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://hp.zhonguo2118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://cd.zhonguo3118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://zw.zhonguo1118.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：https://pp.zhonguo8118.cn

Java: String name = "Alex"; int age = 20;
来源：https://vg.zhonguo8118.cn

Go:   name := "Alex"; age := 20
来源：https://ss.zhonguo1118.cn

Ruby: name = "Alex"; age = 20
来源：https://hw.zhonguo8118.cn

C#:   string name = "Alex"; int age = 20;
来源：https://tj.zhonguo1118.cn

[A03] 常量定义
来源：https://kf.zhonguo7118.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：https://ni.zhonguo2118.cn

PHP:  const PI = 3.14159;
来源：https://fa.zhonguo1118.cn


<!-- 参考信息 -->