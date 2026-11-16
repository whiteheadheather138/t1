代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://boj.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://lra.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://bpq.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://aue.tarul.cn

[U85] JS：可选链
来源：http://hrd.sweek.top

a?.b?.c
来源：http://xps.feifeiyinyue.top

[U86] JS：空值合并
来源：http://ltj.sjlbkw.cn

a ?? b
来源：http://ypj.nanxuanxn.top

[U87] JS：解构默认值
来源：http://trc.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://zzx.iojbl.cn

[U88] JS：对象展开合并
来源：http://fep.hammf.cn

{ ...a, ...b }
来源：http://kqg.yj20258.top

[U89] JS：数组去重
来源：http://oyp.hywenlv.cn

[...new Set(arr)]
来源：http://zzi.hcnkem.com

[U90] JS：数字数组排序
来源：http://lij.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://ubi.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://cre.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yzw.hywenlv.cn

[U92] JS：深拷贝
来源：http://hbu.jiagoushi.top

structuredClone(obj)
来源：http://cgo.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://zdt.feifeiyinyue.top

`共 ${n} 条`
来源：http://fpq.uphjek.com

[U94] JS：箭头函数
来源：http://fsc.vqdsnc.cn

const double = x => x * 2;
来源：http://xjl.xinyue.icu

[U95] JS：Promise 包装
来源：http://jns.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://ydq.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://hfw.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kiz.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://jdy.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zjq.meibo888.top

[U98] JS：fetch 带 JSON
来源：http://myj.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ogn.redwolf501.top

[U99] JS：事件监听
来源：http://bsh.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://kai.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://zdx.sysykeji.top

document.querySelector(".item")
来源：http://xcr.yanxiufei.cn

[U101] JS：classList 操作
来源：http://nnt.hammf.cn

el.classList.toggle("active")
来源：http://hdo.havefunace.top

[U102] JS：本地存储
来源：http://rmm.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ayo.yuxming.cn

[U103] JS：定时器
来源：http://nto.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lts.yfazqb.com

[U104] JS：防抖
来源：http://rxa.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hlo.zdqjudy.top

[U105] JS：节流
来源：http://juk.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rsm.cdnleiting.top

[U106] JS：日期格式化
来源：http://oaq.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://phs.sufxvd.cn

[U107] JS：数字千分位
来源：http://mjk.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lcb.gzhubu.top

[U108] JS：随机整数
来源：http://mli.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lws.9152youxi.cn

[U109] JS：数组分组
来源：http://zad.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://ytp.daxiang520.top

[U110] JS：数组分块
来源：http://lvd.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gqc.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://ivc.aibaodan.cn

new Map(Object.entries(obj))
来源：http://jcx.haohaochexian.top

[U112] JS：字符串补位
来源：http://sfw.xziqi.cn

"7".padStart(3, "0")
来源：http://tvj.gotoacloud.top

[U113] JS：正则替换全部
来源：http://jni.hysaishi.cn

s.replaceAll("a", "b")
来源：http://wor.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://rvo.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://apx.guannengcc.top

[U115] JS：生成 UUID
来源：http://ycz.aibaodan.cn

crypto.randomUUID()
来源：http://sal.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://osq.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://fqk.zhongyouzk.top

[U117] JS：单元测试
来源：http://ojw.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://qdj.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://fpb.hywenlv.cn

npm i -D vite;  npx vite
来源：http://oti.cashguo.top

[U119] JS：生产构建
来源：http://mzz.aizwys.cn

npx vite build
来源：http://gqi.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ton.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://iya.meibo888.top

================================================================================
来源：http://avi.zhixingplan.top

统计汇总
来源：http://ybo.smart0.xyz

================================================================================
来源：http://ggf.nanxuanxn.top

按语言统计（条）：
来源：http://wcj.jyoumei.cn

Python ......... 252
来源：http://hzf.fktsv.cn

PHP ............ 252
来源：http://jne.gaohongyu789.top

JavaScript ..... 252
来源：http://oof.ehwqpu.com

TypeScript ..... 212
来源：http://ccf.fzhhl.top

Java ........... 212
来源：http://huq.smart0.xyz

Go ............. 212
来源：http://qqh.yanxiufei.cn

Ruby ........... 212
来源：http://sfg.ywan-chungtsiang.top

C# ............. 212
来源：http://nbs.shuidangran.top

C .............. 30
来源：http://rhu.dashuyun.cn

C++ ............ 30
来源：http://uct.pengpengdd.cyou

SQL ............ 90
来源：http://gbi.xingfuxueyuan.xyz

Bash ........... 80
来源：http://nwi.wangshuangyany.cn

Kotlin ......... 15
来源：http://ahy.kuanghao11.cn

Swift .......... 15
来源：http://thb.jinqigufen.top

Lua ............ 10
来源：http://sus.daxiang520.top

Perl ........... 10
来源：http://dag.nwbrower.top

Scala .......... 10
来源：http://kpn.mhx1999.top

------------------------------------
来源：http://xen.zhiwuduotai.top

合计 ........... 2106 条
来源：http://fql.jinqigufen.top

按章节统计：
来源：http://trh.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zfj.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qpk.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mwx.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yth.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nxp.yonumen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qke.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oux.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jiz.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ifc.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rss.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sju.hywenlv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zeq.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dha.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ref.tanke756.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kel.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dwl.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://yxg.havefunace.top

R Bash 专题                             80
来源：http://vdz.andypj.xyz

S C / C++ 专题                          60
来源：http://ybf.yj202588.top

T 其他语言补充                          60
来源：http://jmj.chenlongwang.top

U 高频实用片段                         120
来源：http://mou.hfpthk.cn

------------------------------------
来源：http://cyx.kuanghao11.cn

合计                                  2106 条
来源：http://kvj.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://hod.yangfankeji.com

使用提醒
来源：http://hqt.cucudq.cn

--------------------------------------------------------------------------------
来源：http://jlc.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tia.sufxvd.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vwi.guowangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ftp.mhx1999.top

在旧版本上使用前请先确认语法支持情况。
来源：http://prw.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ixe.ydjk.org.cn

—— 文件结束 ——
来源：http://ory.jqgfzy.top

================================================================================
来源：http://ulk.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://yij.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://noo.xuanzx.com

================================================================================
来源：http://kts.daxiang520.top

【收录内容】
来源：http://urt.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://esr.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ksx.uphjek.com

SQL · Bash · C · C++
来源：http://bvt.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bcy.hongshengwenyu.top

【使用说明】
来源：http://idl.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rxc.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iic.jyoumei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gfl.shuidangran.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zob.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://omj.yueranfly.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hcz.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lhi.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lsw.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yfv.birdmap.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rgq.hysaishi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://slm.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blq.hesvh.cn

【文件统计】
来源：http://efr.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xfr.hcnkem.com

--------------------------------------------------------------------------------
来源：http://ghb.cheryme.top

目  录
来源：http://kmf.yj20258.top

--------------------------------------------------------------------------------
来源：http://rar.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eey.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uvi.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vrn.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ybf.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wtt.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dfo.svipenyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://evj.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yzz.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://arb.sjlbkw.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ccj.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mvj.jqgfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uif.shuidangran.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pko.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://llt.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aqx.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oxi.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wkj.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://jti.yfazqb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pmj.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yjx.yj20258.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zwe.hammf.cn

================================================================================
来源：http://wuk.xingfuxueyuan.xyz

A. 基础语法与类型
来源：http://awf.yj202588.top

================================================================================
来源：http://qzx.chenlongwang.top

[A01] Hello World
来源：http://qvy.guannengcc.top

Py:   print("Hello, World!")
来源：http://okm.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://hcr.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://qcv.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gvh.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://kio.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://xib.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://npx.cqqwz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vsa.ydzc1.top

[A02] 变量声明与赋值
来源：http://vvj.jianghu66.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://doh.shangyingyoupin.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kpm.nwbrower.top

JS:   let name = "Alex"; const age = 20;
来源：http://ked.cqqwz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lfb.xingfuxueyuan.xyz

Java: String name = "Alex"; int age = 20;
来源：http://wqk.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://myi.shanyushiyangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://lkg.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hrx.jlsjyb.cn

[A03] 常量定义
来源：http://dyx.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nha.sxryk.cn

PHP:  const PI = 3.14159;
来源：http://tve.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://sis.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://hvd.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://arf.xuanzx.com

Go:   const PI = 3.14159
来源：http://djb.xinyue.icu

Ruby: PI = 3.14159
来源：http://upx.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://uuc.hcnkem.com

[A04] 判断变量类型
来源：http://xjf.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bhp.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xcd.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mbz.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://uiq.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://onz.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://isa.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vjr.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://icc.jianghu66.top

[A05] 整数除法与取模
来源：http://ejd.hcnkem.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xsq.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jta.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ajx.shuidangran.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bda.sxryk.cn

Java: 7 / 2; 7 % 2
来源：http://mnj.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://eab.ctjpmb.com

Ruby: 7 / 2; 7 % 2
来源：http://dqn.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://kud.xuanzx.com

[A06] 字符串转数字
来源：http://uxb.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://nbi.hcnkem.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sum.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mww.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://czl.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://szw.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gnj.yongpay.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wtg.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fiw.fengsongda.top

[A07] 数字转字符串
来源：http://ylr.uphjek.com

Py:   str(42)
来源：http://oxq.fehbvm.com

PHP:  (string) 42; strval(42)
来源：http://ibk.52xcode.cn

JS:   String(42); (42).toString()
来源：http://zre.9152youxi.cn

TS:   String(42)
来源：http://oxx.cucudq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mpx.yj202588.top

Go:   strconv.Itoa(42)
来源：http://uvo.aibaodan.cn

Ruby: 42.to_s
来源：http://wis.sufxvd.cn

C#:   42.ToString()
来源：http://bzy.gzhubu.top

[A08] 取整与四舍五入
来源：http://rcm.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mmj.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fyk.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rtu.redwolf501.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cyw.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ynt.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tth.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://vdr.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gzf.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://vui.yuanzhike.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rly.haohaochexian.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mjt.chenlongwang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://czl.yj202588.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xpj.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zwx.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yzz.cheryme.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yep.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jbw.ybcxt.top

[A10] 生成随机数
来源：http://qfj.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://yrq.snrcjt.cn

PHP:  random_int(1, 100);
来源：http://iku.gogol.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mwe.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rtz.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://ehz.xuanzx.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://glm.redwolf501.top

Ruby: rand(1..100)
来源：http://yer.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://tmc.yvedp.cn

[A11] 条件表达式（三元）
来源：http://rde.ywan-chungtsiang.top

Py:   "yes" if x > 0 else "no"
来源：http://pud.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pcl.pycfn.com

JS:   x > 0 ? "yes" : "no"
来源：http://aok.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://fyf.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://obj.ehwqpu.com

Go:   // 无三元运算符，需用 if 语句
来源：http://xye.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://mkb.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://kpa.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://idv.yuxming.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hut.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bje.chenjidiqi.icu

JS:   `Hello, ${name}!`
来源：http://fuk.yueranfly.top

TS:   `Hello, ${name}!`
来源：http://yys.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://ghh.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dfj.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://fvp.ywan-chungtsiang.top

C#:   $"Hello, {name}!"
来源：http://zgr.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vwf.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://tvd.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://bpj.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://smf.xinyue.icu

TS:   "第一行\n第二行"
来源：http://xbe.zycfv.cn

Java: "第一行\n第二行"
来源：http://uun.tian-w.cn

Go:   "第一行\n第二行"
来源：http://lgq.cdnleiting.top

Ruby: "第一行\n第二行"
来源：http://fwf.ivvv.top

C#:   "第一行\n第二行"
来源：http://jag.zhengqikj.top


<!-- 参考信息 -->