代发 wailian999

[U75] PHP：依赖注入
来源：http://vis.gotoacloud.top

composer require psr/container
来源：http://qxa.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://wxu.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qcj.fengsongda.top

[U77] PHP：模板渲染
来源：http://kxd.zhoulong.xyz

composer require twig/twig
来源：http://cio.52xcode.cn

[U78] PHP：单元测试
来源：http://uex.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://nky.yanxiufei.cn

[U79] PHP：静态分析
来源：http://nhx.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://qiu.tian-w.cn

[U80] PHP：代码规范修复
来源：http://cxh.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ffr.aibaodan.cn

[U81] JS：初始化项目
来源：http://gpq.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://ouw.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://qoh.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ump.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://wgy.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fxa.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://tne.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://pii.cdnleiting.top

[U85] JS：可选链
来源：http://doj.gzhubu.top

a?.b?.c
来源：http://yas.52xcode.cn

[U86] JS：空值合并
来源：http://lvf.hysaishi.cn

a ?? b
来源：http://xgn.yfazqb.com

[U87] JS：解构默认值
来源：http://qdu.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://zgn.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://csf.andypj.xyz

{ ...a, ...b }
来源：http://pzr.ctjpmb.com

[U89] JS：数组去重
来源：http://pai.cashguo.top

[...new Set(arr)]
来源：http://bcu.aizwys.cn

[U90] JS：数字数组排序
来源：http://bmu.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://xph.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://nrk.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zre.9152youxi.cn

[U92] JS：深拷贝
来源：http://lem.fehbvm.com

structuredClone(obj)
来源：http://jxp.jqgufenzy.top

[U93] JS：模板字符串
来源：http://gpj.quarkkingdee.top

`共 ${n} 条`
来源：http://wuv.yangfankeji.com

[U94] JS：箭头函数
来源：http://blz.cqqwz.cn

const double = x => x * 2;
来源：http://nnc.c1oappe.top

[U95] JS：Promise 包装
来源：http://ofk.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://dyu.hammf.cn

[U96] JS：async/await 与异常
来源：http://fih.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ymq.tarul.cn

[U97] JS：并发请求
来源：http://erj.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fva.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://ewq.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://snx.snrcjt.cn

[U99] JS：事件监听
来源：http://xwc.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://ogm.yongpay.top

[U100] JS：DOM 查询
来源：http://xlu.hongshengwenyu.top

document.querySelector(".item")
来源：http://vke.fzhhl.top

[U101] JS：classList 操作
来源：http://tmt.wangdashe.top

el.classList.toggle("active")
来源：http://gdl.hnxiangtu.top

[U102] JS：本地存储
来源：http://zdw.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cph.yj20258888.top

[U103] JS：定时器
来源：http://dus.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://laz.chenzaomai.com

[U104] JS：防抖
来源：http://spp.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://igt.gogol.net.cn

[U105] JS：节流
来源：http://xbh.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://evi.sjlbkw.cn

[U106] JS：日期格式化
来源：http://zco.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qpw.yj202588.top

[U107] JS：数字千分位
来源：http://tua.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dav.ctjpmb.com

[U108] JS：随机整数
来源：http://atz.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jxv.pycfn.com

[U109] JS：数组分组
来源：http://hox.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://qot.nanxinkj.top

[U110] JS：数组分块
来源：http://wcz.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pny.haohaochexian.top

[U111] JS：对象转 Map
来源：http://bzi.jqgfzy.top

new Map(Object.entries(obj))
来源：http://lpi.cashguo.top

[U112] JS：字符串补位
来源：http://itv.xylfe.cn

"7".padStart(3, "0")
来源：http://aey.shzxlz.cn

[U113] JS：正则替换全部
来源：http://dmw.guannengcc.top

s.replaceAll("a", "b")
来源：http://cbp.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://ejt.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://gpg.bbcook.cn

[U115] JS：生成 UUID
来源：http://cta.yanxiufei.cn

crypto.randomUUID()
来源：http://xko.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://dwm.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://ftq.shzxlz.cn

[U117] JS：单元测试
来源：http://gvj.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://guz.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://bwy.mhx1999.top

npm i -D vite;  npx vite
来源：http://qmm.sysykeji.top

[U119] JS：生产构建
来源：http://xxy.hfpthk.cn

npx vite build
来源：http://frr.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://azx.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://zxb.jinqigfzy.top

================================================================================
来源：http://cum.smart0.xyz

统计汇总
来源：http://kpj.zhengqikj.top

================================================================================
来源：http://jks.snrcjt.cn

按语言统计（条）：
来源：http://egc.andypj.xyz

Python ......... 252
来源：http://yew.jinqigufen.top

PHP ............ 252
来源：http://oso.gotoacloud.top

JavaScript ..... 252
来源：http://rfe.zdbjq.cn

TypeScript ..... 212
来源：http://dgp.vehdjk.com

Java ........... 212
来源：http://lvp.yueranfly.top

Go ............. 212
来源：http://guj.jinqigfzy.top

Ruby ........... 212
来源：http://zir.yonumen.top

C# ............. 212
来源：http://akk.zdqjudy.top

C .............. 30
来源：http://qbx.jiagoushi.top

C++ ............ 30
来源：http://emm.ivvv.top

SQL ............ 90
来源：http://tqa.jqgufenzy.top

Bash ........... 80
来源：http://ihe.fktsv.cn

Kotlin ......... 15
来源：http://zpi.vehdjk.com

Swift .......... 15
来源：http://rym.dianchejie.cn

Lua ............ 10
来源：http://jmq.yfazqb.com

Perl ........... 10
来源：http://zen.dashuyun.cn

Scala .......... 10
来源：http://ufo.hnxiangtu.top

------------------------------------
来源：http://rzn.yongpay.top

合计 ........... 2106 条
来源：http://izp.jinqigufen.top

按章节统计：
来源：http://cra.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xwa.yfazqb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jyw.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fpf.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tyh.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://isx.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://neb.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://omm.sysykeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dei.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bew.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fgz.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mhi.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oid.cheryme.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://igs.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rby.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hdt.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wak.haohaochexian.top

Q SQL 专题                              90
来源：http://zgb.hnxiangtu.top

R Bash 专题                             80
来源：http://nuy.andypj.xyz

S C / C++ 专题                          60
来源：http://wun.feifeiyinyue.top

T 其他语言补充                          60
来源：http://emv.tianlin.xyz

U 高频实用片段                         120
来源：http://wex.dianchejie.cn

------------------------------------
来源：http://whe.epnwcf.com

合计                                  2106 条
来源：http://jan.yonumen.top

--------------------------------------------------------------------------------
来源：http://wax.smart0.xyz

使用提醒
来源：http://iuv.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://haw.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iti.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hox.yueranfly.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sxh.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rio.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jqh.vehdjk.com

—— 文件结束 ——
来源：http://xpk.hongshengwenyu.top

================================================================================
来源：http://ayy.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://xma.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://rqd.zhaomingkeji.xyz

================================================================================
来源：http://rrr.xinyue.icu

【收录内容】
来源：http://zhg.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pbt.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sbd.hnqzz.top

SQL · Bash · C · C++
来源：http://cgy.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jdz.fktsv.cn

【使用说明】
来源：http://zsi.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ajk.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://chz.jianghu66.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://myk.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ngj.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pbj.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nku.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zlu.nwbrower.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bla.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://muj.xylfe.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://llc.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hys.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://svx.tianlin.xyz

【文件统计】
来源：http://jbh.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dyi.andypj.xyz

--------------------------------------------------------------------------------
来源：http://uvs.xuetiantiany.cn

目  录
来源：http://lfe.shuidangran.top

--------------------------------------------------------------------------------
来源：http://xms.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iww.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ztm.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fwt.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://egu.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jbh.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zvc.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://adw.epnwcf.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qhi.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oht.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jtk.meibo888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vxv.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tfw.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://byq.birdmap.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vsx.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hsy.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mgh.shuidangran.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zlr.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://vih.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lln.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://psz.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://psq.yonumen.top

================================================================================
来源：http://bko.c1oappe.top

A. 基础语法与类型
来源：http://loc.ivvv.top

================================================================================
来源：http://qqh.guowangkeji.top

[A01] Hello World
来源：http://hbx.chenlongwang.top

Py:   print("Hello, World!")
来源：http://ahs.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://ogo.birdmap.top

JS:   console.log("Hello, World!");
来源：http://kiz.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bue.ppjwa.cn

Java: System.out.println("Hello, World!");
来源：http://zjq.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://naq.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://wtc.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://dnh.ivvv.top

[A02] 变量声明与赋值
来源：http://ucw.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lnq.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sis.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://hxs.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://njf.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://uvj.sysykeji.top

Go:   name := "Alex"; age := 20
来源：http://fpm.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://akg.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kmh.shangyingyoupin.top

[A03] 常量定义
来源：http://fir.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cuh.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://qjc.svipenyu.cn

JS:   const PI = 3.14159;
来源：http://aif.xinyue.icu

TS:   const PI: number = 3.14159;
来源：http://xxm.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://rcp.yongpay.top

Go:   const PI = 3.14159
来源：http://nlw.jyoumei.cn

Ruby: PI = 3.14159
来源：http://zje.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://cyo.tianlin.xyz

[A04] 判断变量类型
来源：http://rpe.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kql.xylfe.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://buf.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bvo.wangdashe.top

TS:   typeof x; x instanceof Date
来源：http://hdp.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ycj.zdqjudy.top

Go:   reflect.TypeOf(x).Name()
来源：http://rxu.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://fbv.nanxuanxn.top

C#:   x.GetType().Name; x is int
来源：http://rmk.cdnleiting.top

[A05] 整数除法与取模
来源：http://jkd.shanyushiyangtech.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tns.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bcs.zhiwuduotai.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lpj.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pgj.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://tga.ydzc1.top

Go:   7 / 2; 7 % 2
来源：http://cjx.shanyushiyangtech.top

Ruby: 7 / 2; 7 % 2
来源：http://hro.quarkkingdee.top

C#:   7 / 2; 7 % 2
来源：http://pjf.cheryme.top

[A06] 字符串转数字
来源：http://dww.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://snf.chenlongwang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cih.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tkm.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://ylx.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wgu.jinghuilouyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pjz.yueranfly.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nen.cheryme.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sza.cashguo.top

[A07] 数字转字符串
来源：http://rta.cqqwz.cn

Py:   str(42)
来源：http://nkf.zdbjq.cn

PHP:  (string) 42; strval(42)
来源：http://brx.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://lxz.yangfankeji.com

TS:   String(42)
来源：http://wjt.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mgr.yj20258888.top

Go:   strconv.Itoa(42)
来源：http://trk.tian-w.cn

Ruby: 42.to_s
来源：http://oal.xziqi.cn

C#:   42.ToString()
来源：http://vqg.chenjidiqi.icu

[A08] 取整与四舍五入
来源：http://sud.svipenyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vgz.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ygu.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nsa.dashuyun.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qev.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://itj.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vlf.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fzw.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jym.epnwcf.com

[A09] 绝对值与最大最小值
来源：http://jyl.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kdm.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ibu.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cec.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qyf.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cgt.yuanzhike.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uce.ctjpmb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://plv.xziqi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ism.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://lob.redwolf501.top

Py:   import random; random.randint(1, 100)
来源：http://omy.tanke756.top

PHP:  random_int(1, 100);
来源：http://zmy.sjlbkw.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iqk.birdmap.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mvq.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://hpr.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lbg.jinqigufen.top

Ruby: rand(1..100)
来源：http://lzf.gaohongyu789.top

C#:   new Random().Next(1, 101)
来源：http://spb.redwolf501.top

[A11] 条件表达式（三元）
来源：http://eic.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://msc.c1oappe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zgm.tanke756.top

JS:   x > 0 ? "yes" : "no"
来源：http://dlm.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://wib.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://rcf.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nyl.zhixingplan.top

Ruby: x > 0 ? "yes" : "no"
来源：http://roq.chenzaomai.com

C#:   x > 0 ? "yes" : "no"
来源：http://efr.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://kbz.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hdd.yueranfly.top


<!-- 参考信息 -->