代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://usm.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://skh.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://lnk.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wav.xziqi.cn

[U43] PHP：声明命名空间
来源：http://cfd.ywan-chungtsiang.top

namespace App\Http;
来源：http://gci.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://vxt.zdbjq.cn

declare(strict_types=1);
来源：http://tja.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://bcb.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xdo.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://gqp.hcnkem.com

?string $name = null
来源：http://ukn.sjlbkw.cn

[U47] PHP：联合类型
来源：http://gub.shuidangran.top

int|string $id
来源：http://vir.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://kki.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kwv.dianchejie.cn

[U49] PHP：只读属性
来源：http://qya.feifeiyinyue.top

public readonly string $name
来源：http://bsu.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://wqa.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://hkg.chenlongwang.top

[U51] PHP：数组解构
来源：http://zgd.bjfxy.top

[$a, $b] = $arr;
来源：http://whw.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://gej.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://yvg.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://lln.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://bvp.jqgfzy.top

[U54] PHP：空安全调用
来源：http://ryx.cqqwz.cn

$obj?->method()
来源：http://plh.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://wol.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pyi.0kj1m.cn

[U56] PHP：命名参数
来源：http://rlu.cdnleiting.top

f(a: 1, b: 2)
来源：http://eir.havefunace.top

[U57] PHP：字符串插值
来源：http://klt.svipenyu.cn

"值: {$a}"
来源：http://uca.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://zwe.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zro.chenzaomai.com

[U59] PHP：自定义排序
来源：http://dep.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nwt.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://xyd.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ouh.aibaodan.cn

[U61] PHP：正则
来源：http://ifa.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lxp.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://csb.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xix.dashuyun.cn

[U63] PHP：文件读写
来源：http://euq.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ecl.cqqwz.cn

[U64] PHP：目录遍历
来源：http://kcc.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://udb.cashguo.top

[U65] PHP：会话
来源：http://crq.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://oft.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://aje.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zlh.tian-w.cn

[U67] PHP：处理文件上传
来源：http://qdo.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nze.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://ohy.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://biq.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://fwu.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fmf.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://ahs.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sle.xziqi.cn

[U71] PHP：抛出异常
来源：http://seu.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://jpb.nanxinkj.top

[U72] PHP：写错误日志
来源：http://hgl.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://axa.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://ace.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://aag.havefunace.top

[U74] PHP：读取环境变量
来源：http://odr.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://nat.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://rrf.hywenlv.cn

composer require psr/container
来源：http://huf.0kj1m.cn

[U76] PHP：简单路由
来源：http://fxs.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jsy.shzxlz.cn

[U77] PHP：模板渲染
来源：http://ljw.jinyuanbaomall.cn

composer require twig/twig
来源：http://jbc.hnxiangtu.top

[U78] PHP：单元测试
来源：http://alr.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://pit.uphjek.com

[U79] PHP：静态分析
来源：http://ykt.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://txp.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://dmi.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://oka.gaohongyu789.top

[U81] JS：初始化项目
来源：http://nzs.c1oappe.top

npm init -y;  npm i express
来源：http://gvd.tanke756.top

[U82] JS：package.json 脚本
来源：http://xcp.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://afa.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://ltn.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pzf.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://moc.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://kbr.fehbvm.com

[U85] JS：可选链
来源：http://iwn.jqgufenzy.top

a?.b?.c
来源：http://tvr.cheryme.top

[U86] JS：空值合并
来源：http://fzo.ppjwa.cn

a ?? b
来源：http://whh.vqdsnc.cn

[U87] JS：解构默认值
来源：http://fsx.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://dph.bbcook.cn

[U88] JS：对象展开合并
来源：http://gkq.chenlongwang.top

{ ...a, ...b }
来源：http://dwr.xinyue.icu

[U89] JS：数组去重
来源：http://ijq.aibaodan.cn

[...new Set(arr)]
来源：http://mjk.gotoacloud.top

[U90] JS：数字数组排序
来源：http://lmy.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://lif.bjfxy.top

[U91] JS：对象键值遍历
来源：http://qnj.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qgk.zhongyouzk.top

[U92] JS：深拷贝
来源：http://nrn.guowangkeji.top

structuredClone(obj)
来源：http://mch.nanxinkj.top

[U93] JS：模板字符串
来源：http://smy.mhx1999.top

`共 ${n} 条`
来源：http://hmv.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://lhi.fzhhl.top

const double = x => x * 2;
来源：http://ezg.daria6918.cn

[U95] JS：Promise 包装
来源：http://znx.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://aol.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://dnj.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nov.zhixingplan.top

[U97] JS：并发请求
来源：http://twt.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vfw.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://swe.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ttu.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://lyw.fktsv.cn

el.addEventListener("click", e => {})
来源：http://idg.gogol.net.cn

[U100] JS：DOM 查询
来源：http://bqs.ydjk.org.cn

document.querySelector(".item")
来源：http://mhl.aizwys.cn

[U101] JS：classList 操作
来源：http://emb.birdmap.top

el.classList.toggle("active")
来源：http://vmq.hnxiangtu.top

[U102] JS：本地存储
来源：http://okv.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xnd.sxryk.cn

[U103] JS：定时器
来源：http://tur.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nkk.hywenlv.cn

[U104] JS：防抖
来源：http://bls.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyr.9152youxi.cn

[U105] JS：节流
来源：http://mau.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blg.sweek.top

[U106] JS：日期格式化
来源：http://lzp.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://orq.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://cqx.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nwl.fengsongda.top

[U108] JS：随机整数
来源：http://tun.jqgufenzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iro.tian-w.cn

[U109] JS：数组分组
来源：http://oel.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://zxt.hongshengwenyu.top

[U110] JS：数组分块
来源：http://crr.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oer.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://xkr.tanke756.top

new Map(Object.entries(obj))
来源：http://jin.yj20258888.top

[U112] JS：字符串补位
来源：http://gyv.vehdjk.com

"7".padStart(3, "0")
来源：http://xyv.jiagoushi.top

[U113] JS：正则替换全部
来源：http://vbt.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://alc.cucudq.cn

[U114] JS：JSON 深比较
来源：http://vui.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kgv.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://cmf.hammf.cn

crypto.randomUUID()
来源：http://nfl.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://tbb.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://dqp.jqgfzy.top

[U117] JS：单元测试
来源：http://owf.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://oks.nwbrower.top

[U118] JS：开发服务器
来源：http://ddu.sufxvd.cn

npm i -D vite;  npx vite
来源：http://yvd.havefunace.top

[U119] JS：生产构建
来源：http://zvg.xylfe.cn

npx vite build
来源：http://lzq.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://lhp.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://njy.yueranfly.top

================================================================================
来源：http://way.yfazqb.com

统计汇总
来源：http://hkq.316326.xyz

================================================================================
来源：http://usx.hesvh.cn

按语言统计（条）：
来源：http://vto.xinyue.icu

Python ......... 252
来源：http://oou.redwolf501.top

PHP ............ 252
来源：http://qrd.dashuyun.cn

JavaScript ..... 252
来源：http://ucf.hnqzz.top

TypeScript ..... 212
来源：http://olz.guowangkeji.top

Java ........... 212
来源：http://glk.sxryk.cn

Go ............. 212
来源：http://hhc.gogol.net.cn

Ruby ........... 212
来源：http://eoi.iojbl.cn

C# ............. 212
来源：http://nxk.fengsongda.top

C .............. 30
来源：http://jij.fanxiaobao.xyz

C++ ............ 30
来源：http://zoc.hcnkem.com

SQL ............ 90
来源：http://nkk.zhixingplan.top

Bash ........... 80
来源：http://esz.pengpengdd.cyou

Kotlin ......... 15
来源：http://lri.guannengcc.top

Swift .......... 15
来源：http://wsh.yangfankeji.com

Lua ............ 10
来源：http://atx.tianlin.xyz

Perl ........... 10
来源：http://sss.birdmap.top

Scala .......... 10
来源：http://ugp.ydzc1.top

------------------------------------
来源：http://kqp.tianlin.xyz

合计 ........... 2106 条
来源：http://adv.fktsv.cn

按章节统计：
来源：http://ckw.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tlq.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rho.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jab.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ngo.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jkq.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tnu.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tcb.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eou.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lek.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hbg.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xrr.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fts.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zkg.vehdjk.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://diu.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://azc.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cup.nwbrower.top

Q SQL 专题                              90
来源：http://iku.hesvh.cn

R Bash 专题                             80
来源：http://buo.quarkkingdee.top

S C / C++ 专题                          60
来源：http://piu.daxiang520.top

T 其他语言补充                          60
来源：http://fya.tianlin.xyz

U 高频实用片段                         120
来源：http://vto.dianchejie.cn

------------------------------------
来源：http://cda.tian-w.cn

合计                                  2106 条
来源：http://bwv.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://kzf.cqqwz.cn

使用提醒
来源：http://vil.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://yws.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://seh.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://igl.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wrn.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tja.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jsz.shuidangran.top

—— 文件结束 ——
来源：http://hjg.guannengcc.top

================================================================================
来源：http://lfo.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://jev.aizwys.cn

Common Programming Examples Cheat Book
来源：http://lok.uphjek.com

================================================================================
来源：http://inb.sxryk.cn

【收录内容】
来源：http://mwa.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gnn.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qbh.tian-w.cn

SQL · Bash · C · C++
来源：http://afn.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ggw.chenjidiqi.icu

【使用说明】
来源：http://oge.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tcg.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zja.sjlbkw.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zem.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uni.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wek.hammf.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sox.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wsh.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://erv.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lco.yj20258.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ton.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mde.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pca.ppjwa.cn

【文件统计】
来源：http://uph.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cyk.jianghu66.top

--------------------------------------------------------------------------------
来源：http://uky.ydzc1.top

目  录
来源：http://eiy.meibo888.top

--------------------------------------------------------------------------------
来源：http://tts.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tae.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jgy.cheryme.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mtw.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wqo.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://puj.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bum.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://txt.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://foc.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://azu.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://caf.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zdv.zhaomingkeji.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jkc.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://odh.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rzt.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cya.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bxz.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cbd.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lgn.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jrc.ctjpmb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gjl.cucudq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qfb.snrcjt.cn

================================================================================
来源：http://xnv.ctjpmb.com

A. 基础语法与类型
来源：http://jyn.ydjk.org.cn

================================================================================
来源：http://otv.cucudq.cn

[A01] Hello World
来源：http://diy.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://wll.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://lvb.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://xpf.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lok.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://zgn.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://ddq.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://dqr.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://omm.ctjpmb.com

[A02] 变量声明与赋值
来源：http://cig.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mfq.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://csq.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://lpm.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jzj.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://fxh.bjfxy.top

Go:   name := "Alex"; age := 20
来源：http://pjd.sweek.top

Ruby: name = "Alex"; age = 20
来源：http://mds.cheryme.top

C#:   string name = "Alex"; int age = 20;
来源：http://xhg.zhongyouzk.top

[A03] 常量定义
来源：http://qtb.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://alh.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://hco.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://qcw.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://koj.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://gop.yj202588.top

Go:   const PI = 3.14159
来源：http://mjw.9152youxi.cn

Ruby: PI = 3.14159
来源：http://plz.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://zew.zdbjq.cn

[A04] 判断变量类型
来源：http://ijf.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qhg.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hhi.feifeiyinyue.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ffz.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://tmd.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://scy.zhixingplan.top


<!-- 参考信息 -->