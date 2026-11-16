代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://pot.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dmn.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://esc.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gjb.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://iel.hammf.cn

namespace App\Http;
来源：http://bmo.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://vjn.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://iwo.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://cdo.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ptl.birdmap.top

[U46] PHP：可空类型
来源：http://gpn.jqgfzy.top

?string $name = null
来源：http://lvv.fehbvm.com

[U47] PHP：联合类型
来源：http://czt.yueranfly.top

int|string $id
来源：http://wer.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://cfa.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ryn.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://hes.hesvh.cn

public readonly string $name
来源：http://jym.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://hce.yuanzhike.top

public function __construct(private int $id) {}
来源：http://xxl.sxryk.cn

[U51] PHP：数组解构
来源：http://hys.redwolf501.top

[$a, $b] = $arr;
来源：http://zfb.wangshuangyany.cn

[U52] PHP：箭头函数
来源：http://grn.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://wol.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://ybu.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://mus.iojbl.cn

[U54] PHP：空安全调用
来源：http://bul.sysykeji.top

$obj?->method()
来源：http://rmc.dashuyun.cn

[U55] PHP：match 表达式
来源：http://inh.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eir.cashguo.top

[U56] PHP：命名参数
来源：http://wws.ydzc1.top

f(a: 1, b: 2)
来源：http://rai.hnqzz.top

[U57] PHP：字符串插值
来源：http://poo.hammf.cn

"值: {$a}"
来源：http://vnj.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://uqt.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gbu.xylfe.cn

[U59] PHP：自定义排序
来源：http://gjm.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cnh.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://rwd.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yme.jiagoushi.top

[U61] PHP：正则
来源：http://gbz.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mai.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://rne.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ibr.zhijiandao.cn

[U63] PHP：文件读写
来源：http://mpa.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fzn.ybcxt.top

[U64] PHP：目录遍历
来源：http://tup.ctjpmb.com

glob("dir/*.php");  scandir("dir");
来源：http://mlg.redwolf501.top

[U65] PHP：会话
来源：http://hmd.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kux.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://kum.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://znd.redwolf501.top

[U67] PHP：处理文件上传
来源：http://uay.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ucu.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://vpu.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://saj.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://xsv.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dmb.daria6918.cn

[U70] PHP：PDO 事务
来源：http://lui.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://thk.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://qsx.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://eyo.c1oappe.top

[U72] PHP：写错误日志
来源：http://xam.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://nxu.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://qvx.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://gkw.fehbvm.com

[U74] PHP：读取环境变量
来源：http://pil.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://hws.xziqi.cn

[U75] PHP：依赖注入
来源：http://uma.smart0.xyz

composer require psr/container
来源：http://bul.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://nlu.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://csu.hnqzz.top

[U77] PHP：模板渲染
来源：http://iqr.tianlin.xyz

composer require twig/twig
来源：http://hlu.redwolf501.top

[U78] PHP：单元测试
来源：http://rnw.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://wgz.snrcjt.cn

[U79] PHP：静态分析
来源：http://ont.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://mzp.ydzc1.top

[U80] PHP：代码规范修复
来源：http://rfm.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mhh.smart0.xyz

[U81] JS：初始化项目
来源：http://rby.316326.xyz

npm init -y;  npm i express
来源：http://qwn.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://dmg.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://syu.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://cny.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://poc.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://lxv.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://vgr.bjfxy.top

[U85] JS：可选链
来源：http://omn.feifeiyinyue.top

a?.b?.c
来源：http://cod.chenlongwang.top

[U86] JS：空值合并
来源：http://tgl.fengsongda.top

a ?? b
来源：http://ojm.aizwys.cn

[U87] JS：解构默认值
来源：http://qrr.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://aev.vehdjk.com

[U88] JS：对象展开合并
来源：http://ysl.andypj.xyz

{ ...a, ...b }
来源：http://zmt.svipenyu.cn

[U89] JS：数组去重
来源：http://qps.wangshuangyany.cn

[...new Set(arr)]
来源：http://tba.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://kxc.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://sez.ivvv.top

[U91] JS：对象键值遍历
来源：http://jkr.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xou.guannengcc.top

[U92] JS：深拷贝
来源：http://rpi.aizwys.cn

structuredClone(obj)
来源：http://oem.cdnleiting.top

[U93] JS：模板字符串
来源：http://kft.ppjwa.cn

`共 ${n} 条`
来源：http://xwx.yj20258.top

[U94] JS：箭头函数
来源：http://iyk.cqqwz.cn

const double = x => x * 2;
来源：http://auz.jqgfzy.top

[U95] JS：Promise 包装
来源：http://zcu.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://tph.52xcode.cn

[U96] JS：async/await 与异常
来源：http://ume.yuanzhike.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xxi.ydjk.org.cn

[U97] JS：并发请求
来源：http://kye.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://llg.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://ekk.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cut.kuanghao11.cn

[U99] JS：事件监听
来源：http://kub.sweek.top

el.addEventListener("click", e => {})
来源：http://kpj.xziqi.cn

[U100] JS：DOM 查询
来源：http://tnl.yvedp.cn

document.querySelector(".item")
来源：http://tue.jinqigfzy.top

[U101] JS：classList 操作
来源：http://nbl.yj20258888.top

el.classList.toggle("active")
来源：http://fer.kuanghao11.cn

[U102] JS：本地存储
来源：http://sek.wangshuangyany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ztn.sweek.top

[U103] JS：定时器
来源：http://dkp.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vfd.9152youxi.cn

[U104] JS：防抖
来源：http://dnq.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygr.nanxuanxn.top

[U105] JS：节流
来源：http://rul.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gog.sweek.top

[U106] JS：日期格式化
来源：http://rlh.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nkq.guowangkeji.top

[U107] JS：数字千分位
来源：http://hcs.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wdt.ctjpmb.com

[U108] JS：随机整数
来源：http://ivu.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qxf.ppjwa.cn

[U109] JS：数组分组
来源：http://fpo.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://zov.cdnleiting.top

[U110] JS：数组分块
来源：http://frz.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dwm.pycfn.com

[U111] JS：对象转 Map
来源：http://hsj.shanyushiyangkeji.top

new Map(Object.entries(obj))
来源：http://iuo.sweek.top

[U112] JS：字符串补位
来源：http://xfe.ydjk.org.cn

"7".padStart(3, "0")
来源：http://cvc.jinghuilouyu.cn

[U113] JS：正则替换全部
来源：http://jyo.hesvh.cn

s.replaceAll("a", "b")
来源：http://utm.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://kvz.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xxq.sxryk.cn

[U115] JS：生成 UUID
来源：http://awt.daxiang520.top

crypto.randomUUID()
来源：http://pzv.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://cbe.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://bjf.zdbjq.cn

[U117] JS：单元测试
来源：http://gbc.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://mjf.jyoumei.cn

[U118] JS：开发服务器
来源：http://jsz.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://lah.zhengqikj.top

[U119] JS：生产构建
来源：http://rfx.pycfn.com

npx vite build
来源：http://dbk.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://ppl.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://axh.guannengcc.top

================================================================================
来源：http://tsb.sxryk.cn

统计汇总
来源：http://gyd.zhoulong.xyz

================================================================================
来源：http://ffa.aibaodan.cn

按语言统计（条）：
来源：http://omq.hnxiangtu.top

Python ......... 252
来源：http://iri.jlsjyb.cn

PHP ............ 252
来源：http://ilj.ybcxt.top

JavaScript ..... 252
来源：http://cwz.gaohongyu789.top

TypeScript ..... 212
来源：http://gmb.hcnkem.com

Java ........... 212
来源：http://rgt.yj20258888.top

Go ............. 212
来源：http://uzz.hammf.cn

Ruby ........... 212
来源：http://wtd.tanke756.top

C# ............. 212
来源：http://rzw.yfazqb.com

C .............. 30
来源：http://xck.gotoacloud.top

C++ ............ 30
来源：http://pwj.fanxiaobao.xyz

SQL ............ 90
来源：http://naq.zdbjq.cn

Bash ........... 80
来源：http://fod.ivvv.top

Kotlin ......... 15
来源：http://cpk.316326.xyz

Swift .......... 15
来源：http://rss.ywan-chungtsiang.top

Lua ............ 10
来源：http://wlu.sjlbkw.cn

Perl ........... 10
来源：http://wae.cashguo.top

Scala .......... 10
来源：http://gkf.fktsv.cn

------------------------------------
来源：http://lkj.svipenyu.cn

合计 ........... 2106 条
来源：http://jgw.zdbjq.cn

按章节统计：
来源：http://hfz.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vpq.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lkt.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yyj.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ymq.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hje.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://byc.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nxs.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ysa.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bgb.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kyo.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fmh.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ogr.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iyk.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vuk.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cyl.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ycu.wangshuangyany.cn

Q SQL 专题                              90
来源：http://kxo.shzxlz.cn

R Bash 专题                             80
来源：http://mut.cqqwz.cn

S C / C++ 专题                          60
来源：http://fnq.epnwcf.com

T 其他语言补充                          60
来源：http://nji.fzhhl.top

U 高频实用片段                         120
来源：http://gjq.feifeiyinyue.top

------------------------------------
来源：http://nwv.daxiang520.top

合计                                  2106 条
来源：http://wpa.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://hvx.sweek.top

使用提醒
来源：http://vtl.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://xpo.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ybt.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mtn.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://byk.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://yeq.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ady.gotoacloud.top

—— 文件结束 ——
来源：http://hja.birdmap.top

================================================================================
来源：http://qvn.aizwys.cn

程序语言常见例子速查手册（2024 版）
来源：http://wvu.cheryme.top

Common Programming Examples Cheat Book
来源：http://dqi.feifeiyinyue.top

================================================================================
来源：http://dle.tian-w.cn

【收录内容】
来源：http://srn.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nmx.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xxp.zdbjq.cn

SQL · Bash · C · C++
来源：http://ihf.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://psy.hysaishi.cn

【使用说明】
来源：http://hon.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mqu.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rbv.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ses.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aoe.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lxg.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ptr.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://spr.wangshuangyany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aag.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bxz.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bbd.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qhv.mhx1999.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hmw.ivvv.top

【文件统计】
来源：http://jqo.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rjz.tian-w.cn

--------------------------------------------------------------------------------
来源：http://fmz.vehdjk.com

目  录
来源：http://bqg.smart0.xyz

--------------------------------------------------------------------------------
来源：http://wqx.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sgl.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rry.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pnc.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://axv.yvedp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://spi.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lnl.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jpy.hammf.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oyh.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zmx.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kdi.hysaishi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://chm.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ztp.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxw.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dhf.zhoulong.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ieu.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mgq.jlsjyb.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nap.jqgufenzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lrc.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xjo.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pxe.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qhf.fktsv.cn

================================================================================
来源：http://hfh.dashuyun.cn

A. 基础语法与类型
来源：http://key.wangshuangyany.cn

================================================================================
来源：http://ldx.c1oappe.top

[A01] Hello World
来源：http://fma.sxryk.cn

Py:   print("Hello, World!")
来源：http://loc.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://kvy.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://fuw.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oho.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://anx.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://mbg.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://rmr.yj202588.top

C#:   Console.WriteLine("Hello, World!");
来源：http://quk.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://kmr.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vlv.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://mqy.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gqo.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://woa.sufxvd.cn

Java: String name = "Alex"; int age = 20;
来源：http://qkj.jinqigfzy.top

Go:   name := "Alex"; age := 20
来源：http://dxo.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://gst.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hnn.gogol.net.cn

[A03] 常量定义
来源：http://muo.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ast.meibo888.top

PHP:  const PI = 3.14159;
来源：http://wrd.jinqigfzy.top

JS:   const PI = 3.14159;
来源：http://uua.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://qsn.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://drv.zhengqikj.top

Go:   const PI = 3.14159
来源：http://xou.fktsv.cn

Ruby: PI = 3.14159
来源：http://hik.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://ykb.hnqzz.top

[A04] 判断变量类型
来源：http://dbq.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://jwx.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mhy.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eyc.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://cww.quarkkingdee.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iaa.zdqjudy.top


<!-- 参考信息 -->