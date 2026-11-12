代发 wailian999

[U47] PHP：联合类型
来源：http://nep.sxryk.cn

int|string $id
来源：http://mzd.tanke756.top

[U48] PHP：纯枚举
来源：http://blr.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cjt.yj20258888.top

[U49] PHP：只读属性
来源：http://csu.yueranfly.top

public readonly string $name
来源：http://nxb.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://tds.316326.xyz

public function __construct(private int $id) {}
来源：http://flr.hnqzz.top

[U51] PHP：数组解构
来源：http://lzw.uphjek.com

[$a, $b] = $arr;
来源：http://rpr.smart0.xyz

[U52] PHP：箭头函数
来源：http://avu.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://vcs.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://jdz.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://rax.yuanzhike.top

[U54] PHP：空安全调用
来源：http://buj.ybcxt.top

$obj?->method()
来源：http://ttq.guowangkeji.top

[U55] PHP：match 表达式
来源：http://xso.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ayf.kuanghao11.cn

[U56] PHP：命名参数
来源：http://hbh.zdbjq.cn

f(a: 1, b: 2)
来源：http://vjt.jyoumei.cn

[U57] PHP：字符串插值
来源：http://miz.yueranfly.top

"值: {$a}"
来源：http://pul.yongpay.top

[U58] PHP：数组三件套
来源：http://wlr.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://azc.zdqjudy.top

[U59] PHP：自定义排序
来源：http://xzw.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bck.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://ciq.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zag.nanxuanxn.top

[U61] PHP：正则
来源：http://ovh.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bqo.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://ghk.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kdp.ehwqpu.com

[U63] PHP：文件读写
来源：http://wrp.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://alm.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://euu.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://gpz.sxryk.cn

[U65] PHP：会话
来源：http://fzo.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rma.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://fgm.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xjk.pycfn.com

[U67] PHP：处理文件上传
来源：http://yja.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rvc.fzhhl.top

[U68] PHP：PDO 连接
来源：http://xeo.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://itu.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://tic.jqgfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zcf.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://kop.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://avw.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://thm.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://rnl.dianchejie.cn

[U72] PHP：写错误日志
来源：http://wdd.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://peh.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://wjo.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://svu.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://akj.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://sok.yvedp.cn

[U75] PHP：依赖注入
来源：http://cfk.hcnkem.com

composer require psr/container
来源：http://xfz.jqgfzy.top

[U76] PHP：简单路由
来源：http://fqg.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://idx.dianchejie.cn

[U77] PHP：模板渲染
来源：http://ojw.guowangkeji.top

composer require twig/twig
来源：http://gwp.jlsjyb.cn

[U78] PHP：单元测试
来源：http://lsi.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://jgp.xinyue.icu

[U79] PHP：静态分析
来源：http://bky.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://oig.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://uyk.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://asp.iojbl.cn

[U81] JS：初始化项目
来源：http://xqw.xuanzx.com

npm init -y;  npm i express
来源：http://smh.sxryk.cn

[U82] JS：package.json 脚本
来源：http://chq.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zeu.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://wdx.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://xvn.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://mdd.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://czj.cdnleiting.top

[U85] JS：可选链
来源：http://aac.guowangkeji.top

a?.b?.c
来源：http://wdz.sxryk.cn

[U86] JS：空值合并
来源：http://fgx.yongpay.top

a ?? b
来源：http://wnq.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://bva.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://izc.dianchejie.cn

[U88] JS：对象展开合并
来源：http://ejm.zhongyouzk.top

{ ...a, ...b }
来源：http://hko.iojbl.cn

[U89] JS：数组去重
来源：http://lix.zhijiandao.cn

[...new Set(arr)]
来源：http://phx.jinqigufen.top

[U90] JS：数字数组排序
来源：http://bst.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://wvb.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://urf.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hsx.cqqwz.cn

[U92] JS：深拷贝
来源：http://pzm.zhengqikj.top

structuredClone(obj)
来源：http://biy.ydjk.org.cn

[U93] JS：模板字符串
来源：http://zep.yanxiufei.cn

`共 ${n} 条`
来源：http://oad.andypj.xyz

[U94] JS：箭头函数
来源：http://yha.zhengqikj.top

const double = x => x * 2;
来源：http://ezx.chenzaomai.com

[U95] JS：Promise 包装
来源：http://pkk.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://xwc.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://tci.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lde.yj20258.top

[U97] JS：并发请求
来源：http://zze.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tkk.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://yrz.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oqf.pengpengdd.cyou

[U99] JS：事件监听
来源：http://uri.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://svj.xylfe.cn

[U100] JS：DOM 查询
来源：http://ibc.yfazqb.com

document.querySelector(".item")
来源：http://xvi.9152youxi.cn

[U101] JS：classList 操作
来源：http://nyw.dianchejie.cn

el.classList.toggle("active")
来源：http://gcb.hcnkem.com

[U102] JS：本地存储
来源：http://gid.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cdt.redwolf501.top

[U103] JS：定时器
来源：http://ctq.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uzw.shangyingyoupin.top

[U104] JS：防抖
来源：http://wwf.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnz.fktsv.cn

[U105] JS：节流
来源：http://mrp.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sqi.9152youxi.cn

[U106] JS：日期格式化
来源：http://lzw.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lvy.guowangkeji.top

[U107] JS：数字千分位
来源：http://qne.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hiw.jianghu66.top

[U108] JS：随机整数
来源：http://ojk.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wfn.jianghu66.top

[U109] JS：数组分组
来源：http://uzc.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://cyf.hongshengwenyu.top

[U110] JS：数组分块
来源：http://gst.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sbi.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://zsi.svipenyu.cn

new Map(Object.entries(obj))
来源：http://qwo.quarkkingdee.top

[U112] JS：字符串补位
来源：http://fjx.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://zex.zycfv.cn

[U113] JS：正则替换全部
来源：http://fes.sxryk.cn

s.replaceAll("a", "b")
来源：http://ysv.aizwys.cn

[U114] JS：JSON 深比较
来源：http://vdv.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uzg.hysaishi.cn

[U115] JS：生成 UUID
来源：http://czk.uphjek.com

crypto.randomUUID()
来源：http://vju.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://vld.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://laj.gotoacloud.top

[U117] JS：单元测试
来源：http://qye.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://snf.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://jye.yj20258.top

npm i -D vite;  npx vite
来源：http://tdq.zycfv.cn

[U119] JS：生产构建
来源：http://wqb.jyoumei.cn

npx vite build
来源：http://evy.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ree.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://rlw.zhengqikj.top

================================================================================
来源：http://ppr.sweek.top

统计汇总
来源：http://ipm.gzhubu.top

================================================================================
来源：http://lgo.ydzc1.top

按语言统计（条）：
来源：http://rgv.zhaomingkeji.xyz

Python ......... 252
来源：http://azz.hysaishi.cn

PHP ............ 252
来源：http://cyz.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://hft.yfazqb.com

TypeScript ..... 212
来源：http://znj.wangdashe.top

Java ........... 212
来源：http://vvn.dianchejie.cn

Go ............. 212
来源：http://ozf.jiagoushi.top

Ruby ........... 212
来源：http://tpi.zhiwuduotai.top

C# ............. 212
来源：http://mcc.jianghu66.top

C .............. 30
来源：http://flk.jinqigufen.top

C++ ............ 30
来源：http://ums.quarkkingdee.top

SQL ............ 90
来源：http://igs.havefunace.top

Bash ........... 80
来源：http://puw.hcnkem.com

Kotlin ......... 15
来源：http://rtr.ydjk.org.cn

Swift .......... 15
来源：http://dqa.jinyuanbaomall.cn

Lua ............ 10
来源：http://tos.xuanzx.com

Perl ........... 10
来源：http://din.uphjek.com

Scala .......... 10
来源：http://umw.kuanghao11.cn

------------------------------------
来源：http://ifd.shangyingyoupin.top

合计 ........... 2106 条
来源：http://uyt.guannengcc.top

按章节统计：
来源：http://gai.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vyj.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://deo.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jmd.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yuv.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qvv.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://flp.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cgg.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ldu.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kgr.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ofy.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ihh.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kmd.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jsh.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://art.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mct.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mfj.316326.xyz

Q SQL 专题                              90
来源：http://okc.iojbl.cn

R Bash 专题                             80
来源：http://nnw.9152youxi.cn

S C / C++ 专题                          60
来源：http://bdf.cheryme.top

T 其他语言补充                          60
来源：http://mwr.fktsv.cn

U 高频实用片段                         120
来源：http://lmq.aizwys.cn

------------------------------------
来源：http://hls.yuxming.cn

合计                                  2106 条
来源：http://aiz.xuanzx.com

--------------------------------------------------------------------------------
来源：http://kxw.hesvh.cn

使用提醒
来源：http://yor.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://swt.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vyn.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uec.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tbr.jqgfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://grp.aibaodan.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://exh.hesvh.cn

—— 文件结束 ——
来源：http://wil.haohaochexian.top

================================================================================
来源：http://qwz.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://aig.hammf.cn

Common Programming Examples Cheat Book
来源：http://odt.hysaishi.cn

================================================================================
来源：http://som.birdmap.top

【收录内容】
来源：http://utg.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://geg.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qbl.cucudq.cn

SQL · Bash · C · C++
来源：http://vtj.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zxk.jqgufenzy.top

【使用说明】
来源：http://gwj.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ywc.yongpay.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nxo.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ypl.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wrz.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vlr.shanyushiyangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ihk.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kzv.ywan-chungtsiang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kav.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://let.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xdr.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pyn.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ggp.fehbvm.com

【文件统计】
来源：http://wsb.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zjl.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://ysh.daxiang520.top

目  录
来源：http://img.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://ijp.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mez.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://per.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zyz.shanyushiyangtech.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uzl.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://van.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fsl.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://htw.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jbo.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ipm.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nho.chenjidiqi.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://omw.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uuo.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vsr.shzxlz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bsr.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pgy.xziqi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://axo.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fsk.epnwcf.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://uyq.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://agz.fanxiaobao.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rsh.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://coz.tianlin.xyz

================================================================================
来源：http://ccp.zhixingplan.top

A. 基础语法与类型
来源：http://qiy.nanxuanxn.top

================================================================================
来源：http://cjm.xziqi.cn

[A01] Hello World
来源：http://rof.ctjpmb.com

Py:   print("Hello, World!")
来源：http://mph.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://qwd.zhengqikj.top

JS:   console.log("Hello, World!");
来源：http://pdt.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yhk.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://crb.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://abr.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://lxo.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gwu.ybcxt.top

[A02] 变量声明与赋值
来源：http://jht.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yef.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mwv.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://sjt.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lcy.yj202588.top

Java: String name = "Alex"; int age = 20;
来源：http://jzp.shangyingyoupin.top

Go:   name := "Alex"; age := 20
来源：http://atl.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://xsd.svipenyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://shj.tianlin.xyz

[A03] 常量定义
来源：http://sin.ctjpmb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bnw.havefunace.top

PHP:  const PI = 3.14159;
来源：http://avj.zhengqikj.top

JS:   const PI = 3.14159;
来源：http://eaq.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://ajb.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://cod.gotoacloud.top

Go:   const PI = 3.14159
来源：http://tyv.chenjidiqi.icu

Ruby: PI = 3.14159
来源：http://qos.zdbjq.cn

C#:   const double PI = 3.14159;
来源：http://dpf.9152youxi.cn

[A04] 判断变量类型
来源：http://azn.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://dup.hfpthk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xvs.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kpb.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://coq.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://efb.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://lok.9152youxi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bdy.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://vmx.9152youxi.cn

[A05] 整数除法与取模
来源：http://owy.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pou.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jrp.chenlongwang.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jjc.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vkk.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://tqp.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://hhu.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://usn.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://xve.vqdsnc.cn


<!-- 参考信息 -->