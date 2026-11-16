代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://ebq.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://axr.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://lek.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ark.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://shu.xinyue.icu

namespace App\Http;
来源：http://eql.gzhubu.top

[U44] PHP：开启严格类型
来源：http://xdq.fanxiaobao.xyz

declare(strict_types=1);
来源：http://iiq.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://sbk.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yjt.meibo888.top

[U46] PHP：可空类型
来源：http://shl.haohaochexian.top

?string $name = null
来源：http://kbq.yueranfly.top

[U47] PHP：联合类型
来源：http://daa.nwbrower.top

int|string $id
来源：http://ihm.wangdashe.top

[U48] PHP：纯枚举
来源：http://erq.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bce.sweek.top

[U49] PHP：只读属性
来源：http://cqd.shuidangran.top

public readonly string $name
来源：http://fwy.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://mtl.0kj1m.cn

public function __construct(private int $id) {}
来源：http://imm.yvedp.cn

[U51] PHP：数组解构
来源：http://ejl.nanxinkj.top

[$a, $b] = $arr;
来源：http://bve.gogol.net.cn

[U52] PHP：箭头函数
来源：http://idt.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://ufy.hcnkem.com

[U53] PHP：空合并运算符
来源：http://vab.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://fxm.shzxlz.cn

[U54] PHP：空安全调用
来源：http://ziv.fktsv.cn

$obj?->method()
来源：http://fjn.yuxming.cn

[U55] PHP：match 表达式
来源：http://kej.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xkx.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://wth.9152youxi.cn

f(a: 1, b: 2)
来源：http://vsy.yonumen.top

[U57] PHP：字符串插值
来源：http://mxj.zycfv.cn

"值: {$a}"
来源：http://sbb.ivvv.top

[U58] PHP：数组三件套
来源：http://pgp.hnxiangtu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pkd.0kj1m.cn

[U59] PHP：自定义排序
来源：http://tqk.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lfo.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://abw.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nie.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://grq.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://olx.vehdjk.com

[U62] PHP：日期对象
来源：http://ayh.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fzv.zycfv.cn

[U63] PHP：文件读写
来源：http://krf.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hyc.cucudq.cn

[U64] PHP：目录遍历
来源：http://ejx.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://ygt.jyoumei.cn

[U65] PHP：会话
来源：http://fua.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gso.zhiwuduotai.top

[U66] PHP：设置 Cookie
来源：http://pti.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://niq.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://jfv.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ggi.yueranfly.top

[U68] PHP：PDO 连接
来源：http://fmi.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vbr.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://rdk.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ruy.wangdashe.top

[U70] PHP：PDO 事务
来源：http://yoa.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qas.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://tun.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://hqj.ppjwa.cn

[U72] PHP：写错误日志
来源：http://zid.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://ubx.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://maq.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://thl.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://gyk.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://hqg.sxryk.cn

[U75] PHP：依赖注入
来源：http://mdt.andypj.xyz

composer require psr/container
来源：http://qep.xuanzx.com

[U76] PHP：简单路由
来源：http://ehd.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lnj.aizwys.cn

[U77] PHP：模板渲染
来源：http://grw.bjfxy.top

composer require twig/twig
来源：http://mzn.fzhhl.top

[U78] PHP：单元测试
来源：http://zrj.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://xxy.0kj1m.cn

[U79] PHP：静态分析
来源：http://jsa.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://cnj.cheryme.top

[U80] PHP：代码规范修复
来源：http://ltb.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cfz.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://osi.vqdsnc.cn

npm init -y;  npm i express
来源：http://koy.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://fgu.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sgd.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://iro.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://jpy.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://roc.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mud.fzhhl.top

[U85] JS：可选链
来源：http://msw.andypj.xyz

a?.b?.c
来源：http://tkh.feifeiyinyue.top

[U86] JS：空值合并
来源：http://ucv.tianlin.xyz

a ?? b
来源：http://ssf.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://lrq.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://xqm.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://nyz.52xcode.cn

{ ...a, ...b }
来源：http://ctj.hywenlv.cn

[U89] JS：数组去重
来源：http://pcc.iojbl.cn

[...new Set(arr)]
来源：http://vss.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://aag.zhaomingkeji.xyz

[...arr].sort((a, b) => a - b)
来源：http://ngt.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://kch.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zrf.sweek.top

[U92] JS：深拷贝
来源：http://iux.zdqjudy.top

structuredClone(obj)
来源：http://lad.hnqzz.top

[U93] JS：模板字符串
来源：http://kft.dashuyun.cn

`共 ${n} 条`
来源：http://inr.hywenlv.cn

[U94] JS：箭头函数
来源：http://uvm.guowangkeji.top

const double = x => x * 2;
来源：http://xhq.epnwcf.com

[U95] JS：Promise 包装
来源：http://rta.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://mdn.daxiang520.top

[U96] JS：async/await 与异常
来源：http://kvr.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://abf.ivvv.top

[U97] JS：并发请求
来源：http://ads.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://afq.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://app.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wmo.cashguo.top

[U99] JS：事件监听
来源：http://wjj.sweek.top

el.addEventListener("click", e => {})
来源：http://veo.yongpay.top

[U100] JS：DOM 查询
来源：http://qpq.svipenyu.cn

document.querySelector(".item")
来源：http://kex.guannengcc.top

[U101] JS：classList 操作
来源：http://ajn.ydzc1.top

el.classList.toggle("active")
来源：http://pub.tianlin.xyz

[U102] JS：本地存储
来源：http://uvh.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tjz.svipenyu.cn

[U103] JS：定时器
来源：http://qxx.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://avj.fengsongda.top

[U104] JS：防抖
来源：http://kkd.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wcn.gotoacloud.top

[U105] JS：节流
来源：http://wao.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hrj.zdbjq.cn

[U106] JS：日期格式化
来源：http://bbo.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://agq.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://kdp.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kjz.zhongyouzk.top

[U108] JS：随机整数
来源：http://fnr.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gda.mhx1999.top

[U109] JS：数组分组
来源：http://rjx.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://kkf.xuanzx.com

[U110] JS：数组分块
来源：http://nbj.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tyg.sufxvd.cn

[U111] JS：对象转 Map
来源：http://jft.hcnkem.com

new Map(Object.entries(obj))
来源：http://bbp.hywenlv.cn

[U112] JS：字符串补位
来源：http://yfx.sysykeji.top

"7".padStart(3, "0")
来源：http://vkm.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://wxp.hywenlv.cn

s.replaceAll("a", "b")
来源：http://mjk.mhx1999.top

[U114] JS：JSON 深比较
来源：http://pax.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vif.yuxming.cn

[U115] JS：生成 UUID
来源：http://plc.nanxuanxn.top

crypto.randomUUID()
来源：http://gyl.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://hpz.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://ijc.nwbrower.top

[U117] JS：单元测试
来源：http://xxt.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://yev.zhijiandao.cn

[U118] JS：开发服务器
来源：http://ojw.havefunace.top

npm i -D vite;  npx vite
来源：http://imh.hnqzz.top

[U119] JS：生产构建
来源：http://sik.sufxvd.cn

npx vite build
来源：http://lww.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://oay.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://njr.shzxlz.cn

================================================================================
来源：http://lwi.mhx1999.top

统计汇总
来源：http://cku.cdnleiting.top

================================================================================
来源：http://wmn.havefunace.top

按语言统计（条）：
来源：http://zvj.epnwcf.com

Python ......... 252
来源：http://env.guannengcc.top

PHP ............ 252
来源：http://jfn.tanke756.top

JavaScript ..... 252
来源：http://wdl.shanyushiyangtech.top

TypeScript ..... 212
来源：http://yza.jyoumei.cn

Java ........... 212
来源：http://koq.tarul.cn

Go ............. 212
来源：http://jni.wangdashe.top

Ruby ........... 212
来源：http://haz.jinqigufen.top

C# ............. 212
来源：http://crd.andypj.xyz

C .............. 30
来源：http://ppn.ivvv.top

C++ ............ 30
来源：http://qwz.pengpengdd.cyou

SQL ............ 90
来源：http://csw.yuanzhike.top

Bash ........... 80
来源：http://jag.xziqi.cn

Kotlin ......... 15
来源：http://mmw.guannengcc.top

Swift .......... 15
来源：http://piy.gaohongyu789.top

Lua ............ 10
来源：http://zst.shanyushiyangkeji.top

Perl ........... 10
来源：http://yjh.iojbl.cn

Scala .......... 10
来源：http://oyg.xuetiantiany.cn

------------------------------------
来源：http://our.yuanzhike.top

合计 ........... 2106 条
来源：http://pwy.cucudq.cn

按章节统计：
来源：http://ovv.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yyh.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://drp.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tbl.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vke.hammf.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eyw.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lkj.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kpj.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wej.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gci.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cdx.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://has.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tfk.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aeq.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wrz.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dax.shangyingyoupin.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://adm.xuetiantiany.cn

Q SQL 专题                              90
来源：http://bdb.kuanghao11.cn

R Bash 专题                             80
来源：http://sbm.zhixingplan.top

S C / C++ 专题                          60
来源：http://pdl.shzxlz.cn

T 其他语言补充                          60
来源：http://vkh.zhiwuduotai.top

U 高频实用片段                         120
来源：http://yoo.jianghu66.top

------------------------------------
来源：http://cgd.gaohongyu789.top

合计                                  2106 条
来源：http://sgl.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://ykc.sufxvd.cn

使用提醒
来源：http://sjb.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://fjt.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://agx.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dkq.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qhi.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vqq.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vvk.hfpthk.cn

—— 文件结束 ——
来源：http://axi.zdqjudy.top

================================================================================
来源：http://wyd.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://kmt.guannengcc.top

Common Programming Examples Cheat Book
来源：http://gze.hcnkem.com

================================================================================
来源：http://zoj.uphjek.com

【收录内容】
来源：http://whx.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://uxc.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eqs.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://vok.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oan.zhengqikj.top

【使用说明】
来源：http://ahg.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xjr.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://htr.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hap.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rfd.xziqi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://awi.chenjidiqi.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vts.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xyc.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ngu.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rbu.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://trz.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cxn.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ggu.zhixingplan.top

【文件统计】
来源：http://eks.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vtb.fengsongda.top

--------------------------------------------------------------------------------
来源：http://dhh.tianlin.xyz

目  录
来源：http://sey.shuidangran.top

--------------------------------------------------------------------------------
来源：http://jlg.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iej.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cxp.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jgq.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wgf.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ybh.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jpr.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fjv.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ugq.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uak.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wdl.guowangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ihv.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xhs.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kbm.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://itn.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kle.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jgn.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://agl.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rkz.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lrs.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://leh.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gbp.yuxming.cn

================================================================================
来源：http://gmz.shanyushiyangtech.top

A. 基础语法与类型
来源：http://nwk.nwbrower.top

================================================================================
来源：http://ika.pycfn.com

[A01] Hello World
来源：http://zqc.shzxlz.cn

Py:   print("Hello, World!")
来源：http://irf.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://wis.xuanzx.com

JS:   console.log("Hello, World!");
来源：http://day.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://csg.fanxiaobao.xyz

Java: System.out.println("Hello, World!");
来源：http://enc.zhiwuduotai.top

Go:   fmt.Println("Hello, World!")
来源：http://uon.yongpay.top

Ruby: puts "Hello, World!"
来源：http://hsw.tarul.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://whw.jianghu66.top

[A02] 变量声明与赋值
来源：http://hmt.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mgx.ctjpmb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ahs.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://mti.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wkz.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://xzk.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://vlw.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://fdj.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://riy.shanyushiyangkeji.top

[A03] 常量定义
来源：http://xph.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qkb.yj202588.top

PHP:  const PI = 3.14159;
来源：http://utf.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://xme.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://qha.redwolf501.top

Java: static final double PI = 3.14159;
来源：http://gpu.vehdjk.com

Go:   const PI = 3.14159
来源：http://eie.tianlin.xyz

Ruby: PI = 3.14159
来源：http://lwh.havefunace.top

C#:   const double PI = 3.14159;
来源：http://flv.vqdsnc.cn

[A04] 判断变量类型
来源：http://wbs.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dkx.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pwc.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://toz.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://oly.sweek.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nta.yongpay.top


<!-- 参考信息 -->