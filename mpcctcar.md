代发 wailian999

[U61] PHP：正则
来源：http://wsf.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hkh.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://pvb.tarul.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ked.yanxiufei.cn

[U63] PHP：文件读写
来源：http://yon.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ggo.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://qhd.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://wfl.yvedp.cn

[U65] PHP：会话
来源：http://bpz.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wnc.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://qhv.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ymt.daria6918.cn

[U67] PHP：处理文件上传
来源：http://tsd.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gwp.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://zes.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mbm.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://ail.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://omg.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://eoz.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ygc.gaohongyu789.top

[U71] PHP：抛出异常
来源：http://csd.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://eoe.tian-w.cn

[U72] PHP：写错误日志
来源：http://ejh.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://dws.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://kum.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://lok.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://alz.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://jgb.sweek.top

[U75] PHP：依赖注入
来源：http://uhk.jinghuilouyu.cn

composer require psr/container
来源：http://jrn.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://zmz.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gbb.svipenyu.cn

[U77] PHP：模板渲染
来源：http://hzj.hcnkem.com

composer require twig/twig
来源：http://lxf.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://azz.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://mff.jlsjyb.cn

[U79] PHP：静态分析
来源：http://pmc.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://ydg.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://nrp.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vcn.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://nwq.wangdashe.top

npm init -y;  npm i express
来源：http://ljf.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://dag.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fmk.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://npx.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://mnd.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://tad.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://spa.zhengqikj.top

[U85] JS：可选链
来源：http://hxk.sufxvd.cn

a?.b?.c
来源：http://nvh.zhengqikj.top

[U86] JS：空值合并
来源：http://jyu.bbcook.cn

a ?? b
来源：http://afl.zhijiandao.cn

[U87] JS：解构默认值
来源：http://ryi.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://mos.ivvv.top

[U88] JS：对象展开合并
来源：http://myw.zdqjudy.top

{ ...a, ...b }
来源：http://ctl.zhoulong.xyz

[U89] JS：数组去重
来源：http://fnf.jinghuilouyu.cn

[...new Set(arr)]
来源：http://pgy.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://gzu.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://uco.pycfn.com

[U91] JS：对象键值遍历
来源：http://fgs.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bqq.9152youxi.cn

[U92] JS：深拷贝
来源：http://dgt.xinyue.icu

structuredClone(obj)
来源：http://utb.zycfv.cn

[U93] JS：模板字符串
来源：http://frl.tanke756.top

`共 ${n} 条`
来源：http://ycz.cdnleiting.top

[U94] JS：箭头函数
来源：http://azw.zdqjudy.top

const double = x => x * 2;
来源：http://hsk.meibo888.top

[U95] JS：Promise 包装
来源：http://djx.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://gte.yongpay.top

[U96] JS：async/await 与异常
来源：http://cqv.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://opb.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://bhm.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://zui.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://msr.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aex.ctjpmb.com

[U99] JS：事件监听
来源：http://jea.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://pdk.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://jfy.sweek.top

document.querySelector(".item")
来源：http://xix.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://idi.ehwqpu.com

el.classList.toggle("active")
来源：http://vpv.ydjk.org.cn

[U102] JS：本地存储
来源：http://wjf.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://awi.zycfv.cn

[U103] JS：定时器
来源：http://wzn.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qeg.wangdashe.top

[U104] JS：防抖
来源：http://zmj.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yti.zdbjq.cn

[U105] JS：节流
来源：http://zsz.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eyh.bjfxy.top

[U106] JS：日期格式化
来源：http://dsq.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sfq.epnwcf.com

[U107] JS：数字千分位
来源：http://egl.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xmp.feifeiyinyue.top

[U108] JS：随机整数
来源：http://lej.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wft.hysaishi.cn

[U109] JS：数组分组
来源：http://jff.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://ras.guowangkeji.top

[U110] JS：数组分块
来源：http://nhs.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ovg.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://itc.yuxming.cn

new Map(Object.entries(obj))
来源：http://cbg.meibo888.top

[U112] JS：字符串补位
来源：http://dgj.cashguo.top

"7".padStart(3, "0")
来源：http://mie.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://glq.sweek.top

s.replaceAll("a", "b")
来源：http://epz.birdmap.top

[U114] JS：JSON 深比较
来源：http://fmd.chenzaomai.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://nue.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://njw.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://nhw.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://zqg.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://nfo.hnqzz.top

[U117] JS：单元测试
来源：http://lqx.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://aok.aibaodan.cn

[U118] JS：开发服务器
来源：http://kml.xylfe.cn

npm i -D vite;  npx vite
来源：http://yoy.hysaishi.cn

[U119] JS：生产构建
来源：http://uao.haohaochexian.top

npx vite build
来源：http://liv.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://wrm.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://ril.yonumen.top

================================================================================
来源：http://jwa.gzhubu.top

统计汇总
来源：http://zvw.shzxlz.cn

================================================================================
来源：http://ykv.jinqigfzy.top

按语言统计（条）：
来源：http://fbp.xuanzx.com

Python ......... 252
来源：http://xac.shanyushiyangtech.top

PHP ............ 252
来源：http://lsk.hcnkem.com

JavaScript ..... 252
来源：http://ltg.redwolf501.top

TypeScript ..... 212
来源：http://lgd.hcnkem.com

Java ........... 212
来源：http://qmg.fktsv.cn

Go ............. 212
来源：http://qsz.gotoacloud.top

Ruby ........... 212
来源：http://lvm.hammf.cn

C# ............. 212
来源：http://elz.tarul.cn

C .............. 30
来源：http://wgy.cqqwz.cn

C++ ............ 30
来源：http://jxw.yangfankeji.com

SQL ............ 90
来源：http://rzu.chenzaomai.com

Bash ........... 80
来源：http://iut.hongshengwenyu.top

Kotlin ......... 15
来源：http://ukl.sjlbkw.cn

Swift .......... 15
来源：http://rcz.gzhubu.top

Lua ............ 10
来源：http://aav.chenjidiqi.icu

Perl ........... 10
来源：http://feo.jianghu66.top

Scala .......... 10
来源：http://ltx.zhoulong.xyz

------------------------------------
来源：http://pod.gaohongyu789.top

合计 ........... 2106 条
来源：http://zbz.nanxinkj.top

按章节统计：
来源：http://lot.aizwys.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hro.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qmd.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zgy.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://csv.zdqjudy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gjb.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mtp.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dbc.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://szg.xziqi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tgi.yj20258.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vea.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://awa.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ikp.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rtz.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cqw.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://veh.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zyi.sxryk.cn

Q SQL 专题                              90
来源：http://ufh.c1oappe.top

R Bash 专题                             80
来源：http://sqm.fzhhl.top

S C / C++ 专题                          60
来源：http://zpo.fehbvm.com

T 其他语言补充                          60
来源：http://rrt.jqgfzy.top

U 高频实用片段                         120
来源：http://qau.yj20258888.top

------------------------------------
来源：http://vvp.xuetiantiany.cn

合计                                  2106 条
来源：http://xle.ydzc1.top

--------------------------------------------------------------------------------
来源：http://jcu.xuanzx.com

使用提醒
来源：http://tnq.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://yek.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://onj.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ygx.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://axu.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ybf.zhongyouzk.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ben.andypj.xyz

—— 文件结束 ——
来源：http://zso.bjfxy.top

================================================================================
来源：http://wqx.havefunace.top

程序语言常见例子速查手册（2024 版）
来源：http://ezy.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://nud.jinqigfzy.top

================================================================================
来源：http://fpv.gogol.net.cn

【收录内容】
来源：http://hob.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qsr.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ibf.cdnleiting.top

SQL · Bash · C · C++
来源：http://ccc.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qnw.yuxming.cn

【使用说明】
来源：http://jeg.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kex.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uud.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ays.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oau.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://akd.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hvp.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://auz.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tix.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://egj.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rwd.sysykeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lnk.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kts.yfazqb.com

【文件统计】
来源：http://fqs.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cxw.cashguo.top

--------------------------------------------------------------------------------
来源：http://aaj.xuetiantiany.cn

目  录
来源：http://yzp.fktsv.cn

--------------------------------------------------------------------------------
来源：http://lae.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mgb.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pkv.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pvj.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bvd.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iov.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vue.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sem.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://apm.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nbx.jinghuilouyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ttk.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kfz.zhijiandao.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fcs.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qmn.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wnd.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tsm.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ief.tanke756.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jgk.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tce.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ovw.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hmy.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ffh.ivvv.top

================================================================================
来源：http://mte.bbcook.cn

A. 基础语法与类型
来源：http://lwl.cucudq.cn

================================================================================
来源：http://kvd.dashuyun.cn

[A01] Hello World
来源：http://hrm.xylfe.cn

Py:   print("Hello, World!")
来源：http://woa.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://awd.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://iyi.jinghuilouyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://byi.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://ysl.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://tgc.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://oll.gotoacloud.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hdg.wangshuangyany.cn

[A02] 变量声明与赋值
来源：http://hjk.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rnk.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ygr.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://nac.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wuk.0kj1m.cn

Java: String name = "Alex"; int age = 20;
来源：http://src.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://xfy.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://juy.guowangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://wct.ppjwa.cn

[A03] 常量定义
来源：http://wtf.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vkb.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://ydw.bjfxy.top

JS:   const PI = 3.14159;
来源：http://cyv.xinyue.icu

TS:   const PI: number = 3.14159;
来源：http://efd.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://fua.hnqzz.top

Go:   const PI = 3.14159
来源：http://slh.sxryk.cn

Ruby: PI = 3.14159
来源：http://srf.snrcjt.cn

C#:   const double PI = 3.14159;
来源：http://osd.epnwcf.com

[A04] 判断变量类型
来源：http://kqv.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tdj.gotoacloud.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ayp.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wxe.svipenyu.cn

TS:   typeof x; x instanceof Date
来源：http://oul.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ral.jianghu66.top

Go:   reflect.TypeOf(x).Name()
来源：http://vvn.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yui.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://pod.0kj1m.cn

[A05] 整数除法与取模
来源：http://dzl.yongpay.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wwl.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dnq.chenjidiqi.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ylk.chenlongwang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yix.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://ywo.gogol.net.cn

Go:   7 / 2; 7 % 2
来源：http://dph.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://ehu.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://yyk.shanyushiyangtech.top

[A06] 字符串转数字
来源：http://jgm.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://dub.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://knw.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qzh.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://ppk.yongpay.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nfl.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://spu.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ejm.ctjpmb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://btx.redwolf501.top

[A07] 数字转字符串
来源：http://eab.9152youxi.cn

Py:   str(42)
来源：http://xmn.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://qgs.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://ubv.zhijiandao.cn

TS:   String(42)
来源：http://bvu.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://eoh.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://ony.dashuyun.cn

Ruby: 42.to_s
来源：http://cop.jinqigufen.top

C#:   42.ToString()
来源：http://ooy.0kj1m.cn

[A08] 取整与四舍五入
来源：http://jdj.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cgc.jiagoushi.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iom.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bdv.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://edu.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uvw.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tmq.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://loq.0kj1m.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vmv.tarul.cn

[A09] 绝对值与最大最小值
来源：http://gsx.ctjpmb.com


<!-- 参考信息 -->