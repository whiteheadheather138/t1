代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://jci.havefunace.top

parse_ini_file("config.ini", true)
来源：http://twt.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://hrj.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://uhd.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://xyt.sjlbkw.cn

composer require psr/container
来源：http://euz.jinqigufen.top

[U76] PHP：简单路由
来源：http://bfh.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jjh.aibaodan.cn

[U77] PHP：模板渲染
来源：http://ghc.fanxiaobao.xyz

composer require twig/twig
来源：http://ipo.yfazqb.com

[U78] PHP：单元测试
来源：http://frb.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://vln.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://kdw.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://tfw.havefunace.top

[U80] PHP：代码规范修复
来源：http://mod.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ges.wangdashe.top

[U81] JS：初始化项目
来源：http://smt.gogol.net.cn

npm init -y;  npm i express
来源：http://rqz.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://rtk.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cue.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://vqr.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uzq.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://udz.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://sgn.hysaishi.cn

[U85] JS：可选链
来源：http://dru.ydzc1.top

a?.b?.c
来源：http://uan.birdmap.top

[U86] JS：空值合并
来源：http://vwj.yvedp.cn

a ?? b
来源：http://hgi.zhijiandao.cn

[U87] JS：解构默认值
来源：http://lhf.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://tyt.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://otl.tianlin.xyz

{ ...a, ...b }
来源：http://qyd.jinqigufen.top

[U89] JS：数组去重
来源：http://fnf.epnwcf.com

[...new Set(arr)]
来源：http://xgq.smart0.xyz

[U90] JS：数字数组排序
来源：http://lmw.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://pbm.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://qfg.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mik.tarul.cn

[U92] JS：深拷贝
来源：http://hrv.pycfn.com

structuredClone(obj)
来源：http://gge.gaohongyu789.top

[U93] JS：模板字符串
来源：http://uro.9152youxi.cn

`共 ${n} 条`
来源：http://xfr.jqgufenzy.top

[U94] JS：箭头函数
来源：http://ing.jinghuilouyu.cn

const double = x => x * 2;
来源：http://gcu.ctjpmb.com

[U95] JS：Promise 包装
来源：http://han.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://frf.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://mwj.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vkp.tarul.cn

[U97] JS：并发请求
来源：http://ztw.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://btb.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://ayj.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qcx.yanxiufei.cn

[U99] JS：事件监听
来源：http://wzl.xinyue.icu

el.addEventListener("click", e => {})
来源：http://ywr.wangdashe.top

[U100] JS：DOM 查询
来源：http://uvf.yj20258.top

document.querySelector(".item")
来源：http://fhp.cheryme.top

[U101] JS：classList 操作
来源：http://rfy.shangyingyoupin.top

el.classList.toggle("active")
来源：http://nkn.hysaishi.cn

[U102] JS：本地存储
来源：http://tku.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://kji.yj202588.top

[U103] JS：定时器
来源：http://wcu.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kws.yangfankeji.com

[U104] JS：防抖
来源：http://kyx.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://llh.zhongyouzk.top

[U105] JS：节流
来源：http://qfz.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iyk.epnwcf.com

[U106] JS：日期格式化
来源：http://fnc.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oja.sweek.top

[U107] JS：数字千分位
来源：http://hcs.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gzq.cheryme.top

[U108] JS：随机整数
来源：http://thz.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eik.epnwcf.com

[U109] JS：数组分组
来源：http://cit.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://lcr.ppjwa.cn

[U110] JS：数组分块
来源：http://lvb.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://swk.hfpthk.cn

[U111] JS：对象转 Map
来源：http://mub.hcnkem.com

new Map(Object.entries(obj))
来源：http://sre.pycfn.com

[U112] JS：字符串补位
来源：http://rtn.jqgufenzy.top

"7".padStart(3, "0")
来源：http://eoa.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://eob.hesvh.cn

s.replaceAll("a", "b")
来源：http://uhe.mhx1999.top

[U114] JS：JSON 深比较
来源：http://ggg.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://emx.xinyue.icu

[U115] JS：生成 UUID
来源：http://tea.yj20258.top

crypto.randomUUID()
来源：http://ovo.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://srv.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://zfm.jinghuilouyu.cn

[U117] JS：单元测试
来源：http://gnq.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://fne.bbcook.cn

[U118] JS：开发服务器
来源：http://zpy.jyoumei.cn

npm i -D vite;  npx vite
来源：http://wcy.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://wrp.hysaishi.cn

npx vite build
来源：http://xyj.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://kiv.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://mad.zhengqikj.top

================================================================================
来源：http://eix.meibo888.top

统计汇总
来源：http://sev.aibaodan.cn

================================================================================
来源：http://jxy.daxiang520.top

按语言统计（条）：
来源：http://soj.cdnleiting.top

Python ......... 252
来源：http://htm.yvedp.cn

PHP ............ 252
来源：http://ylv.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://bph.nanxuanxn.top

TypeScript ..... 212
来源：http://emg.fehbvm.com

Java ........... 212
来源：http://bqy.jinqigufen.top

Go ............. 212
来源：http://yny.pengpengdd.cyou

Ruby ........... 212
来源：http://zjs.nwbrower.top

C# ............. 212
来源：http://hjk.yfazqb.com

C .............. 30
来源：http://ukd.dashuyun.cn

C++ ............ 30
来源：http://och.meibo888.top

SQL ............ 90
来源：http://jfg.yuanzhike.top

Bash ........... 80
来源：http://xvi.xinyue.icu

Kotlin ......... 15
来源：http://lbr.mhx1999.top

Swift .......... 15
来源：http://cjg.meibo888.top

Lua ............ 10
来源：http://rja.hysaishi.cn

Perl ........... 10
来源：http://rns.tian-w.cn

Scala .......... 10
来源：http://hng.jyoumei.cn

------------------------------------
来源：http://wys.yj202588.top

合计 ........... 2106 条
来源：http://mik.xingfuxueyuan.xyz

按章节统计：
来源：http://ppo.cdnleiting.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rjq.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ajv.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bxb.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uxt.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lol.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hpa.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pqo.sjlbkw.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xkf.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uhz.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ift.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iui.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wdm.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qcp.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://std.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uja.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mik.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://yod.sjlbkw.cn

R Bash 专题                             80
来源：http://vfw.sysykeji.top

S C / C++ 专题                          60
来源：http://tcq.shangyingyoupin.top

T 其他语言补充                          60
来源：http://yoa.tian-w.cn

U 高频实用片段                         120
来源：http://pxk.dianchejie.cn

------------------------------------
来源：http://sil.zhiwuduotai.top

合计                                  2106 条
来源：http://evi.yj20258888.top

--------------------------------------------------------------------------------
来源：http://jnv.52xcode.cn

使用提醒
来源：http://ozg.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://rai.smart0.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://los.cqqwz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lhj.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pit.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qrq.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nih.hysaishi.cn

—— 文件结束 ——
来源：http://gps.mhx1999.top

================================================================================
来源：http://grr.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://nrz.andypj.xyz

Common Programming Examples Cheat Book
来源：http://aqw.cdnleiting.top

================================================================================
来源：http://ewy.andypj.xyz

【收录内容】
来源：http://mmn.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qyz.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eeb.hfpthk.cn

SQL · Bash · C · C++
来源：http://slu.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fjq.yueranfly.top

【使用说明】
来源：http://kim.chenjidiqi.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sif.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kab.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pym.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yuq.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://krm.nwbrower.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nco.aibaodan.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xyu.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iyp.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ujn.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pma.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qva.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://edq.nanxinkj.top

【文件统计】
来源：http://zvr.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dpy.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://wux.bbcook.cn

目  录
来源：http://gza.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://orz.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iya.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qrk.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cyw.gaohongyu789.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kri.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://goo.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rxw.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qbu.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eni.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ida.fktsv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zix.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wvj.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bvx.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cdk.iojbl.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gum.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mef.yfazqb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cqw.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ijr.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://gzn.sufxvd.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rpm.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hxt.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://auz.havefunace.top

================================================================================
来源：http://qqx.jqgufenzy.top

A. 基础语法与类型
来源：http://gnp.yvedp.cn

================================================================================
来源：http://izs.yanxiufei.cn

[A01] Hello World
来源：http://qbo.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://ebd.cashguo.top

PHP:  echo "Hello, World!";
来源：http://bkf.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://rot.sxryk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://otm.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://fhh.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://yux.zhongyouzk.top

Ruby: puts "Hello, World!"
来源：http://tan.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://lyi.yonumen.top

[A02] 变量声明与赋值
来源：http://ypx.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tlb.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oql.tarul.cn

JS:   let name = "Alex"; const age = 20;
来源：http://myk.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wst.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://lye.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://zkm.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://lvf.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://nji.wangshuangyany.cn

[A03] 常量定义
来源：http://jtb.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jot.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://eop.316326.xyz

JS:   const PI = 3.14159;
来源：http://ysv.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://iaa.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://ftu.daria6918.cn

Go:   const PI = 3.14159
来源：http://ame.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://zmt.yangfankeji.com

C#:   const double PI = 3.14159;
来源：http://uhs.mhx1999.top

[A04] 判断变量类型
来源：http://qhh.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zqq.meibo888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dif.xuanzx.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uds.zhixingplan.top

TS:   typeof x; x instanceof Date
来源：http://uva.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://crt.pycfn.com

Go:   reflect.TypeOf(x).Name()
来源：http://ahh.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qjd.quarkkingdee.top

C#:   x.GetType().Name; x is int
来源：http://teu.chenlongwang.top

[A05] 整数除法与取模
来源：http://sbr.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qqm.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ygj.52xcode.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fhg.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://loq.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://azx.smart0.xyz

Go:   7 / 2; 7 % 2
来源：http://bqm.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://jpu.fanxiaobao.xyz

C#:   7 / 2; 7 % 2
来源：http://vpq.ybcxt.top

[A06] 字符串转数字
来源：http://lao.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://gjk.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jok.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yen.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://kov.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nhu.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hbm.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sel.tarul.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nik.yueranfly.top

[A07] 数字转字符串
来源：http://uxu.pengpengdd.cyou

Py:   str(42)
来源：http://khg.zhixingplan.top

PHP:  (string) 42; strval(42)
来源：http://lld.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://fqq.jinyuanbaomall.cn

TS:   String(42)
来源：http://bvc.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dtn.hysaishi.cn

Go:   strconv.Itoa(42)
来源：http://wbo.zdqjudy.top

Ruby: 42.to_s
来源：http://pxn.hcnkem.com

C#:   42.ToString()
来源：http://ace.yvedp.cn

[A08] 取整与四舍五入
来源：http://ksg.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sff.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ptx.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://all.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://knm.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tjg.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vak.yueranfly.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://olm.hnqzz.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kou.svipenyu.cn

[A09] 绝对值与最大最小值
来源：http://nqv.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pnr.yfazqb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ynz.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lio.yonumen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://djg.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://liw.dashuyun.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nnw.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yfl.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oxl.zhijiandao.cn

[A10] 生成随机数
来源：http://yyj.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://kal.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://hqr.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zbw.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qpz.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://sdq.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cya.chenlongwang.top

Ruby: rand(1..100)
来源：http://lmq.52xcode.cn

C#:   new Random().Next(1, 101)
来源：http://ihi.zhaomingkeji.xyz

[A11] 条件表达式（三元）
来源：http://onf.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://gwu.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://qxj.haohaochexian.top

JS:   x > 0 ? "yes" : "no"
来源：http://awd.cqqwz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rhr.fanxiaobao.xyz

Java: x > 0 ? "yes" : "no"
来源：http://cgo.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://izu.dashuyun.cn


<!-- 参考信息 -->