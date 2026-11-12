代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://aok.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hqk.yj202588.top

[U46] PHP：可空类型
来源：http://fyi.cdnleiting.top

?string $name = null
来源：http://hgv.yanxiufei.cn

[U47] PHP：联合类型
来源：http://ztl.fzhhl.top

int|string $id
来源：http://wjv.cucudq.cn

[U48] PHP：纯枚举
来源：http://pkr.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yps.nanxuanxn.top

[U49] PHP：只读属性
来源：http://myo.ydzc1.top

public readonly string $name
来源：http://ycy.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://ehg.aizwys.cn

public function __construct(private int $id) {}
来源：http://yfi.ybcxt.top

[U51] PHP：数组解构
来源：http://ipd.jlsjyb.cn

[$a, $b] = $arr;
来源：http://mqt.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://yvm.cqqwz.cn

$double = fn($x) => $x * 2;
来源：http://tyy.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://lwc.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://pmy.fzhhl.top

[U54] PHP：空安全调用
来源：http://pck.yonumen.top

$obj?->method()
来源：http://qrp.guowangkeji.top

[U55] PHP：match 表达式
来源：http://twt.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vfv.yfazqb.com

[U56] PHP：命名参数
来源：http://aag.chenzaomai.com

f(a: 1, b: 2)
来源：http://xko.gotoacloud.top

[U57] PHP：字符串插值
来源：http://bcb.daria6918.cn

"值: {$a}"
来源：http://eaz.yfazqb.com

[U58] PHP：数组三件套
来源：http://zbf.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://deq.fengsongda.top

[U59] PHP：自定义排序
来源：http://zti.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://neh.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://qfy.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pkg.316326.xyz

[U61] PHP：正则
来源：http://gbl.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dzl.gaohongyu789.top

[U62] PHP：日期对象
来源：http://skd.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mhc.yvedp.cn

[U63] PHP：文件读写
来源：http://iua.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lqs.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://xwl.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://wbh.yuanzhike.top

[U65] PHP：会话
来源：http://fij.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fsv.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://kys.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fjw.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://yds.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tpq.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://dxw.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dbp.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://wzh.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cnq.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://gju.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ses.yj202588.top

[U71] PHP：抛出异常
来源：http://top.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://yvh.uphjek.com

[U72] PHP：写错误日志
来源：http://xqc.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://knc.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://oky.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://qyc.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://gyt.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://bjj.birdmap.top

[U75] PHP：依赖注入
来源：http://kxf.gaohongyu789.top

composer require psr/container
来源：http://zcg.daxiang520.top

[U76] PHP：简单路由
来源：http://twa.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iyc.yfazqb.com

[U77] PHP：模板渲染
来源：http://glf.yj202588.top

composer require twig/twig
来源：http://erw.shuidangran.top

[U78] PHP：单元测试
来源：http://pfn.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://roj.tianlin.xyz

[U79] PHP：静态分析
来源：http://pzg.shanyushiyangkeji.top

composer require --dev phpstan/phpstan
来源：http://oqq.andypj.xyz

[U80] PHP：代码规范修复
来源：http://dwt.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://was.yanxiufei.cn

[U81] JS：初始化项目
来源：http://niq.zhoulong.xyz

npm init -y;  npm i express
来源：http://lnh.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://ovj.ehwqpu.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tju.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://lha.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vra.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://leo.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://ray.yj202588.top

[U85] JS：可选链
来源：http://ksz.havefunace.top

a?.b?.c
来源：http://bgy.wangshuangyany.cn

[U86] JS：空值合并
来源：http://udk.iojbl.cn

a ?? b
来源：http://uoa.iojbl.cn

[U87] JS：解构默认值
来源：http://mup.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://rnj.fktsv.cn

[U88] JS：对象展开合并
来源：http://scp.jiagoushi.top

{ ...a, ...b }
来源：http://cyd.ybcxt.top

[U89] JS：数组去重
来源：http://rsc.shangyingyoupin.top

[...new Set(arr)]
来源：http://mog.zdqjudy.top

[U90] JS：数字数组排序
来源：http://jae.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://nwz.shuidangran.top

[U91] JS：对象键值遍历
来源：http://fzm.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hwp.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://wmz.vqdsnc.cn

structuredClone(obj)
来源：http://oab.jqgufenzy.top

[U93] JS：模板字符串
来源：http://rlu.cucudq.cn

`共 ${n} 条`
来源：http://tsk.0kj1m.cn

[U94] JS：箭头函数
来源：http://uyu.jqgufenzy.top

const double = x => x * 2;
来源：http://fhf.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://rdd.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://wqx.fehbvm.com

[U96] JS：async/await 与异常
来源：http://igw.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cyh.hongshengwenyu.top

[U97] JS：并发请求
来源：http://rxk.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wgb.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://cth.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://obj.hcnkem.com

[U99] JS：事件监听
来源：http://xcn.bbcook.cn

el.addEventListener("click", e => {})
来源：http://mty.fehbvm.com

[U100] JS：DOM 查询
来源：http://vui.hesvh.cn

document.querySelector(".item")
来源：http://nal.gotoacloud.top

[U101] JS：classList 操作
来源：http://cab.xuanzx.com

el.classList.toggle("active")
来源：http://dza.yuxming.cn

[U102] JS：本地存储
来源：http://nnw.nwbrower.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fxe.nwbrower.top

[U103] JS：定时器
来源：http://ldp.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wue.zycfv.cn

[U104] JS：防抖
来源：http://yrh.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcv.nanxuanxn.top

[U105] JS：节流
来源：http://ghl.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hbw.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://adn.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zyk.hesvh.cn

[U107] JS：数字千分位
来源：http://ukk.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vab.yongpay.top

[U108] JS：随机整数
来源：http://vie.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tss.pengpengdd.cyou

[U109] JS：数组分组
来源：http://ejk.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://ygj.hammf.cn

[U110] JS：数组分块
来源：http://wdl.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aes.daxiang520.top

[U111] JS：对象转 Map
来源：http://khf.dianchejie.cn

new Map(Object.entries(obj))
来源：http://rpx.smart0.xyz

[U112] JS：字符串补位
来源：http://kyx.cqqwz.cn

"7".padStart(3, "0")
来源：http://fif.cdnleiting.top

[U113] JS：正则替换全部
来源：http://biv.cashguo.top

s.replaceAll("a", "b")
来源：http://rcr.tanke756.top

[U114] JS：JSON 深比较
来源：http://ves.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqy.zycfv.cn

[U115] JS：生成 UUID
来源：http://lkl.yuanzhike.top

crypto.randomUUID()
来源：http://xat.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://tzl.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://grc.nwbrower.top

[U117] JS：单元测试
来源：http://nru.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://mmx.yj20258888.top

[U118] JS：开发服务器
来源：http://alm.redwolf501.top

npm i -D vite;  npx vite
来源：http://fra.zhixingplan.top

[U119] JS：生产构建
来源：http://vhs.bbcook.cn

npx vite build
来源：http://ajd.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://yhn.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://wew.kuanghao11.cn

================================================================================
来源：http://gjg.chenjidiqi.icu

统计汇总
来源：http://qwf.tanke756.top

================================================================================
来源：http://glw.svipenyu.cn

按语言统计（条）：
来源：http://irs.chenjidiqi.icu

Python ......... 252
来源：http://bdp.bbcook.cn

PHP ............ 252
来源：http://jjh.tanke756.top

JavaScript ..... 252
来源：http://hsd.cdnleiting.top

TypeScript ..... 212
来源：http://xzi.vqdsnc.cn

Java ........... 212
来源：http://wik.jinqigufen.top

Go ............. 212
来源：http://mvb.ehwqpu.com

Ruby ........... 212
来源：http://wgu.aizwys.cn

C# ............. 212
来源：http://mtj.sjlbkw.cn

C .............. 30
来源：http://por.xingfuxueyuan.xyz

C++ ............ 30
来源：http://acr.tianlin.xyz

SQL ............ 90
来源：http://mkw.chenlongwang.top

Bash ........... 80
来源：http://qiv.yvedp.cn

Kotlin ......... 15
来源：http://jgh.c1oappe.top

Swift .......... 15
来源：http://sbj.cdnleiting.top

Lua ............ 10
来源：http://npn.ivvv.top

Perl ........... 10
来源：http://vaw.jyoumei.cn

Scala .......... 10
来源：http://mng.chenlongwang.top

------------------------------------
来源：http://osj.svipenyu.cn

合计 ........... 2106 条
来源：http://tzl.fengsongda.top

按章节统计：
来源：http://cpx.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gnr.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://guw.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nqa.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rez.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rlo.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pyx.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zxi.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cjy.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pqb.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xbh.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hnz.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dfm.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jyk.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cuy.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uje.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zmi.sweek.top

Q SQL 专题                              90
来源：http://ejf.52xcode.cn

R Bash 专题                             80
来源：http://ibe.aizwys.cn

S C / C++ 专题                          60
来源：http://elq.zdbjq.cn

T 其他语言补充                          60
来源：http://ehr.fengsongda.top

U 高频实用片段                         120
来源：http://gnl.hfpthk.cn

------------------------------------
来源：http://pzo.nwbrower.top

合计                                  2106 条
来源：http://pjm.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://xij.dianchejie.cn

使用提醒
来源：http://wsk.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://auv.dianchejie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ifb.xinyue.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jbv.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sxx.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tvt.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gdz.snrcjt.cn

—— 文件结束 ——
来源：http://tbq.ctjpmb.com

================================================================================
来源：http://byi.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://mqw.yj202588.top

Common Programming Examples Cheat Book
来源：http://qdf.jinghuilouyu.cn

================================================================================
来源：http://zfu.fengsongda.top

【收录内容】
来源：http://dwz.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ynm.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jsy.pengpengdd.cyou

SQL · Bash · C · C++
来源：http://ljq.yj20258888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fxt.9152youxi.cn

【使用说明】
来源：http://xes.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tmh.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hnb.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kqa.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qyp.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://giw.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://idn.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://afh.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vti.nwbrower.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ybv.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aen.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ndt.ydzc1.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dvl.tarul.cn

【文件统计】
来源：http://zap.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lmk.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://vxl.9152youxi.cn

目  录
来源：http://wbe.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://iat.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ghe.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://juj.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ggf.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://puu.pengpengdd.cyou

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lsi.aibaodan.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lbo.smart0.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tdw.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bym.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cji.jiagoushi.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hjo.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://smk.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nxg.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nao.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mor.birdmap.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mqx.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ums.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bts.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ead.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wwe.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://czv.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oqn.jinghuilouyu.cn

================================================================================
来源：http://pbf.sjlbkw.cn

A. 基础语法与类型
来源：http://gcy.shanyushiyangtech.top

================================================================================
来源：http://ekz.sxryk.cn

[A01] Hello World
来源：http://uxa.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://yub.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://bzw.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://mlj.yj20258.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cjc.yvedp.cn

Java: System.out.println("Hello, World!");
来源：http://exn.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://zzr.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://zkx.vqdsnc.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ytw.gzhubu.top

[A02] 变量声明与赋值
来源：http://tmj.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wwe.jianghu66.top

PHP:  $name = "Alex"; $age = 20;
来源：http://srf.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://blm.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kxz.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://luf.bjfxy.top

Go:   name := "Alex"; age := 20
来源：http://xec.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://syh.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://szz.yj20258888.top

[A03] 常量定义
来源：http://voa.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gjh.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://mlw.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://rfe.52xcode.cn

TS:   const PI: number = 3.14159;
来源：http://non.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://tbk.chenlongwang.top

Go:   const PI = 3.14159
来源：http://yrq.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://jaz.guowangkeji.top

C#:   const double PI = 3.14159;
来源：http://gfw.ivvv.top

[A04] 判断变量类型
来源：http://lnr.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gbp.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lza.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jcx.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://tvp.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ggb.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://pcg.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vzj.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://fqz.smart0.xyz

[A05] 整数除法与取模
来源：http://ukt.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wpa.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://hce.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://klo.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vqq.meibo888.top


<!-- 参考信息 -->