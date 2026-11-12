代发 wailian999

[U43] PHP：声明命名空间
来源：http://dgr.yvedp.cn

namespace App\Http;
来源：http://qbo.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://zbp.haohaochexian.top

declare(strict_types=1);
来源：http://ysl.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://hgz.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jmv.52xcode.cn

[U46] PHP：可空类型
来源：http://fyy.vqdsnc.cn

?string $name = null
来源：http://udg.zdqjudy.top

[U47] PHP：联合类型
来源：http://ryo.snrcjt.cn

int|string $id
来源：http://nhy.fengsongda.top

[U48] PHP：纯枚举
来源：http://nqu.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ond.c1oappe.top

[U49] PHP：只读属性
来源：http://jin.yj202588.top

public readonly string $name
来源：http://vqq.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://fnz.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://nxo.zhongyouzk.top

[U51] PHP：数组解构
来源：http://xxb.jianghu66.top

[$a, $b] = $arr;
来源：http://mpi.yuxming.cn

[U52] PHP：箭头函数
来源：http://xnv.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://syk.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://mgm.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://kbn.yangfankeji.com

[U54] PHP：空安全调用
来源：http://yfa.vqdsnc.cn

$obj?->method()
来源：http://fqf.guannengcc.top

[U55] PHP：match 表达式
来源：http://wwz.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://msx.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://nwg.yvedp.cn

f(a: 1, b: 2)
来源：http://vtl.yj202588.top

[U57] PHP：字符串插值
来源：http://nnj.hongshengwenyu.top

"值: {$a}"
来源：http://kic.dianchejie.cn

[U58] PHP：数组三件套
来源：http://mwl.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dbk.yueranfly.top

[U59] PHP：自定义排序
来源：http://lmr.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bqq.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://nrm.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://byg.gaohongyu789.top

[U61] PHP：正则
来源：http://hct.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ial.jyoumei.cn

[U62] PHP：日期对象
来源：http://edw.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ifg.havefunace.top

[U63] PHP：文件读写
来源：http://pvs.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hzq.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://xdj.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://itk.vqdsnc.cn

[U65] PHP：会话
来源：http://wou.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gyg.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://buc.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yhf.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://qku.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qxb.xylfe.cn

[U68] PHP：PDO 连接
来源：http://cpf.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nrd.hnqzz.top

[U69] PHP：PDO 预处理
来源：http://swj.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eeo.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://nhk.zdqjudy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xpv.vehdjk.com

[U71] PHP：抛出异常
来源：http://aai.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://xvo.snrcjt.cn

[U72] PHP：写错误日志
来源：http://dsk.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://nda.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://uha.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://tjj.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://imt.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://mat.shuidangran.top

[U75] PHP：依赖注入
来源：http://bes.316326.xyz

composer require psr/container
来源：http://ntk.tianlin.xyz

[U76] PHP：简单路由
来源：http://lvc.xylfe.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zfg.yueranfly.top

[U77] PHP：模板渲染
来源：http://hof.316326.xyz

composer require twig/twig
来源：http://uly.redwolf501.top

[U78] PHP：单元测试
来源：http://mlg.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://imd.hnxiangtu.top

[U79] PHP：静态分析
来源：http://zxa.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://fxm.daxiang520.top

[U80] PHP：代码规范修复
来源：http://ypk.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lbw.zdqjudy.top

[U81] JS：初始化项目
来源：http://srf.wangshuangyany.cn

npm init -y;  npm i express
来源：http://eha.fehbvm.com

[U82] JS：package.json 脚本
来源：http://aah.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zfg.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://osn.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://opa.316326.xyz

[U84] JS：CommonJS 写法
来源：http://dgw.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ofi.quarkkingdee.top

[U85] JS：可选链
来源：http://abb.chenjidiqi.icu

a?.b?.c
来源：http://twr.ivvv.top

[U86] JS：空值合并
来源：http://lxs.jinyuanbaomall.cn

a ?? b
来源：http://ytl.fehbvm.com

[U87] JS：解构默认值
来源：http://ymk.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://tcn.yongpay.top

[U88] JS：对象展开合并
来源：http://wao.yuxming.cn

{ ...a, ...b }
来源：http://poy.jinqigfzy.top

[U89] JS：数组去重
来源：http://phn.hysaishi.cn

[...new Set(arr)]
来源：http://uhl.tian-w.cn

[U90] JS：数字数组排序
来源：http://fmk.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://nrk.gzhubu.top

[U91] JS：对象键值遍历
来源：http://gwj.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://myo.aizwys.cn

[U92] JS：深拷贝
来源：http://fhd.feifeiyinyue.top

structuredClone(obj)
来源：http://zzx.jiagoushi.top

[U93] JS：模板字符串
来源：http://fkt.gogol.net.cn

`共 ${n} 条`
来源：http://pji.zhijiandao.cn

[U94] JS：箭头函数
来源：http://fka.yj202588.top

const double = x => x * 2;
来源：http://hpt.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://cgj.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://qbq.zycfv.cn

[U96] JS：async/await 与异常
来源：http://cqc.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jlx.dianchejie.cn

[U97] JS：并发请求
来源：http://opm.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rbn.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://tpu.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iki.fehbvm.com

[U99] JS：事件监听
来源：http://xge.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://ooo.52xcode.cn

[U100] JS：DOM 查询
来源：http://xlw.zhengqikj.top

document.querySelector(".item")
来源：http://msy.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://slk.ctjpmb.com

el.classList.toggle("active")
来源：http://lvn.snrcjt.cn

[U102] JS：本地存储
来源：http://pqz.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yev.hammf.cn

[U103] JS：定时器
来源：http://mom.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eir.guannengcc.top

[U104] JS：防抖
来源：http://cyg.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bvn.sjlbkw.cn

[U105] JS：节流
来源：http://eqi.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ihs.iojbl.cn

[U106] JS：日期格式化
来源：http://kvh.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://owf.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://qdu.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gdi.zdbjq.cn

[U108] JS：随机整数
来源：http://smi.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vkb.ctjpmb.com

[U109] JS：数组分组
来源：http://dpo.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://jmu.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://ghw.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://piu.jqgfzy.top

[U111] JS：对象转 Map
来源：http://ofr.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://ist.mhx1999.top

[U112] JS：字符串补位
来源：http://tyd.jqgufenzy.top

"7".padStart(3, "0")
来源：http://eve.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://tkq.jqgfzy.top

s.replaceAll("a", "b")
来源：http://tcj.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://svj.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ffm.meibo888.top

[U115] JS：生成 UUID
来源：http://pwr.guowangkeji.top

crypto.randomUUID()
来源：http://cns.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://eqo.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://lkw.316326.xyz

[U117] JS：单元测试
来源：http://wiw.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://tzt.yvedp.cn

[U118] JS：开发服务器
来源：http://dvq.hesvh.cn

npm i -D vite;  npx vite
来源：http://mzw.ydjk.org.cn

[U119] JS：生产构建
来源：http://qqc.sxryk.cn

npx vite build
来源：http://xed.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://sbd.tarul.cn

import.meta.env.VITE_API_URL
来源：http://ypq.havefunace.top

================================================================================
来源：http://eoj.hesvh.cn

统计汇总
来源：http://vdl.feifeiyinyue.top

================================================================================
来源：http://uts.ybcxt.top

按语言统计（条）：
来源：http://gyf.xziqi.cn

Python ......... 252
来源：http://xvq.yj20258.top

PHP ............ 252
来源：http://ygm.pycfn.com

JavaScript ..... 252
来源：http://bhs.hammf.cn

TypeScript ..... 212
来源：http://rsm.tianlin.xyz

Java ........... 212
来源：http://gxh.zhixingplan.top

Go ............. 212
来源：http://abj.fzhhl.top

Ruby ........... 212
来源：http://rmw.mhx1999.top

C# ............. 212
来源：http://tel.yonumen.top

C .............. 30
来源：http://pjb.tianlin.xyz

C++ ............ 30
来源：http://vms.zycfv.cn

SQL ............ 90
来源：http://ril.zhoulong.xyz

Bash ........... 80
来源：http://qjs.tarul.cn

Kotlin ......... 15
来源：http://kbw.hfpthk.cn

Swift .......... 15
来源：http://ygo.hammf.cn

Lua ............ 10
来源：http://sdp.hammf.cn

Perl ........... 10
来源：http://obd.cdnleiting.top

Scala .......... 10
来源：http://sir.yueranfly.top

------------------------------------
来源：http://zan.feifeiyinyue.top

合计 ........... 2106 条
来源：http://boy.zhongyouzk.top

按章节统计：
来源：http://rvf.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ajn.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://umk.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vpt.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jyo.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nps.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oie.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bkg.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pnd.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ufh.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xhc.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ivn.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yrj.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://frq.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://riv.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vqm.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xqa.shuidangran.top

Q SQL 专题                              90
来源：http://mds.meibo888.top

R Bash 专题                             80
来源：http://ghi.fktsv.cn

S C / C++ 专题                          60
来源：http://its.fengsongda.top

T 其他语言补充                          60
来源：http://oku.yuxming.cn

U 高频实用片段                         120
来源：http://jot.wangdashe.top

------------------------------------
来源：http://iuc.jlsjyb.cn

合计                                  2106 条
来源：http://epz.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://nwe.ywan-chungtsiang.top

使用提醒
来源：http://jaw.smart0.xyz

--------------------------------------------------------------------------------
来源：http://vcr.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kas.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://biw.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yav.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://vlm.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://trz.zhongyouzk.top

—— 文件结束 ——
来源：http://tne.ivvv.top

================================================================================
来源：http://jcb.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://bpz.xziqi.cn

Common Programming Examples Cheat Book
来源：http://bqq.yongpay.top

================================================================================
来源：http://ilt.9152youxi.cn

【收录内容】
来源：http://meb.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vjl.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vei.guowangkeji.top

SQL · Bash · C · C++
来源：http://xip.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lmu.bjfxy.top

【使用说明】
来源：http://ekz.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xqr.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tgm.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://quv.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qsw.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://pwb.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zsk.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pqw.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cch.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tqh.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tam.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ymg.guannengcc.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kbw.hongshengwenyu.top

【文件统计】
来源：http://vwr.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mvj.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://fjk.zhongyouzk.top

目  录
来源：http://lot.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://stt.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yib.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xau.316326.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://etg.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yal.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gye.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ezk.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ntr.gzhubu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zmh.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zvf.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://elq.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fhb.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://guy.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jed.ybcxt.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nqq.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rav.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cft.jyoumei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://phn.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fbf.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://guu.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bvp.hcnkem.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qkk.sxryk.cn

================================================================================
来源：http://mxj.guowangkeji.top

A. 基础语法与类型
来源：http://jvh.fzhhl.top

================================================================================
来源：http://ofy.pycfn.com

[A01] Hello World
来源：http://ata.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://qlh.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://coa.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://vrz.xinyue.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ezo.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://pgl.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://obr.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://fms.kuanghao11.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bpp.chenzaomai.com

[A02] 变量声明与赋值
来源：http://vcx.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zzc.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fhv.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://ged.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://csp.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://ook.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://vwm.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://zxu.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wmj.hammf.cn

[A03] 常量定义
来源：http://jog.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xsv.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://plp.cashguo.top

JS:   const PI = 3.14159;
来源：http://txt.yvedp.cn

TS:   const PI: number = 3.14159;
来源：http://vug.wangshuangyany.cn

Java: static final double PI = 3.14159;
来源：http://yiy.cdnleiting.top

Go:   const PI = 3.14159
来源：http://fnd.ydzc1.top

Ruby: PI = 3.14159
来源：http://utl.pycfn.com

C#:   const double PI = 3.14159;
来源：http://okk.cqqwz.cn

[A04] 判断变量类型
来源：http://scv.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ran.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://czd.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xjc.sweek.top

TS:   typeof x; x instanceof Date
来源：http://fte.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yfb.xylfe.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pvj.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kuf.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://klw.gaohongyu789.top

[A05] 整数除法与取模
来源：http://byv.sweek.top


<!-- 参考信息 -->