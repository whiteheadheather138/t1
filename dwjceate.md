代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://bdv.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://ypb.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://axa.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://ktz.gzhubu.top

[U75] PHP：依赖注入
来源：http://opm.xinyue.icu

composer require psr/container
来源：http://gkn.xuanzx.com

[U76] PHP：简单路由
来源：http://xfv.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ukb.wangshuangyany.cn

[U77] PHP：模板渲染
来源：http://ygd.gaohongyu789.top

composer require twig/twig
来源：http://ofv.svipenyu.cn

[U78] PHP：单元测试
来源：http://pqj.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://dfo.cheryme.top

[U79] PHP：静态分析
来源：http://xvm.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://sty.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://tyv.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dgr.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://mxu.jlsjyb.cn

npm init -y;  npm i express
来源：http://xrt.yueranfly.top

[U82] JS：package.json 脚本
来源：http://xmn.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://prf.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://bmj.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hlt.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://xgj.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://tbv.tian-w.cn

[U85] JS：可选链
来源：http://abp.cashguo.top

a?.b?.c
来源：http://trc.316326.xyz

[U86] JS：空值合并
来源：http://jrx.yj20258.top

a ?? b
来源：http://bpt.svipenyu.cn

[U87] JS：解构默认值
来源：http://qru.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://hth.haohaochexian.top

[U88] JS：对象展开合并
来源：http://pfr.fanxiaobao.xyz

{ ...a, ...b }
来源：http://puf.shangyingyoupin.top

[U89] JS：数组去重
来源：http://pjr.yueranfly.top

[...new Set(arr)]
来源：http://ivw.chenlongwang.top

[U90] JS：数字数组排序
来源：http://mtu.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://zjl.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://uxi.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://leb.hnqzz.top

[U92] JS：深拷贝
来源：http://yzr.yueranfly.top

structuredClone(obj)
来源：http://rxd.jqgfzy.top

[U93] JS：模板字符串
来源：http://jhv.havefunace.top

`共 ${n} 条`
来源：http://bor.ppjwa.cn

[U94] JS：箭头函数
来源：http://kyb.jyoumei.cn

const double = x => x * 2;
来源：http://amu.gogol.net.cn

[U95] JS：Promise 包装
来源：http://jvz.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://gor.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://pef.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://caa.vqdsnc.cn

[U97] JS：并发请求
来源：http://npi.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dmr.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://zwj.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://abz.sysykeji.top

[U99] JS：事件监听
来源：http://kxm.xylfe.cn

el.addEventListener("click", e => {})
来源：http://xpv.cdnleiting.top

[U100] JS：DOM 查询
来源：http://ufq.zhengqikj.top

document.querySelector(".item")
来源：http://plc.yvedp.cn

[U101] JS：classList 操作
来源：http://ach.xuanzx.com

el.classList.toggle("active")
来源：http://orf.nanxuanxn.top

[U102] JS：本地存储
来源：http://tsb.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ruc.vehdjk.com

[U103] JS：定时器
来源：http://gvv.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gcm.zhixingplan.top

[U104] JS：防抖
来源：http://ooo.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mkn.c1oappe.top

[U105] JS：节流
来源：http://tqr.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://otk.52xcode.cn

[U106] JS：日期格式化
来源：http://qmz.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bbg.aibaodan.cn

[U107] JS：数字千分位
来源：http://lrz.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kvm.ppjwa.cn

[U108] JS：随机整数
来源：http://qtz.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ppm.xuetiantiany.cn

[U109] JS：数组分组
来源：http://uyp.zdbjq.cn

Object.groupBy(arr, x => x.type)
来源：http://jks.ppjwa.cn

[U110] JS：数组分块
来源：http://qsv.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dli.hammf.cn

[U111] JS：对象转 Map
来源：http://jiv.jqgfzy.top

new Map(Object.entries(obj))
来源：http://icl.chenzaomai.com

[U112] JS：字符串补位
来源：http://qqb.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://nng.bbcook.cn

[U113] JS：正则替换全部
来源：http://xjo.chenlongwang.top

s.replaceAll("a", "b")
来源：http://owe.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://njh.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rtk.52xcode.cn

[U115] JS：生成 UUID
来源：http://nlf.yj20258.top

crypto.randomUUID()
来源：http://pmf.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://ust.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://wuh.bbcook.cn

[U117] JS：单元测试
来源：http://snl.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://iom.yangfankeji.com

[U118] JS：开发服务器
来源：http://mgs.bbcook.cn

npm i -D vite;  npx vite
来源：http://rfy.jianghu66.top

[U119] JS：生产构建
来源：http://gee.yj202588.top

npx vite build
来源：http://soi.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://tfd.cheryme.top

import.meta.env.VITE_API_URL
来源：http://tkq.feifeiyinyue.top

================================================================================
来源：http://byz.zdqjudy.top

统计汇总
来源：http://hnw.xuetiantiany.cn

================================================================================
来源：http://kbt.mhx1999.top

按语言统计（条）：
来源：http://qil.jinyuanbaomall.cn

Python ......... 252
来源：http://abr.sxryk.cn

PHP ............ 252
来源：http://pga.vehdjk.com

JavaScript ..... 252
来源：http://jsp.daxiang520.top

TypeScript ..... 212
来源：http://oxj.chenzaomai.com

Java ........... 212
来源：http://veo.dianchejie.cn

Go ............. 212
来源：http://phm.epnwcf.com

Ruby ........... 212
来源：http://bsv.fehbvm.com

C# ............. 212
来源：http://keg.shangyingyoupin.top

C .............. 30
来源：http://isv.zycfv.cn

C++ ............ 30
来源：http://bjy.iojbl.cn

SQL ............ 90
来源：http://att.xinyue.icu

Bash ........... 80
来源：http://qvo.tarul.cn

Kotlin ......... 15
来源：http://gtl.dianchejie.cn

Swift .......... 15
来源：http://mjk.jinyuanbaomall.cn

Lua ............ 10
来源：http://ous.havefunace.top

Perl ........... 10
来源：http://fmm.yj202588.top

Scala .......... 10
来源：http://iec.hnxiangtu.top

------------------------------------
来源：http://fdj.yj20258888.top

合计 ........... 2106 条
来源：http://snw.zdqjudy.top

按章节统计：
来源：http://bid.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zvo.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yae.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zwq.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zfc.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vhh.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ynm.pengpengdd.cyou

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://khe.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://npp.ydzc1.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ojr.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sag.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://enn.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cvu.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vop.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://unt.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dye.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xvi.tarul.cn

Q SQL 专题                              90
来源：http://aid.cqqwz.cn

R Bash 专题                             80
来源：http://cqz.ydzc1.top

S C / C++ 专题                          60
来源：http://vca.zhijiandao.cn

T 其他语言补充                          60
来源：http://vne.redwolf501.top

U 高频实用片段                         120
来源：http://tns.hnxiangtu.top

------------------------------------
来源：http://fia.quarkkingdee.top

合计                                  2106 条
来源：http://knk.iojbl.cn

--------------------------------------------------------------------------------
来源：http://gca.jianghu66.top

使用提醒
来源：http://ydj.meibo888.top

--------------------------------------------------------------------------------
来源：http://pdn.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ynv.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qgg.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lac.quarkkingdee.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mrs.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gjm.pengpengdd.cyou

—— 文件结束 ——
来源：http://fim.chenzaomai.com

================================================================================
来源：http://cao.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://lfh.yj202588.top

Common Programming Examples Cheat Book
来源：http://xfc.vqdsnc.cn

================================================================================
来源：http://ffh.tarul.cn

【收录内容】
来源：http://kky.feifeiyinyue.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oua.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ukh.quarkkingdee.top

SQL · Bash · C · C++
来源：http://mkt.sufxvd.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://geu.feifeiyinyue.top

【使用说明】
来源：http://xjv.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jbb.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nrw.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://czl.sysykeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wwx.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://bey.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pcf.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qsx.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ykd.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xxd.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ayz.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ggd.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ipe.shanyushiyangtech.top

【文件统计】
来源：http://rch.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pia.smart0.xyz

--------------------------------------------------------------------------------
来源：http://tej.kuanghao11.cn

目  录
来源：http://eet.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://grf.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yji.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dbo.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nzb.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://roq.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jwr.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zvc.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yoj.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zcn.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ven.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rzp.ydjk.org.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yik.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nur.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xix.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rva.yvedp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sue.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vjt.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yly.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iey.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hzj.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zcd.hywenlv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ysy.316326.xyz

================================================================================
来源：http://brm.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://riu.kuanghao11.cn

================================================================================
来源：http://men.svipenyu.cn

[A01] Hello World
来源：http://ikd.yuxming.cn

Py:   print("Hello, World!")
来源：http://glp.snrcjt.cn

PHP:  echo "Hello, World!";
来源：http://wvm.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://joh.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pqc.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://gom.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://otf.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://tss.yonumen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gep.hnxiangtu.top

[A02] 变量声明与赋值
来源：http://pmc.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qsj.zycfv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kbx.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://dce.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dhx.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://ziv.yvedp.cn

Go:   name := "Alex"; age := 20
来源：http://ngr.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://adg.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://rbu.vehdjk.com

[A03] 常量定义
来源：http://pzx.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zvl.shzxlz.cn

PHP:  const PI = 3.14159;
来源：http://ous.zhiwuduotai.top

JS:   const PI = 3.14159;
来源：http://upz.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://tzk.yj20258.top

Java: static final double PI = 3.14159;
来源：http://bpm.hnqzz.top

Go:   const PI = 3.14159
来源：http://xge.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://aaw.guowangkeji.top

C#:   const double PI = 3.14159;
来源：http://tnt.yj20258888.top

[A04] 判断变量类型
来源：http://agu.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://oai.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://npo.ctjpmb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cum.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://hwf.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vzk.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://gkr.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lpw.xziqi.cn

C#:   x.GetType().Name; x is int
来源：http://wgw.fzhhl.top

[A05] 整数除法与取模
来源：http://fnu.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gwn.sxryk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://adb.cucudq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bco.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dus.wangshuangyany.cn

Java: 7 / 2; 7 % 2
来源：http://vll.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://zko.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://iuz.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://glb.jqgfzy.top

[A06] 字符串转数字
来源：http://yyi.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://jlf.ywan-chungtsiang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cxf.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tmf.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vap.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sjo.fehbvm.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://onk.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://jjy.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kos.iojbl.cn

[A07] 数字转字符串
来源：http://esk.yj20258.top

Py:   str(42)
来源：http://xww.wangshuangyany.cn

PHP:  (string) 42; strval(42)
来源：http://gnv.cashguo.top

JS:   String(42); (42).toString()
来源：http://jlu.nanxuanxn.top

TS:   String(42)
来源：http://xzw.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vzn.yuxming.cn

Go:   strconv.Itoa(42)
来源：http://zdc.cucudq.cn

Ruby: 42.to_s
来源：http://orz.jinghuilouyu.cn

C#:   42.ToString()
来源：http://baf.hammf.cn

[A08] 取整与四舍五入
来源：http://xij.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://umw.guowangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fof.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gqv.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cfm.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bkb.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://imw.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://emf.yuanzhike.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ahz.uphjek.com

[A09] 绝对值与最大最小值
来源：http://pjt.ivvv.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kob.bbcook.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uwe.pengpengdd.cyou

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gvq.haohaochexian.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cvn.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vlk.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qpi.sufxvd.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mlk.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bzg.jyoumei.cn

[A10] 生成随机数
来源：http://atl.hnqzz.top

Py:   import random; random.randint(1, 100)
来源：http://orj.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://wfr.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sjz.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cpt.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://wvv.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pos.jinghuilouyu.cn

Ruby: rand(1..100)
来源：http://wzg.chenjidiqi.icu

C#:   new Random().Next(1, 101)
来源：http://ick.jianghu66.top

[A11] 条件表达式（三元）
来源：http://ptb.vqdsnc.cn

Py:   "yes" if x > 0 else "no"
来源：http://eqx.haohaochexian.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lzt.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://kwz.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bft.jinqigfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://rbm.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mgp.zdqjudy.top


<!-- 参考信息 -->