代发 wailian999

[U43] PHP：声明命名空间
来源：http://zep.daria6918.cn

namespace App\Http;
来源：http://idt.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://lai.hcnkem.com

declare(strict_types=1);
来源：http://xse.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://idf.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://anq.aizwys.cn

[U46] PHP：可空类型
来源：http://grw.ybcxt.top

?string $name = null
来源：http://nau.tianlin.xyz

[U47] PHP：联合类型
来源：http://age.jqgufenzy.top

int|string $id
来源：http://zjo.hysaishi.cn

[U48] PHP：纯枚举
来源：http://xkv.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bpq.ppjwa.cn

[U49] PHP：只读属性
来源：http://vut.nwbrower.top

public readonly string $name
来源：http://awk.yongpay.top

[U50] PHP：构造器属性提升
来源：http://uwu.daria6918.cn

public function __construct(private int $id) {}
来源：http://dik.shzxlz.cn

[U51] PHP：数组解构
来源：http://lev.nanxuanxn.top

[$a, $b] = $arr;
来源：http://slv.zhixingplan.top

[U52] PHP：箭头函数
来源：http://uug.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://uve.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://dem.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://hne.zhengqikj.top

[U54] PHP：空安全调用
来源：http://kxx.smart0.xyz

$obj?->method()
来源：http://vck.c1oappe.top

[U55] PHP：match 表达式
来源：http://xdm.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kvm.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://yvi.pycfn.com

f(a: 1, b: 2)
来源：http://whe.epnwcf.com

[U57] PHP：字符串插值
来源：http://vva.tian-w.cn

"值: {$a}"
来源：http://mdj.yvedp.cn

[U58] PHP：数组三件套
来源：http://qzt.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bqo.hysaishi.cn

[U59] PHP：自定义排序
来源：http://ghw.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqe.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://mzi.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uwc.jqgufenzy.top

[U61] PHP：正则
来源：http://def.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aol.ctjpmb.com

[U62] PHP：日期对象
来源：http://gsn.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dht.daxiang520.top

[U63] PHP：文件读写
来源：http://ssv.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hxv.vehdjk.com

[U64] PHP：目录遍历
来源：http://ife.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://nrh.zycfv.cn

[U65] PHP：会话
来源：http://gum.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lqp.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://tcc.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pyx.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://ybr.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgy.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://rql.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vya.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://emi.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qdb.316326.xyz

[U70] PHP：PDO 事务
来源：http://osd.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tce.aizwys.cn

[U71] PHP：抛出异常
来源：http://zun.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://hgp.yonumen.top

[U72] PHP：写错误日志
来源：http://qvp.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://lnx.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://nul.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://aht.havefunace.top

[U74] PHP：读取环境变量
来源：http://ptf.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://gjt.zdbjq.cn

[U75] PHP：依赖注入
来源：http://pza.jinyuanbaomall.cn

composer require psr/container
来源：http://jbr.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://gft.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qwh.svipenyu.cn

[U77] PHP：模板渲染
来源：http://ion.yj20258888.top

composer require twig/twig
来源：http://tbc.vqdsnc.cn

[U78] PHP：单元测试
来源：http://kbn.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://fbu.gotoacloud.top

[U79] PHP：静态分析
来源：http://xnp.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://oyg.shuidangran.top

[U80] PHP：代码规范修复
来源：http://tae.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hda.ivvv.top

[U81] JS：初始化项目
来源：http://rfe.daria6918.cn

npm init -y;  npm i express
来源：http://qsn.xylfe.cn

[U82] JS：package.json 脚本
来源：http://xff.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ylq.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://ual.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://gdp.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://ush.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://bjx.hammf.cn

[U85] JS：可选链
来源：http://lzc.shuidangran.top

a?.b?.c
来源：http://jdt.yueranfly.top

[U86] JS：空值合并
来源：http://rcb.zhoulong.xyz

a ?? b
来源：http://tji.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://omy.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://aaf.guannengcc.top

[U88] JS：对象展开合并
来源：http://uaa.xuetiantiany.cn

{ ...a, ...b }
来源：http://cml.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://sec.dashuyun.cn

[...new Set(arr)]
来源：http://nol.hywenlv.cn

[U90] JS：数字数组排序
来源：http://ado.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://xmm.chenlongwang.top

[U91] JS：对象键值遍历
来源：http://rgy.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mby.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://ofy.0kj1m.cn

structuredClone(obj)
来源：http://mvp.yj202588.top

[U93] JS：模板字符串
来源：http://ucv.fengsongda.top

`共 ${n} 条`
来源：http://blt.guannengcc.top

[U94] JS：箭头函数
来源：http://qjv.zhijiandao.cn

const double = x => x * 2;
来源：http://xjf.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://pfx.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://foc.gzhubu.top

[U96] JS：async/await 与异常
来源：http://utv.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sys.yueranfly.top

[U97] JS：并发请求
来源：http://plj.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tps.ydjk.org.cn

[U98] JS：fetch 带 JSON
来源：http://cou.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ndf.epnwcf.com

[U99] JS：事件监听
来源：http://nfb.fengsongda.top

el.addEventListener("click", e => {})
来源：http://cxs.hfpthk.cn

[U100] JS：DOM 查询
来源：http://btx.fanxiaobao.xyz

document.querySelector(".item")
来源：http://eky.yangfankeji.com

[U101] JS：classList 操作
来源：http://yos.andypj.xyz

el.classList.toggle("active")
来源：http://dvx.cqqwz.cn

[U102] JS：本地存储
来源：http://nzt.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gjn.shuidangran.top

[U103] JS：定时器
来源：http://vny.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lxs.xinyue.icu

[U104] JS：防抖
来源：http://aje.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gum.hongshengwenyu.top

[U105] JS：节流
来源：http://vha.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxz.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://oyh.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hmy.redwolf501.top

[U107] JS：数字千分位
来源：http://rzx.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gmt.sweek.top

[U108] JS：随机整数
来源：http://vhk.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ljf.hfpthk.cn

[U109] JS：数组分组
来源：http://ejg.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://iyg.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://vfh.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://enf.yuanzhike.top

[U111] JS：对象转 Map
来源：http://jon.guowangkeji.top

new Map(Object.entries(obj))
来源：http://goz.chenlongwang.top

[U112] JS：字符串补位
来源：http://akj.gaohongyu789.top

"7".padStart(3, "0")
来源：http://euv.uphjek.com

[U113] JS：正则替换全部
来源：http://zrn.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://qvy.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://gbu.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lzu.yongpay.top

[U115] JS：生成 UUID
来源：http://krb.vqdsnc.cn

crypto.randomUUID()
来源：http://pac.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://gpk.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://rrt.hywenlv.cn

[U117] JS：单元测试
来源：http://skf.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://toc.zhixingplan.top

[U118] JS：开发服务器
来源：http://lat.guannengcc.top

npm i -D vite;  npx vite
来源：http://oux.ehwqpu.com

[U119] JS：生产构建
来源：http://ocf.zhiwuduotai.top

npx vite build
来源：http://qmy.aibaodan.cn

[U120] JS：读取环境变量（Vite）
来源：http://jwd.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://lbc.jinqigfzy.top

================================================================================
来源：http://nxa.xuanzx.com

统计汇总
来源：http://cll.kuanghao11.cn

================================================================================
来源：http://tzc.yuanzhike.top

按语言统计（条）：
来源：http://cyt.xuanzx.com

Python ......... 252
来源：http://ekc.yueranfly.top

PHP ............ 252
来源：http://tnp.guannengcc.top

JavaScript ..... 252
来源：http://nqb.bbcook.cn

TypeScript ..... 212
来源：http://xfq.hnqzz.top

Java ........... 212
来源：http://bhq.chenzaomai.com

Go ............. 212
来源：http://ttz.yj20258888.top

Ruby ........... 212
来源：http://aws.zhaomingkeji.xyz

C# ............. 212
来源：http://yls.nanxuanxn.top

C .............. 30
来源：http://fkd.hfpthk.cn

C++ ............ 30
来源：http://wnx.pycfn.com

SQL ............ 90
来源：http://iqt.guannengcc.top

Bash ........... 80
来源：http://swm.gzhubu.top

Kotlin ......... 15
来源：http://mlo.sysykeji.top

Swift .......... 15
来源：http://kae.bbcook.cn

Lua ............ 10
来源：http://iup.ehwqpu.com

Perl ........... 10
来源：http://qrb.jlsjyb.cn

Scala .......... 10
来源：http://ykz.chenjidiqi.icu

------------------------------------
来源：http://tcg.jianghu66.top

合计 ........... 2106 条
来源：http://pon.hammf.cn

按章节统计：
来源：http://lgu.shuidangran.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gae.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zsf.vqdsnc.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uio.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ovx.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hea.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://swa.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tac.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dcr.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xlt.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uld.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://stv.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oyb.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vav.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xdv.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wsd.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://azl.redwolf501.top

Q SQL 专题                              90
来源：http://nxw.daxiang520.top

R Bash 专题                             80
来源：http://fsg.gzhubu.top

S C / C++ 专题                          60
来源：http://qqx.jiagoushi.top

T 其他语言补充                          60
来源：http://dzd.jiagoushi.top

U 高频实用片段                         120
来源：http://cwf.bjfxy.top

------------------------------------
来源：http://iqw.shuidangran.top

合计                                  2106 条
来源：http://krr.yvedp.cn

--------------------------------------------------------------------------------
来源：http://fct.yuxming.cn

使用提醒
来源：http://uff.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://hqx.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uis.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vgs.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fwl.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vwm.xylfe.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ard.yuanzhike.top

—— 文件结束 ——
来源：http://ixw.0kj1m.cn

================================================================================
来源：http://sqj.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://ylq.hammf.cn

Common Programming Examples Cheat Book
来源：http://koc.zdbjq.cn

================================================================================
来源：http://get.svipenyu.cn

【收录内容】
来源：http://wck.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://blh.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://szb.cqqwz.cn

SQL · Bash · C · C++
来源：http://qff.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tfk.zhoulong.xyz

【使用说明】
来源：http://lwe.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eph.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rga.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nom.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dvi.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://emp.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rar.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://psm.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ljp.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gph.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gyn.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://obk.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rqj.sweek.top

【文件统计】
来源：http://bjk.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mcv.c1oappe.top

--------------------------------------------------------------------------------
来源：http://qzu.birdmap.top

目  录
来源：http://cxr.cheryme.top

--------------------------------------------------------------------------------
来源：http://dlt.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ngv.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://efj.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uwf.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iuw.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://agm.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://awq.hfpthk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://skl.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dbb.bbcook.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bsv.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oag.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vgr.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qni.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ngj.pycfn.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nox.fktsv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://odd.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kgn.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iut.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wjn.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ryb.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://opn.xuetiantiany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pgz.redwolf501.top

================================================================================
来源：http://hcf.xuetiantiany.cn

A. 基础语法与类型
来源：http://ghu.yueranfly.top

================================================================================
来源：http://gfw.zhiwuduotai.top

[A01] Hello World
来源：http://wsy.zhengqikj.top

Py:   print("Hello, World!")
来源：http://tie.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://fdz.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://alc.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lvp.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://szi.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://tyg.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://sqt.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kec.52xcode.cn

[A02] 变量声明与赋值
来源：http://lyk.aibaodan.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://btk.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://cep.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bmu.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gsv.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://wwy.hfpthk.cn

Go:   name := "Alex"; age := 20
来源：http://qxz.xuetiantiany.cn

Ruby: name = "Alex"; age = 20
来源：http://wba.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://pkj.gzhubu.top

[A03] 常量定义
来源：http://vbk.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lfo.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://peq.xylfe.cn

JS:   const PI = 3.14159;
来源：http://vrh.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://yon.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://jal.cqqwz.cn

Go:   const PI = 3.14159
来源：http://wjh.jianghu66.top

Ruby: PI = 3.14159
来源：http://mgu.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://ukp.fanxiaobao.xyz

[A04] 判断变量类型
来源：http://nym.sweek.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://klf.hfpthk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://syu.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hgf.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://roa.yvedp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eex.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://qvt.uphjek.com

Ruby: x.class; x.is_a?(Integer)
来源：http://eoy.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://zbq.aizwys.cn

[A05] 整数除法与取模
来源：http://csj.tianlin.xyz


<!-- 参考信息 -->