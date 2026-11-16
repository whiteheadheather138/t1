代发 wailian999

[U63] PHP：文件读写
来源：http://yif.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cfa.smart0.xyz

[U64] PHP：目录遍历
来源：http://vyx.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://blg.havefunace.top

[U65] PHP：会话
来源：http://vav.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hmc.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://wjx.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oga.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://sxd.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://owk.cucudq.cn

[U68] PHP：PDO 连接
来源：http://zbz.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gkm.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://vtc.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kak.yj202588.top

[U70] PHP：PDO 事务
来源：http://cyh.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uxe.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://vxt.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://lkr.cucudq.cn

[U72] PHP：写错误日志
来源：http://hxf.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://isd.9152youxi.cn

[U73] PHP：读取 ini 配置
来源：http://fsu.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://vzt.smart0.xyz

[U74] PHP：读取环境变量
来源：http://off.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://eia.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://snw.jinqigfzy.top

composer require psr/container
来源：http://jcj.bbcook.cn

[U76] PHP：简单路由
来源：http://vsb.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://djy.guowangkeji.top

[U77] PHP：模板渲染
来源：http://rcr.bbcook.cn

composer require twig/twig
来源：http://cwq.316326.xyz

[U78] PHP：单元测试
来源：http://trp.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://eaa.0kj1m.cn

[U79] PHP：静态分析
来源：http://bby.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://fha.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://xig.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kju.bbcook.cn

[U81] JS：初始化项目
来源：http://igu.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://rxi.yongpay.top

[U82] JS：package.json 脚本
来源：http://wnd.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gjy.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://omw.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://ydy.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://jvr.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ipf.0kj1m.cn

[U85] JS：可选链
来源：http://rnx.cashguo.top

a?.b?.c
来源：http://npa.zhoulong.xyz

[U86] JS：空值合并
来源：http://puy.xuetiantiany.cn

a ?? b
来源：http://kad.gotoacloud.top

[U87] JS：解构默认值
来源：http://itp.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://urx.ctjpmb.com

[U88] JS：对象展开合并
来源：http://jar.fzhhl.top

{ ...a, ...b }
来源：http://hcl.cheryme.top

[U89] JS：数组去重
来源：http://ppr.yj20258.top

[...new Set(arr)]
来源：http://kti.mhx1999.top

[U90] JS：数字数组排序
来源：http://erk.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://mar.daria6918.cn

[U91] JS：对象键值遍历
来源：http://gqb.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wnh.hammf.cn

[U92] JS：深拷贝
来源：http://wim.vehdjk.com

structuredClone(obj)
来源：http://tnc.daxiang520.top

[U93] JS：模板字符串
来源：http://qev.dashuyun.cn

`共 ${n} 条`
来源：http://kob.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://rzt.bjfxy.top

const double = x => x * 2;
来源：http://vbe.xinyue.icu

[U95] JS：Promise 包装
来源：http://viw.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://psp.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://ubx.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://frq.shangyingyoupin.top

[U97] JS：并发请求
来源：http://eis.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://udt.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://byt.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wmh.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://qpp.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://pab.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://gam.52xcode.cn

document.querySelector(".item")
来源：http://emn.ppjwa.cn

[U101] JS：classList 操作
来源：http://fpo.bbcook.cn

el.classList.toggle("active")
来源：http://ujy.sjlbkw.cn

[U102] JS：本地存储
来源：http://bel.c1oappe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jpa.aizwys.cn

[U103] JS：定时器
来源：http://juw.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://udn.jyoumei.cn

[U104] JS：防抖
来源：http://vky.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://plb.316326.xyz

[U105] JS：节流
来源：http://mxp.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xpt.ydjk.org.cn

[U106] JS：日期格式化
来源：http://asb.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gaq.zhongyouzk.top

[U107] JS：数字千分位
来源：http://ugi.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mhx.cheryme.top

[U108] JS：随机整数
来源：http://hzz.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bsd.xinyue.icu

[U109] JS：数组分组
来源：http://azb.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://rzy.pycfn.com

[U110] JS：数组分块
来源：http://btx.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iag.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://ulb.snrcjt.cn

new Map(Object.entries(obj))
来源：http://vmt.tianlin.xyz

[U112] JS：字符串补位
来源：http://xoo.ehwqpu.com

"7".padStart(3, "0")
来源：http://ybq.nwbrower.top

[U113] JS：正则替换全部
来源：http://tgr.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://iwp.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://erg.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tkt.pycfn.com

[U115] JS：生成 UUID
来源：http://upd.vehdjk.com

crypto.randomUUID()
来源：http://nie.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://ndr.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://bsy.feifeiyinyue.top

[U117] JS：单元测试
来源：http://umm.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://gth.sjlbkw.cn

[U118] JS：开发服务器
来源：http://ovm.nwbrower.top

npm i -D vite;  npx vite
来源：http://ath.daria6918.cn

[U119] JS：生产构建
来源：http://ouf.cqqwz.cn

npx vite build
来源：http://shh.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://nyr.tarul.cn

import.meta.env.VITE_API_URL
来源：http://thc.haohaochexian.top

================================================================================
来源：http://cpf.hesvh.cn

统计汇总
来源：http://baz.yuanzhike.top

================================================================================
来源：http://iss.birdmap.top

按语言统计（条）：
来源：http://luh.jlsjyb.cn

Python ......... 252
来源：http://mjm.ivvv.top

PHP ............ 252
来源：http://fvc.chenlongwang.top

JavaScript ..... 252
来源：http://thl.jlsjyb.cn

TypeScript ..... 212
来源：http://nna.316326.xyz

Java ........... 212
来源：http://xrn.ctjpmb.com

Go ............. 212
来源：http://ure.sjlbkw.cn

Ruby ........... 212
来源：http://cui.hcnkem.com

C# ............. 212
来源：http://few.ppjwa.cn

C .............. 30
来源：http://nre.pengpengdd.cyou

C++ ............ 30
来源：http://fiw.xylfe.cn

SQL ............ 90
来源：http://thi.dianchejie.cn

Bash ........... 80
来源：http://bcu.fehbvm.com

Kotlin ......... 15
来源：http://swj.fzhhl.top

Swift .......... 15
来源：http://naj.zdbjq.cn

Lua ............ 10
来源：http://njt.andypj.xyz

Perl ........... 10
来源：http://qgi.wangshuangyany.cn

Scala .......... 10
来源：http://akj.jinqigufen.top

------------------------------------
来源：http://vjc.snrcjt.cn

合计 ........... 2106 条
来源：http://fdc.ydjk.org.cn

按章节统计：
来源：http://bta.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xvc.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nwo.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://igz.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qiu.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fpk.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nwn.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zga.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mop.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hsk.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wep.sxryk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cdq.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://edu.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zmd.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vbx.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://umc.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://glk.pycfn.com

Q SQL 专题                              90
来源：http://mau.sxryk.cn

R Bash 专题                             80
来源：http://ykb.yonumen.top

S C / C++ 专题                          60
来源：http://vxc.316326.xyz

T 其他语言补充                          60
来源：http://rrj.svipenyu.cn

U 高频实用片段                         120
来源：http://axo.dashuyun.cn

------------------------------------
来源：http://ubt.yj202588.top

合计                                  2106 条
来源：http://guh.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://njj.zycfv.cn

使用提醒
来源：http://wyq.hnqzz.top

--------------------------------------------------------------------------------
来源：http://gea.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zyx.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xtz.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ajg.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://iux.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oqn.epnwcf.com

—— 文件结束 ——
来源：http://tbp.jqgufenzy.top

================================================================================
来源：http://zau.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://wck.ybcxt.top

Common Programming Examples Cheat Book
来源：http://kyc.0kj1m.cn

================================================================================
来源：http://psm.xziqi.cn

【收录内容】
来源：http://pcz.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ynb.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ubn.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://dsg.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xmf.shanyushiyangkeji.top

【使用说明】
来源：http://ckd.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tkq.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kdr.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wtx.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qwc.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://reg.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pvd.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oac.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uxa.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gve.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xgi.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eqz.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qen.tarul.cn

【文件统计】
来源：http://cze.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xqv.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://bbc.aibaodan.cn

目  录
来源：http://grw.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://vro.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ggt.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ipx.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yas.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wpc.jinqigufen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://akp.dashuyun.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qqx.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fpe.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://abs.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wdn.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ckv.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baw.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://orp.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tcl.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gpe.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aaz.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jqt.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qar.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://voi.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://znj.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vri.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vgs.iojbl.cn

================================================================================
来源：http://whr.cqqwz.cn

A. 基础语法与类型
来源：http://som.yj202588.top

================================================================================
来源：http://axa.andypj.xyz

[A01] Hello World
来源：http://vjm.hywenlv.cn

Py:   print("Hello, World!")
来源：http://kby.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://jaq.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://rjx.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zln.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://mub.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://qsj.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://yob.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://taf.yfazqb.com

[A02] 变量声明与赋值
来源：http://qyy.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lvv.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hzn.svipenyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vqo.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hug.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://flc.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://sid.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://zro.cucudq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vek.tian-w.cn

[A03] 常量定义
来源：http://dbt.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pfl.ydzc1.top

PHP:  const PI = 3.14159;
来源：http://jwj.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://udw.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://zub.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://lpd.chenzaomai.com

Go:   const PI = 3.14159
来源：http://ylh.cqqwz.cn

Ruby: PI = 3.14159
来源：http://krc.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://oji.hesvh.cn

[A04] 判断变量类型
来源：http://wjv.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://asl.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nkv.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sxc.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://hgb.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hic.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dqz.shanyushiyangtech.top

Ruby: x.class; x.is_a?(Integer)
来源：http://nrg.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://xxr.yueranfly.top

[A05] 整数除法与取模
来源：http://ljc.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gnq.jinqigfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nmu.wangdashe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dyv.jinyuanbaomall.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jwa.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://eix.dashuyun.cn

Go:   7 / 2; 7 % 2
来源：http://ssl.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://myb.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://cxk.yj20258.top

[A06] 字符串转数字
来源：http://pke.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://dre.fehbvm.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://loh.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bhs.fktsv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ade.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rlk.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uhi.jyoumei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qat.fehbvm.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gir.hysaishi.cn

[A07] 数字转字符串
来源：http://gik.hfpthk.cn

Py:   str(42)
来源：http://qlc.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://mii.bbcook.cn

JS:   String(42); (42).toString()
来源：http://lzg.guowangkeji.top

TS:   String(42)
来源：http://apw.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nwi.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://jai.yuxming.cn

Ruby: 42.to_s
来源：http://crs.fzhhl.top

C#:   42.ToString()
来源：http://xkz.jianghu66.top

[A08] 取整与四舍五入
来源：http://eyu.nwbrower.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://njf.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://khy.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://arb.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://avp.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gga.shangyingyoupin.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ofb.tian-w.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bhd.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xax.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://yps.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gch.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yph.ywan-chungtsiang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ddm.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hjr.jinqigfzy.top


<!-- 参考信息 -->