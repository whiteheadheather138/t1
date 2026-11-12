代发 wailian999

[U43] PHP：声明命名空间
来源：http://uci.zhongyouzk.top

namespace App\Http;
来源：http://rcl.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://xuo.yuanzhike.top

declare(strict_types=1);
来源：http://itx.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://cvl.shuidangran.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uqe.hcnkem.com

[U46] PHP：可空类型
来源：http://nmg.chenlongwang.top

?string $name = null
来源：http://gsn.aizwys.cn

[U47] PHP：联合类型
来源：http://xvv.hfpthk.cn

int|string $id
来源：http://igg.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://fhq.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hla.yangfankeji.com

[U49] PHP：只读属性
来源：http://ecs.redwolf501.top

public readonly string $name
来源：http://rod.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://xhz.hcnkem.com

public function __construct(private int $id) {}
来源：http://okk.epnwcf.com

[U51] PHP：数组解构
来源：http://dbt.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://skf.guannengcc.top

[U52] PHP：箭头函数
来源：http://lwt.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://krw.0kj1m.cn

[U53] PHP：空合并运算符
来源：http://xfw.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://rik.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://zmc.ywan-chungtsiang.top

$obj?->method()
来源：http://ixv.andypj.xyz

[U55] PHP：match 表达式
来源：http://qfv.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jdi.cdnleiting.top

[U56] PHP：命名参数
来源：http://iyo.yanxiufei.cn

f(a: 1, b: 2)
来源：http://ile.yvedp.cn

[U57] PHP：字符串插值
来源：http://dep.cashguo.top

"值: {$a}"
来源：http://lso.jqgfzy.top

[U58] PHP：数组三件套
来源：http://ymn.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xjl.hysaishi.cn

[U59] PHP：自定义排序
来源：http://raj.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ugd.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://mts.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zqg.jqgufenzy.top

[U61] PHP：正则
来源：http://czr.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bou.sweek.top

[U62] PHP：日期对象
来源：http://rpv.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kcl.52xcode.cn

[U63] PHP：文件读写
来源：http://pgt.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jeb.xuanzx.com

[U64] PHP：目录遍历
来源：http://pup.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://odt.yonumen.top

[U65] PHP：会话
来源：http://ffw.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vrj.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://gcv.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gkj.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://dvu.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ynb.yfazqb.com

[U68] PHP：PDO 连接
来源：http://tyb.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://prr.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://dxs.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kmg.smart0.xyz

[U70] PHP：PDO 事务
来源：http://atf.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://otw.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://zfi.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://kwo.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://rkk.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://vqe.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://nmb.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://vyy.yonumen.top

[U74] PHP：读取环境变量
来源：http://rtk.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://yya.zycfv.cn

[U75] PHP：依赖注入
来源：http://olm.hfpthk.cn

composer require psr/container
来源：http://xpl.mhx1999.top

[U76] PHP：简单路由
来源：http://nqu.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://unv.epnwcf.com

[U77] PHP：模板渲染
来源：http://oat.ydjk.org.cn

composer require twig/twig
来源：http://uig.ydjk.org.cn

[U78] PHP：单元测试
来源：http://gcf.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://tir.quarkkingdee.top

[U79] PHP：静态分析
来源：http://hxg.tarul.cn

composer require --dev phpstan/phpstan
来源：http://rbm.pycfn.com

[U80] PHP：代码规范修复
来源：http://irz.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://onc.dashuyun.cn

[U81] JS：初始化项目
来源：http://qjw.yj20258.top

npm init -y;  npm i express
来源：http://gel.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://ioc.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wct.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://axg.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hbb.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://zpq.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://klv.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://rav.sjlbkw.cn

a?.b?.c
来源：http://svr.yj20258.top

[U86] JS：空值合并
来源：http://yly.smart0.xyz

a ?? b
来源：http://ffz.dashuyun.cn

[U87] JS：解构默认值
来源：http://jma.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://omt.pycfn.com

[U88] JS：对象展开合并
来源：http://fpl.mhx1999.top

{ ...a, ...b }
来源：http://zgd.hfpthk.cn

[U89] JS：数组去重
来源：http://odv.yj20258.top

[...new Set(arr)]
来源：http://gbg.sufxvd.cn

[U90] JS：数字数组排序
来源：http://dxn.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://hlk.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://blq.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qfv.ydzc1.top

[U92] JS：深拷贝
来源：http://suh.jqgfzy.top

structuredClone(obj)
来源：http://wrq.sweek.top

[U93] JS：模板字符串
来源：http://psh.yongpay.top

`共 ${n} 条`
来源：http://hrs.cheryme.top

[U94] JS：箭头函数
来源：http://gdm.cdnleiting.top

const double = x => x * 2;
来源：http://nns.xuanzx.com

[U95] JS：Promise 包装
来源：http://dqp.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://pja.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://bzz.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fzx.hesvh.cn

[U97] JS：并发请求
来源：http://tkl.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tnw.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://zal.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mlo.gzhubu.top

[U99] JS：事件监听
来源：http://gkr.nanxinkj.top

el.addEventListener("click", e => {})
来源：http://oft.tianlin.xyz

[U100] JS：DOM 查询
来源：http://eib.sxryk.cn

document.querySelector(".item")
来源：http://hqm.guowangkeji.top

[U101] JS：classList 操作
来源：http://wiu.nwbrower.top

el.classList.toggle("active")
来源：http://heq.jlsjyb.cn

[U102] JS：本地存储
来源：http://jrv.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wyg.aibaodan.cn

[U103] JS：定时器
来源：http://ljk.fzhhl.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://otz.hnxiangtu.top

[U104] JS：防抖
来源：http://ncj.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srb.9152youxi.cn

[U105] JS：节流
来源：http://jie.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fcb.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://iac.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uyq.chenlongwang.top

[U107] JS：数字千分位
来源：http://abp.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ggy.nanxuanxn.top

[U108] JS：随机整数
来源：http://csa.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://unl.ivvv.top

[U109] JS：数组分组
来源：http://eoc.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://fwm.yangfankeji.com

[U110] JS：数组分块
来源：http://hxw.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rkb.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://qcz.gzhubu.top

new Map(Object.entries(obj))
来源：http://pub.52xcode.cn

[U112] JS：字符串补位
来源：http://rgn.fktsv.cn

"7".padStart(3, "0")
来源：http://wpo.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://wmf.chenzaomai.com

s.replaceAll("a", "b")
来源：http://xxl.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://plb.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://phb.cqqwz.cn

[U115] JS：生成 UUID
来源：http://dzo.vqdsnc.cn

crypto.randomUUID()
来源：http://ype.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://abz.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://nrl.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://xru.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://wju.wangdashe.top

[U118] JS：开发服务器
来源：http://urj.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://omv.hywenlv.cn

[U119] JS：生产构建
来源：http://per.xinyue.icu

npx vite build
来源：http://gig.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://yjb.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://oez.jyoumei.cn

================================================================================
来源：http://mfl.hesvh.cn

统计汇总
来源：http://sju.zhoulong.xyz

================================================================================
来源：http://ykh.zhaomingkeji.xyz

按语言统计（条）：
来源：http://uia.dianchejie.cn

Python ......... 252
来源：http://ccz.meibo888.top

PHP ............ 252
来源：http://fsm.sufxvd.cn

JavaScript ..... 252
来源：http://nkp.yonumen.top

TypeScript ..... 212
来源：http://hcm.hysaishi.cn

Java ........... 212
来源：http://boy.shanyushiyangtech.top

Go ............. 212
来源：http://qhy.fehbvm.com

Ruby ........... 212
来源：http://ajn.hammf.cn

C# ............. 212
来源：http://xxx.yuxming.cn

C .............. 30
来源：http://jcr.hnqzz.top

C++ ............ 30
来源：http://azm.tanke756.top

SQL ............ 90
来源：http://cpk.shanyushiyangkeji.top

Bash ........... 80
来源：http://fsw.dianchejie.cn

Kotlin ......... 15
来源：http://ekn.hesvh.cn

Swift .......... 15
来源：http://ntr.aibaodan.cn

Lua ............ 10
来源：http://blr.andypj.xyz

Perl ........... 10
来源：http://ulx.nanxuanxn.top

Scala .......... 10
来源：http://wjz.shzxlz.cn

------------------------------------
来源：http://roj.fehbvm.com

合计 ........... 2106 条
来源：http://rng.zhixingplan.top

按章节统计：
来源：http://urn.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rhc.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bkx.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zwe.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://inb.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sxv.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eaq.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iib.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://njg.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ogk.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rhq.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ipn.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wpc.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://myc.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zsu.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bld.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sog.zdbjq.cn

Q SQL 专题                              90
来源：http://etv.wangdashe.top

R Bash 专题                             80
来源：http://eng.xuanzx.com

S C / C++ 专题                          60
来源：http://ltu.ydjk.org.cn

T 其他语言补充                          60
来源：http://wee.cdnleiting.top

U 高频实用片段                         120
来源：http://hbg.yj20258.top

------------------------------------
来源：http://lmj.jinghuilouyu.cn

合计                                  2106 条
来源：http://qrs.pycfn.com

--------------------------------------------------------------------------------
来源：http://tuz.sxryk.cn

使用提醒
来源：http://ycd.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ump.sufxvd.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ylo.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hpj.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hws.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jyf.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mlh.gogol.net.cn

—— 文件结束 ——
来源：http://nls.ydzc1.top

================================================================================
来源：http://xcn.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://pok.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://lba.fengsongda.top

================================================================================
来源：http://zha.hammf.cn

【收录内容】
来源：http://zem.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ase.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yia.tarul.cn

SQL · Bash · C · C++
来源：http://rbp.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zsc.52xcode.cn

【使用说明】
来源：http://njv.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ouh.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tgr.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wsb.yvedp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uar.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xpp.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iab.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bpe.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rno.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ccd.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cqd.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://agn.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zlq.ywan-chungtsiang.top

【文件统计】
来源：http://eqh.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iyo.havefunace.top

--------------------------------------------------------------------------------
来源：http://jrt.vqdsnc.cn

目  录
来源：http://mxe.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://hzl.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qon.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://emz.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://axu.dashuyun.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://obu.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lcu.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kah.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zla.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rux.andypj.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vvm.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://omz.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://svy.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rml.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mvm.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dig.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pde.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ccu.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fdw.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kvb.hnqzz.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mbc.ctjpmb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://upd.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zgd.uphjek.com

================================================================================
来源：http://piu.pycfn.com

A. 基础语法与类型
来源：http://hzm.daria6918.cn

================================================================================
来源：http://fgq.jqgfzy.top

[A01] Hello World
来源：http://sxv.zhengqikj.top

Py:   print("Hello, World!")
来源：http://ihe.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://yqw.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://mdw.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fgx.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://wqv.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://zcu.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://ufw.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://dbi.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://xcd.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://obu.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://amd.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pdq.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fbd.jinghuilouyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://tgi.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://xzw.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://lip.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dmj.vehdjk.com

[A03] 常量定义
来源：http://oiv.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://idq.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://ogu.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://urf.yj202588.top

TS:   const PI: number = 3.14159;
来源：http://cld.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://rty.tian-w.cn

Go:   const PI = 3.14159
来源：http://soo.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://kye.shzxlz.cn

C#:   const double PI = 3.14159;
来源：http://ikx.ctjpmb.com

[A04] 判断变量类型
来源：http://ukv.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://jki.havefunace.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wlx.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://obz.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://jsl.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jaq.c1oappe.top

Go:   reflect.TypeOf(x).Name()
来源：http://dnd.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hmh.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://wdo.zhiwuduotai.top

[A05] 整数除法与取模
来源：http://gxd.cqqwz.cn


<!-- 参考信息 -->