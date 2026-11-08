代发 wailian999

[U31] Py：单测
来源：https://rk.zhonguo1118.cn

python -m pytest -q
来源：https://rn.zhonguo1118.cn

[U32] Py：代码格式化
来源：https://cp.zhonguo5118.cn

ruff format . && ruff check --fix .
来源：https://rr.zhonguo4118.cn

[U33] Py：打包发布
来源：https://zr.zhonguo5118.cn

python -m build  （依赖 pyproject.toml）
来源：https://ak.zhonguo3118.cn

[U34] Py：判断编码
来源：https://ic.zhonguo7118.cn

chardet.detect(raw)
来源：https://sg.zhonguo5118.cn

[U35] Py：发送邮件
来源：https://ls.zhonguo4118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://rb.zhonguo8118.cn

[U36] Py：定时任务
来源：https://sm.zhonguo2118.cn

schedule.every(10).minutes.do(job)
来源：https://oo.zhonguo6118.cn

[U37] Py：读写 Excel
来源：https://hj.zhonguo4118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://at.zhonguo2118.cn

[U38] Py：获取脚本所在目录
来源：https://nr.zhonguo2118.cn

Path(__file__).resolve().parent
来源：https://kd.zhonguo6118.cn

[U39] Py：判断是否在交互环境
来源：https://lg.zhonguo1118.cn

sys.stdout.isatty()
来源：https://jf.zhonguo2118.cn

[U40] Py：打印到标准错误
来源：https://kc.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://yh.zhonguo5118.cn

[U41] PHP：初始化 Composer 项目
来源：https://cw.zhonguo8118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://of.zhonguo5118.cn

[U42] PHP：PSR-4 自动加载
来源：https://yo.zhonguo2118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://lo.zhonguo4118.cn

[U43] PHP：声明命名空间
来源：https://lp.zhonguo6118.cn

namespace App\Http;
来源：https://sh.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://lr.zhonguo8118.cn

declare(strict_types=1);
来源：https://hn.zhonguo6118.cn

[U45] PHP：类型声明与返回类型
来源：https://ef.zhonguo6118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://uh.zhonguo3118.cn

[U46] PHP：可空类型
来源：https://yr.zhonguo8118.cn

?string $name = null
来源：https://gp.zhonguo1118.cn

[U47] PHP：联合类型
来源：https://aa.zhonguo1118.cn

int|string $id
来源：https://uv.zhonguo7118.cn

[U48] PHP：纯枚举
来源：https://an.zhonguo5118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://la.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://nd.zhonguo7118.cn

public readonly string $name
来源：https://td.zhonguo7118.cn

[U50] PHP：构造器属性提升
来源：https://cq.zhonguo5118.cn

public function __construct(private int $id) {}
来源：https://ib.zhonguo2118.cn

[U51] PHP：数组解构
来源：https://lr.zhonguo5118.cn

[$a, $b] = $arr;
来源：https://fw.zhonguo1118.cn

[U52] PHP：箭头函数
来源：https://ep.zhonguo7118.cn

$double = fn($x) => $x * 2;
来源：https://bu.zhonguo6118.cn

[U53] PHP：空合并运算符
来源：https://cn.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://pe.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://ri.zhonguo8118.cn

$obj?->method()
来源：https://lj.zhonguo7118.cn

[U55] PHP：match 表达式
来源：https://wp.zhonguo8118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://mr.zhonguo1118.cn

[U56] PHP：命名参数
来源：https://um.zhonguo7118.cn

f(a: 1, b: 2)
来源：https://kw.zhonguo8118.cn

[U57] PHP：字符串插值
来源：https://ue.zhonguo2118.cn

"值: {$a}"
来源：https://rq.zhonguo5118.cn

[U58] PHP：数组三件套
来源：https://fl.zhonguo8118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://xu.zhonguo8118.cn

[U59] PHP：自定义排序
来源：https://oi.zhonguo4118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://wh.zhonguo4118.cn

[U60] PHP：JSON 编解码
来源：https://le.zhonguo4118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://un.zhonguo5118.cn

[U61] PHP：正则
来源：https://hk.zhonguo4118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://vh.zhonguo3118.cn

[U62] PHP：日期对象
来源：https://ip.zhonguo3118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://rm.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://si.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://uk.zhonguo8118.cn

[U64] PHP：目录遍历
来源：https://zg.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://rl.zhonguo5118.cn

[U65] PHP：会话
来源：https://bo.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://uc.zhonguo2118.cn

[U66] PHP：设置 Cookie
来源：https://wo.zhonguo3118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://nv.zhonguo4118.cn

[U67] PHP：处理文件上传
来源：https://jz.zhonguo1118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://av.zhonguo7118.cn

[U68] PHP：PDO 连接
来源：https://ol.zhonguo6118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ss.zhonguo3118.cn

[U69] PHP：PDO 预处理
来源：https://vn.zhonguo1118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://wl.zhonguo5118.cn

[U70] PHP：PDO 事务
来源：https://oz.zhonguo8118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://zl.zhonguo8118.cn

[U71] PHP：抛出异常
来源：https://sr.zhonguo3118.cn

throw new RuntimeException("失败", 500);
来源：https://kb.zhonguo2118.cn

[U72] PHP：写错误日志
来源：https://so.zhonguo6118.cn

error_log("失败: " . $e->getMessage());
来源：https://le.zhonguo5118.cn

[U73] PHP：读取 ini 配置
来源：https://dm.zhonguo7118.cn

parse_ini_file("config.ini", true)
来源：https://xd.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://kt.zhonguo5118.cn

getenv("APP_ENV") ?: "production"
来源：https://ye.zhonguo3118.cn

[U75] PHP：依赖注入
来源：https://le.zhonguo4118.cn

composer require psr/container
来源：https://ky.zhonguo1118.cn

[U76] PHP：简单路由
来源：https://gy.zhonguo1118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://fl.zhonguo8118.cn

[U77] PHP：模板渲染
来源：https://qw.zhonguo7118.cn

composer require twig/twig
来源：https://ew.zhonguo6118.cn

[U78] PHP：单元测试
来源：https://er.zhonguo3118.cn

composer require --dev phpunit/phpunit
来源：https://fr.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://gp.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://eq.zhonguo2118.cn

[U80] PHP：代码规范修复
来源：https://mj.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://xi.zhonguo6118.cn

[U81] JS：初始化项目
来源：https://yw.zhonguo2118.cn

npm init -y;  npm i express
来源：https://lu.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://oa.zhonguo2118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://nt.zhonguo5118.cn

[U83] JS：ES Module 导入导出
来源：https://jh.zhonguo6118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://tt.zhonguo6118.cn

[U84] JS：CommonJS 写法
来源：https://ul.zhonguo6118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://cr.zhonguo7118.cn

[U85] JS：可选链
来源：https://nj.zhonguo5118.cn

a?.b?.c
来源：https://cl.zhonguo6118.cn

[U86] JS：空值合并
来源：https://ky.zhonguo4118.cn

a ?? b
来源：https://tt.zhonguo3118.cn

[U87] JS：解构默认值
来源：https://cf.zhonguo8118.cn

const { a = 1, b = 2 } = obj;
来源：https://hh.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://ei.zhonguo7118.cn

{ ...a, ...b }
来源：https://xu.zhonguo7118.cn

[U89] JS：数组去重
来源：https://wj.zhonguo3118.cn

[...new Set(arr)]
来源：https://qf.zhonguo7118.cn

[U90] JS：数字数组排序
来源：https://yi.zhonguo2118.cn

[...arr].sort((a, b) => a - b)
来源：https://pf.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://wj.zhonguo3118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://vi.zhonguo2118.cn

[U92] JS：深拷贝
来源：https://ds.zhonguo1118.cn

structuredClone(obj)
来源：https://xx.zhonguo5118.cn

[U93] JS：模板字符串
来源：https://ul.zhonguo1118.cn

`共 ${n} 条`
来源：https://qc.zhonguo5118.cn

[U94] JS：箭头函数
来源：https://pm.zhonguo7118.cn

const double = x => x * 2;
来源：https://wd.zhonguo4118.cn

[U95] JS：Promise 包装
来源：https://hk.zhonguo5118.cn

new Promise((resolve, reject) => {})
来源：https://gf.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://ha.zhonguo5118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://uc.zhonguo2118.cn

[U97] JS：并发请求
来源：https://xu.zhonguo1118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://ks.zhonguo5118.cn

[U98] JS：fetch 带 JSON
来源：https://fw.zhonguo3118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://vo.zhonguo3118.cn

[U99] JS：事件监听
来源：https://dx.zhonguo2118.cn

el.addEventListener("click", e => {})
来源：https://ku.zhonguo1118.cn

[U100] JS：DOM 查询
来源：https://ar.zhonguo8118.cn

document.querySelector(".item")
来源：https://vs.zhonguo6118.cn

[U101] JS：classList 操作
来源：https://ee.zhonguo6118.cn

el.classList.toggle("active")
来源：https://xf.zhonguo2118.cn

[U102] JS：本地存储
来源：https://kq.zhonguo6118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://bv.zhonguo2118.cn

[U103] JS：定时器
来源：https://lw.zhonguo2118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://qj.zhonguo1118.cn

[U104] JS：防抖
来源：https://de.zhonguo7118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://ms.zhonguo4118.cn

[U105] JS：节流
来源：https://st.zhonguo8118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://mi.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://yr.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://kl.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://nn.zhonguo6118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://rf.zhonguo7118.cn

[U108] JS：随机整数
来源：https://wo.zhonguo2118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://fg.zhonguo1118.cn

[U109] JS：数组分组
来源：https://dv.zhonguo6118.cn

Object.groupBy(arr, x => x.type)
来源：https://dm.zhonguo7118.cn

[U110] JS：数组分块
来源：https://iz.zhonguo8118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://jt.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://oe.zhonguo6118.cn

new Map(Object.entries(obj))
来源：https://ps.zhonguo2118.cn

[U112] JS：字符串补位
来源：https://pi.zhonguo1118.cn

"7".padStart(3, "0")
来源：https://wa.zhonguo5118.cn

[U113] JS：正则替换全部
来源：https://qc.zhonguo4118.cn

s.replaceAll("a", "b")
来源：https://jc.zhonguo2118.cn

[U114] JS：JSON 深比较
来源：https://rv.zhonguo8118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://pb.zhonguo3118.cn

[U115] JS：生成 UUID
来源：https://ii.zhonguo8118.cn

crypto.randomUUID()
来源：https://kv.zhonguo5118.cn

[U116] JS：类型检查（JSDoc）
来源：https://dl.zhonguo8118.cn

/** @param {string} name */ function f(name) {}
来源：https://zh.zhonguo8118.cn

[U117] JS：单元测试
来源：https://we.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://wm.zhonguo5118.cn

[U118] JS：开发服务器
来源：https://gn.zhonguo3118.cn

npm i -D vite;  npx vite
来源：https://ir.zhonguo7118.cn

[U119] JS：生产构建
来源：https://fm.zhonguo1118.cn

npx vite build
来源：https://bo.zhonguo5118.cn

[U120] JS：读取环境变量（Vite）
来源：https://jn.zhonguo5118.cn

import.meta.env.VITE_API_URL
来源：https://yf.zhonguo7118.cn

================================================================================
来源：https://xk.zhonguo8118.cn

统计汇总
来源：https://he.zhonguo4118.cn

================================================================================
来源：https://yo.zhonguo4118.cn

按语言统计（条）：
来源：https://fg.zhonguo2118.cn

Python ......... 252
来源：https://od.zhonguo3118.cn

PHP ............ 252
来源：https://nq.zhonguo2118.cn

JavaScript ..... 252
来源：https://fo.zhonguo5118.cn

TypeScript ..... 212
来源：https://ug.zhonguo3118.cn

Java ........... 212
来源：https://te.zhonguo8118.cn

Go ............. 212
来源：https://dd.zhonguo3118.cn

Ruby ........... 212
来源：https://yw.zhonguo3118.cn

C# ............. 212
来源：https://vq.zhonguo2118.cn

C .............. 30
来源：https://rp.zhonguo7118.cn

C++ ............ 30
来源：https://ko.zhonguo3118.cn

SQL ............ 90
来源：https://xf.zhonguo4118.cn

Bash ........... 80
来源：https://qq.zhonguo7118.cn

Kotlin ......... 15
来源：https://js.zhonguo1118.cn

Swift .......... 15
来源：https://vv.zhonguo5118.cn

Lua ............ 10
来源：https://sq.zhonguo5118.cn

Perl ........... 10
来源：https://fp.zhonguo4118.cn

Scala .......... 10
来源：https://db.zhonguo1118.cn

------------------------------------
来源：https://pe.zhonguo3118.cn

合计 ........... 2106 条
来源：https://fx.zhonguo3118.cn

按章节统计：
来源：https://te.zhonguo4118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://qk.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://gj.zhonguo8118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://pz.zhonguo1118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://aa.zhonguo6118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://pi.zhonguo8118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://xs.zhonguo5118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://xe.zhonguo3118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://sa.zhonguo2118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://oe.zhonguo5118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://pj.zhonguo2118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://hy.zhonguo2118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://si.zhonguo3118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://xe.zhonguo7118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://jr.zhonguo3118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://ip.zhonguo7118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://yz.zhonguo1118.cn

Q SQL 专题                              90
来源：https://sx.zhonguo5118.cn

R Bash 专题                             80
来源：https://ax.zhonguo7118.cn

S C / C++ 专题                          60
来源：https://mt.zhonguo7118.cn

T 其他语言补充                          60
来源：https://ja.zhonguo3118.cn

U 高频实用片段                         120
来源：https://mq.zhonguo4118.cn

------------------------------------
来源：https://ov.zhonguo7118.cn

合计                                  2106 条
来源：https://se.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://hv.zhonguo7118.cn

使用提醒
来源：https://ql.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://zy.zhonguo5118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://bu.zhonguo6118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://mk.zhonguo3118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://hg.zhonguo7118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://ew.zhonguo7118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://dz.zhonguo8118.cn

—— 文件结束 ——
来源：https://dc.zhonguo5118.cn

================================================================================
来源：https://mx.zhonguo2118.cn

程序语言常见例子速查手册（2024 版）
来源：https://ye.zhonguo6118.cn

Common Programming Examples Cheat Book
来源：https://ah.zhonguo1118.cn

================================================================================
来源：https://xk.zhonguo7118.cn

【收录内容】
来源：https://ui.zhonguo8118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://kz.zhonguo2118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://if.zhonguo6118.cn

SQL · Bash · C · C++
来源：https://sd.zhonguo4118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://av.zhonguo4118.cn

【使用说明】
来源：https://un.zhonguo2118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://lw.zhonguo8118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://ih.zhonguo8118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://yv.zhonguo4118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://xs.zhonguo4118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://nn.zhonguo7118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://mv.zhonguo7118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://js.zhonguo4118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://st.zhonguo5118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://mp.zhonguo3118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://rw.zhonguo8118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://jf.zhonguo6118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://hu.zhonguo6118.cn

【文件统计】
来源：https://ah.zhonguo1118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://cs.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://cy.zhonguo3118.cn

目  录
来源：https://na.zhonguo4118.cn

--------------------------------------------------------------------------------
来源：https://qk.zhonguo7118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://ro.zhonguo4118.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：https://jb.zhonguo5118.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：https://od.zhonguo7118.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：https://yi.zhonguo3118.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：https://so.zhonguo3118.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：https://ed.zhonguo8118.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：https://vs.zhonguo3118.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：https://nj.zhonguo1118.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：https://rv.zhonguo3118.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：https://td.zhonguo2118.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：https://ls.zhonguo4118.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：https://gz.zhonguo6118.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：https://or.zhonguo3118.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：https://mu.zhonguo4118.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：https://lv.zhonguo6118.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：https://js.zhonguo8118.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：https://ta.zhonguo1118.cn

R. Bash 专题                   （第 18 节，80 条）
来源：https://fi.zhonguo3118.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：https://ag.zhonguo8118.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：https://ei.zhonguo6118.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：https://cp.zhonguo6118.cn

================================================================================
来源：https://rn.zhonguo1118.cn

A. 基础语法与类型
来源：https://ig.zhonguo3118.cn

================================================================================
来源：https://zr.zhonguo1118.cn

[A01] Hello World
来源：https://uy.zhonguo1118.cn

Py:   print("Hello, World!")
来源：https://th.zhonguo8118.cn

PHP:  echo "Hello, World!";
来源：https://yk.zhonguo1118.cn

JS:   console.log("Hello, World!");
来源：https://yy.zhonguo1118.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：https://vh.zhonguo7118.cn

Java: System.out.println("Hello, World!");
来源：https://rs.zhonguo6118.cn

Go:   fmt.Println("Hello, World!")
来源：https://ah.zhonguo1118.cn

Ruby: puts "Hello, World!"
来源：https://fw.zhonguo5118.cn

C#:   Console.WriteLine("Hello, World!");
来源：https://cb.zhonguo6118.cn

[A02] 变量声明与赋值
来源：https://sz.zhonguo6118.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：https://wc.zhonguo6118.cn

PHP:  $name = "Alex"; $age = 20;
来源：https://nc.zhonguo6118.cn

JS:   let name = "Alex"; const age = 20;
来源：https://vz.zhonguo8118.cn


<!-- 参考信息 -->