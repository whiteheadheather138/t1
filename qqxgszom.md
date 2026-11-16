代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://khk.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kwi.gotoacloud.top

[U46] PHP：可空类型
来源：http://dog.jqgfzy.top

?string $name = null
来源：http://uvn.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://yuf.svipenyu.cn

int|string $id
来源：http://rwo.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://hbf.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mst.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://vou.xinyue.icu

public readonly string $name
来源：http://shf.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://kho.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://npq.yj20258888.top

[U51] PHP：数组解构
来源：http://rtk.ivvv.top

[$a, $b] = $arr;
来源：http://diy.guannengcc.top

[U52] PHP：箭头函数
来源：http://mud.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://iom.shuidangran.top

[U53] PHP：空合并运算符
来源：http://sji.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://iad.fktsv.cn

[U54] PHP：空安全调用
来源：http://gjj.zhijiandao.cn

$obj?->method()
来源：http://pne.uphjek.com

[U55] PHP：match 表达式
来源：http://fcy.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dxj.gogol.net.cn

[U56] PHP：命名参数
来源：http://qdw.vqdsnc.cn

f(a: 1, b: 2)
来源：http://mux.smart0.xyz

[U57] PHP：字符串插值
来源：http://pgc.chenjidiqi.icu

"值: {$a}"
来源：http://tbu.chenlongwang.top

[U58] PHP：数组三件套
来源：http://yxd.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kav.tanke756.top

[U59] PHP：自定义排序
来源：http://vku.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ivj.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://csk.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wls.quarkkingdee.top

[U61] PHP：正则
来源：http://tge.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://knr.hywenlv.cn

[U62] PHP：日期对象
来源：http://qbk.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nvo.tianlin.xyz

[U63] PHP：文件读写
来源：http://zfs.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ulh.sxryk.cn

[U64] PHP：目录遍历
来源：http://lam.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://chr.zycfv.cn

[U65] PHP：会话
来源：http://efh.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bnf.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://cwy.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zuz.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://lbg.ctjpmb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugg.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://bjj.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ycv.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://ose.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oit.tarul.cn

[U70] PHP：PDO 事务
来源：http://hfn.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gcp.daria6918.cn

[U71] PHP：抛出异常
来源：http://roz.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://ino.cashguo.top

[U72] PHP：写错误日志
来源：http://wql.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://dkt.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://wna.havefunace.top

parse_ini_file("config.ini", true)
来源：http://bqn.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://qqq.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://ufn.dashuyun.cn

[U75] PHP：依赖注入
来源：http://orv.ctjpmb.com

composer require psr/container
来源：http://ndg.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://iqu.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jmt.hfpthk.cn

[U77] PHP：模板渲染
来源：http://xyl.daria6918.cn

composer require twig/twig
来源：http://xmf.ydjk.org.cn

[U78] PHP：单元测试
来源：http://icf.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://vdk.jianghu66.top

[U79] PHP：静态分析
来源：http://bfd.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://ndx.yj20258888.top

[U80] PHP：代码规范修复
来源：http://knz.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://txr.gogol.net.cn

[U81] JS：初始化项目
来源：http://ikr.tarul.cn

npm init -y;  npm i express
来源：http://csp.xziqi.cn

[U82] JS：package.json 脚本
来源：http://ouh.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fod.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://ajr.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wuk.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://dgf.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://gcp.uphjek.com

[U85] JS：可选链
来源：http://jst.jlsjyb.cn

a?.b?.c
来源：http://mos.52xcode.cn

[U86] JS：空值合并
来源：http://tdb.feifeiyinyue.top

a ?? b
来源：http://hbg.shuidangran.top

[U87] JS：解构默认值
来源：http://tsx.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://aqq.epnwcf.com

[U88] JS：对象展开合并
来源：http://hez.hcnkem.com

{ ...a, ...b }
来源：http://gmf.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://wpd.bbcook.cn

[...new Set(arr)]
来源：http://iod.c1oappe.top

[U90] JS：数字数组排序
来源：http://qpc.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://poc.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://vew.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ito.zhijiandao.cn

[U92] JS：深拷贝
来源：http://vay.tarul.cn

structuredClone(obj)
来源：http://vnl.fengsongda.top

[U93] JS：模板字符串
来源：http://vfq.nwbrower.top

`共 ${n} 条`
来源：http://wli.pycfn.com

[U94] JS：箭头函数
来源：http://wof.daria6918.cn

const double = x => x * 2;
来源：http://vwp.yongpay.top

[U95] JS：Promise 包装
来源：http://pqj.cashguo.top

new Promise((resolve, reject) => {})
来源：http://gom.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://mdw.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xiw.quarkkingdee.top

[U97] JS：并发请求
来源：http://bzf.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fza.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://seq.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iuo.zhijiandao.cn

[U99] JS：事件监听
来源：http://lej.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://svh.cqqwz.cn

[U100] JS：DOM 查询
来源：http://ndl.zhixingplan.top

document.querySelector(".item")
来源：http://wxr.redwolf501.top

[U101] JS：classList 操作
来源：http://alr.ivvv.top

el.classList.toggle("active")
来源：http://yvv.cdnleiting.top

[U102] JS：本地存储
来源：http://lzi.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hdv.yj202588.top

[U103] JS：定时器
来源：http://pku.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wwh.zycfv.cn

[U104] JS：防抖
来源：http://ojl.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ivs.jinqigfzy.top

[U105] JS：节流
来源：http://yrb.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dgi.cashguo.top

[U106] JS：日期格式化
来源：http://gqy.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nbj.gaohongyu789.top

[U107] JS：数字千分位
来源：http://suj.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://msm.bbcook.cn

[U108] JS：随机整数
来源：http://krb.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csh.kuanghao11.cn

[U109] JS：数组分组
来源：http://fyq.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://esb.gotoacloud.top

[U110] JS：数组分块
来源：http://xla.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jha.mhx1999.top

[U111] JS：对象转 Map
来源：http://ril.hywenlv.cn

new Map(Object.entries(obj))
来源：http://qcj.hnqzz.top

[U112] JS：字符串补位
来源：http://dde.zycfv.cn

"7".padStart(3, "0")
来源：http://wwy.epnwcf.com

[U113] JS：正则替换全部
来源：http://ycf.chenzaomai.com

s.replaceAll("a", "b")
来源：http://pwn.uphjek.com

[U114] JS：JSON 深比较
来源：http://fev.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wps.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://kol.quarkkingdee.top

crypto.randomUUID()
来源：http://etn.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://sob.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://cxm.sysykeji.top

[U117] JS：单元测试
来源：http://vvb.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://vye.dianchejie.cn

[U118] JS：开发服务器
来源：http://pvz.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://pdj.mhx1999.top

[U119] JS：生产构建
来源：http://uvw.meibo888.top

npx vite build
来源：http://mud.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://csg.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://awa.sxryk.cn

================================================================================
来源：http://tcm.tian-w.cn

统计汇总
来源：http://agj.zhaomingkeji.xyz

================================================================================
来源：http://nqd.ctjpmb.com

按语言统计（条）：
来源：http://ixa.xuanzx.com

Python ......... 252
来源：http://ksx.sjlbkw.cn

PHP ............ 252
来源：http://jdc.quarkkingdee.top

JavaScript ..... 252
来源：http://tls.nwbrower.top

TypeScript ..... 212
来源：http://zcp.zhixingplan.top

Java ........... 212
来源：http://oxs.9152youxi.cn

Go ............. 212
来源：http://tta.shanyushiyangkeji.top

Ruby ........... 212
来源：http://vvz.nwbrower.top

C# ............. 212
来源：http://fht.hongshengwenyu.top

C .............. 30
来源：http://mte.gaohongyu789.top

C++ ............ 30
来源：http://pqr.meibo888.top

SQL ............ 90
来源：http://suh.sweek.top

Bash ........... 80
来源：http://wal.wangshuangyany.cn

Kotlin ......... 15
来源：http://tat.jyoumei.cn

Swift .......... 15
来源：http://dke.jqgufenzy.top

Lua ............ 10
来源：http://uyo.yanxiufei.cn

Perl ........... 10
来源：http://akg.fengsongda.top

Scala .......... 10
来源：http://fwb.meibo888.top

------------------------------------
来源：http://gni.kuanghao11.cn

合计 ........... 2106 条
来源：http://ted.ctjpmb.com

按章节统计：
来源：http://nuq.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vyk.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://alc.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jjq.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tdp.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qde.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ybl.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://njl.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mqm.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zer.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bvd.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fqa.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hvm.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nbp.sysykeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cce.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fws.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kmy.kuanghao11.cn

Q SQL 专题                              90
来源：http://ich.cdnleiting.top

R Bash 专题                             80
来源：http://vhq.yuanzhike.top

S C / C++ 专题                          60
来源：http://rau.hnqzz.top

T 其他语言补充                          60
来源：http://pow.yonumen.top

U 高频实用片段                         120
来源：http://svq.snrcjt.cn

------------------------------------
来源：http://wha.zdqjudy.top

合计                                  2106 条
来源：http://jfi.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://whm.andypj.xyz

使用提醒
来源：http://nkl.zycfv.cn

--------------------------------------------------------------------------------
来源：http://jgw.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rwq.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uhk.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gew.xuanzx.com

在旧版本上使用前请先确认语法支持情况。
来源：http://pax.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jdu.sysykeji.top

—— 文件结束 ——
来源：http://iag.fengsongda.top

================================================================================
来源：http://sgr.cqqwz.cn

程序语言常见例子速查手册（2024 版）
来源：http://jhs.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://ijr.zhijiandao.cn

================================================================================
来源：http://men.zhoulong.xyz

【收录内容】
来源：http://lix.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fxo.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://riw.hywenlv.cn

SQL · Bash · C · C++
来源：http://xti.tianlin.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qxi.feifeiyinyue.top

【使用说明】
来源：http://gtj.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yis.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wde.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://efb.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mzv.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://msa.yvedp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nhv.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pid.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tsj.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hqt.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fap.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rkd.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ual.feifeiyinyue.top

【文件统计】
来源：http://rqn.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zcl.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://hmv.zhengqikj.top

目  录
来源：http://ckj.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://gnc.gotoacloud.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ihp.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gnt.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uzd.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jmy.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://twl.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bpa.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vjf.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zjz.yj202588.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ehb.xylfe.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://phy.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dkf.pengpengdd.cyou

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zmx.zhoulong.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uhi.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qxb.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tpp.ydjk.org.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sdm.zhixingplan.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kzb.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://seq.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vhv.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://riv.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mya.xingfuxueyuan.xyz

================================================================================
来源：http://wuq.kuanghao11.cn

A. 基础语法与类型
来源：http://qtb.zdbjq.cn

================================================================================
来源：http://kyk.smart0.xyz

[A01] Hello World
来源：http://tel.birdmap.top

Py:   print("Hello, World!")
来源：http://jqn.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://abg.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://wet.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qyu.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://gwb.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://qst.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://gvw.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ypq.jianghu66.top

[A02] 变量声明与赋值
来源：http://weg.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ejw.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://poo.chenzaomai.com

JS:   let name = "Alex"; const age = 20;
来源：http://bfd.shanyushiyangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sla.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ymw.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://osc.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://atm.ydjk.org.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jxm.guannengcc.top

[A03] 常量定义
来源：http://dkh.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dcc.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://oyh.shuidangran.top

JS:   const PI = 3.14159;
来源：http://byr.nwbrower.top

TS:   const PI: number = 3.14159;
来源：http://oze.316326.xyz

Java: static final double PI = 3.14159;
来源：http://wad.yfazqb.com

Go:   const PI = 3.14159
来源：http://wff.chenzaomai.com

Ruby: PI = 3.14159
来源：http://rwi.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://sad.guannengcc.top

[A04] 判断变量类型
来源：http://xpb.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ijf.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ooh.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ihv.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://anw.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jlv.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://dbl.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iic.epnwcf.com

C#:   x.GetType().Name; x is int
来源：http://pxm.xylfe.cn

[A05] 整数除法与取模
来源：http://ahr.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tvu.9152youxi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sqh.nwbrower.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gsn.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://piu.iojbl.cn


<!-- 参考信息 -->