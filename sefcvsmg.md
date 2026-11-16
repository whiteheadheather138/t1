代发 wailian999

[U47] PHP：联合类型
来源：http://gon.nanxuanxn.top

int|string $id
来源：http://fen.tian-w.cn

[U48] PHP：纯枚举
来源：http://plb.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sgu.hfpthk.cn

[U49] PHP：只读属性
来源：http://thl.ppjwa.cn

public readonly string $name
来源：http://act.gogol.net.cn

[U50] PHP：构造器属性提升
来源：http://zua.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://vjz.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://orq.yanxiufei.cn

[$a, $b] = $arr;
来源：http://klf.yj20258.top

[U52] PHP：箭头函数
来源：http://hse.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://pzr.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://vgo.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://kng.vehdjk.com

[U54] PHP：空安全调用
来源：http://ljf.guannengcc.top

$obj?->method()
来源：http://sqi.shzxlz.cn

[U55] PHP：match 表达式
来源：http://dfn.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nhq.zhixingplan.top

[U56] PHP：命名参数
来源：http://qza.9152youxi.cn

f(a: 1, b: 2)
来源：http://ldb.aizwys.cn

[U57] PHP：字符串插值
来源：http://iae.ppjwa.cn

"值: {$a}"
来源：http://ryt.fzhhl.top

[U58] PHP：数组三件套
来源：http://ybg.zhoulong.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gmf.pycfn.com

[U59] PHP：自定义排序
来源：http://qfi.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hvf.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://dcc.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xbo.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://slp.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dii.cdnleiting.top

[U62] PHP：日期对象
来源：http://eqc.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aob.cqqwz.cn

[U63] PHP：文件读写
来源：http://oyo.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tvd.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://yhf.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://tch.redwolf501.top

[U65] PHP：会话
来源：http://hcb.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mmz.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://lnx.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jle.bbcook.cn

[U67] PHP：处理文件上传
来源：http://oaz.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zgv.bjfxy.top

[U68] PHP：PDO 连接
来源：http://ior.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qso.ivvv.top

[U69] PHP：PDO 预处理
来源：http://chv.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ylj.sysykeji.top

[U70] PHP：PDO 事务
来源：http://vff.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dxy.daxiang520.top

[U71] PHP：抛出异常
来源：http://dkv.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://tsk.jinqigfzy.top

[U72] PHP：写错误日志
来源：http://hbd.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://ztt.kuanghao11.cn

[U73] PHP：读取 ini 配置
来源：http://wlm.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://mul.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://jwc.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://ggz.tianlin.xyz

[U75] PHP：依赖注入
来源：http://fik.aibaodan.cn

composer require psr/container
来源：http://rrw.jyoumei.cn

[U76] PHP：简单路由
来源：http://ocw.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fen.c1oappe.top

[U77] PHP：模板渲染
来源：http://ydo.guannengcc.top

composer require twig/twig
来源：http://mlh.jiagoushi.top

[U78] PHP：单元测试
来源：http://ney.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://ijc.nwbrower.top

[U79] PHP：静态分析
来源：http://iuy.zhiwuduotai.top

composer require --dev phpstan/phpstan
来源：http://yso.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://vlu.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://agf.iojbl.cn

[U81] JS：初始化项目
来源：http://rwl.hysaishi.cn

npm init -y;  npm i express
来源：http://jem.sweek.top

[U82] JS：package.json 脚本
来源：http://gzr.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nom.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://dtt.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://miu.meibo888.top

[U84] JS：CommonJS 写法
来源：http://zxd.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://djz.ydjk.org.cn

[U85] JS：可选链
来源：http://xhi.sufxvd.cn

a?.b?.c
来源：http://ozl.jianghu66.top

[U86] JS：空值合并
来源：http://igw.tanke756.top

a ?? b
来源：http://pgg.9152youxi.cn

[U87] JS：解构默认值
来源：http://uiz.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://sfn.cucudq.cn

[U88] JS：对象展开合并
来源：http://hxa.vehdjk.com

{ ...a, ...b }
来源：http://vdq.fktsv.cn

[U89] JS：数组去重
来源：http://bly.zhiwuduotai.top

[...new Set(arr)]
来源：http://wed.xuanzx.com

[U90] JS：数字数组排序
来源：http://abe.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://egu.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://tdg.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hnw.xuetiantiany.cn

[U92] JS：深拷贝
来源：http://qqp.hnxiangtu.top

structuredClone(obj)
来源：http://aya.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://rud.shuidangran.top

`共 ${n} 条`
来源：http://ime.shzxlz.cn

[U94] JS：箭头函数
来源：http://crb.jinqigfzy.top

const double = x => x * 2;
来源：http://mzg.cheryme.top

[U95] JS：Promise 包装
来源：http://azq.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://ajs.sweek.top

[U96] JS：async/await 与异常
来源：http://fih.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kkm.yvedp.cn

[U97] JS：并发请求
来源：http://rbi.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://doi.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://zyr.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mfo.sjlbkw.cn

[U99] JS：事件监听
来源：http://rzh.meibo888.top

el.addEventListener("click", e => {})
来源：http://bjn.chenlongwang.top

[U100] JS：DOM 查询
来源：http://miw.hesvh.cn

document.querySelector(".item")
来源：http://imd.gogol.net.cn

[U101] JS：classList 操作
来源：http://ixo.fzhhl.top

el.classList.toggle("active")
来源：http://bux.c1oappe.top

[U102] JS：本地存储
来源：http://yon.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vaj.bbcook.cn

[U103] JS：定时器
来源：http://lpl.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lpl.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://uic.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqd.sjlbkw.cn

[U105] JS：节流
来源：http://snd.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://huu.smart0.xyz

[U106] JS：日期格式化
来源：http://kst.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kym.cqqwz.cn

[U107] JS：数字千分位
来源：http://wrk.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sth.nwbrower.top

[U108] JS：随机整数
来源：http://amm.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ygs.snrcjt.cn

[U109] JS：数组分组
来源：http://lis.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://nzv.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://vks.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yuq.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://css.yfazqb.com

new Map(Object.entries(obj))
来源：http://qcc.nanxuanxn.top

[U112] JS：字符串补位
来源：http://gxd.zhixingplan.top

"7".padStart(3, "0")
来源：http://usj.jqgfzy.top

[U113] JS：正则替换全部
来源：http://bcg.yueranfly.top

s.replaceAll("a", "b")
来源：http://qgn.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://kxd.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mzg.yj20258888.top

[U115] JS：生成 UUID
来源：http://tgg.cucudq.cn

crypto.randomUUID()
来源：http://vzd.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://kgj.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://mke.chenjidiqi.icu

[U117] JS：单元测试
来源：http://tbv.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://lpg.shuidangran.top

[U118] JS：开发服务器
来源：http://dzh.hnqzz.top

npm i -D vite;  npx vite
来源：http://beb.aizwys.cn

[U119] JS：生产构建
来源：http://quk.hesvh.cn

npx vite build
来源：http://yts.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://cez.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://gnl.zhijiandao.cn

================================================================================
来源：http://ahw.zhengqikj.top

统计汇总
来源：http://jbh.hnxiangtu.top

================================================================================
来源：http://bpu.kuanghao11.cn

按语言统计（条）：
来源：http://xlh.yonumen.top

Python ......... 252
来源：http://ldn.hywenlv.cn

PHP ............ 252
来源：http://fqk.tian-w.cn

JavaScript ..... 252
来源：http://wbe.ybcxt.top

TypeScript ..... 212
来源：http://aoa.ywan-chungtsiang.top

Java ........... 212
来源：http://muy.daxiang520.top

Go ............. 212
来源：http://kxr.cdnleiting.top

Ruby ........... 212
来源：http://dtz.yongpay.top

C# ............. 212
来源：http://ogp.jqgufenzy.top

C .............. 30
来源：http://pul.pengpengdd.cyou

C++ ............ 30
来源：http://fsj.sysykeji.top

SQL ............ 90
来源：http://lig.zhaomingkeji.xyz

Bash ........... 80
来源：http://miq.tanke756.top

Kotlin ......... 15
来源：http://gha.ctjpmb.com

Swift .......... 15
来源：http://azg.zhoulong.xyz

Lua ............ 10
来源：http://sop.zhiwuduotai.top

Perl ........... 10
来源：http://uhp.zdqjudy.top

Scala .......... 10
来源：http://agq.jinqigfzy.top

------------------------------------
来源：http://tba.aizwys.cn

合计 ........... 2106 条
来源：http://zoe.zhongyouzk.top

按章节统计：
来源：http://uyx.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tfy.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oqh.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lkz.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tpj.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dnf.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fqi.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bwo.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gbj.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tca.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nkp.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://olm.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mgv.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ecc.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://trn.tanke756.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kdf.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rgh.hnqzz.top

Q SQL 专题                              90
来源：http://cof.cashguo.top

R Bash 专题                             80
来源：http://ywv.sxryk.cn

S C / C++ 专题                          60
来源：http://oxs.bjfxy.top

T 其他语言补充                          60
来源：http://sbz.ehwqpu.com

U 高频实用片段                         120
来源：http://amu.ywan-chungtsiang.top

------------------------------------
来源：http://tuo.sweek.top

合计                                  2106 条
来源：http://qbv.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://ynj.chenzaomai.com

使用提醒
来源：http://uoh.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://qan.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gng.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vuo.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://usu.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://asb.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://she.sjlbkw.cn

—— 文件结束 ——
来源：http://ojt.52xcode.cn

================================================================================
来源：http://tmq.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://zxa.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://pbg.gotoacloud.top

================================================================================
来源：http://gtv.dashuyun.cn

【收录内容】
来源：http://gdy.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ccd.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tzr.jianghu66.top

SQL · Bash · C · C++
来源：http://mqi.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zux.shanyushiyangkeji.top

【使用说明】
来源：http://ivy.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ree.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dtw.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ntb.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://efx.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gip.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nym.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fgo.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ypx.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://org.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mkq.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ppg.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ljl.xylfe.cn

【文件统计】
来源：http://muu.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fpu.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://jep.pengpengdd.cyou

目  录
来源：http://lmx.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://ujw.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://naj.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cec.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sux.fktsv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ccq.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iwj.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pcb.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ewh.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sfc.nwbrower.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ukb.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cqg.chenzaomai.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wul.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gtz.redwolf501.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gpz.sjlbkw.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yko.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sgi.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rlt.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iqc.shanyushiyangtech.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zhh.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://poe.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xtt.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zjm.yuxming.cn

================================================================================
来源：http://gyq.fanxiaobao.xyz

A. 基础语法与类型
来源：http://qcq.iojbl.cn

================================================================================
来源：http://qth.quarkkingdee.top

[A01] Hello World
来源：http://vlb.jianghu66.top

Py:   print("Hello, World!")
来源：http://cbu.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://udk.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://awd.gzhubu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xsn.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://fbr.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://cks.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://nrq.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://thq.yonumen.top

[A02] 变量声明与赋值
来源：http://ffe.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yzm.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ssl.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hlo.nanxuanxn.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ysh.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://qlu.pycfn.com

Go:   name := "Alex"; age := 20
来源：http://chw.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://scm.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qqc.ppjwa.cn

[A03] 常量定义
来源：http://gbd.daxiang520.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://scq.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://utj.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://pff.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://tvp.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://sri.tarul.cn

Go:   const PI = 3.14159
来源：http://kem.tianlin.xyz

Ruby: PI = 3.14159
来源：http://ien.yongpay.top

C#:   const double PI = 3.14159;
来源：http://bdb.ehwqpu.com

[A04] 判断变量类型
来源：http://rrf.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://jvx.52xcode.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cdq.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dvc.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://bza.wangdashe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fav.yuxming.cn

Go:   reflect.TypeOf(x).Name()
来源：http://blf.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xmd.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://jze.hysaishi.cn

[A05] 整数除法与取模
来源：http://ury.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ckr.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xww.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ued.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zhf.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://bey.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://wew.shzxlz.cn

Ruby: 7 / 2; 7 % 2
来源：http://rvx.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://nsx.gzhubu.top


<!-- 参考信息 -->