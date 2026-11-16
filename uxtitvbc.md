代发 wailian999

[U35] Py：发送邮件
来源：http://qlr.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xaz.tarul.cn

[U36] Py：定时任务
来源：http://afs.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://ekj.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://cri.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://bum.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://okm.vehdjk.com

Path(__file__).resolve().parent
来源：http://lau.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://llc.316326.xyz

sys.stdout.isatty()
来源：http://qmc.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://myz.daria6918.cn

print("err", file=sys.stderr)
来源：http://tqw.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://gfw.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pdg.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://bma.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://boy.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://iyi.sjlbkw.cn

namespace App\Http;
来源：http://xjf.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://ued.chenjidiqi.icu

declare(strict_types=1);
来源：http://das.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://fjj.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zki.epnwcf.com

[U46] PHP：可空类型
来源：http://rts.zdqjudy.top

?string $name = null
来源：http://cmw.zhongyouzk.top

[U47] PHP：联合类型
来源：http://vhi.hysaishi.cn

int|string $id
来源：http://zop.hammf.cn

[U48] PHP：纯枚举
来源：http://mlj.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ydo.daxiang520.top

[U49] PHP：只读属性
来源：http://cwh.tarul.cn

public readonly string $name
来源：http://clj.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://niu.chenzaomai.com

public function __construct(private int $id) {}
来源：http://gor.pycfn.com

[U51] PHP：数组解构
来源：http://pkw.jinqigfzy.top

[$a, $b] = $arr;
来源：http://cvy.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://iuv.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://owi.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://boh.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://rmc.fzhhl.top

[U54] PHP：空安全调用
来源：http://usf.zhoulong.xyz

$obj?->method()
来源：http://hct.dashuyun.cn

[U55] PHP：match 表达式
来源：http://apf.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fhy.hfpthk.cn

[U56] PHP：命名参数
来源：http://pqr.fktsv.cn

f(a: 1, b: 2)
来源：http://til.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://luq.yonumen.top

"值: {$a}"
来源：http://swo.yfazqb.com

[U58] PHP：数组三件套
来源：http://nmz.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://chu.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://wch.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://llt.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://gbe.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xeh.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://opa.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ggv.sysykeji.top

[U62] PHP：日期对象
来源：http://qsn.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vtm.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://eon.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eye.c1oappe.top

[U64] PHP：目录遍历
来源：http://hjz.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://bhn.chenzaomai.com

[U65] PHP：会话
来源：http://vvv.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dsd.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://bjj.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zvc.52xcode.cn

[U67] PHP：处理文件上传
来源：http://scs.fanxiaobao.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ruf.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://djc.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ary.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://cbc.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sfs.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://uik.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jii.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://skf.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://smx.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://drt.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://ptw.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://ehk.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://dsb.yuxming.cn

[U74] PHP：读取环境变量
来源：http://vrk.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://dgm.chenzaomai.com

[U75] PHP：依赖注入
来源：http://txy.ppjwa.cn

composer require psr/container
来源：http://gte.daria6918.cn

[U76] PHP：简单路由
来源：http://pka.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oab.chenlongwang.top

[U77] PHP：模板渲染
来源：http://fxc.pengpengdd.cyou

composer require twig/twig
来源：http://uki.fehbvm.com

[U78] PHP：单元测试
来源：http://kup.ivvv.top

composer require --dev phpunit/phpunit
来源：http://xxb.tanke756.top

[U79] PHP：静态分析
来源：http://fdb.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://neb.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://bqt.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vjn.0kj1m.cn

[U81] JS：初始化项目
来源：http://mgn.daria6918.cn

npm init -y;  npm i express
来源：http://wea.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://ful.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uqi.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://zgu.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://awz.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://jpo.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vdy.sweek.top

[U85] JS：可选链
来源：http://bcs.daria6918.cn

a?.b?.c
来源：http://oun.iojbl.cn

[U86] JS：空值合并
来源：http://nii.shzxlz.cn

a ?? b
来源：http://obd.cdnleiting.top

[U87] JS：解构默认值
来源：http://ppp.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://pyy.sysykeji.top

[U88] JS：对象展开合并
来源：http://oqt.xziqi.cn

{ ...a, ...b }
来源：http://rth.jiagoushi.top

[U89] JS：数组去重
来源：http://mvu.iojbl.cn

[...new Set(arr)]
来源：http://xrr.zhengqikj.top

[U90] JS：数字数组排序
来源：http://rmq.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://alg.mhx1999.top

[U91] JS：对象键值遍历
来源：http://ewb.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fof.gotoacloud.top

[U92] JS：深拷贝
来源：http://nqj.xylfe.cn

structuredClone(obj)
来源：http://oyd.52xcode.cn

[U93] JS：模板字符串
来源：http://rwu.52xcode.cn

`共 ${n} 条`
来源：http://chx.daria6918.cn

[U94] JS：箭头函数
来源：http://pez.jinghuilouyu.cn

const double = x => x * 2;
来源：http://pjx.hywenlv.cn

[U95] JS：Promise 包装
来源：http://nci.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://ief.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://beo.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://szh.316326.xyz

[U97] JS：并发请求
来源：http://tet.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kru.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://eds.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wyo.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://uov.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://tlj.cucudq.cn

[U100] JS：DOM 查询
来源：http://ogl.yueranfly.top

document.querySelector(".item")
来源：http://huu.ywan-chungtsiang.top

[U101] JS：classList 操作
来源：http://icj.0kj1m.cn

el.classList.toggle("active")
来源：http://pun.gzhubu.top

[U102] JS：本地存储
来源：http://fez.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://nza.tarul.cn

[U103] JS：定时器
来源：http://xzb.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://stv.xuetiantiany.cn

[U104] JS：防抖
来源：http://yts.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jeg.gotoacloud.top

[U105] JS：节流
来源：http://ncl.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hci.xylfe.cn

[U106] JS：日期格式化
来源：http://tfq.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sws.c1oappe.top

[U107] JS：数字千分位
来源：http://jjj.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pjs.ctjpmb.com

[U108] JS：随机整数
来源：http://slu.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eyc.ydzc1.top

[U109] JS：数组分组
来源：http://bmq.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://mxw.yuxming.cn

[U110] JS：数组分块
来源：http://fqe.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qba.hfpthk.cn

[U111] JS：对象转 Map
来源：http://dfy.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://uar.yfazqb.com

[U112] JS：字符串补位
来源：http://imo.jyoumei.cn

"7".padStart(3, "0")
来源：http://pgq.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://quy.uphjek.com

s.replaceAll("a", "b")
来源：http://maq.hcnkem.com

[U114] JS：JSON 深比较
来源：http://vdg.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ecm.yongpay.top

[U115] JS：生成 UUID
来源：http://mxk.ivvv.top

crypto.randomUUID()
来源：http://nrj.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://xuy.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://hlc.hywenlv.cn

[U117] JS：单元测试
来源：http://syg.birdmap.top

npm i -D vitest;  npx vitest
来源：http://pip.xinyue.icu

[U118] JS：开发服务器
来源：http://mfm.0kj1m.cn

npm i -D vite;  npx vite
来源：http://frl.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://sqr.shanyushiyangkeji.top

npx vite build
来源：http://umz.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://del.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://mnc.sjlbkw.cn

================================================================================
来源：http://smj.jinghuilouyu.cn

统计汇总
来源：http://ova.daria6918.cn

================================================================================
来源：http://cxh.nanxuanxn.top

按语言统计（条）：
来源：http://rui.fanxiaobao.xyz

Python ......... 252
来源：http://fnb.hammf.cn

PHP ............ 252
来源：http://iig.jqgfzy.top

JavaScript ..... 252
来源：http://akq.smart0.xyz

TypeScript ..... 212
来源：http://tfz.feifeiyinyue.top

Java ........... 212
来源：http://amv.vqdsnc.cn

Go ............. 212
来源：http://jvf.zhongyouzk.top

Ruby ........... 212
来源：http://chq.ywan-chungtsiang.top

C# ............. 212
来源：http://hjh.zhijiandao.cn

C .............. 30
来源：http://lhi.cheryme.top

C++ ............ 30
来源：http://ugc.ehwqpu.com

SQL ............ 90
来源：http://jmn.birdmap.top

Bash ........... 80
来源：http://pfy.hongshengwenyu.top

Kotlin ......... 15
来源：http://wiu.ywan-chungtsiang.top

Swift .......... 15
来源：http://gvb.dianchejie.cn

Lua ............ 10
来源：http://atr.xuanzx.com

Perl ........... 10
来源：http://ldn.meibo888.top

Scala .......... 10
来源：http://nir.jqgfzy.top

------------------------------------
来源：http://dqz.sweek.top

合计 ........... 2106 条
来源：http://zfl.52xcode.cn

按章节统计：
来源：http://qoe.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rkd.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bxe.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qmx.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ozl.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://znm.pycfn.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rxn.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dts.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rlk.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://snk.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lta.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wri.shangyingyoupin.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lcd.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wei.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jrg.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sjc.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iaq.nwbrower.top

Q SQL 专题                              90
来源：http://nbj.hcnkem.com

R Bash 专题                             80
来源：http://kij.cqqwz.cn

S C / C++ 专题                          60
来源：http://hyp.c1oappe.top

T 其他语言补充                          60
来源：http://qcz.nanxinkj.top

U 高频实用片段                         120
来源：http://syr.mhx1999.top

------------------------------------
来源：http://kuc.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://bsz.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://aqh.mhx1999.top

使用提醒
来源：http://wiy.havefunace.top

--------------------------------------------------------------------------------
来源：http://kqj.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dbb.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iqx.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uyu.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://utb.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jzu.xylfe.cn

—— 文件结束 ——
来源：http://dcn.chenjidiqi.icu

================================================================================
来源：http://fov.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://qpd.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://gvt.jqgufenzy.top

================================================================================
来源：http://fwg.zhongyouzk.top

【收录内容】
来源：http://jfm.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://rfm.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pmu.epnwcf.com

SQL · Bash · C · C++
来源：http://fnw.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fvj.haohaochexian.top

【使用说明】
来源：http://vyw.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dix.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vct.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fma.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yrp.fktsv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://red.shanyushiyangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ibf.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://abs.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wlc.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bmm.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bir.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yzw.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lkx.guowangkeji.top

【文件统计】
来源：http://moa.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zxv.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://qec.yvedp.cn

目  录
来源：http://ejn.ydzc1.top

--------------------------------------------------------------------------------
来源：http://tup.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yer.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ftr.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fmt.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://swe.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mid.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zgt.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nwb.yangfankeji.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rlp.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://leh.hfpthk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ljw.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vbn.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jbr.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://trf.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lln.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tmb.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rbq.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://igb.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zsm.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hox.bbcook.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yhe.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fsi.yangfankeji.com

================================================================================
来源：http://rui.vehdjk.com

A. 基础语法与类型
来源：http://opd.jqgfzy.top

================================================================================
来源：http://qiw.sjlbkw.cn

[A01] Hello World
来源：http://brl.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://etp.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://jji.cdnleiting.top

JS:   console.log("Hello, World!");
来源：http://zpp.hysaishi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xpg.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://yqc.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://ysf.cheryme.top

Ruby: puts "Hello, World!"
来源：http://bmt.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rzx.xuanzx.com

[A02] 变量声明与赋值
来源：http://jlg.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ejz.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ggr.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://cge.tian-w.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://olr.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://lpz.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://awy.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://niy.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://wwe.aizwys.cn

[A03] 常量定义
来源：http://frx.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wvv.epnwcf.com

PHP:  const PI = 3.14159;
来源：http://yar.yongpay.top


<!-- 参考信息 -->