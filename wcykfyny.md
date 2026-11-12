代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://slg.tian-w.cn

sys.stdout.isatty()
来源：http://rxg.epnwcf.com

[U40] Py：打印到标准错误
来源：http://tdr.hesvh.cn

print("err", file=sys.stderr)
来源：http://opt.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://twc.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jxf.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://qud.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xsn.bbcook.cn

[U43] PHP：声明命名空间
来源：http://hiq.zhoulong.xyz

namespace App\Http;
来源：http://euu.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://xew.iojbl.cn

declare(strict_types=1);
来源：http://jds.nanxinkj.top

[U45] PHP：类型声明与返回类型
来源：http://ptf.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rpp.jianghu66.top

[U46] PHP：可空类型
来源：http://dpn.ivvv.top

?string $name = null
来源：http://osb.quarkkingdee.top

[U47] PHP：联合类型
来源：http://xio.ppjwa.cn

int|string $id
来源：http://dre.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://wtu.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xaf.gzhubu.top

[U49] PHP：只读属性
来源：http://bcn.ppjwa.cn

public readonly string $name
来源：http://eox.yongpay.top

[U50] PHP：构造器属性提升
来源：http://lpm.zycfv.cn

public function __construct(private int $id) {}
来源：http://wov.9152youxi.cn

[U51] PHP：数组解构
来源：http://jpa.xziqi.cn

[$a, $b] = $arr;
来源：http://juh.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://vwo.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://mnv.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://gtr.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://fxy.cashguo.top

[U54] PHP：空安全调用
来源：http://rne.vqdsnc.cn

$obj?->method()
来源：http://spb.zycfv.cn

[U55] PHP：match 表达式
来源：http://qio.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kjh.chenlongwang.top

[U56] PHP：命名参数
来源：http://byr.cheryme.top

f(a: 1, b: 2)
来源：http://fpx.ivvv.top

[U57] PHP：字符串插值
来源：http://mgx.zdqjudy.top

"值: {$a}"
来源：http://ekx.epnwcf.com

[U58] PHP：数组三件套
来源：http://oqr.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zek.xziqi.cn

[U59] PHP：自定义排序
来源：http://wam.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yfz.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://vjn.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tod.ppjwa.cn

[U61] PHP：正则
来源：http://ofm.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nym.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://vzs.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xqp.hammf.cn

[U63] PHP：文件读写
来源：http://tlb.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://shu.yj202588.top

[U64] PHP：目录遍历
来源：http://vfy.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://lkx.c1oappe.top

[U65] PHP：会话
来源：http://opd.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://bvw.sweek.top

[U66] PHP：设置 Cookie
来源：http://ipm.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kbo.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://uan.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uic.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://xpd.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://axb.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://ljh.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://drd.fzhhl.top

[U70] PHP：PDO 事务
来源：http://zdo.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://svf.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://feb.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://lvu.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://pmx.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://sru.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://ltu.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://pxv.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://yui.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://fgl.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://jqs.jqgufenzy.top

composer require psr/container
来源：http://qfe.jiagoushi.top

[U76] PHP：简单路由
来源：http://etw.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://spy.chenzaomai.com

[U77] PHP：模板渲染
来源：http://hqt.tian-w.cn

composer require twig/twig
来源：http://dep.wangdashe.top

[U78] PHP：单元测试
来源：http://ier.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://ezz.redwolf501.top

[U79] PHP：静态分析
来源：http://dmg.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://jlj.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://mgk.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://cvq.yj20258888.top

[U81] JS：初始化项目
来源：http://vjb.dianchejie.cn

npm init -y;  npm i express
来源：http://tie.cashguo.top

[U82] JS：package.json 脚本
来源：http://hnd.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hco.dashuyun.cn

[U83] JS：ES Module 导入导出
来源：http://fuf.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://aab.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://wan.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://jfc.zhengqikj.top

[U85] JS：可选链
来源：http://fmj.fehbvm.com

a?.b?.c
来源：http://vdf.hongshengwenyu.top

[U86] JS：空值合并
来源：http://iyr.sjlbkw.cn

a ?? b
来源：http://xim.yuanzhike.top

[U87] JS：解构默认值
来源：http://wor.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://olx.yj20258888.top

[U88] JS：对象展开合并
来源：http://ljq.jyoumei.cn

{ ...a, ...b }
来源：http://tuv.hesvh.cn

[U89] JS：数组去重
来源：http://sxn.redwolf501.top

[...new Set(arr)]
来源：http://zur.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://qpq.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://nvx.meibo888.top

[U91] JS：对象键值遍历
来源：http://czn.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zfc.316326.xyz

[U92] JS：深拷贝
来源：http://bcy.haohaochexian.top

structuredClone(obj)
来源：http://djf.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://qdq.aibaodan.cn

`共 ${n} 条`
来源：http://mza.gaohongyu789.top

[U94] JS：箭头函数
来源：http://psg.kuanghao11.cn

const double = x => x * 2;
来源：http://zjr.guowangkeji.top

[U95] JS：Promise 包装
来源：http://dep.yongpay.top

new Promise((resolve, reject) => {})
来源：http://mnn.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://bqh.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mur.nanxinkj.top

[U97] JS：并发请求
来源：http://uuh.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://psy.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://bud.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aqa.snrcjt.cn

[U99] JS：事件监听
来源：http://tkf.zycfv.cn

el.addEventListener("click", e => {})
来源：http://rff.chenzaomai.com

[U100] JS：DOM 查询
来源：http://tbt.redwolf501.top

document.querySelector(".item")
来源：http://juh.iojbl.cn

[U101] JS：classList 操作
来源：http://gsi.fengsongda.top

el.classList.toggle("active")
来源：http://krx.jlsjyb.cn

[U102] JS：本地存储
来源：http://mmc.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://eqq.9152youxi.cn

[U103] JS：定时器
来源：http://fyq.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mui.vqdsnc.cn

[U104] JS：防抖
来源：http://bis.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://owp.vehdjk.com

[U105] JS：节流
来源：http://kfu.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pjg.c1oappe.top

[U106] JS：日期格式化
来源：http://pxr.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cee.gotoacloud.top

[U107] JS：数字千分位
来源：http://ywt.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://paa.ivvv.top

[U108] JS：随机整数
来源：http://yck.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kgt.havefunace.top

[U109] JS：数组分组
来源：http://omb.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://yzk.316326.xyz

[U110] JS：数组分块
来源：http://izm.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nav.shzxlz.cn

[U111] JS：对象转 Map
来源：http://tzf.iojbl.cn

new Map(Object.entries(obj))
来源：http://mxj.ctjpmb.com

[U112] JS：字符串补位
来源：http://zlm.aizwys.cn

"7".padStart(3, "0")
来源：http://cgw.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://uwy.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://omu.aizwys.cn

[U114] JS：JSON 深比较
来源：http://okr.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xal.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://gxb.aibaodan.cn

crypto.randomUUID()
来源：http://kho.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://nsm.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://thb.cdnleiting.top

[U117] JS：单元测试
来源：http://jut.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://ywm.daria6918.cn

[U118] JS：开发服务器
来源：http://xkz.havefunace.top

npm i -D vite;  npx vite
来源：http://bdv.aibaodan.cn

[U119] JS：生产构建
来源：http://ohb.bbcook.cn

npx vite build
来源：http://xwa.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://mmq.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://pxz.yj20258888.top

================================================================================
来源：http://flt.ehwqpu.com

统计汇总
来源：http://tfx.ehwqpu.com

================================================================================
来源：http://ulo.vqdsnc.cn

按语言统计（条）：
来源：http://ekv.redwolf501.top

Python ......... 252
来源：http://nnn.cdnleiting.top

PHP ............ 252
来源：http://dah.jyoumei.cn

JavaScript ..... 252
来源：http://oaz.zhiwuduotai.top

TypeScript ..... 212
来源：http://xuh.pycfn.com

Java ........... 212
来源：http://rra.jinqigfzy.top

Go ............. 212
来源：http://pfh.snrcjt.cn

Ruby ........... 212
来源：http://pim.hysaishi.cn

C# ............. 212
来源：http://niu.kuanghao11.cn

C .............. 30
来源：http://qdz.tanke756.top

C++ ............ 30
来源：http://jce.cqqwz.cn

SQL ............ 90
来源：http://isl.dianchejie.cn

Bash ........... 80
来源：http://nqq.tanke756.top

Kotlin ......... 15
来源：http://itf.quarkkingdee.top

Swift .......... 15
来源：http://pfz.jiagoushi.top

Lua ............ 10
来源：http://snp.jinqigufen.top

Perl ........... 10
来源：http://gbt.daria6918.cn

Scala .......... 10
来源：http://gph.zhijiandao.cn

------------------------------------
来源：http://pre.yuanzhike.top

合计 ........... 2106 条
来源：http://kme.zhengqikj.top

按章节统计：
来源：http://cuu.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kqo.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aym.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lkl.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ynq.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kwr.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rmc.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yge.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jpc.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://umg.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cau.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vmi.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hyq.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://djq.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://axs.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sfh.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rzn.fehbvm.com

Q SQL 专题                              90
来源：http://qmg.yj20258888.top

R Bash 专题                             80
来源：http://wut.c1oappe.top

S C / C++ 专题                          60
来源：http://nuf.hywenlv.cn

T 其他语言补充                          60
来源：http://dgr.tianlin.xyz

U 高频实用片段                         120
来源：http://kgz.cdnleiting.top

------------------------------------
来源：http://bah.hammf.cn

合计                                  2106 条
来源：http://fsq.wangdashe.top

--------------------------------------------------------------------------------
来源：http://saq.chenlongwang.top

使用提醒
来源：http://baq.xuanzx.com

--------------------------------------------------------------------------------
来源：http://cqu.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ytu.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cka.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qyl.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xsb.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pah.hysaishi.cn

—— 文件结束 ——
来源：http://jzb.yfazqb.com

================================================================================
来源：http://plo.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://gsr.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://jry.cqqwz.cn

================================================================================
来源：http://rrt.jinghuilouyu.cn

【收录内容】
来源：http://pbd.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dec.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rpa.yuanzhike.top

SQL · Bash · C · C++
来源：http://zkm.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bfp.cucudq.cn

【使用说明】
来源：http://jdw.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rhs.tian-w.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xmy.jlsjyb.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cnt.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jxq.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ycz.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zoq.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fis.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qhg.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vut.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wmo.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qvp.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aco.jyoumei.cn

【文件统计】
来源：http://gpl.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://twa.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://dys.dashuyun.cn

目  录
来源：http://ylb.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://fhb.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kgj.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qzh.pycfn.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qyf.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fzr.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nwh.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bkk.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ejz.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mmm.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ntu.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wwl.xuetiantiany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oet.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ogo.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zxe.0kj1m.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gsv.zhoulong.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nqi.tanke756.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wco.yvedp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sjl.ybcxt.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vku.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oao.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvb.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hpu.jinqigufen.top

================================================================================
来源：http://ijx.chenlongwang.top

A. 基础语法与类型
来源：http://ztb.shangyingyoupin.top

================================================================================
来源：http://olw.dianchejie.cn

[A01] Hello World
来源：http://scr.haohaochexian.top

Py:   print("Hello, World!")
来源：http://yfv.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://egz.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://qgo.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vrw.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://rll.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://yil.aibaodan.cn

Ruby: puts "Hello, World!"
来源：http://noq.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gbv.bbcook.cn

[A02] 变量声明与赋值
来源：http://jhe.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ycj.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://lhk.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://gds.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aro.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://pzr.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://svk.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://ist.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://phf.uphjek.com

[A03] 常量定义
来源：http://wna.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dwx.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://ydx.smart0.xyz

JS:   const PI = 3.14159;
来源：http://yoc.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://pah.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://qag.nwbrower.top

Go:   const PI = 3.14159
来源：http://ykh.ybcxt.top

Ruby: PI = 3.14159
来源：http://wlc.yj20258.top

C#:   const double PI = 3.14159;
来源：http://avm.hfpthk.cn

[A04] 判断变量类型
来源：http://wnu.xinyue.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://lpx.hammf.cn


<!-- 参考信息 -->