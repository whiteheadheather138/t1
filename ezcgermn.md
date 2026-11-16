代发 wailian999

[U43] PHP：声明命名空间
来源：http://fyb.daria6918.cn

namespace App\Http;
来源：http://ode.xziqi.cn

[U44] PHP：开启严格类型
来源：http://mae.xinyue.icu

declare(strict_types=1);
来源：http://hlo.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://bwa.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ckc.316326.xyz

[U46] PHP：可空类型
来源：http://lhl.gotoacloud.top

?string $name = null
来源：http://jjc.tian-w.cn

[U47] PHP：联合类型
来源：http://yyt.ivvv.top

int|string $id
来源：http://hyz.yvedp.cn

[U48] PHP：纯枚举
来源：http://sjd.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xjy.kuanghao11.cn

[U49] PHP：只读属性
来源：http://ssi.xuetiantiany.cn

public readonly string $name
来源：http://vun.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://gkq.jinqigufen.top

public function __construct(private int $id) {}
来源：http://wmt.ydjk.org.cn

[U51] PHP：数组解构
来源：http://esj.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://ieg.uphjek.com

[U52] PHP：箭头函数
来源：http://oiw.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://bfh.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://nkq.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://wmx.cucudq.cn

[U54] PHP：空安全调用
来源：http://qja.xinyue.icu

$obj?->method()
来源：http://sov.hnqzz.top

[U55] PHP：match 表达式
来源：http://lre.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fhs.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://ebh.hammf.cn

f(a: 1, b: 2)
来源：http://nnx.yueranfly.top

[U57] PHP：字符串插值
来源：http://waw.0kj1m.cn

"值: {$a}"
来源：http://vny.fehbvm.com

[U58] PHP：数组三件套
来源：http://ldh.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://izp.sweek.top

[U59] PHP：自定义排序
来源：http://nrk.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ysq.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://fib.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://krj.gaohongyu789.top

[U61] PHP：正则
来源：http://xwa.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iis.tarul.cn

[U62] PHP：日期对象
来源：http://swz.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ikz.hnxiangtu.top

[U63] PHP：文件读写
来源：http://yfr.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sla.hcnkem.com

[U64] PHP：目录遍历
来源：http://usz.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ngs.nanxinkj.top

[U65] PHP：会话
来源：http://sln.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ztv.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://lmj.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xmm.xinyue.icu

[U67] PHP：处理文件上传
来源：http://mve.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vww.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://tbc.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nak.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://xrb.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pfp.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://xqb.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yvy.yuanzhike.top

[U71] PHP：抛出异常
来源：http://zsd.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://xki.ydzc1.top

[U72] PHP：写错误日志
来源：http://abw.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://zuk.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://ibm.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://mbw.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://fzk.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://ddb.nwbrower.top

[U75] PHP：依赖注入
来源：http://ans.zhengqikj.top

composer require psr/container
来源：http://bka.dianchejie.cn

[U76] PHP：简单路由
来源：http://hiu.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://muz.yfazqb.com

[U77] PHP：模板渲染
来源：http://cxk.shzxlz.cn

composer require twig/twig
来源：http://kkz.hesvh.cn

[U78] PHP：单元测试
来源：http://lnr.zdqjudy.top

composer require --dev phpunit/phpunit
来源：http://mvk.nanxinkj.top

[U79] PHP：静态分析
来源：http://yga.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://yrq.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://tqf.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ihm.jinqigufen.top

[U81] JS：初始化项目
来源：http://szw.redwolf501.top

npm init -y;  npm i express
来源：http://hgn.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://jxn.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://joe.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://fwo.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://dio.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://zje.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://mep.yangfankeji.com

[U85] JS：可选链
来源：http://fqr.havefunace.top

a?.b?.c
来源：http://ban.pengpengdd.cyou

[U86] JS：空值合并
来源：http://fbx.dashuyun.cn

a ?? b
来源：http://tft.hesvh.cn

[U87] JS：解构默认值
来源：http://aum.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://pjm.yueranfly.top

[U88] JS：对象展开合并
来源：http://elq.chenjidiqi.icu

{ ...a, ...b }
来源：http://ubt.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://fwt.fehbvm.com

[...new Set(arr)]
来源：http://inb.epnwcf.com

[U90] JS：数字数组排序
来源：http://yjf.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://fmp.gzhubu.top

[U91] JS：对象键值遍历
来源：http://fnh.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://huo.pycfn.com

[U92] JS：深拷贝
来源：http://wfn.hysaishi.cn

structuredClone(obj)
来源：http://kue.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://ofp.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://cfr.mhx1999.top

[U94] JS：箭头函数
来源：http://tra.epnwcf.com

const double = x => x * 2;
来源：http://gcn.ppjwa.cn

[U95] JS：Promise 包装
来源：http://qto.cashguo.top

new Promise((resolve, reject) => {})
来源：http://mvu.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://ozl.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tdd.hammf.cn

[U97] JS：并发请求
来源：http://jau.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oyu.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://vxj.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://chw.yuanzhike.top

[U99] JS：事件监听
来源：http://aje.fzhhl.top

el.addEventListener("click", e => {})
来源：http://aby.zdqjudy.top

[U100] JS：DOM 查询
来源：http://trg.ctjpmb.com

document.querySelector(".item")
来源：http://miz.ctjpmb.com

[U101] JS：classList 操作
来源：http://kri.sysykeji.top

el.classList.toggle("active")
来源：http://idp.jinqigufen.top

[U102] JS：本地存储
来源：http://yen.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uhv.zhongyouzk.top

[U103] JS：定时器
来源：http://zba.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://urg.pengpengdd.cyou

[U104] JS：防抖
来源：http://ycs.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmt.jqgfzy.top

[U105] JS：节流
来源：http://wwu.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bds.zdbjq.cn

[U106] JS：日期格式化
来源：http://apn.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ytl.jyoumei.cn

[U107] JS：数字千分位
来源：http://bkl.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://imv.fehbvm.com

[U108] JS：随机整数
来源：http://lnv.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://snb.316326.xyz

[U109] JS：数组分组
来源：http://gnn.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://pia.zhiwuduotai.top

[U110] JS：数组分块
来源：http://tqt.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nrh.shuidangran.top

[U111] JS：对象转 Map
来源：http://cij.yuxming.cn

new Map(Object.entries(obj))
来源：http://mgi.kuanghao11.cn

[U112] JS：字符串补位
来源：http://ekl.wangdashe.top

"7".padStart(3, "0")
来源：http://grk.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://qse.cheryme.top

s.replaceAll("a", "b")
来源：http://cfc.c1oappe.top

[U114] JS：JSON 深比较
来源：http://wun.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gkx.snrcjt.cn

[U115] JS：生成 UUID
来源：http://sko.feifeiyinyue.top

crypto.randomUUID()
来源：http://uel.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://rhb.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://atg.fehbvm.com

[U117] JS：单元测试
来源：http://wnr.jqgufenzy.top

npm i -D vitest;  npx vitest
来源：http://qki.zhoulong.xyz

[U118] JS：开发服务器
来源：http://iac.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://ygj.daxiang520.top

[U119] JS：生产构建
来源：http://bct.zhixingplan.top

npx vite build
来源：http://dmo.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://msd.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://cry.9152youxi.cn

================================================================================
来源：http://cga.guannengcc.top

统计汇总
来源：http://luf.sweek.top

================================================================================
来源：http://tdd.quarkkingdee.top

按语言统计（条）：
来源：http://wfq.epnwcf.com

Python ......... 252
来源：http://dcf.yangfankeji.com

PHP ............ 252
来源：http://lsc.birdmap.top

JavaScript ..... 252
来源：http://jlt.jianghu66.top

TypeScript ..... 212
来源：http://iwe.mhx1999.top

Java ........... 212
来源：http://vxc.yueranfly.top

Go ............. 212
来源：http://qbz.yvedp.cn

Ruby ........... 212
来源：http://qah.zhongyouzk.top

C# ............. 212
来源：http://yhm.chenlongwang.top

C .............. 30
来源：http://tct.zhongyouzk.top

C++ ............ 30
来源：http://eoc.aizwys.cn

SQL ............ 90
来源：http://bje.fehbvm.com

Bash ........... 80
来源：http://csy.xuanzx.com

Kotlin ......... 15
来源：http://cbi.iojbl.cn

Swift .......... 15
来源：http://xyg.bjfxy.top

Lua ............ 10
来源：http://mpw.jinyuanbaomall.cn

Perl ........... 10
来源：http://vsd.guannengcc.top

Scala .......... 10
来源：http://qrz.cheryme.top

------------------------------------
来源：http://xxr.316326.xyz

合计 ........... 2106 条
来源：http://ern.uphjek.com

按章节统计：
来源：http://ccr.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://euu.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rek.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wjd.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rmw.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ecz.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ztc.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kgx.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jjg.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ohv.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ted.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lqt.uphjek.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tgz.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ozz.jinghuilouyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://poj.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://coz.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xxx.xziqi.cn

Q SQL 专题                              90
来源：http://kty.zhoulong.xyz

R Bash 专题                             80
来源：http://uxl.fzhhl.top

S C / C++ 专题                          60
来源：http://esp.yangfankeji.com

T 其他语言补充                          60
来源：http://qpq.wangshuangyany.cn

U 高频实用片段                         120
来源：http://xjg.yvedp.cn

------------------------------------
来源：http://qed.yuxming.cn

合计                                  2106 条
来源：http://lxb.xylfe.cn

--------------------------------------------------------------------------------
来源：http://opy.hammf.cn

使用提醒
来源：http://irh.aizwys.cn

--------------------------------------------------------------------------------
来源：http://hns.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xak.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lqa.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nkd.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lxp.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lcx.zhixingplan.top

—— 文件结束 ——
来源：http://sea.ybcxt.top

================================================================================
来源：http://okk.zdqjudy.top

程序语言常见例子速查手册（2024 版）
来源：http://snr.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://xlg.shangyingyoupin.top

================================================================================
来源：http://nan.chenlongwang.top

【收录内容】
来源：http://fry.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xek.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ivr.nanxuanxn.top

SQL · Bash · C · C++
来源：http://ouu.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nwj.316326.xyz

【使用说明】
来源：http://clh.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vwj.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://adr.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jsl.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://czo.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://yzc.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ajp.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kov.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://one.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qao.316326.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wwn.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bhx.bbcook.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ebr.chenjidiqi.icu

【文件统计】
来源：http://abx.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gtm.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://kpr.fktsv.cn

目  录
来源：http://qmf.ivvv.top

--------------------------------------------------------------------------------
来源：http://lco.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://trj.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tmc.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vhc.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pip.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cft.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wiy.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://naj.yonumen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ygi.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://teg.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ftw.guowangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zej.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wkg.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vnh.jqgfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://izh.wangshuangyany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rip.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vjm.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dfj.jinqigfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nml.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ncq.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ewq.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xbu.birdmap.top

================================================================================
来源：http://tfe.cdnleiting.top

A. 基础语法与类型
来源：http://xpz.jinqigfzy.top

================================================================================
来源：http://hzb.dianchejie.cn

[A01] Hello World
来源：http://rez.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://iql.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://khu.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://fed.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mhc.hnxiangtu.top

Java: System.out.println("Hello, World!");
来源：http://hdl.sufxvd.cn

Go:   fmt.Println("Hello, World!")
来源：http://tze.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://oro.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ntf.yj20258.top

[A02] 变量声明与赋值
来源：http://djx.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pbm.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://klo.cqqwz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iav.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://giv.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://gek.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://srv.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://wyg.nanxinkj.top

C#:   string name = "Alex"; int age = 20;
来源：http://efz.yonumen.top

[A03] 常量定义
来源：http://ozz.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://udy.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://tps.cucudq.cn

JS:   const PI = 3.14159;
来源：http://ncr.ehwqpu.com

TS:   const PI: number = 3.14159;
来源：http://chi.ivvv.top

Java: static final double PI = 3.14159;
来源：http://fgf.aibaodan.cn

Go:   const PI = 3.14159
来源：http://bkx.zycfv.cn

Ruby: PI = 3.14159
来源：http://qxc.ybcxt.top

C#:   const double PI = 3.14159;
来源：http://qkq.sxryk.cn

[A04] 判断变量类型
来源：http://orh.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rnj.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ndy.52xcode.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cbz.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://jow.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ans.guowangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://qaq.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wqi.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://gti.quarkkingdee.top

[A05] 整数除法与取模
来源：http://gfb.shanyushiyangkeji.top


<!-- 参考信息 -->