代发 wailian999

[U37] Py：读写 Excel
来源：http://nhg.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://wgo.yfazqb.com

[U38] Py：获取脚本所在目录
来源：http://kxg.sweek.top

Path(__file__).resolve().parent
来源：http://bna.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://rtl.jyoumei.cn

sys.stdout.isatty()
来源：http://alx.yj20258888.top

[U40] Py：打印到标准错误
来源：http://aib.fzhhl.top

print("err", file=sys.stderr)
来源：http://abo.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://trj.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://erb.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://ege.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ice.316326.xyz

[U43] PHP：声明命名空间
来源：http://nyw.sufxvd.cn

namespace App\Http;
来源：http://hvc.vehdjk.com

[U44] PHP：开启严格类型
来源：http://xmw.sweek.top

declare(strict_types=1);
来源：http://cbe.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://jxb.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://arp.dashuyun.cn

[U46] PHP：可空类型
来源：http://gqs.wangdashe.top

?string $name = null
来源：http://thp.zdqjudy.top

[U47] PHP：联合类型
来源：http://abq.bjfxy.top

int|string $id
来源：http://bbk.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://eac.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hre.cucudq.cn

[U49] PHP：只读属性
来源：http://feo.zhongyouzk.top

public readonly string $name
来源：http://vwq.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://ktv.zdqjudy.top

public function __construct(private int $id) {}
来源：http://tlu.chenzaomai.com

[U51] PHP：数组解构
来源：http://lsj.zdbjq.cn

[$a, $b] = $arr;
来源：http://wgo.sufxvd.cn

[U52] PHP：箭头函数
来源：http://alo.sweek.top

$double = fn($x) => $x * 2;
来源：http://jwa.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://lhm.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://hoh.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://sxu.zhongyouzk.top

$obj?->method()
来源：http://qsw.aibaodan.cn

[U55] PHP：match 表达式
来源：http://tis.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://llx.tian-w.cn

[U56] PHP：命名参数
来源：http://cxd.fzhhl.top

f(a: 1, b: 2)
来源：http://sow.yonumen.top

[U57] PHP：字符串插值
来源：http://lwh.yj20258888.top

"值: {$a}"
来源：http://ube.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://ior.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bws.gzhubu.top

[U59] PHP：自定义排序
来源：http://hoc.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xpc.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://fpx.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hfz.mhx1999.top

[U61] PHP：正则
来源：http://sqe.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jil.hcnkem.com

[U62] PHP：日期对象
来源：http://vgt.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tzh.daxiang520.top

[U63] PHP：文件读写
来源：http://ggo.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oyc.yangfankeji.com

[U64] PHP：目录遍历
来源：http://syb.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ngi.jlsjyb.cn

[U65] PHP：会话
来源：http://osl.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://aei.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://rog.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tre.yvedp.cn

[U67] PHP：处理文件上传
来源：http://ldg.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bsj.hcnkem.com

[U68] PHP：PDO 连接
来源：http://dqj.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sat.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://suf.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://igw.yj20258.top

[U70] PHP：PDO 事务
来源：http://pph.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pcu.gaohongyu789.top

[U71] PHP：抛出异常
来源：http://mgb.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://yqb.snrcjt.cn

[U72] PHP：写错误日志
来源：http://hbk.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://nbs.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://gyp.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://hyr.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://eoz.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://fjh.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://kem.fanxiaobao.xyz

composer require psr/container
来源：http://sub.yj202588.top

[U76] PHP：简单路由
来源：http://mzk.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bbq.zdqjudy.top

[U77] PHP：模板渲染
来源：http://tyo.smart0.xyz

composer require twig/twig
来源：http://tpb.cucudq.cn

[U78] PHP：单元测试
来源：http://kmq.ivvv.top

composer require --dev phpunit/phpunit
来源：http://yhj.yueranfly.top

[U79] PHP：静态分析
来源：http://frb.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://loj.daxiang520.top

[U80] PHP：代码规范修复
来源：http://bos.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://thg.jinqigfzy.top

[U81] JS：初始化项目
来源：http://kkm.316326.xyz

npm init -y;  npm i express
来源：http://pov.sxryk.cn

[U82] JS：package.json 脚本
来源：http://vdr.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jid.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://zbo.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://knm.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://tti.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://iee.52xcode.cn

[U85] JS：可选链
来源：http://vwz.uphjek.com

a?.b?.c
来源：http://vmb.hcnkem.com

[U86] JS：空值合并
来源：http://qyb.hesvh.cn

a ?? b
来源：http://fef.aizwys.cn

[U87] JS：解构默认值
来源：http://hvg.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://nch.bbcook.cn

[U88] JS：对象展开合并
来源：http://jha.c1oappe.top

{ ...a, ...b }
来源：http://iya.c1oappe.top

[U89] JS：数组去重
来源：http://uii.chenzaomai.com

[...new Set(arr)]
来源：http://uch.cucudq.cn

[U90] JS：数字数组排序
来源：http://grl.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://jzw.pycfn.com

[U91] JS：对象键值遍历
来源：http://cnn.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kvs.0kj1m.cn

[U92] JS：深拷贝
来源：http://mes.fehbvm.com

structuredClone(obj)
来源：http://lgm.tarul.cn

[U93] JS：模板字符串
来源：http://xdv.kuanghao11.cn

`共 ${n} 条`
来源：http://xyy.guowangkeji.top

[U94] JS：箭头函数
来源：http://ipd.andypj.xyz

const double = x => x * 2;
来源：http://nwz.c1oappe.top

[U95] JS：Promise 包装
来源：http://yij.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://qqy.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://itv.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oon.ydzc1.top

[U97] JS：并发请求
来源：http://tqq.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://aht.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://lyg.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ynv.hcnkem.com

[U99] JS：事件监听
来源：http://xhi.shuidangran.top

el.addEventListener("click", e => {})
来源：http://ptf.aizwys.cn

[U100] JS：DOM 查询
来源：http://twt.hfpthk.cn

document.querySelector(".item")
来源：http://kds.chenlongwang.top

[U101] JS：classList 操作
来源：http://akn.ctjpmb.com

el.classList.toggle("active")
来源：http://qzb.fktsv.cn

[U102] JS：本地存储
来源：http://pph.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pxr.kuanghao11.cn

[U103] JS：定时器
来源：http://xvg.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://otm.yj20258888.top

[U104] JS：防抖
来源：http://qxg.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xds.ywan-chungtsiang.top

[U105] JS：节流
来源：http://cxo.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jle.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://rbz.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hpb.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://dob.cucudq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eqt.wangshuangyany.cn

[U108] JS：随机整数
来源：http://mcj.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rki.dashuyun.cn

[U109] JS：数组分组
来源：http://tta.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://agw.yanxiufei.cn

[U110] JS：数组分块
来源：http://vqw.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oxj.ybcxt.top

[U111] JS：对象转 Map
来源：http://cpl.c1oappe.top

new Map(Object.entries(obj))
来源：http://hzs.0kj1m.cn

[U112] JS：字符串补位
来源：http://cnr.yfazqb.com

"7".padStart(3, "0")
来源：http://mok.jinqigufen.top

[U113] JS：正则替换全部
来源：http://krm.xylfe.cn

s.replaceAll("a", "b")
来源：http://qwp.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://zwg.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pod.shuidangran.top

[U115] JS：生成 UUID
来源：http://dbz.ppjwa.cn

crypto.randomUUID()
来源：http://pap.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://yut.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://hcz.jinqigfzy.top

[U117] JS：单元测试
来源：http://bds.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://wud.haohaochexian.top

[U118] JS：开发服务器
来源：http://oca.epnwcf.com

npm i -D vite;  npx vite
来源：http://rbj.xuanzx.com

[U119] JS：生产构建
来源：http://vnq.52xcode.cn

npx vite build
来源：http://jvt.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://fqr.yj20258.top

import.meta.env.VITE_API_URL
来源：http://phj.guowangkeji.top

================================================================================
来源：http://czi.haohaochexian.top

统计汇总
来源：http://uck.ydjk.org.cn

================================================================================
来源：http://ddl.xuetiantiany.cn

按语言统计（条）：
来源：http://mua.zhoulong.xyz

Python ......... 252
来源：http://ndm.ybcxt.top

PHP ............ 252
来源：http://bbe.shanyushiyangtech.top

JavaScript ..... 252
来源：http://led.wangdashe.top

TypeScript ..... 212
来源：http://tui.fktsv.cn

Java ........... 212
来源：http://ipf.xingfuxueyuan.xyz

Go ............. 212
来源：http://pod.shangyingyoupin.top

Ruby ........... 212
来源：http://dnr.kuanghao11.cn

C# ............. 212
来源：http://tax.jlsjyb.cn

C .............. 30
来源：http://pbg.sxryk.cn

C++ ............ 30
来源：http://lij.tarul.cn

SQL ............ 90
来源：http://twj.iojbl.cn

Bash ........... 80
来源：http://aof.mhx1999.top

Kotlin ......... 15
来源：http://yuk.ydjk.org.cn

Swift .......... 15
来源：http://aqi.gotoacloud.top

Lua ............ 10
来源：http://bsf.cqqwz.cn

Perl ........... 10
来源：http://jhk.pycfn.com

Scala .......... 10
来源：http://mho.snrcjt.cn

------------------------------------
来源：http://zgr.tanke756.top

合计 ........... 2106 条
来源：http://qlz.jiagoushi.top

按章节统计：
来源：http://yal.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ovg.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fwx.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://irk.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sly.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mcq.wangshuangyany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kld.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kmj.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qrn.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://glb.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hni.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lfw.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zjl.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xtm.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uys.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ltt.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nlv.ybcxt.top

Q SQL 专题                              90
来源：http://vjc.jqgufenzy.top

R Bash 专题                             80
来源：http://rjt.zhiwuduotai.top

S C / C++ 专题                          60
来源：http://cmo.ctjpmb.com

T 其他语言补充                          60
来源：http://ywh.52xcode.cn

U 高频实用片段                         120
来源：http://loq.xuetiantiany.cn

------------------------------------
来源：http://bua.daxiang520.top

合计                                  2106 条
来源：http://qwf.andypj.xyz

--------------------------------------------------------------------------------
来源：http://ovg.andypj.xyz

使用提醒
来源：http://wcx.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://mhc.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wql.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://smp.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://udm.chenzaomai.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dqr.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mqs.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://yym.yvedp.cn

================================================================================
来源：http://rfz.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://gpw.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://byk.zdqjudy.top

================================================================================
来源：http://kff.guowangkeji.top

【收录内容】
来源：http://gvk.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ezl.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oee.316326.xyz

SQL · Bash · C · C++
来源：http://sji.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://snl.vqdsnc.cn

【使用说明】
来源：http://cas.zycfv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qxw.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hcf.aizwys.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://boi.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bfn.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://xmc.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ziy.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cdt.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qes.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://esl.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hcx.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://biy.birdmap.top

【文件统计】
来源：http://xof.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gup.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://yqo.shzxlz.cn

目  录
来源：http://dxc.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://mcs.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bbr.hnqzz.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jhq.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kxv.feifeiyinyue.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://teh.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vtt.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eha.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dfr.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ksj.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fjk.fengsongda.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xxv.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fzb.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ehg.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cip.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kwg.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://spo.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://azu.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ipp.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://vyk.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ayy.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yup.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fyn.smart0.xyz

================================================================================
来源：http://fgh.yonumen.top

A. 基础语法与类型
来源：http://ebg.sufxvd.cn

================================================================================
来源：http://wlp.andypj.xyz

[A01] Hello World
来源：http://mgx.aibaodan.cn

Py:   print("Hello, World!")
来源：http://luu.jqgufenzy.top

PHP:  echo "Hello, World!";
来源：http://vff.316326.xyz

JS:   console.log("Hello, World!");
来源：http://abz.ppjwa.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wch.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://obg.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://mhw.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://iuw.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qtr.tarul.cn

[A02] 变量声明与赋值
来源：http://hwv.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mgd.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://duq.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://deb.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pyn.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://tvk.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://xil.shzxlz.cn

Ruby: name = "Alex"; age = 20
来源：http://vim.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://rhg.svipenyu.cn

[A03] 常量定义
来源：http://uqn.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ylb.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://xsy.hywenlv.cn

JS:   const PI = 3.14159;
来源：http://ego.sweek.top

TS:   const PI: number = 3.14159;
来源：http://gpf.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://fuq.c1oappe.top

Go:   const PI = 3.14159
来源：http://tps.ydzc1.top


<!-- 参考信息 -->