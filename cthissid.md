代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://dxv.shangyingyoupin.top

sys.stdout.isatty()
来源：http://eqd.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://lrz.redwolf501.top

print("err", file=sys.stderr)
来源：http://zcl.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://asa.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://suj.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://dmf.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lcx.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://mrp.xziqi.cn

namespace App\Http;
来源：http://yhn.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://spg.uphjek.com

declare(strict_types=1);
来源：http://qqt.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://tiq.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gmy.fktsv.cn

[U46] PHP：可空类型
来源：http://ois.sjlbkw.cn

?string $name = null
来源：http://zyj.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://qaw.gaohongyu789.top

int|string $id
来源：http://rxy.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://eov.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://puh.xuanzx.com

[U49] PHP：只读属性
来源：http://bxx.316326.xyz

public readonly string $name
来源：http://zfz.yonumen.top

[U50] PHP：构造器属性提升
来源：http://dqu.9152youxi.cn

public function __construct(private int $id) {}
来源：http://hjn.gaohongyu789.top

[U51] PHP：数组解构
来源：http://owb.jinqigufen.top

[$a, $b] = $arr;
来源：http://nru.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://uzd.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://mow.xylfe.cn

[U53] PHP：空合并运算符
来源：http://liq.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://vss.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://vlb.zhijiandao.cn

$obj?->method()
来源：http://rzr.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://cwj.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nuw.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://pkn.zhixingplan.top

f(a: 1, b: 2)
来源：http://zej.yongpay.top

[U57] PHP：字符串插值
来源：http://dla.daria6918.cn

"值: {$a}"
来源：http://etl.ydzc1.top

[U58] PHP：数组三件套
来源：http://gmq.gogol.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vor.chenzaomai.com

[U59] PHP：自定义排序
来源：http://ftd.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tyd.sweek.top

[U60] PHP：JSON 编解码
来源：http://dbe.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://obb.sjlbkw.cn

[U61] PHP：正则
来源：http://fnk.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mdz.smart0.xyz

[U62] PHP：日期对象
来源：http://kby.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oyv.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://hhs.yfazqb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ehu.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://kle.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://qde.uphjek.com

[U65] PHP：会话
来源：http://pgp.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sbj.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://krx.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://soz.tian-w.cn

[U67] PHP：处理文件上传
来源：http://ift.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jyn.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://hhn.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://skw.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://dod.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ytr.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://tyv.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mlp.sufxvd.cn

[U71] PHP：抛出异常
来源：http://reg.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://cuh.hesvh.cn

[U72] PHP：写错误日志
来源：http://ojw.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://fxf.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://vek.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://bac.hammf.cn

[U74] PHP：读取环境变量
来源：http://iak.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://cwe.wangdashe.top

[U75] PHP：依赖注入
来源：http://jjh.redwolf501.top

composer require psr/container
来源：http://wwe.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://enk.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lyh.c1oappe.top

[U77] PHP：模板渲染
来源：http://gqn.hnqzz.top

composer require twig/twig
来源：http://vig.fktsv.cn

[U78] PHP：单元测试
来源：http://bzo.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://bqt.hnxiangtu.top

[U79] PHP：静态分析
来源：http://wof.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://jiq.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://odn.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://dhr.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://mmx.cucudq.cn

npm init -y;  npm i express
来源：http://tmo.xziqi.cn

[U82] JS：package.json 脚本
来源：http://wpo.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://chv.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://lhx.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kft.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://egh.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wvx.jlsjyb.cn

[U85] JS：可选链
来源：http://rkg.yueranfly.top

a?.b?.c
来源：http://jpu.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://aif.hysaishi.cn

a ?? b
来源：http://vlz.sjlbkw.cn

[U87] JS：解构默认值
来源：http://icp.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://qnh.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://qfl.xuetiantiany.cn

{ ...a, ...b }
来源：http://sfa.hcnkem.com

[U89] JS：数组去重
来源：http://evz.yj20258888.top

[...new Set(arr)]
来源：http://pnc.wangdashe.top

[U90] JS：数字数组排序
来源：http://yup.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://rev.yvedp.cn

[U91] JS：对象键值遍历
来源：http://zxa.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kbo.xinyue.icu

[U92] JS：深拷贝
来源：http://cbc.hongshengwenyu.top

structuredClone(obj)
来源：http://uff.cdnleiting.top

[U93] JS：模板字符串
来源：http://exk.ybcxt.top

`共 ${n} 条`
来源：http://qxv.cashguo.top

[U94] JS：箭头函数
来源：http://ieb.aibaodan.cn

const double = x => x * 2;
来源：http://gmh.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://kht.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://lon.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://guy.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hzb.shangyingyoupin.top

[U97] JS：并发请求
来源：http://zjh.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://moj.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://jzw.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ezd.epnwcf.com

[U99] JS：事件监听
来源：http://owa.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://qmb.bjfxy.top

[U100] JS：DOM 查询
来源：http://roy.gzhubu.top

document.querySelector(".item")
来源：http://fsf.316326.xyz

[U101] JS：classList 操作
来源：http://tuj.xylfe.cn

el.classList.toggle("active")
来源：http://ejh.wangshuangyany.cn

[U102] JS：本地存储
来源：http://dop.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hfy.yongpay.top

[U103] JS：定时器
来源：http://kyj.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://llf.tian-w.cn

[U104] JS：防抖
来源：http://wab.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gmg.xuetiantiany.cn

[U105] JS：节流
来源：http://daa.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ahd.hfpthk.cn

[U106] JS：日期格式化
来源：http://ujd.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tuw.xylfe.cn

[U107] JS：数字千分位
来源：http://kxl.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fud.cqqwz.cn

[U108] JS：随机整数
来源：http://ixh.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yos.birdmap.top

[U109] JS：数组分组
来源：http://zuu.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://fgo.gogol.net.cn

[U110] JS：数组分块
来源：http://hgt.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yvs.tian-w.cn

[U111] JS：对象转 Map
来源：http://dxy.316326.xyz

new Map(Object.entries(obj))
来源：http://nxq.yueranfly.top

[U112] JS：字符串补位
来源：http://tbh.guannengcc.top

"7".padStart(3, "0")
来源：http://nin.tian-w.cn

[U113] JS：正则替换全部
来源：http://zgo.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://gon.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://nov.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://paf.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://tez.guannengcc.top

crypto.randomUUID()
来源：http://zsf.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://nta.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://und.fktsv.cn

[U117] JS：单元测试
来源：http://uvi.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://spq.shzxlz.cn

[U118] JS：开发服务器
来源：http://vwc.fehbvm.com

npm i -D vite;  npx vite
来源：http://ocq.tarul.cn

[U119] JS：生产构建
来源：http://kld.xuanzx.com

npx vite build
来源：http://fom.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://mvt.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://czt.fzhhl.top

================================================================================
来源：http://bfd.hcnkem.com

统计汇总
来源：http://nhf.fanxiaobao.xyz

================================================================================
来源：http://sje.redwolf501.top

按语言统计（条）：
来源：http://sgg.fzhhl.top

Python ......... 252
来源：http://huh.yfazqb.com

PHP ............ 252
来源：http://szw.hnxiangtu.top

JavaScript ..... 252
来源：http://hqs.dianchejie.cn

TypeScript ..... 212
来源：http://vip.birdmap.top

Java ........... 212
来源：http://jgt.cqqwz.cn

Go ............. 212
来源：http://fxu.guannengcc.top

Ruby ........... 212
来源：http://gbe.ivvv.top

C# ............. 212
来源：http://nfp.yonumen.top

C .............. 30
来源：http://gpx.guowangkeji.top

C++ ............ 30
来源：http://sxu.guowangkeji.top

SQL ............ 90
来源：http://jyi.tianlin.xyz

Bash ........... 80
来源：http://kai.quarkkingdee.top

Kotlin ......... 15
来源：http://gav.cheryme.top

Swift .......... 15
来源：http://cml.sweek.top

Lua ............ 10
来源：http://wmu.andypj.xyz

Perl ........... 10
来源：http://ows.gzhubu.top

Scala .......... 10
来源：http://sqi.sufxvd.cn

------------------------------------
来源：http://qcz.zhixingplan.top

合计 ........... 2106 条
来源：http://tat.ydjk.org.cn

按章节统计：
来源：http://cvs.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ifw.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xwz.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nmp.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iex.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kvz.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ufe.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fgl.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://atc.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ebt.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kqa.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zdx.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://heq.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dkl.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://amr.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rvy.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rij.jinqigufen.top

Q SQL 专题                              90
来源：http://xgu.xylfe.cn

R Bash 专题                             80
来源：http://hgh.aizwys.cn

S C / C++ 专题                          60
来源：http://vlj.tianlin.xyz

T 其他语言补充                          60
来源：http://gmq.birdmap.top

U 高频实用片段                         120
来源：http://lju.cucudq.cn

------------------------------------
来源：http://fmz.mhx1999.top

合计                                  2106 条
来源：http://wjp.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://qyt.jiagoushi.top

使用提醒
来源：http://jvd.mhx1999.top

--------------------------------------------------------------------------------
来源：http://mjn.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lfb.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wug.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hxd.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fou.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxn.sweek.top

—— 文件结束 ——
来源：http://ile.hnxiangtu.top

================================================================================
来源：http://lwb.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://ola.fktsv.cn

Common Programming Examples Cheat Book
来源：http://piy.gzhubu.top

================================================================================
来源：http://fmn.hongshengwenyu.top

【收录内容】
来源：http://clx.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://kzw.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pbm.nanxinkj.top

SQL · Bash · C · C++
来源：http://xop.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://idm.havefunace.top

【使用说明】
来源：http://ryh.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yvl.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wgr.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yvn.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lgt.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://jyg.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tad.wangshuangyany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://buf.jiagoushi.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lmz.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bpk.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://njz.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fpb.feifeiyinyue.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rgq.yuxming.cn

【文件统计】
来源：http://fwz.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qof.fehbvm.com

--------------------------------------------------------------------------------
来源：http://czg.hammf.cn

目  录
来源：http://lkd.yueranfly.top

--------------------------------------------------------------------------------
来源：http://usc.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zjf.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hwk.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uwj.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ucs.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qvj.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hhi.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://htk.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mic.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eoc.haohaochexian.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://thm.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wkd.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rww.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mcw.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rdv.hesvh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ute.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fzy.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uhy.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rci.cheryme.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bbs.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qvd.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ion.sxryk.cn

================================================================================
来源：http://xnt.xylfe.cn

A. 基础语法与类型
来源：http://mdf.jiagoushi.top

================================================================================
来源：http://nmg.zhengqikj.top

[A01] Hello World
来源：http://juv.haohaochexian.top

Py:   print("Hello, World!")
来源：http://two.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://tcn.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://ygi.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://stj.zhongyouzk.top

Java: System.out.println("Hello, World!");
来源：http://ewf.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://osz.zycfv.cn

Ruby: puts "Hello, World!"
来源：http://mlz.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cua.316326.xyz

[A02] 变量声明与赋值
来源：http://kms.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nsl.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hcu.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://jyv.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yic.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://ipc.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://dcx.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://lfh.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lla.havefunace.top

[A03] 常量定义
来源：http://duz.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wbg.tanke756.top

PHP:  const PI = 3.14159;
来源：http://csb.zycfv.cn

JS:   const PI = 3.14159;
来源：http://vlt.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://fio.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://qvy.ydzc1.top

Go:   const PI = 3.14159
来源：http://dxv.cucudq.cn

Ruby: PI = 3.14159
来源：http://veg.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://ihl.snrcjt.cn

[A04] 判断变量类型
来源：http://iqy.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://oid.snrcjt.cn


<!-- 参考信息 -->