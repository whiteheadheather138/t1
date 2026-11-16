代发 wailian999

[U49] PHP：只读属性
来源：http://vya.hnxiangtu.top

public readonly string $name
来源：http://kgm.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://afy.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://pxv.vehdjk.com

[U51] PHP：数组解构
来源：http://pys.iojbl.cn

[$a, $b] = $arr;
来源：http://qip.jiagoushi.top

[U52] PHP：箭头函数
来源：http://vnw.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://cmj.mhx1999.top

[U53] PHP：空合并运算符
来源：http://iow.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://hyg.wangdashe.top

[U54] PHP：空安全调用
来源：http://ogt.hcnkem.com

$obj?->method()
来源：http://wyr.fengsongda.top

[U55] PHP：match 表达式
来源：http://blz.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fdo.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://erv.jianghu66.top

f(a: 1, b: 2)
来源：http://ukm.ppjwa.cn

[U57] PHP：字符串插值
来源：http://sqp.meibo888.top

"值: {$a}"
来源：http://klu.sxryk.cn

[U58] PHP：数组三件套
来源：http://xkn.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xkw.fktsv.cn

[U59] PHP：自定义排序
来源：http://qhh.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hhd.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://ybi.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wkb.hywenlv.cn

[U61] PHP：正则
来源：http://vyz.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jzl.ppjwa.cn

[U62] PHP：日期对象
来源：http://hic.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hlt.nanxuanxn.top

[U63] PHP：文件读写
来源：http://adg.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://epv.yuanzhike.top

[U64] PHP：目录遍历
来源：http://btt.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://cnw.ehwqpu.com

[U65] PHP：会话
来源：http://mak.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qoh.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://tgp.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nkx.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://sdo.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ulq.zycfv.cn

[U68] PHP：PDO 连接
来源：http://slv.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vou.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://nsd.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wsr.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://tjr.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bzz.dashuyun.cn

[U71] PHP：抛出异常
来源：http://syy.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://gho.jqgfzy.top

[U72] PHP：写错误日志
来源：http://xdh.cheryme.top

error_log("失败: " . $e->getMessage());
来源：http://ufo.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://uxb.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://ylp.yj20258.top

[U74] PHP：读取环境变量
来源：http://fkn.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://ypg.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://lvg.nwbrower.top

composer require psr/container
来源：http://lml.ydzc1.top

[U76] PHP：简单路由
来源：http://uzl.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://swn.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://ewr.jiagoushi.top

composer require twig/twig
来源：http://bdt.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://gug.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://qgw.gaohongyu789.top

[U79] PHP：静态分析
来源：http://hvd.ivvv.top

composer require --dev phpstan/phpstan
来源：http://dwn.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://gsi.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://dfz.redwolf501.top

[U81] JS：初始化项目
来源：http://bae.jlsjyb.cn

npm init -y;  npm i express
来源：http://xjf.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://fvg.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://got.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://qaa.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://udq.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://ibu.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://eob.yueranfly.top

[U85] JS：可选链
来源：http://oio.yangfankeji.com

a?.b?.c
来源：http://tsk.gzhubu.top

[U86] JS：空值合并
来源：http://bmo.aibaodan.cn

a ?? b
来源：http://ytv.ctjpmb.com

[U87] JS：解构默认值
来源：http://dhe.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://qre.daria6918.cn

[U88] JS：对象展开合并
来源：http://rtm.ctjpmb.com

{ ...a, ...b }
来源：http://whv.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://qxx.gzhubu.top

[...new Set(arr)]
来源：http://vnr.hnqzz.top

[U90] JS：数字数组排序
来源：http://kxp.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://rur.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://pkw.shuidangran.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iiv.yueranfly.top

[U92] JS：深拷贝
来源：http://bat.sufxvd.cn

structuredClone(obj)
来源：http://jdp.dianchejie.cn

[U93] JS：模板字符串
来源：http://mnz.kuanghao11.cn

`共 ${n} 条`
来源：http://lzh.cucudq.cn

[U94] JS：箭头函数
来源：http://ygi.ydjk.org.cn

const double = x => x * 2;
来源：http://sow.jinqigufen.top

[U95] JS：Promise 包装
来源：http://ors.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://mwg.cucudq.cn

[U96] JS：async/await 与异常
来源：http://lby.yuanzhike.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jgq.dashuyun.cn

[U97] JS：并发请求
来源：http://ffj.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xhz.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://bss.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hzs.yonumen.top

[U99] JS：事件监听
来源：http://fmu.nwbrower.top

el.addEventListener("click", e => {})
来源：http://lds.haohaochexian.top

[U100] JS：DOM 查询
来源：http://hzb.xuanzx.com

document.querySelector(".item")
来源：http://wqe.haohaochexian.top

[U101] JS：classList 操作
来源：http://oar.sjlbkw.cn

el.classList.toggle("active")
来源：http://mmx.yuanzhike.top

[U102] JS：本地存储
来源：http://lsi.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ejg.jqgufenzy.top

[U103] JS：定时器
来源：http://xwu.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zqn.smart0.xyz

[U104] JS：防抖
来源：http://upw.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hox.sysykeji.top

[U105] JS：节流
来源：http://omk.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xei.hammf.cn

[U106] JS：日期格式化
来源：http://amt.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ape.jinqigfzy.top

[U107] JS：数字千分位
来源：http://gnt.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mbk.sysykeji.top

[U108] JS：随机整数
来源：http://dyr.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vsh.vehdjk.com

[U109] JS：数组分组
来源：http://zhr.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://pbj.hfpthk.cn

[U110] JS：数组分块
来源：http://fzt.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://odf.hfpthk.cn

[U111] JS：对象转 Map
来源：http://smi.iojbl.cn

new Map(Object.entries(obj))
来源：http://qou.guowangkeji.top

[U112] JS：字符串补位
来源：http://lfh.tarul.cn

"7".padStart(3, "0")
来源：http://wuk.hesvh.cn

[U113] JS：正则替换全部
来源：http://fai.yvedp.cn

s.replaceAll("a", "b")
来源：http://vun.yueranfly.top

[U114] JS：JSON 深比较
来源：http://vkv.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xca.ehwqpu.com

[U115] JS：生成 UUID
来源：http://xdk.shuidangran.top

crypto.randomUUID()
来源：http://jti.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://ttp.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://lyd.sxryk.cn

[U117] JS：单元测试
来源：http://cvz.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://enj.jinqigfzy.top

[U118] JS：开发服务器
来源：http://wak.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://ynn.yj20258888.top

[U119] JS：生产构建
来源：http://rsh.vqdsnc.cn

npx vite build
来源：http://wdo.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://mdp.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://xld.hywenlv.cn

================================================================================
来源：http://oxq.fehbvm.com

统计汇总
来源：http://nmi.cqqwz.cn

================================================================================
来源：http://srl.tanke756.top

按语言统计（条）：
来源：http://tyo.ywan-chungtsiang.top

Python ......... 252
来源：http://xhm.xylfe.cn

PHP ............ 252
来源：http://yes.jyoumei.cn

JavaScript ..... 252
来源：http://zss.yongpay.top

TypeScript ..... 212
来源：http://vbi.316326.xyz

Java ........... 212
来源：http://wfp.nwbrower.top

Go ............. 212
来源：http://hpl.gaohongyu789.top

Ruby ........... 212
来源：http://lzx.cheryme.top

C# ............. 212
来源：http://rap.quarkkingdee.top

C .............. 30
来源：http://xus.xuanzx.com

C++ ............ 30
来源：http://lgt.cdnleiting.top

SQL ............ 90
来源：http://bcg.daxiang520.top

Bash ........... 80
来源：http://iub.ydjk.org.cn

Kotlin ......... 15
来源：http://lxl.zhongyouzk.top

Swift .......... 15
来源：http://kwt.ywan-chungtsiang.top

Lua ............ 10
来源：http://fex.9152youxi.cn

Perl ........... 10
来源：http://igj.chenzaomai.com

Scala .......... 10
来源：http://wuc.meibo888.top

------------------------------------
来源：http://ngq.tianlin.xyz

合计 ........... 2106 条
来源：http://oir.fktsv.cn

按章节统计：
来源：http://iry.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rce.bbcook.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lhb.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jyf.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://akc.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://npw.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nvy.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xpd.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xbf.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pca.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://utp.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://etp.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vxn.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bck.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kyw.pycfn.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://llw.zhengqikj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bij.zhengqikj.top

Q SQL 专题                              90
来源：http://hco.meibo888.top

R Bash 专题                             80
来源：http://mzw.52xcode.cn

S C / C++ 专题                          60
来源：http://ydv.tarul.cn

T 其他语言补充                          60
来源：http://dqj.tanke756.top

U 高频实用片段                         120
来源：http://aec.fengsongda.top

------------------------------------
来源：http://ufa.cucudq.cn

合计                                  2106 条
来源：http://wmg.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://dyo.shuidangran.top

使用提醒
来源：http://oce.cashguo.top

--------------------------------------------------------------------------------
来源：http://num.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wnn.xinyue.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qih.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dya.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://nmm.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://shc.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://jzq.yvedp.cn

================================================================================
来源：http://ojr.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://fbx.fehbvm.com

Common Programming Examples Cheat Book
来源：http://tcc.nanxinkj.top

================================================================================
来源：http://bdq.c1oappe.top

【收录内容】
来源：http://vvu.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ung.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ees.hcnkem.com

SQL · Bash · C · C++
来源：http://fnf.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ccd.zhengqikj.top

【使用说明】
来源：http://pqr.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gmu.shanyushiyangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fzp.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uir.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zkw.nwbrower.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uwd.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hwe.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://iom.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ybq.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oes.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qvk.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ute.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wkt.chenzaomai.com

【文件统计】
来源：http://sic.pycfn.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bda.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://sgd.cucudq.cn

目  录
来源：http://mpk.hesvh.cn

--------------------------------------------------------------------------------
来源：http://wcl.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zso.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://twb.zycfv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wrv.tianlin.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iyh.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sgl.xuanzx.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nzt.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://utp.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aqe.sufxvd.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bih.wangdashe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ctz.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://niw.shzxlz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qcg.sjlbkw.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dgw.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qka.ctjpmb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hdm.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uvg.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ojb.jinqigufen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qvj.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cvj.pengpengdd.cyou

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vgg.shangyingyoupin.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yae.ywan-chungtsiang.top

================================================================================
来源：http://nds.ivvv.top

A. 基础语法与类型
来源：http://dgo.zhiwuduotai.top

================================================================================
来源：http://grx.hnqzz.top

[A01] Hello World
来源：http://hys.jyoumei.cn

Py:   print("Hello, World!")
来源：http://gwb.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://fhx.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://khd.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uck.yvedp.cn

Java: System.out.println("Hello, World!");
来源：http://fdm.fzhhl.top

Go:   fmt.Println("Hello, World!")
来源：http://vxs.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://jpd.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://but.c1oappe.top

[A02] 变量声明与赋值
来源：http://rqh.chenzaomai.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ldx.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kdn.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dck.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://luq.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://vgf.yvedp.cn

Go:   name := "Alex"; age := 20
来源：http://cys.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://aij.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://czx.ybcxt.top

[A03] 常量定义
来源：http://xsz.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cld.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://nje.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://ixn.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://rdy.meibo888.top

Java: static final double PI = 3.14159;
来源：http://uoc.iojbl.cn

Go:   const PI = 3.14159
来源：http://dgu.jinqigfzy.top

Ruby: PI = 3.14159
来源：http://ptr.dashuyun.cn

C#:   const double PI = 3.14159;
来源：http://yrk.redwolf501.top

[A04] 判断变量类型
来源：http://qre.bbcook.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gmm.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ctd.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hhj.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://qow.jlsjyb.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://elq.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://jqj.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jbp.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://kgw.svipenyu.cn

[A05] 整数除法与取模
来源：http://oba.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bdh.hnqzz.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gzf.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uch.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hka.sysykeji.top

Java: 7 / 2; 7 % 2
来源：http://paj.yangfankeji.com

Go:   7 / 2; 7 % 2
来源：http://hab.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://yqt.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://azg.birdmap.top

[A06] 字符串转数字
来源：http://eou.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://agf.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xda.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zto.xingfuxueyuan.xyz


<!-- 参考信息 -->