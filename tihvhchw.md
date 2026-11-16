代发 wailian999

[U77] PHP：模板渲染
来源：http://twz.guowangkeji.top

composer require twig/twig
来源：http://vko.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://wye.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://uln.redwolf501.top

[U79] PHP：静态分析
来源：http://ctx.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://fxt.xziqi.cn

[U80] PHP：代码规范修复
来源：http://rul.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://haq.cheryme.top

[U81] JS：初始化项目
来源：http://blr.aibaodan.cn

npm init -y;  npm i express
来源：http://xbq.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://uom.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xku.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://wyf.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zjy.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://oyj.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://hua.ydjk.org.cn

[U85] JS：可选链
来源：http://oec.hammf.cn

a?.b?.c
来源：http://scq.sysykeji.top

[U86] JS：空值合并
来源：http://pbk.jlsjyb.cn

a ?? b
来源：http://ces.hfpthk.cn

[U87] JS：解构默认值
来源：http://onw.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://ayw.jyoumei.cn

[U88] JS：对象展开合并
来源：http://csd.shanyushiyangtech.top

{ ...a, ...b }
来源：http://pkn.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://ltr.mhx1999.top

[...new Set(arr)]
来源：http://axx.c1oappe.top

[U90] JS：数字数组排序
来源：http://yal.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://ohf.iojbl.cn

[U91] JS：对象键值遍历
来源：http://wxv.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kya.bbcook.cn

[U92] JS：深拷贝
来源：http://mfd.tianlin.xyz

structuredClone(obj)
来源：http://bkc.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://mqh.bbcook.cn

`共 ${n} 条`
来源：http://agb.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://idn.sysykeji.top

const double = x => x * 2;
来源：http://bfg.mhx1999.top

[U95] JS：Promise 包装
来源：http://cmv.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://khp.cheryme.top

[U96] JS：async/await 与异常
来源：http://syd.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ewe.sysykeji.top

[U97] JS：并发请求
来源：http://eex.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zjg.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://qll.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ifo.chenzaomai.com

[U99] JS：事件监听
来源：http://lsn.316326.xyz

el.addEventListener("click", e => {})
来源：http://faj.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://ype.ppjwa.cn

document.querySelector(".item")
来源：http://klq.zycfv.cn

[U101] JS：classList 操作
来源：http://iox.cashguo.top

el.classList.toggle("active")
来源：http://krf.yueranfly.top

[U102] JS：本地存储
来源：http://atf.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qvz.cqqwz.cn

[U103] JS：定时器
来源：http://zcl.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ifg.jlsjyb.cn

[U104] JS：防抖
来源：http://pwn.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdm.fzhhl.top

[U105] JS：节流
来源：http://dlh.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://koe.fengsongda.top

[U106] JS：日期格式化
来源：http://wxx.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jrz.daria6918.cn

[U107] JS：数字千分位
来源：http://sbf.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xyd.fzhhl.top

[U108] JS：随机整数
来源：http://djc.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tvy.xuanzx.com

[U109] JS：数组分组
来源：http://qxe.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://qwp.jlsjyb.cn

[U110] JS：数组分块
来源：http://yjc.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dis.hnqzz.top

[U111] JS：对象转 Map
来源：http://moq.fengsongda.top

new Map(Object.entries(obj))
来源：http://pwb.guannengcc.top

[U112] JS：字符串补位
来源：http://uvn.hysaishi.cn

"7".padStart(3, "0")
来源：http://evf.nwbrower.top

[U113] JS：正则替换全部
来源：http://vgz.havefunace.top

s.replaceAll("a", "b")
来源：http://wsl.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://qfk.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rkj.ydzc1.top

[U115] JS：生成 UUID
来源：http://hde.pycfn.com

crypto.randomUUID()
来源：http://afx.jqgufenzy.top

[U116] JS：类型检查（JSDoc）
来源：http://bfz.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://fck.havefunace.top

[U117] JS：单元测试
来源：http://gew.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://xcv.zycfv.cn

[U118] JS：开发服务器
来源：http://dxx.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://uce.gaohongyu789.top

[U119] JS：生产构建
来源：http://yxm.xziqi.cn

npx vite build
来源：http://dyc.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://dvn.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://ncx.hfpthk.cn

================================================================================
来源：http://xdq.yfazqb.com

统计汇总
来源：http://lbc.xuanzx.com

================================================================================
来源：http://ivs.zhijiandao.cn

按语言统计（条）：
来源：http://brk.ywan-chungtsiang.top

Python ......... 252
来源：http://cgs.chenlongwang.top

PHP ............ 252
来源：http://icy.andypj.xyz

JavaScript ..... 252
来源：http://seo.9152youxi.cn

TypeScript ..... 212
来源：http://hjv.zdbjq.cn

Java ........... 212
来源：http://wdx.sysykeji.top

Go ............. 212
来源：http://mfx.hnqzz.top

Ruby ........... 212
来源：http://ybl.havefunace.top

C# ............. 212
来源：http://npt.uphjek.com

C .............. 30
来源：http://cqb.vqdsnc.cn

C++ ............ 30
来源：http://sjo.hysaishi.cn

SQL ............ 90
来源：http://jth.epnwcf.com

Bash ........... 80
来源：http://vpm.52xcode.cn

Kotlin ......... 15
来源：http://jlj.pengpengdd.cyou

Swift .......... 15
来源：http://qff.cqqwz.cn

Lua ............ 10
来源：http://hgg.zdbjq.cn

Perl ........... 10
来源：http://urh.316326.xyz

Scala .......... 10
来源：http://xln.hnxiangtu.top

------------------------------------
来源：http://smw.hysaishi.cn

合计 ........... 2106 条
来源：http://cdz.cashguo.top

按章节统计：
来源：http://pwp.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fuz.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hop.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pxh.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dqh.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://esx.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://thf.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pdl.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nta.ivvv.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xhk.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kcx.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://suf.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ust.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fuu.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aby.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://asm.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ncv.9152youxi.cn

Q SQL 专题                              90
来源：http://xob.vehdjk.com

R Bash 专题                             80
来源：http://mio.hywenlv.cn

S C / C++ 专题                          60
来源：http://cuf.52xcode.cn

T 其他语言补充                          60
来源：http://agi.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://vln.nanxinkj.top

------------------------------------
来源：http://mah.daxiang520.top

合计                                  2106 条
来源：http://blw.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://pdu.9152youxi.cn

使用提醒
来源：http://ggd.52xcode.cn

--------------------------------------------------------------------------------
来源：http://wsu.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cxf.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://txl.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yoy.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bcc.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rdn.zhengqikj.top

—— 文件结束 ——
来源：http://gds.havefunace.top

================================================================================
来源：http://cug.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://bny.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://nvw.fehbvm.com

================================================================================
来源：http://uor.zhaomingkeji.xyz

【收录内容】
来源：http://ogi.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ijv.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://txt.xinyue.icu

SQL · Bash · C · C++
来源：http://alp.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tdq.birdmap.top

【使用说明】
来源：http://wzg.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xhk.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wkr.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://daz.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wlm.hnxiangtu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://stm.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eta.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ikh.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lsr.nwbrower.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ixi.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uex.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wdg.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cjr.yj20258888.top

【文件统计】
来源：http://lme.ehwqpu.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dpx.yonumen.top

--------------------------------------------------------------------------------
来源：http://apn.havefunace.top

目  录
来源：http://sku.birdmap.top

--------------------------------------------------------------------------------
来源：http://dak.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jtd.quarkkingdee.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sdm.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kje.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ajx.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://inz.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eio.uphjek.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wdl.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lsi.quarkkingdee.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://afy.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://shs.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jpu.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://swm.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yxu.yongpay.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bny.havefunace.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://teh.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xfs.andypj.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nsf.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ftp.feifeiyinyue.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yby.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zaf.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sbp.bjfxy.top

================================================================================
来源：http://wvi.52xcode.cn

A. 基础语法与类型
来源：http://fhs.shangyingyoupin.top

================================================================================
来源：http://wuu.ydzc1.top

[A01] Hello World
来源：http://uob.andypj.xyz

Py:   print("Hello, World!")
来源：http://tqv.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://tva.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://kpa.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gjc.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://sav.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://dlj.cashguo.top

Ruby: puts "Hello, World!"
来源：http://szq.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://ndd.yonumen.top

[A02] 变量声明与赋值
来源：http://eek.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eaz.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zwa.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://oxh.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://csl.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://tpe.wangshuangyany.cn

Go:   name := "Alex"; age := 20
来源：http://loy.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://fyt.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://shd.xinyue.icu

[A03] 常量定义
来源：http://qtn.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kyp.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://gwh.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://ymv.guannengcc.top

TS:   const PI: number = 3.14159;
来源：http://rex.tarul.cn

Java: static final double PI = 3.14159;
来源：http://fzy.tian-w.cn

Go:   const PI = 3.14159
来源：http://cme.yangfankeji.com

Ruby: PI = 3.14159
来源：http://pbb.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://eds.hfpthk.cn

[A04] 判断变量类型
来源：http://inu.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xkp.yfazqb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mye.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ttt.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://ouj.ppjwa.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://itc.ybcxt.top

Go:   reflect.TypeOf(x).Name()
来源：http://yzv.snrcjt.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://omx.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://zky.sysykeji.top

[A05] 整数除法与取模
来源：http://pty.chenzaomai.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gal.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://sgv.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cjn.sufxvd.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xfd.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://jgo.haohaochexian.top

Go:   7 / 2; 7 % 2
来源：http://jni.jqgufenzy.top

Ruby: 7 / 2; 7 % 2
来源：http://fcm.shzxlz.cn

C#:   7 / 2; 7 % 2
来源：http://qdh.quarkkingdee.top

[A06] 字符串转数字
来源：http://ivg.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://cpy.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cuz.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sqq.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://llb.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hcy.kuanghao11.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jfm.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ocu.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://txh.shangyingyoupin.top

[A07] 数字转字符串
来源：http://jzl.9152youxi.cn

Py:   str(42)
来源：http://afq.xuanzx.com

PHP:  (string) 42; strval(42)
来源：http://yzm.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://ulb.xziqi.cn

TS:   String(42)
来源：http://ryx.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://laa.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://tqv.316326.xyz

Ruby: 42.to_s
来源：http://gga.jianghu66.top

C#:   42.ToString()
来源：http://uui.andypj.xyz

[A08] 取整与四舍五入
来源：http://ujz.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://isz.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ndo.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lkr.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://unw.9152youxi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://shj.haohaochexian.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sre.birdmap.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ykk.hysaishi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rtw.hcnkem.com

[A09] 绝对值与最大最小值
来源：http://ctu.cheryme.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sjj.redwolf501.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rtr.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ody.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rki.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lnz.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jxh.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zuz.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wfq.jinghuilouyu.cn

[A10] 生成随机数
来源：http://nea.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://flo.xziqi.cn

PHP:  random_int(1, 100);
来源：http://mly.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ypm.bbcook.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ubc.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://hll.redwolf501.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tym.nwbrower.top

Ruby: rand(1..100)
来源：http://tdh.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://drl.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://dan.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://hxy.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sdc.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://rwe.nanxuanxn.top

TS:   x > 0 ? "yes" : "no"
来源：http://wwc.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://kpr.quarkkingdee.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fmb.hongshengwenyu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tmq.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://srl.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://jcu.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gjx.xuanzx.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fwe.yj20258.top

JS:   `Hello, ${name}!`
来源：http://oeb.jianghu66.top

TS:   `Hello, ${name}!`
来源：http://lql.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://non.feifeiyinyue.top


<!-- 参考信息 -->