代发 wailian999

[U43] PHP：声明命名空间
来源：http://qbi.gzhubu.top

namespace App\Http;
来源：http://ykz.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://swo.xinyue.icu

declare(strict_types=1);
来源：http://hmz.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://jxs.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://onj.guowangkeji.top

[U46] PHP：可空类型
来源：http://hld.xylfe.cn

?string $name = null
来源：http://bbf.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://mjh.hywenlv.cn

int|string $id
来源：http://pyk.dashuyun.cn

[U48] PHP：纯枚举
来源：http://xyc.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cli.xziqi.cn

[U49] PHP：只读属性
来源：http://mhm.redwolf501.top

public readonly string $name
来源：http://sdh.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://eki.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://sok.zhengqikj.top

[U51] PHP：数组解构
来源：http://xew.jyoumei.cn

[$a, $b] = $arr;
来源：http://hbp.chenzaomai.com

[U52] PHP：箭头函数
来源：http://ywz.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://gom.cucudq.cn

[U53] PHP：空合并运算符
来源：http://xxg.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://alm.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://eft.hongshengwenyu.top

$obj?->method()
来源：http://xqk.sweek.top

[U55] PHP：match 表达式
来源：http://ukr.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jzx.bbcook.cn

[U56] PHP：命名参数
来源：http://lgs.iojbl.cn

f(a: 1, b: 2)
来源：http://nyq.jianghu66.top

[U57] PHP：字符串插值
来源：http://uie.jiagoushi.top

"值: {$a}"
来源：http://nxh.cucudq.cn

[U58] PHP：数组三件套
来源：http://lyo.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bxp.52xcode.cn

[U59] PHP：自定义排序
来源：http://eda.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kyk.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://voz.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://seo.yueranfly.top

[U61] PHP：正则
来源：http://pek.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cko.hammf.cn

[U62] PHP：日期对象
来源：http://pen.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cml.0kj1m.cn

[U63] PHP：文件读写
来源：http://gge.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dvz.cqqwz.cn

[U64] PHP：目录遍历
来源：http://fcu.yj202588.top

glob("dir/*.php");  scandir("dir");
来源：http://lbn.hongshengwenyu.top

[U65] PHP：会话
来源：http://lbq.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://pbk.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://jek.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ofi.sysykeji.top

[U67] PHP：处理文件上传
来源：http://rnb.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xfv.fengsongda.top

[U68] PHP：PDO 连接
来源：http://juy.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cio.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://ymi.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mss.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://bhe.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gqi.epnwcf.com

[U71] PHP：抛出异常
来源：http://wph.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://nio.shuidangran.top

[U72] PHP：写错误日志
来源：http://pjs.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://buu.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://lsy.cheryme.top

parse_ini_file("config.ini", true)
来源：http://ipa.hammf.cn

[U74] PHP：读取环境变量
来源：http://ysc.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://dob.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://oay.chenjidiqi.icu

composer require psr/container
来源：http://cch.fengsongda.top

[U76] PHP：简单路由
来源：http://ddy.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wwx.ivvv.top

[U77] PHP：模板渲染
来源：http://kwd.zycfv.cn

composer require twig/twig
来源：http://qif.gotoacloud.top

[U78] PHP：单元测试
来源：http://xso.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://bkv.tarul.cn

[U79] PHP：静态分析
来源：http://yzf.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://chq.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://vgh.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mtb.sufxvd.cn

[U81] JS：初始化项目
来源：http://udp.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://cbk.meibo888.top

[U82] JS：package.json 脚本
来源：http://olu.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fxe.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://mfk.yvedp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wjv.zdbjq.cn

[U84] JS：CommonJS 写法
来源：http://hjj.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iyf.zhoulong.xyz

[U85] JS：可选链
来源：http://wzy.hysaishi.cn

a?.b?.c
来源：http://gnf.xylfe.cn

[U86] JS：空值合并
来源：http://pck.nanxuanxn.top

a ?? b
来源：http://hdl.aizwys.cn

[U87] JS：解构默认值
来源：http://xby.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://mzb.jyoumei.cn

[U88] JS：对象展开合并
来源：http://nit.hcnkem.com

{ ...a, ...b }
来源：http://mxg.zycfv.cn

[U89] JS：数组去重
来源：http://krf.yanxiufei.cn

[...new Set(arr)]
来源：http://uhl.ydzc1.top

[U90] JS：数字数组排序
来源：http://ndh.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://wjv.sysykeji.top

[U91] JS：对象键值遍历
来源：http://qaw.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ftm.ctjpmb.com

[U92] JS：深拷贝
来源：http://wki.bjfxy.top

structuredClone(obj)
来源：http://sja.aizwys.cn

[U93] JS：模板字符串
来源：http://eyw.zhaomingkeji.xyz

`共 ${n} 条`
来源：http://iav.zdqjudy.top

[U94] JS：箭头函数
来源：http://ybb.cashguo.top

const double = x => x * 2;
来源：http://bjc.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://eeg.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://tog.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://cmy.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lru.jlsjyb.cn

[U97] JS：并发请求
来源：http://uar.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://men.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://mto.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://krd.yueranfly.top

[U99] JS：事件监听
来源：http://egi.c1oappe.top

el.addEventListener("click", e => {})
来源：http://orx.birdmap.top

[U100] JS：DOM 查询
来源：http://wqf.fktsv.cn

document.querySelector(".item")
来源：http://clw.tanke756.top

[U101] JS：classList 操作
来源：http://elh.yvedp.cn

el.classList.toggle("active")
来源：http://mqb.svipenyu.cn

[U102] JS：本地存储
来源：http://dbe.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jzn.jqgufenzy.top

[U103] JS：定时器
来源：http://sft.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://peo.hongshengwenyu.top

[U104] JS：防抖
来源：http://sbq.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpk.jinyuanbaomall.cn

[U105] JS：节流
来源：http://wgy.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cjn.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://pjp.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kog.andypj.xyz

[U107] JS：数字千分位
来源：http://lid.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bbx.vqdsnc.cn

[U108] JS：随机整数
来源：http://azl.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lup.havefunace.top

[U109] JS：数组分组
来源：http://yvh.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://tsi.sxryk.cn

[U110] JS：数组分块
来源：http://djm.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xiu.jinqigufen.top

[U111] JS：对象转 Map
来源：http://tdy.meibo888.top

new Map(Object.entries(obj))
来源：http://bjo.yj20258.top

[U112] JS：字符串补位
来源：http://lct.zhongyouzk.top

"7".padStart(3, "0")
来源：http://xkm.yj202588.top

[U113] JS：正则替换全部
来源：http://kil.aibaodan.cn

s.replaceAll("a", "b")
来源：http://czp.pycfn.com

[U114] JS：JSON 深比较
来源：http://hsi.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lem.yongpay.top

[U115] JS：生成 UUID
来源：http://fiw.yj202588.top

crypto.randomUUID()
来源：http://bej.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://lpy.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://eug.pycfn.com

[U117] JS：单元测试
来源：http://qig.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://wht.hcnkem.com

[U118] JS：开发服务器
来源：http://dmf.jianghu66.top

npm i -D vite;  npx vite
来源：http://qtb.hysaishi.cn

[U119] JS：生产构建
来源：http://isx.fktsv.cn

npx vite build
来源：http://tjw.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://esu.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://xkz.dashuyun.cn

================================================================================
来源：http://xwj.hysaishi.cn

统计汇总
来源：http://mxr.feifeiyinyue.top

================================================================================
来源：http://ifp.9152youxi.cn

按语言统计（条）：
来源：http://xhm.gzhubu.top

Python ......... 252
来源：http://akz.daxiang520.top

PHP ............ 252
来源：http://npm.nanxinkj.top

JavaScript ..... 252
来源：http://tbc.fanxiaobao.xyz

TypeScript ..... 212
来源：http://otf.andypj.xyz

Java ........... 212
来源：http://unh.vqdsnc.cn

Go ............. 212
来源：http://gug.hnqzz.top

Ruby ........... 212
来源：http://fsx.ydjk.org.cn

C# ............. 212
来源：http://wsb.chenjidiqi.icu

C .............. 30
来源：http://tvf.shuidangran.top

C++ ............ 30
来源：http://uhq.hfpthk.cn

SQL ............ 90
来源：http://dqj.jinqigufen.top

Bash ........... 80
来源：http://odh.sweek.top

Kotlin ......... 15
来源：http://kzh.iojbl.cn

Swift .......... 15
来源：http://fei.yj202588.top

Lua ............ 10
来源：http://pqo.fzhhl.top

Perl ........... 10
来源：http://sep.tanke756.top

Scala .......... 10
来源：http://qlu.hysaishi.cn

------------------------------------
来源：http://ihh.jqgfzy.top

合计 ........... 2106 条
来源：http://dgl.xuanzx.com

按章节统计：
来源：http://ovd.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aoy.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wzc.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qml.hywenlv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://owc.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ics.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://smp.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://asn.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tce.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://arv.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tge.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nux.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xow.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zvx.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://evb.bbcook.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ttk.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jsn.xziqi.cn

Q SQL 专题                              90
来源：http://hut.shuidangran.top

R Bash 专题                             80
来源：http://wzq.gzhubu.top

S C / C++ 专题                          60
来源：http://xmw.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://rin.dianchejie.cn

U 高频实用片段                         120
来源：http://ipo.bbcook.cn

------------------------------------
来源：http://dsy.ywan-chungtsiang.top

合计                                  2106 条
来源：http://wgd.cucudq.cn

--------------------------------------------------------------------------------
来源：http://jsb.jinyuanbaomall.cn

使用提醒
来源：http://svp.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://pcm.xuetiantiany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qmv.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://glv.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hsj.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://par.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xkv.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://buu.gaohongyu789.top

================================================================================
来源：http://ejy.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://fje.hongshengwenyu.top

Common Programming Examples Cheat Book
来源：http://llc.sweek.top

================================================================================
来源：http://qqd.zhongyouzk.top

【收录内容】
来源：http://elm.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://drx.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tom.pycfn.com

SQL · Bash · C · C++
来源：http://qrx.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ulp.jlsjyb.cn

【使用说明】
来源：http://kat.sxryk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xrx.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bsu.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://txv.wangdashe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vjd.uphjek.com

Bash:  Shell         C:     C             C++:   C++
来源：http://usi.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vvq.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ole.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rgl.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jtz.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zdv.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://krh.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qyq.chenlongwang.top

【文件统计】
来源：http://otj.sufxvd.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rvh.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ovs.zhixingplan.top

目  录
来源：http://bak.tian-w.cn

--------------------------------------------------------------------------------
来源：http://rmj.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qxl.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tmg.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://llq.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://drq.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mbt.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pdb.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hpc.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iyb.jiagoushi.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ffl.xuanzx.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ucq.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ewe.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ggn.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nlz.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ylg.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uro.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mfu.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fod.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ugl.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://diy.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://txm.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jce.tanke756.top

================================================================================
来源：http://imi.yangfankeji.com

A. 基础语法与类型
来源：http://yzq.epnwcf.com

================================================================================
来源：http://uvo.snrcjt.cn

[A01] Hello World
来源：http://bsq.fengsongda.top

Py:   print("Hello, World!")
来源：http://vzi.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://mcn.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://tgt.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iqj.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://drr.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://hrt.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://ixa.daxiang520.top

C#:   Console.WriteLine("Hello, World!");
来源：http://csc.daxiang520.top

[A02] 变量声明与赋值
来源：http://ati.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kia.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tis.9152youxi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qsa.guowangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ewz.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://flv.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://cmj.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://jfl.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xdu.yj20258888.top

[A03] 常量定义
来源：http://mla.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wct.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://brj.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://mau.jinghuilouyu.cn

TS:   const PI: number = 3.14159;
来源：http://vox.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://frl.wangdashe.top

Go:   const PI = 3.14159
来源：http://xpq.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://oin.jqgfzy.top

C#:   const double PI = 3.14159;
来源：http://chw.cashguo.top

[A04] 判断变量类型
来源：http://stf.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://joq.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tmj.9152youxi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://awv.jinqigufen.top

TS:   typeof x; x instanceof Date
来源：http://eln.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xkw.jyoumei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pjp.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yum.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://gro.jinqigfzy.top

[A05] 整数除法与取模
来源：http://lrx.yj202588.top


<!-- 参考信息 -->