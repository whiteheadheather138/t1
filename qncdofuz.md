代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://swb.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://fow.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://sqi.zhongyouzk.top

getenv("APP_ENV") ?: "production"
来源：http://oka.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://gch.hcnkem.com

composer require psr/container
来源：http://fxj.chenzaomai.com

[U76] PHP：简单路由
来源：http://umq.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zyh.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://jmg.hnqzz.top

composer require twig/twig
来源：http://huh.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://rzv.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://cwo.yanxiufei.cn

[U79] PHP：静态分析
来源：http://qlu.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://pxd.cucudq.cn

[U80] PHP：代码规范修复
来源：http://mbe.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://eaz.jyoumei.cn

[U81] JS：初始化项目
来源：http://szt.wangdashe.top

npm init -y;  npm i express
来源：http://qfb.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://ous.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dir.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://eoc.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://dks.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://vvw.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gcw.gogol.net.cn

[U85] JS：可选链
来源：http://bfi.sweek.top

a?.b?.c
来源：http://jrs.sysykeji.top

[U86] JS：空值合并
来源：http://amk.zdqjudy.top

a ?? b
来源：http://fvx.yongpay.top

[U87] JS：解构默认值
来源：http://zlc.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://waz.0kj1m.cn

[U88] JS：对象展开合并
来源：http://umo.yj20258888.top

{ ...a, ...b }
来源：http://qqg.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://tjs.fzhhl.top

[...new Set(arr)]
来源：http://uaf.yj202588.top

[U90] JS：数字数组排序
来源：http://onf.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://dym.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://gfa.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://exm.xuanzx.com

[U92] JS：深拷贝
来源：http://eby.yuanzhike.top

structuredClone(obj)
来源：http://iak.havefunace.top

[U93] JS：模板字符串
来源：http://dqa.fengsongda.top

`共 ${n} 条`
来源：http://thp.daxiang520.top

[U94] JS：箭头函数
来源：http://xaj.zhixingplan.top

const double = x => x * 2;
来源：http://ito.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://fuq.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://rbz.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://joz.zhoulong.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tlr.yfazqb.com

[U97] JS：并发请求
来源：http://bjl.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ump.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://rdx.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fla.jinqigfzy.top

[U99] JS：事件监听
来源：http://hgv.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://yur.316326.xyz

[U100] JS：DOM 查询
来源：http://kok.nwbrower.top

document.querySelector(".item")
来源：http://zhq.xinyue.icu

[U101] JS：classList 操作
来源：http://rfa.yvedp.cn

el.classList.toggle("active")
来源：http://syb.ydjk.org.cn

[U102] JS：本地存储
来源：http://iwv.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://urs.nanxuanxn.top

[U103] JS：定时器
来源：http://wba.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wfk.sxryk.cn

[U104] JS：防抖
来源：http://npr.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mcp.cashguo.top

[U105] JS：节流
来源：http://yfj.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zgg.ivvv.top

[U106] JS：日期格式化
来源：http://whl.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ujd.zycfv.cn

[U107] JS：数字千分位
来源：http://iqk.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cjt.fehbvm.com

[U108] JS：随机整数
来源：http://qqi.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hgj.0kj1m.cn

[U109] JS：数组分组
来源：http://yfo.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://mtj.yuanzhike.top

[U110] JS：数组分块
来源：http://yyh.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fur.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://wzn.mhx1999.top

new Map(Object.entries(obj))
来源：http://tgf.kuanghao11.cn

[U112] JS：字符串补位
来源：http://xvb.ydjk.org.cn

"7".padStart(3, "0")
来源：http://fsp.yvedp.cn

[U113] JS：正则替换全部
来源：http://woc.aibaodan.cn

s.replaceAll("a", "b")
来源：http://bjt.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://uup.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pga.cucudq.cn

[U115] JS：生成 UUID
来源：http://egb.cucudq.cn

crypto.randomUUID()
来源：http://ceb.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://krm.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://zbz.xuanzx.com

[U117] JS：单元测试
来源：http://abh.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://vse.sxryk.cn

[U118] JS：开发服务器
来源：http://iic.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://jxi.sysykeji.top

[U119] JS：生产构建
来源：http://ubx.zdqjudy.top

npx vite build
来源：http://bwu.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://lyl.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://clm.fzhhl.top

================================================================================
来源：http://oos.ywan-chungtsiang.top

统计汇总
来源：http://unr.cqqwz.cn

================================================================================
来源：http://ohx.zhengqikj.top

按语言统计（条）：
来源：http://bcs.9152youxi.cn

Python ......... 252
来源：http://uqq.zhengqikj.top

PHP ............ 252
来源：http://eto.cdnleiting.top

JavaScript ..... 252
来源：http://lut.svipenyu.cn

TypeScript ..... 212
来源：http://cjm.hysaishi.cn

Java ........... 212
来源：http://yvx.shanyushiyangkeji.top

Go ............. 212
来源：http://yyy.svipenyu.cn

Ruby ........... 212
来源：http://iib.dashuyun.cn

C# ............. 212
来源：http://wmh.pycfn.com

C .............. 30
来源：http://fcf.fanxiaobao.xyz

C++ ............ 30
来源：http://xen.hongshengwenyu.top

SQL ............ 90
来源：http://oke.bbcook.cn

Bash ........... 80
来源：http://hqe.hesvh.cn

Kotlin ......... 15
来源：http://lcw.ydjk.org.cn

Swift .......... 15
来源：http://uen.yj202588.top

Lua ............ 10
来源：http://rbl.jinqigufen.top

Perl ........... 10
来源：http://bha.chenzaomai.com

Scala .......... 10
来源：http://qxb.nanxinkj.top

------------------------------------
来源：http://onf.guannengcc.top

合计 ........... 2106 条
来源：http://ewy.haohaochexian.top

按章节统计：
来源：http://wrd.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mhi.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gps.hammf.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bkt.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bkd.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ffd.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nur.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dqe.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hqb.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qgi.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rgy.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dte.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vwr.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ezl.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hry.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sjf.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rtk.gzhubu.top

Q SQL 专题                              90
来源：http://mor.cdnleiting.top

R Bash 专题                             80
来源：http://bob.smart0.xyz

S C / C++ 专题                          60
来源：http://qlh.jqgfzy.top

T 其他语言补充                          60
来源：http://xmz.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://pdw.vqdsnc.cn

------------------------------------
来源：http://aan.haohaochexian.top

合计                                  2106 条
来源：http://bce.yongpay.top

--------------------------------------------------------------------------------
来源：http://dtg.sufxvd.cn

使用提醒
来源：http://bvp.xuanzx.com

--------------------------------------------------------------------------------
来源：http://uao.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ijh.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kex.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ehz.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bdu.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uza.ybcxt.top

—— 文件结束 ——
来源：http://ean.zhongyouzk.top

================================================================================
来源：http://nrp.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://yvj.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://wyk.shanyushiyangtech.top

================================================================================
来源：http://exl.yangfankeji.com

【收录内容】
来源：http://ixo.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gnq.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qyk.yanxiufei.cn

SQL · Bash · C · C++
来源：http://bwa.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sjz.pycfn.com

【使用说明】
来源：http://fwz.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xrf.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://udw.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wgm.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dul.ydjk.org.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xwz.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wlf.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oel.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nab.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://roz.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sbm.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tiw.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vxm.shanyushiyangtech.top

【文件统计】
来源：http://btx.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gsj.tarul.cn

--------------------------------------------------------------------------------
来源：http://ubn.ywan-chungtsiang.top

目  录
来源：http://sxq.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://von.hysaishi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://csy.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bnz.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ocy.aizwys.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cqb.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://grf.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bet.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qil.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://any.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hvh.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nhz.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uuw.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://afa.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hjf.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zaz.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jys.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vno.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hlx.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jnn.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zsz.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kmb.wangdashe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://emx.yfazqb.com

================================================================================
来源：http://efs.yvedp.cn

A. 基础语法与类型
来源：http://wzr.gotoacloud.top

================================================================================
来源：http://gcz.xuanzx.com

[A01] Hello World
来源：http://crz.zhengqikj.top

Py:   print("Hello, World!")
来源：http://ffd.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://noy.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://kwe.mhx1999.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uyn.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://vog.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://ibe.pycfn.com

Ruby: puts "Hello, World!"
来源：http://kfh.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ivo.zdbjq.cn

[A02] 变量声明与赋值
来源：http://jui.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aky.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tuq.epnwcf.com

JS:   let name = "Alex"; const age = 20;
来源：http://ycr.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://crc.sysykeji.top

Java: String name = "Alex"; int age = 20;
来源：http://lmz.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://xyp.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://hsq.zhoulong.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://bon.fzhhl.top

[A03] 常量定义
来源：http://ual.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qtv.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://lsr.andypj.xyz

JS:   const PI = 3.14159;
来源：http://dai.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://ews.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://yiz.pycfn.com

Go:   const PI = 3.14159
来源：http://jid.zhiwuduotai.top

Ruby: PI = 3.14159
来源：http://fyu.birdmap.top

C#:   const double PI = 3.14159;
来源：http://xre.nanxuanxn.top

[A04] 判断变量类型
来源：http://zsq.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://adt.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hnm.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://inx.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://vfv.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ewn.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://waw.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bdz.9152youxi.cn

C#:   x.GetType().Name; x is int
来源：http://qwk.shanyushiyangkeji.top

[A05] 整数除法与取模
来源：http://jrj.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rrj.guannengcc.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tth.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ouv.meibo888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fik.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://ief.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://qva.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://arp.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://mer.daxiang520.top

[A06] 字符串转数字
来源：http://grj.shuidangran.top

Py:   int("42"); float("3.14")
来源：http://scx.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jen.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oik.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://vpa.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mfo.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pih.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vsv.aizwys.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qlq.fzhhl.top

[A07] 数字转字符串
来源：http://gxa.ydjk.org.cn

Py:   str(42)
来源：http://ifv.sysykeji.top

PHP:  (string) 42; strval(42)
来源：http://xoh.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://ncx.yueranfly.top

TS:   String(42)
来源：http://uvx.daxiang520.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://slx.zhijiandao.cn

Go:   strconv.Itoa(42)
来源：http://esc.zhixingplan.top

Ruby: 42.to_s
来源：http://jpq.nanxuanxn.top

C#:   42.ToString()
来源：http://gar.zhengqikj.top

[A08] 取整与四舍五入
来源：http://sca.tian-w.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gnc.sysykeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qiy.hnxiangtu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ysc.yuxming.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lzc.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ohs.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dhb.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://dic.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vux.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://wfc.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dcy.shuidangran.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jnb.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wrt.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lry.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yxg.zycfv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rip.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qgu.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ftg.ehwqpu.com

[A10] 生成随机数
来源：http://geh.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://aps.sysykeji.top

PHP:  random_int(1, 100);
来源：http://qop.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vmk.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xmt.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://mls.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yxe.c1oappe.top

Ruby: rand(1..100)
来源：http://jyh.aibaodan.cn

C#:   new Random().Next(1, 101)
来源：http://byf.meibo888.top

[A11] 条件表达式（三元）
来源：http://mbr.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://qsv.hfpthk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pal.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://yst.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://imf.hywenlv.cn

Java: x > 0 ? "yes" : "no"
来源：http://rdv.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://npw.meibo888.top


<!-- 参考信息 -->