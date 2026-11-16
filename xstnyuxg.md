代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://sil.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ruf.xuanzx.com

[U46] PHP：可空类型
来源：http://yrx.zycfv.cn

?string $name = null
来源：http://rut.zhengqikj.top

[U47] PHP：联合类型
来源：http://wik.chenzaomai.com

int|string $id
来源：http://trr.yangfankeji.com

[U48] PHP：纯枚举
来源：http://dut.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://flk.fktsv.cn

[U49] PHP：只读属性
来源：http://rqw.zhixingplan.top

public readonly string $name
来源：http://tpd.sweek.top

[U50] PHP：构造器属性提升
来源：http://iyg.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://yhe.vqdsnc.cn

[U51] PHP：数组解构
来源：http://ucf.bjfxy.top

[$a, $b] = $arr;
来源：http://qcb.hfpthk.cn

[U52] PHP：箭头函数
来源：http://qsp.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://vaz.hnqzz.top

[U53] PHP：空合并运算符
来源：http://wby.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://lqo.ctjpmb.com

[U54] PHP：空安全调用
来源：http://kkv.jinqigfzy.top

$obj?->method()
来源：http://qrx.tianlin.xyz

[U55] PHP：match 表达式
来源：http://giw.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fuz.guannengcc.top

[U56] PHP：命名参数
来源：http://qrv.ydjk.org.cn

f(a: 1, b: 2)
来源：http://hnl.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://iqf.tanke756.top

"值: {$a}"
来源：http://hqi.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://kwb.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lea.birdmap.top

[U59] PHP：自定义排序
来源：http://fuj.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrh.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://dvf.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fpu.zdqjudy.top

[U61] PHP：正则
来源：http://tml.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hkr.quarkkingdee.top

[U62] PHP：日期对象
来源：http://xnc.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yfp.zhengqikj.top

[U63] PHP：文件读写
来源：http://eum.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://beo.havefunace.top

[U64] PHP：目录遍历
来源：http://vtd.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://rhn.zhengqikj.top

[U65] PHP：会话
来源：http://uae.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ycf.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://omp.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wwg.xuanzx.com

[U67] PHP：处理文件上传
来源：http://fvv.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hqr.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://ixt.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xqa.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://myp.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yjh.316326.xyz

[U70] PHP：PDO 事务
来源：http://mub.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jae.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://ekb.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://enl.mhx1999.top

[U72] PHP：写错误日志
来源：http://pet.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://fbj.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://gsl.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://uip.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://gzs.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://fjb.sweek.top

[U75] PHP：依赖注入
来源：http://apv.guowangkeji.top

composer require psr/container
来源：http://igz.birdmap.top

[U76] PHP：简单路由
来源：http://jrt.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xeo.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://aau.tianlin.xyz

composer require twig/twig
来源：http://ojh.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://mqr.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://iak.mhx1999.top

[U79] PHP：静态分析
来源：http://idl.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://tjw.redwolf501.top

[U80] PHP：代码规范修复
来源：http://hby.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://vdi.dianchejie.cn

[U81] JS：初始化项目
来源：http://ndp.tarul.cn

npm init -y;  npm i express
来源：http://boh.daxiang520.top

[U82] JS：package.json 脚本
来源：http://osg.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vyp.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://coh.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ytl.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://xab.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://ctc.zhixingplan.top

[U85] JS：可选链
来源：http://btl.jiagoushi.top

a?.b?.c
来源：http://hyl.jianghu66.top

[U86] JS：空值合并
来源：http://ikw.tian-w.cn

a ?? b
来源：http://ord.sweek.top

[U87] JS：解构默认值
来源：http://vqw.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://jji.epnwcf.com

[U88] JS：对象展开合并
来源：http://lgb.xziqi.cn

{ ...a, ...b }
来源：http://ydt.birdmap.top

[U89] JS：数组去重
来源：http://yjs.xuanzx.com

[...new Set(arr)]
来源：http://fwl.zhaomingkeji.xyz

[U90] JS：数字数组排序
来源：http://bcq.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://cfe.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://dea.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jxt.zhoulong.xyz

[U92] JS：深拷贝
来源：http://yjg.epnwcf.com

structuredClone(obj)
来源：http://cqz.sxryk.cn

[U93] JS：模板字符串
来源：http://pgx.shanyushiyangtech.top

`共 ${n} 条`
来源：http://vaa.svipenyu.cn

[U94] JS：箭头函数
来源：http://pcd.nwbrower.top

const double = x => x * 2;
来源：http://jeu.zhaomingkeji.xyz

[U95] JS：Promise 包装
来源：http://qqa.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://bkj.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://eng.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vpo.kuanghao11.cn

[U97] JS：并发请求
来源：http://sre.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iec.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://hax.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blt.guannengcc.top

[U99] JS：事件监听
来源：http://ult.ydzc1.top

el.addEventListener("click", e => {})
来源：http://caq.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://qjk.yuanzhike.top

document.querySelector(".item")
来源：http://zns.smart0.xyz

[U101] JS：classList 操作
来源：http://mdp.hnxiangtu.top

el.classList.toggle("active")
来源：http://hfb.ydjk.org.cn

[U102] JS：本地存储
来源：http://uhv.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://nbs.guannengcc.top

[U103] JS：定时器
来源：http://jlw.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xzi.andypj.xyz

[U104] JS：防抖
来源：http://yvf.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iib.gogol.net.cn

[U105] JS：节流
来源：http://ccc.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jpx.hysaishi.cn

[U106] JS：日期格式化
来源：http://qoe.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rte.nwbrower.top

[U107] JS：数字千分位
来源：http://isv.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sdq.nanxuanxn.top

[U108] JS：随机整数
来源：http://fwq.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tlv.aibaodan.cn

[U109] JS：数组分组
来源：http://zcn.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://oje.jyoumei.cn

[U110] JS：数组分块
来源：http://zcd.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uky.sysykeji.top

[U111] JS：对象转 Map
来源：http://apu.wangdashe.top

new Map(Object.entries(obj))
来源：http://ctp.xuanzx.com

[U112] JS：字符串补位
来源：http://moz.yj20258888.top

"7".padStart(3, "0")
来源：http://olw.jqgfzy.top

[U113] JS：正则替换全部
来源：http://wge.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://zes.fehbvm.com

[U114] JS：JSON 深比较
来源：http://gex.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dbh.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://yuy.guowangkeji.top

crypto.randomUUID()
来源：http://awd.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://obn.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://rkx.cdnleiting.top

[U117] JS：单元测试
来源：http://hep.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://spd.9152youxi.cn

[U118] JS：开发服务器
来源：http://gcw.yj20258.top

npm i -D vite;  npx vite
来源：http://gqw.xuanzx.com

[U119] JS：生产构建
来源：http://lec.shanyushiyangtech.top

npx vite build
来源：http://vsa.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://qnx.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://mzt.gotoacloud.top

================================================================================
来源：http://tfi.nanxuanxn.top

统计汇总
来源：http://mph.cqqwz.cn

================================================================================
来源：http://ggs.cashguo.top

按语言统计（条）：
来源：http://hla.cdnleiting.top

Python ......... 252
来源：http://bpd.aizwys.cn

PHP ............ 252
来源：http://gcg.zdqjudy.top

JavaScript ..... 252
来源：http://ecd.dashuyun.cn

TypeScript ..... 212
来源：http://llz.aizwys.cn

Java ........... 212
来源：http://hch.zhongyouzk.top

Go ............. 212
来源：http://ibg.guannengcc.top

Ruby ........... 212
来源：http://yuq.wangshuangyany.cn

C# ............. 212
来源：http://ihw.nwbrower.top

C .............. 30
来源：http://ubu.smart0.xyz

C++ ............ 30
来源：http://ooz.ydjk.org.cn

SQL ............ 90
来源：http://rfj.nwbrower.top

Bash ........... 80
来源：http://orn.316326.xyz

Kotlin ......... 15
来源：http://zmy.jinyuanbaomall.cn

Swift .......... 15
来源：http://hva.zhijiandao.cn

Lua ............ 10
来源：http://oeb.nanxuanxn.top

Perl ........... 10
来源：http://cqx.kuanghao11.cn

Scala .......... 10
来源：http://kyl.9152youxi.cn

------------------------------------
来源：http://vjw.ppjwa.cn

合计 ........... 2106 条
来源：http://olk.meibo888.top

按章节统计：
来源：http://bks.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vuo.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oaz.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nhw.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://war.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://seq.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wra.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hve.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dsr.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gcf.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wsp.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nzb.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pdp.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xhc.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zyl.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fhy.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oae.yvedp.cn

Q SQL 专题                              90
来源：http://sjp.svipenyu.cn

R Bash 专题                             80
来源：http://azz.tanke756.top

S C / C++ 专题                          60
来源：http://anl.yvedp.cn

T 其他语言补充                          60
来源：http://yrt.cdnleiting.top

U 高频实用片段                         120
来源：http://ebi.shuidangran.top

------------------------------------
来源：http://hjg.jianghu66.top

合计                                  2106 条
来源：http://huf.sxryk.cn

--------------------------------------------------------------------------------
来源：http://uby.feifeiyinyue.top

使用提醒
来源：http://slt.fzhhl.top

--------------------------------------------------------------------------------
来源：http://czf.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://svo.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pev.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://grx.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://noh.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ork.jianghu66.top

—— 文件结束 ——
来源：http://dpe.ppjwa.cn

================================================================================
来源：http://qlo.aibaodan.cn

程序语言常见例子速查手册（2024 版）
来源：http://xju.yj20258.top

Common Programming Examples Cheat Book
来源：http://jqs.zhijiandao.cn

================================================================================
来源：http://qly.9152youxi.cn

【收录内容】
来源：http://tag.sufxvd.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pwj.yueranfly.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dyr.xinyue.icu

SQL · Bash · C · C++
来源：http://grq.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gnf.haohaochexian.top

【使用说明】
来源：http://ypt.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sfs.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oxt.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wxc.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jxm.yanxiufei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fph.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zyp.shuidangran.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ulm.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sbc.zhengqikj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lgh.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ihi.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mgn.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yan.yfazqb.com

【文件统计】
来源：http://bqp.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://usl.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://ypr.52xcode.cn

目  录
来源：http://gxp.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://vbl.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oby.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mqs.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://poi.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cwa.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://trx.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xln.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://koh.yj20258.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kvz.pengpengdd.cyou

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cxr.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kmo.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://awz.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fjy.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kql.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eat.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ksx.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hyr.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ybt.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qjm.wangshuangyany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pdo.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ulp.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qgr.yangfankeji.com

================================================================================
来源：http://skv.jqgufenzy.top

A. 基础语法与类型
来源：http://fxh.tanke756.top

================================================================================
来源：http://bwk.jinghuilouyu.cn

[A01] Hello World
来源：http://myw.yonumen.top

Py:   print("Hello, World!")
来源：http://hae.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://shq.yuanzhike.top

JS:   console.log("Hello, World!");
来源：http://ugw.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jam.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://ewp.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://cgy.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://kwe.jqgfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fzt.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://xrf.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zgq.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://weg.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://xcd.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://egg.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://szd.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://mal.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://hsk.316326.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://mdh.zdbjq.cn

[A03] 常量定义
来源：http://ygh.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kgr.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://cco.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://geb.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://zas.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://nac.tian-w.cn

Go:   const PI = 3.14159
来源：http://rvc.nanxinkj.top

Ruby: PI = 3.14159
来源：http://lkl.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://dgr.jinqigfzy.top

[A04] 判断变量类型
来源：http://xbt.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://tdr.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nhv.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jbz.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://bhe.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ezz.fzhhl.top

Go:   reflect.TypeOf(x).Name()
来源：http://fhd.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dtd.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://oed.birdmap.top

[A05] 整数除法与取模
来源：http://jmd.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://swc.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ttp.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nxp.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://alo.hongshengwenyu.top


<!-- 参考信息 -->