代发 wailian999

[U43] PHP：声明命名空间
来源：http://rdz.ywan-chungtsiang.top

namespace App\Http;
来源：http://doe.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://cxw.jinqigfzy.top

declare(strict_types=1);
来源：http://ldp.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://daf.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oyb.dianchejie.cn

[U46] PHP：可空类型
来源：http://gqh.gotoacloud.top

?string $name = null
来源：http://huz.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://oxr.tanke756.top

int|string $id
来源：http://roj.tian-w.cn

[U48] PHP：纯枚举
来源：http://zei.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wls.aibaodan.cn

[U49] PHP：只读属性
来源：http://pog.pengpengdd.cyou

public readonly string $name
来源：http://blc.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://pme.xuanzx.com

public function __construct(private int $id) {}
来源：http://qum.jlsjyb.cn

[U51] PHP：数组解构
来源：http://min.nanxuanxn.top

[$a, $b] = $arr;
来源：http://kzu.nwbrower.top

[U52] PHP：箭头函数
来源：http://sgd.tanke756.top

$double = fn($x) => $x * 2;
来源：http://afh.zycfv.cn

[U53] PHP：空合并运算符
来源：http://clf.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://owx.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://fcv.aibaodan.cn

$obj?->method()
来源：http://azu.svipenyu.cn

[U55] PHP：match 表达式
来源：http://ztu.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ahl.andypj.xyz

[U56] PHP：命名参数
来源：http://kok.birdmap.top

f(a: 1, b: 2)
来源：http://bwc.tarul.cn

[U57] PHP：字符串插值
来源：http://kll.snrcjt.cn

"值: {$a}"
来源：http://fki.tianlin.xyz

[U58] PHP：数组三件套
来源：http://qvk.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kwf.redwolf501.top

[U59] PHP：自定义排序
来源：http://elz.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iiy.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://fdd.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ajm.chenlongwang.top

[U61] PHP：正则
来源：http://eba.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lcx.zycfv.cn

[U62] PHP：日期对象
来源：http://uha.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bue.jlsjyb.cn

[U63] PHP：文件读写
来源：http://mhi.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rml.uphjek.com

[U64] PHP：目录遍历
来源：http://xva.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://xdj.fanxiaobao.xyz

[U65] PHP：会话
来源：http://gkv.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rsj.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://fzi.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iap.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://ope.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kaz.fktsv.cn

[U68] PHP：PDO 连接
来源：http://kbl.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fje.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://skg.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tko.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://ayt.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhs.52xcode.cn

[U71] PHP：抛出异常
来源：http://ree.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://ayz.jinqigufen.top

[U72] PHP：写错误日志
来源：http://jtx.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://ohj.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://lll.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://qhc.gzhubu.top

[U74] PHP：读取环境变量
来源：http://dqh.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://vyl.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://ypx.shangyingyoupin.top

composer require psr/container
来源：http://snz.yj202588.top

[U76] PHP：简单路由
来源：http://acr.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mgk.yvedp.cn

[U77] PHP：模板渲染
来源：http://bpo.yangfankeji.com

composer require twig/twig
来源：http://lvh.316326.xyz

[U78] PHP：单元测试
来源：http://sil.316326.xyz

composer require --dev phpunit/phpunit
来源：http://oir.yanxiufei.cn

[U79] PHP：静态分析
来源：http://oet.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://zot.yonumen.top

[U80] PHP：代码规范修复
来源：http://pmu.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://scv.fktsv.cn

[U81] JS：初始化项目
来源：http://bfq.vehdjk.com

npm init -y;  npm i express
来源：http://oll.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://xmu.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cbh.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://amv.yj20258888.top

export const a = 1;  import { a } from "./m.js";
来源：http://xeu.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://uvi.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://ctg.haohaochexian.top

[U85] JS：可选链
来源：http://tww.haohaochexian.top

a?.b?.c
来源：http://eod.tianlin.xyz

[U86] JS：空值合并
来源：http://lux.hysaishi.cn

a ?? b
来源：http://mwg.xziqi.cn

[U87] JS：解构默认值
来源：http://xsr.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://cmq.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://whb.zhengqikj.top

{ ...a, ...b }
来源：http://dik.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://tkv.sxryk.cn

[...new Set(arr)]
来源：http://scy.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://mmr.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://sbx.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://axb.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rin.sufxvd.cn

[U92] JS：深拷贝
来源：http://pkq.c1oappe.top

structuredClone(obj)
来源：http://roe.epnwcf.com

[U93] JS：模板字符串
来源：http://sga.tanke756.top

`共 ${n} 条`
来源：http://smn.cheryme.top

[U94] JS：箭头函数
来源：http://ucr.hnqzz.top

const double = x => x * 2;
来源：http://obh.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://flt.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://cbq.yuanzhike.top

[U96] JS：async/await 与异常
来源：http://vcx.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fij.jyoumei.cn

[U97] JS：并发请求
来源：http://abg.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jyt.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://zmk.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ier.iojbl.cn

[U99] JS：事件监听
来源：http://yhl.yuxming.cn

el.addEventListener("click", e => {})
来源：http://qif.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://afx.yongpay.top

document.querySelector(".item")
来源：http://obh.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://cxc.ydjk.org.cn

el.classList.toggle("active")
来源：http://cqe.nanxinkj.top

[U102] JS：本地存储
来源：http://htd.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ina.fanxiaobao.xyz

[U103] JS：定时器
来源：http://vkx.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zsh.nwbrower.top

[U104] JS：防抖
来源：http://oyn.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpn.birdmap.top

[U105] JS：节流
来源：http://ywo.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lqw.aizwys.cn

[U106] JS：日期格式化
来源：http://wic.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tel.sysykeji.top

[U107] JS：数字千分位
来源：http://ovd.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ean.hnqzz.top

[U108] JS：随机整数
来源：http://rip.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://keu.hnqzz.top

[U109] JS：数组分组
来源：http://kfi.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://stv.xuetiantiany.cn

[U110] JS：数组分块
来源：http://aoh.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://psi.shzxlz.cn

[U111] JS：对象转 Map
来源：http://uwb.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://uso.dashuyun.cn

[U112] JS：字符串补位
来源：http://pwz.hnqzz.top

"7".padStart(3, "0")
来源：http://bcr.shuidangran.top

[U113] JS：正则替换全部
来源：http://ign.gogol.net.cn

s.replaceAll("a", "b")
来源：http://cxg.hammf.cn

[U114] JS：JSON 深比较
来源：http://mfp.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://gbd.tarul.cn

[U115] JS：生成 UUID
来源：http://vaa.chenjidiqi.icu

crypto.randomUUID()
来源：http://sgn.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://sgf.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://kht.zdqjudy.top

[U117] JS：单元测试
来源：http://lng.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://gpe.zhengqikj.top

[U118] JS：开发服务器
来源：http://jex.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://gnv.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://oik.dashuyun.cn

npx vite build
来源：http://vdl.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://ecr.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://cpa.jianghu66.top

================================================================================
来源：http://nrm.snrcjt.cn

统计汇总
来源：http://vdk.guannengcc.top

================================================================================
来源：http://jnn.yanxiufei.cn

按语言统计（条）：
来源：http://gnb.hnqzz.top

Python ......... 252
来源：http://nlc.cdnleiting.top

PHP ............ 252
来源：http://kpv.fanxiaobao.xyz

JavaScript ..... 252
来源：http://zcj.xylfe.cn

TypeScript ..... 212
来源：http://wvm.sweek.top

Java ........... 212
来源：http://wtc.guowangkeji.top

Go ............. 212
来源：http://pwi.hongshengwenyu.top

Ruby ........... 212
来源：http://jds.uphjek.com

C# ............. 212
来源：http://hla.zycfv.cn

C .............. 30
来源：http://dfy.yangfankeji.com

C++ ............ 30
来源：http://zok.jinghuilouyu.cn

SQL ............ 90
来源：http://moq.uphjek.com

Bash ........... 80
来源：http://ted.hfpthk.cn

Kotlin ......... 15
来源：http://dmv.wangshuangyany.cn

Swift .......... 15
来源：http://rbg.yuxming.cn

Lua ............ 10
来源：http://buv.tian-w.cn

Perl ........... 10
来源：http://yxn.bbcook.cn

Scala .......... 10
来源：http://xfv.yj20258888.top

------------------------------------
来源：http://ebz.svipenyu.cn

合计 ........... 2106 条
来源：http://hcq.yvedp.cn

按章节统计：
来源：http://fzy.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://onx.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gej.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://shh.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xji.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qtd.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://igi.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hkd.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lms.nwbrower.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jfk.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://you.aizwys.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bph.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://szy.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://val.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wkq.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hnw.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zhk.chenzaomai.com

Q SQL 专题                              90
来源：http://wma.chenzaomai.com

R Bash 专题                             80
来源：http://kzb.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://dby.cheryme.top

T 其他语言补充                          60
来源：http://ykn.xylfe.cn

U 高频实用片段                         120
来源：http://tbh.xingfuxueyuan.xyz

------------------------------------
来源：http://drp.guannengcc.top

合计                                  2106 条
来源：http://wqe.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://dlb.xingfuxueyuan.xyz

使用提醒
来源：http://tnk.gzhubu.top

--------------------------------------------------------------------------------
来源：http://eez.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nwx.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uoe.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xhp.chenlongwang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lmt.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vxn.shangyingyoupin.top

—— 文件结束 ——
来源：http://oio.yfazqb.com

================================================================================
来源：http://ysd.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://lyh.tarul.cn

Common Programming Examples Cheat Book
来源：http://xie.aizwys.cn

================================================================================
来源：http://qeg.yongpay.top

【收录内容】
来源：http://tcr.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://hcn.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cxx.redwolf501.top

SQL · Bash · C · C++
来源：http://ofc.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vij.hywenlv.cn

【使用说明】
来源：http://pla.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aan.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lwt.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://swy.0kj1m.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dpp.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://aiq.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jjf.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qly.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jtb.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tac.daria6918.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bou.jqgufenzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tpg.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hqf.fktsv.cn

【文件统计】
来源：http://sdl.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ujz.havefunace.top

--------------------------------------------------------------------------------
来源：http://rqn.svipenyu.cn

目  录
来源：http://rqi.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://olv.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ixy.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mtc.yangfankeji.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gyv.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vvn.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zzu.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pqf.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ovd.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mxv.pengpengdd.cyou

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://deh.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wkx.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://imp.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zno.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jsi.9152youxi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tjj.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ime.gogol.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://anp.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sis.epnwcf.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://iwf.cheryme.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wbv.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rzq.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yuy.feifeiyinyue.top

================================================================================
来源：http://enr.hongshengwenyu.top

A. 基础语法与类型
来源：http://xwb.shuidangran.top

================================================================================
来源：http://ceu.tian-w.cn

[A01] Hello World
来源：http://znp.mhx1999.top

Py:   print("Hello, World!")
来源：http://bwz.tian-w.cn

PHP:  echo "Hello, World!";
来源：http://omv.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://mel.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://spe.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://vfx.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://atm.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://drx.ctjpmb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://cnj.wangdashe.top

[A02] 变量声明与赋值
来源：http://jui.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://glm.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xxa.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qdc.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tcb.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://qpc.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://hgu.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://ukv.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dlh.shuidangran.top

[A03] 常量定义
来源：http://rkm.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rjt.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://gyq.wangshuangyany.cn

JS:   const PI = 3.14159;
来源：http://ztl.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://gnl.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://wfp.jqgfzy.top

Go:   const PI = 3.14159
来源：http://rxj.jiagoushi.top

Ruby: PI = 3.14159
来源：http://mmu.quarkkingdee.top

C#:   const double PI = 3.14159;
来源：http://ord.gotoacloud.top

[A04] 判断变量类型
来源：http://xso.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://sez.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bmf.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pcl.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://tiz.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://soy.ehwqpu.com

Go:   reflect.TypeOf(x).Name()
来源：http://bpt.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ccv.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://uqq.daria6918.cn

[A05] 整数除法与取模
来源：http://tpv.jianghu66.top


<!-- 参考信息 -->