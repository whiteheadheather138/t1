代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://mwm.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://wqc.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://mxj.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://abm.316326.xyz

[U85] JS：可选链
来源：http://prv.cheryme.top

a?.b?.c
来源：http://cov.wangshuangyany.cn

[U86] JS：空值合并
来源：http://lla.zhiwuduotai.top

a ?? b
来源：http://szj.yvedp.cn

[U87] JS：解构默认值
来源：http://qve.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://mjb.shzxlz.cn

[U88] JS：对象展开合并
来源：http://shq.wangshuangyany.cn

{ ...a, ...b }
来源：http://tnt.zhoulong.xyz

[U89] JS：数组去重
来源：http://jdz.cheryme.top

[...new Set(arr)]
来源：http://wpa.shzxlz.cn

[U90] JS：数字数组排序
来源：http://znq.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://mxi.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://rwd.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ohp.jinqigufen.top

[U92] JS：深拷贝
来源：http://ppw.zhengqikj.top

structuredClone(obj)
来源：http://vgk.zdbjq.cn

[U93] JS：模板字符串
来源：http://jvu.andypj.xyz

`共 ${n} 条`
来源：http://ezq.yfazqb.com

[U94] JS：箭头函数
来源：http://ulc.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://koy.xziqi.cn

[U95] JS：Promise 包装
来源：http://ssr.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://vpg.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://ntt.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vnu.dashuyun.cn

[U97] JS：并发请求
来源：http://ttn.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qff.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://cvr.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nbm.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://ibn.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://quj.cheryme.top

[U100] JS：DOM 查询
来源：http://tlj.andypj.xyz

document.querySelector(".item")
来源：http://jmh.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://dvv.nanxuanxn.top

el.classList.toggle("active")
来源：http://wmr.chenlongwang.top

[U102] JS：本地存储
来源：http://jwk.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vee.0kj1m.cn

[U103] JS：定时器
来源：http://tfq.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lsj.cucudq.cn

[U104] JS：防抖
来源：http://bxh.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofl.jlsjyb.cn

[U105] JS：节流
来源：http://moh.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hnw.gzhubu.top

[U106] JS：日期格式化
来源：http://xri.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mji.zhongyouzk.top

[U107] JS：数字千分位
来源：http://ura.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gaq.snrcjt.cn

[U108] JS：随机整数
来源：http://vab.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dqe.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://zba.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://auv.zhoulong.xyz

[U110] JS：数组分块
来源：http://nsg.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khp.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://vwe.yongpay.top

new Map(Object.entries(obj))
来源：http://wmy.fengsongda.top

[U112] JS：字符串补位
来源：http://gyy.chenzaomai.com

"7".padStart(3, "0")
来源：http://ufz.meibo888.top

[U113] JS：正则替换全部
来源：http://duq.daria6918.cn

s.replaceAll("a", "b")
来源：http://abq.gzhubu.top

[U114] JS：JSON 深比较
来源：http://mtl.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kup.ivvv.top

[U115] JS：生成 UUID
来源：http://tlp.svipenyu.cn

crypto.randomUUID()
来源：http://xbo.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://eju.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://glf.mhx1999.top

[U117] JS：单元测试
来源：http://sft.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://ldl.hcnkem.com

[U118] JS：开发服务器
来源：http://dxc.yangfankeji.com

npm i -D vite;  npx vite
来源：http://ykq.cheryme.top

[U119] JS：生产构建
来源：http://zfm.shanyushiyangtech.top

npx vite build
来源：http://qkd.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://hrf.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://tzy.jiagoushi.top

================================================================================
来源：http://fnh.tarul.cn

统计汇总
来源：http://pkr.xingfuxueyuan.xyz

================================================================================
来源：http://zmj.hcnkem.com

按语言统计（条）：
来源：http://xlc.snrcjt.cn

Python ......... 252
来源：http://usm.cdnleiting.top

PHP ............ 252
来源：http://ebe.yangfankeji.com

JavaScript ..... 252
来源：http://pbc.sxryk.cn

TypeScript ..... 212
来源：http://sri.cucudq.cn

Java ........... 212
来源：http://vwx.feifeiyinyue.top

Go ............. 212
来源：http://yvf.quarkkingdee.top

Ruby ........... 212
来源：http://pjp.nanxuanxn.top

C# ............. 212
来源：http://dmm.aizwys.cn

C .............. 30
来源：http://qgt.cdnleiting.top

C++ ............ 30
来源：http://tog.hnqzz.top

SQL ............ 90
来源：http://uom.fzhhl.top

Bash ........... 80
来源：http://rmo.gaohongyu789.top

Kotlin ......... 15
来源：http://jup.zdqjudy.top

Swift .......... 15
来源：http://pcj.sweek.top

Lua ............ 10
来源：http://vxs.cucudq.cn

Perl ........... 10
来源：http://cax.0kj1m.cn

Scala .......... 10
来源：http://zvz.ctjpmb.com

------------------------------------
来源：http://bfi.hnqzz.top

合计 ........... 2106 条
来源：http://ewq.hcnkem.com

按章节统计：
来源：http://sla.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://guq.cqqwz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mco.vehdjk.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vyn.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://avr.yangfankeji.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tlx.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://izl.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://foh.yj202588.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wnj.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tos.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mrt.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jtf.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zwp.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zuh.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://unt.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mak.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://smy.ydzc1.top

Q SQL 专题                              90
来源：http://wxf.gotoacloud.top

R Bash 专题                             80
来源：http://laf.cucudq.cn

S C / C++ 专题                          60
来源：http://eec.yueranfly.top

T 其他语言补充                          60
来源：http://xye.pycfn.com

U 高频实用片段                         120
来源：http://tzw.sxryk.cn

------------------------------------
来源：http://rzg.shanyushiyangtech.top

合计                                  2106 条
来源：http://tjq.xylfe.cn

--------------------------------------------------------------------------------
来源：http://rdb.yvedp.cn

使用提醒
来源：http://omy.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://lqm.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://akb.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fjc.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kwl.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://coz.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xhq.zycfv.cn

—— 文件结束 ——
来源：http://sef.zhengqikj.top

================================================================================
来源：http://dri.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://wft.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://pek.ivvv.top

================================================================================
来源：http://nhm.xuetiantiany.cn

【收录内容】
来源：http://gck.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bum.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wjo.ydzc1.top

SQL · Bash · C · C++
来源：http://dlj.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rde.sufxvd.cn

【使用说明】
来源：http://cnj.zhixingplan.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fev.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zsa.jianghu66.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wqq.pengpengdd.cyou

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xza.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://cjg.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yaj.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cic.hfpthk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ely.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vmr.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fvg.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://prd.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://myd.xuanzx.com

【文件统计】
来源：http://uun.zhaomingkeji.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rcr.cheryme.top

--------------------------------------------------------------------------------
来源：http://qfz.zhengqikj.top

目  录
来源：http://xnn.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://lsx.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hfe.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ymt.zycfv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sna.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://spr.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://woz.yuxming.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qey.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ahm.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wlv.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://foz.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qgg.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bqi.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hip.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ikp.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tan.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qip.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zsh.sjlbkw.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vaa.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://obg.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bny.gaohongyu789.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sdw.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nsg.iojbl.cn

================================================================================
来源：http://jki.xuanzx.com

A. 基础语法与类型
来源：http://xbc.ywan-chungtsiang.top

================================================================================
来源：http://dfg.aizwys.cn

[A01] Hello World
来源：http://eew.hysaishi.cn

Py:   print("Hello, World!")
来源：http://hzo.ywan-chungtsiang.top

PHP:  echo "Hello, World!";
来源：http://ild.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://vhu.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ehd.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://zzf.yuxming.cn

Go:   fmt.Println("Hello, World!")
来源：http://jbe.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://isu.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pgx.ivvv.top

[A02] 变量声明与赋值
来源：http://ozf.tianlin.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jfb.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hei.epnwcf.com

JS:   let name = "Alex"; const age = 20;
来源：http://gdy.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wwf.hnxiangtu.top

Java: String name = "Alex"; int age = 20;
来源：http://gqg.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://cxz.jinyuanbaomall.cn

Ruby: name = "Alex"; age = 20
来源：http://npc.0kj1m.cn

C#:   string name = "Alex"; int age = 20;
来源：http://frz.cashguo.top

[A03] 常量定义
来源：http://dxu.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://olw.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://eng.jinqigfzy.top

JS:   const PI = 3.14159;
来源：http://mxs.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://cbs.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://bsy.tian-w.cn

Go:   const PI = 3.14159
来源：http://rzf.ehwqpu.com

Ruby: PI = 3.14159
来源：http://jel.yj20258888.top

C#:   const double PI = 3.14159;
来源：http://vfb.c1oappe.top

[A04] 判断变量类型
来源：http://ecl.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xfm.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fpi.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yqm.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://tdz.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hlv.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nmw.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jag.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://usq.shuidangran.top

[A05] 整数除法与取模
来源：http://iiu.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hse.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rwu.smart0.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://udt.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fsh.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://xzi.sjlbkw.cn

Go:   7 / 2; 7 % 2
来源：http://omg.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://yed.ppjwa.cn

C#:   7 / 2; 7 % 2
来源：http://kdk.9152youxi.cn

[A06] 字符串转数字
来源：http://jfc.hysaishi.cn

Py:   int("42"); float("3.14")
来源：http://mco.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aqi.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eic.52xcode.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bnx.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rtb.hongshengwenyu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xlj.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jbh.sweek.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kag.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://ucy.iojbl.cn

Py:   str(42)
来源：http://qyl.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://mwv.zhongyouzk.top

JS:   String(42); (42).toString()
来源：http://xpx.ppjwa.cn

TS:   String(42)
来源：http://rkj.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://err.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://ogr.redwolf501.top

Ruby: 42.to_s
来源：http://ota.hongshengwenyu.top

C#:   42.ToString()
来源：http://vlr.jlsjyb.cn

[A08] 取整与四舍五入
来源：http://ibn.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qhx.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ikb.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sno.nanxinkj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://opn.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tfj.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nfl.gzhubu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bsp.cqqwz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zzh.gogol.net.cn

[A09] 绝对值与最大最小值
来源：http://yrx.316326.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pft.uphjek.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kcy.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kib.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yka.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ung.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zhp.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zwb.hfpthk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eet.kuanghao11.cn

[A10] 生成随机数
来源：http://coc.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://aox.cucudq.cn

PHP:  random_int(1, 100);
来源：http://hqo.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wzm.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nps.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://vjl.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rhu.jqgufenzy.top

Ruby: rand(1..100)
来源：http://tsj.xylfe.cn

C#:   new Random().Next(1, 101)
来源：http://ddg.nwbrower.top

[A11] 条件表达式（三元）
来源：http://bvc.xingfuxueyuan.xyz

Py:   "yes" if x > 0 else "no"
来源：http://hxt.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cwo.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pcm.shangyingyoupin.top

TS:   x > 0 ? "yes" : "no"
来源：http://avn.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://row.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gvu.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hug.hcnkem.com

C#:   x > 0 ? "yes" : "no"
来源：http://wwr.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://srf.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mpw.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://byq.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://yzt.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://saf.yonumen.top

Java: "Hello, %s!".formatted(name)
来源：http://wxt.sxryk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kkh.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://ecv.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://fka.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dxf.cashguo.top

Py:   "第一行\n第二行"
来源：http://lgs.wangdashe.top

PHP:  "第一行\n第二行"
来源：http://wpm.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://zhz.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://zvj.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://xce.yonumen.top

Go:   "第一行\n第二行"
来源：http://kmm.9152youxi.cn

Ruby: "第一行\n第二行"
来源：http://nua.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://hvk.kuanghao11.cn


<!-- 参考信息 -->