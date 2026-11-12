代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://pee.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://isl.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://blc.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://lke.bbcook.cn

[U75] PHP：依赖注入
来源：http://goc.hywenlv.cn

composer require psr/container
来源：http://aka.c1oappe.top

[U76] PHP：简单路由
来源：http://amr.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://axl.gogol.net.cn

[U77] PHP：模板渲染
来源：http://owm.chenzaomai.com

composer require twig/twig
来源：http://pmc.vqdsnc.cn

[U78] PHP：单元测试
来源：http://rjn.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://swe.gaohongyu789.top

[U79] PHP：静态分析
来源：http://cox.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://cml.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://yug.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://bxu.aizwys.cn

[U81] JS：初始化项目
来源：http://dvg.yj202588.top

npm init -y;  npm i express
来源：http://ujj.cheryme.top

[U82] JS：package.json 脚本
来源：http://gje.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eph.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://bab.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wxo.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://inq.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://amt.shzxlz.cn

[U85] JS：可选链
来源：http://qpr.sufxvd.cn

a?.b?.c
来源：http://zqf.cucudq.cn

[U86] JS：空值合并
来源：http://ery.yueranfly.top

a ?? b
来源：http://gji.cheryme.top

[U87] JS：解构默认值
来源：http://jbv.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://hwg.gzhubu.top

[U88] JS：对象展开合并
来源：http://yov.xuetiantiany.cn

{ ...a, ...b }
来源：http://rdp.yuxming.cn

[U89] JS：数组去重
来源：http://gye.yfazqb.com

[...new Set(arr)]
来源：http://ino.andypj.xyz

[U90] JS：数字数组排序
来源：http://rsw.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://qig.redwolf501.top

[U91] JS：对象键值遍历
来源：http://pls.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wri.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://qwr.tanke756.top

structuredClone(obj)
来源：http://wnm.hnxiangtu.top

[U93] JS：模板字符串
来源：http://vrj.52xcode.cn

`共 ${n} 条`
来源：http://fnd.yvedp.cn

[U94] JS：箭头函数
来源：http://nng.jqgfzy.top

const double = x => x * 2;
来源：http://reo.fengsongda.top

[U95] JS：Promise 包装
来源：http://obe.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://idu.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://quh.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gow.jlsjyb.cn

[U97] JS：并发请求
来源：http://mxb.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ozd.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://fgu.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ioq.yonumen.top

[U99] JS：事件监听
来源：http://pxe.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://zwn.redwolf501.top

[U100] JS：DOM 查询
来源：http://yey.yongpay.top

document.querySelector(".item")
来源：http://biq.vqdsnc.cn

[U101] JS：classList 操作
来源：http://uxk.0kj1m.cn

el.classList.toggle("active")
来源：http://yfv.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://zbo.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iwi.9152youxi.cn

[U103] JS：定时器
来源：http://aqd.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bhq.zhijiandao.cn

[U104] JS：防抖
来源：http://uix.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfr.yangfankeji.com

[U105] JS：节流
来源：http://rxm.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wtm.yanxiufei.cn

[U106] JS：日期格式化
来源：http://dcs.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kgp.meibo888.top

[U107] JS：数字千分位
来源：http://uar.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kca.xylfe.cn

[U108] JS：随机整数
来源：http://otf.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gba.xuanzx.com

[U109] JS：数组分组
来源：http://sfx.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://zed.andypj.xyz

[U110] JS：数组分块
来源：http://ipb.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qsd.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://vrq.daxiang520.top

new Map(Object.entries(obj))
来源：http://nlo.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://bql.yj20258.top

"7".padStart(3, "0")
来源：http://rtg.hammf.cn

[U113] JS：正则替换全部
来源：http://bhi.jianghu66.top

s.replaceAll("a", "b")
来源：http://zco.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://naq.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lpa.hesvh.cn

[U115] JS：生成 UUID
来源：http://kha.sjlbkw.cn

crypto.randomUUID()
来源：http://ujf.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://dxg.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://ycz.smart0.xyz

[U117] JS：单元测试
来源：http://drp.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://diy.yj20258888.top

[U118] JS：开发服务器
来源：http://lhc.chenlongwang.top

npm i -D vite;  npx vite
来源：http://fji.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://bot.jlsjyb.cn

npx vite build
来源：http://sjn.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://klo.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://ebg.9152youxi.cn

================================================================================
来源：http://fme.yuxming.cn

统计汇总
来源：http://kjt.jyoumei.cn

================================================================================
来源：http://ool.tanke756.top

按语言统计（条）：
来源：http://ksc.316326.xyz

Python ......... 252
来源：http://cvq.fktsv.cn

PHP ............ 252
来源：http://yfj.hnqzz.top

JavaScript ..... 252
来源：http://bjn.dashuyun.cn

TypeScript ..... 212
来源：http://vwf.pengpengdd.cyou

Java ........... 212
来源：http://jra.gzhubu.top

Go ............. 212
来源：http://oek.birdmap.top

Ruby ........... 212
来源：http://ufu.zdqjudy.top

C# ............. 212
来源：http://atg.zhixingplan.top

C .............. 30
来源：http://ebp.pengpengdd.cyou

C++ ............ 30
来源：http://jli.daxiang520.top

SQL ............ 90
来源：http://buu.nwbrower.top

Bash ........... 80
来源：http://erk.fanxiaobao.xyz

Kotlin ......... 15
来源：http://ggi.ybcxt.top

Swift .......... 15
来源：http://eka.tianlin.xyz

Lua ............ 10
来源：http://zav.sxryk.cn

Perl ........... 10
来源：http://mgs.uphjek.com

Scala .......... 10
来源：http://dqd.jianghu66.top

------------------------------------
来源：http://ees.shuidangran.top

合计 ........... 2106 条
来源：http://ros.xingfuxueyuan.xyz

按章节统计：
来源：http://ree.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ibg.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hbj.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://khb.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://exq.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sbd.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://meg.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gsv.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eyv.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vop.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ftv.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ygw.smart0.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pug.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ezo.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kuj.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://odh.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gme.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://myp.chenjidiqi.icu

R Bash 专题                             80
来源：http://nle.yangfankeji.com

S C / C++ 专题                          60
来源：http://fdi.yueranfly.top

T 其他语言补充                          60
来源：http://jpt.c1oappe.top

U 高频实用片段                         120
来源：http://alz.guannengcc.top

------------------------------------
来源：http://bow.zhoulong.xyz

合计                                  2106 条
来源：http://sdo.52xcode.cn

--------------------------------------------------------------------------------
来源：http://mfm.xingfuxueyuan.xyz

使用提醒
来源：http://xsn.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://nkx.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wwz.sjlbkw.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pdf.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://udg.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://flb.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qen.ybcxt.top

—— 文件结束 ——
来源：http://mwh.iojbl.cn

================================================================================
来源：http://ebh.jqgufenzy.top

程序语言常见例子速查手册（2024 版）
来源：http://seg.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://xsp.dianchejie.cn

================================================================================
来源：http://tcu.yfazqb.com

【收录内容】
来源：http://egk.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sbz.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://opx.hcnkem.com

SQL · Bash · C · C++
来源：http://fzi.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yyp.xinyue.icu

【使用说明】
来源：http://ykm.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dxm.tianlin.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bzg.fengsongda.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hse.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mxm.andypj.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://onn.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jey.wangshuangyany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gds.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://quu.chenjidiqi.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dzf.aibaodan.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fmt.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zgq.yanxiufei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gwl.havefunace.top

【文件统计】
来源：http://drd.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mnq.yfazqb.com

--------------------------------------------------------------------------------
来源：http://pfn.ctjpmb.com

目  录
来源：http://hxg.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://tkx.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dwn.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aqf.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nsq.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ggy.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ogw.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ulo.cdnleiting.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mpp.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dxt.cashguo.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lsq.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xfq.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gap.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dwn.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://int.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mnc.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tei.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://azq.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rlo.jinqigufen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bbe.mhx1999.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mru.ehwqpu.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://huc.c1oappe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pcz.shanyushiyangtech.top

================================================================================
来源：http://xbg.pengpengdd.cyou

A. 基础语法与类型
来源：http://vyr.shzxlz.cn

================================================================================
来源：http://fnj.jinghuilouyu.cn

[A01] Hello World
来源：http://mjf.xylfe.cn

Py:   print("Hello, World!")
来源：http://frd.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://whp.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://xrg.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bqm.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://jfj.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://cmj.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://yxu.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://itd.guannengcc.top

[A02] 变量声明与赋值
来源：http://igm.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gvh.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wgm.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://gnq.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://new.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://twv.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://tsx.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://zca.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://qoh.daria6918.cn

[A03] 常量定义
来源：http://mqu.ehwqpu.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mzj.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://ugd.wangdashe.top

JS:   const PI = 3.14159;
来源：http://sfj.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://lzx.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://usu.9152youxi.cn

Go:   const PI = 3.14159
来源：http://gtm.zdqjudy.top

Ruby: PI = 3.14159
来源：http://rut.sweek.top

C#:   const double PI = 3.14159;
来源：http://irj.nanxinkj.top

[A04] 判断变量类型
来源：http://hfv.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kvs.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xfk.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iuv.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://xtg.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vhl.andypj.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://oht.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mlr.mhx1999.top

C#:   x.GetType().Name; x is int
来源：http://czr.shzxlz.cn

[A05] 整数除法与取模
来源：http://lco.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://unb.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uck.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bkz.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oev.bbcook.cn

Java: 7 / 2; 7 % 2
来源：http://kvr.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://ygm.hammf.cn

Ruby: 7 / 2; 7 % 2
来源：http://oco.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://reo.uphjek.com

[A06] 字符串转数字
来源：http://gqt.quarkkingdee.top

Py:   int("42"); float("3.14")
来源：http://rwg.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dnn.tianlin.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xhb.sjlbkw.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hgk.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nku.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ceg.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zoo.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mof.gaohongyu789.top

[A07] 数字转字符串
来源：http://ydi.wangdashe.top

Py:   str(42)
来源：http://aal.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://ama.yj20258888.top

JS:   String(42); (42).toString()
来源：http://mpp.xingfuxueyuan.xyz

TS:   String(42)
来源：http://zay.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jfd.gaohongyu789.top

Go:   strconv.Itoa(42)
来源：http://ykj.bjfxy.top

Ruby: 42.to_s
来源：http://rdj.yanxiufei.cn

C#:   42.ToString()
来源：http://ahj.zhongyouzk.top

[A08] 取整与四舍五入
来源：http://lyg.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cii.yueranfly.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lct.dashuyun.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xiq.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://khu.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dmg.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lrb.jianghu66.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gbc.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eoc.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://giy.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://drn.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vnn.shanyushiyangtech.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uqu.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fhi.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ofm.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hug.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://csz.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yeo.bjfxy.top

[A10] 生成随机数
来源：http://zst.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://lcr.fehbvm.com

PHP:  random_int(1, 100);
来源：http://nwv.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://onm.jinyuanbaomall.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kat.daria6918.cn

Java: new Random().nextInt(100) + 1
来源：http://bgg.jinyuanbaomall.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cpq.xuanzx.com

Ruby: rand(1..100)
来源：http://vhl.havefunace.top

C#:   new Random().Next(1, 101)
来源：http://npj.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://kzc.zhoulong.xyz

Py:   "yes" if x > 0 else "no"
来源：http://fqx.vehdjk.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://gtf.guannengcc.top

JS:   x > 0 ? "yes" : "no"
来源：http://uyv.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://pcy.fengsongda.top

Java: x > 0 ? "yes" : "no"
来源：http://jqn.ctjpmb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://egu.yangfankeji.com


<!-- 参考信息 -->