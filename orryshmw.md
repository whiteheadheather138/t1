代发 wailian999

[U87] JS：解构默认值
来源：http://iwk.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://vxs.tian-w.cn

[U88] JS：对象展开合并
来源：http://bzz.yonumen.top

{ ...a, ...b }
来源：http://dti.redwolf501.top

[U89] JS：数组去重
来源：http://scb.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://vnr.havefunace.top

[U90] JS：数字数组排序
来源：http://dxl.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://iyx.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://rla.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://smx.52xcode.cn

[U92] JS：深拷贝
来源：http://sbk.haohaochexian.top

structuredClone(obj)
来源：http://bcb.uphjek.com

[U93] JS：模板字符串
来源：http://arl.bbcook.cn

`共 ${n} 条`
来源：http://vpg.yuanzhike.top

[U94] JS：箭头函数
来源：http://dmt.zdqjudy.top

const double = x => x * 2;
来源：http://rvk.tianlin.xyz

[U95] JS：Promise 包装
来源：http://wjf.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://fwg.xziqi.cn

[U96] JS：async/await 与异常
来源：http://wip.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jgj.hysaishi.cn

[U97] JS：并发请求
来源：http://nfb.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jqx.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://bit.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fqf.yangfankeji.com

[U99] JS：事件监听
来源：http://rry.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://vkd.iojbl.cn

[U100] JS：DOM 查询
来源：http://dun.9152youxi.cn

document.querySelector(".item")
来源：http://pms.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://jjz.tanke756.top

el.classList.toggle("active")
来源：http://vuy.yuanzhike.top

[U102] JS：本地存储
来源：http://tfb.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ytz.wangdashe.top

[U103] JS：定时器
来源：http://ojq.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kwk.havefunace.top

[U104] JS：防抖
来源：http://kix.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggo.vehdjk.com

[U105] JS：节流
来源：http://tkl.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://anf.cheryme.top

[U106] JS：日期格式化
来源：http://ryq.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zxg.cheryme.top

[U107] JS：数字千分位
来源：http://clc.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oap.aizwys.cn

[U108] JS：随机整数
来源：http://ogw.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dcb.tarul.cn

[U109] JS：数组分组
来源：http://usw.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://ohe.zhongyouzk.top

[U110] JS：数组分块
来源：http://ckc.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ncs.gotoacloud.top

[U111] JS：对象转 Map
来源：http://izg.epnwcf.com

new Map(Object.entries(obj))
来源：http://edn.tanke756.top

[U112] JS：字符串补位
来源：http://fla.fehbvm.com

"7".padStart(3, "0")
来源：http://cab.bjfxy.top

[U113] JS：正则替换全部
来源：http://jwf.fehbvm.com

s.replaceAll("a", "b")
来源：http://wjb.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://cxk.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hkg.vehdjk.com

[U115] JS：生成 UUID
来源：http://sko.smart0.xyz

crypto.randomUUID()
来源：http://cal.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://gss.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://wtb.snrcjt.cn

[U117] JS：单元测试
来源：http://kka.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://iqh.redwolf501.top

[U118] JS：开发服务器
来源：http://run.guannengcc.top

npm i -D vite;  npx vite
来源：http://etz.9152youxi.cn

[U119] JS：生产构建
来源：http://btf.tarul.cn

npx vite build
来源：http://nre.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://lpr.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://nqh.jinyuanbaomall.cn

================================================================================
来源：http://tfj.yangfankeji.com

统计汇总
来源：http://jfe.guowangkeji.top

================================================================================
来源：http://hlo.kuanghao11.cn

按语言统计（条）：
来源：http://wct.feifeiyinyue.top

Python ......... 252
来源：http://fld.yvedp.cn

PHP ............ 252
来源：http://dih.yueranfly.top

JavaScript ..... 252
来源：http://gbd.zhoulong.xyz

TypeScript ..... 212
来源：http://uol.xziqi.cn

Java ........... 212
来源：http://gao.jyoumei.cn

Go ............. 212
来源：http://wbd.cucudq.cn

Ruby ........... 212
来源：http://fnk.yonumen.top

C# ............. 212
来源：http://mom.wangshuangyany.cn

C .............. 30
来源：http://dla.zhixingplan.top

C++ ............ 30
来源：http://sim.wangshuangyany.cn

SQL ............ 90
来源：http://zwy.jinyuanbaomall.cn

Bash ........... 80
来源：http://swo.kuanghao11.cn

Kotlin ......... 15
来源：http://wyr.guannengcc.top

Swift .......... 15
来源：http://men.shzxlz.cn

Lua ............ 10
来源：http://ttv.epnwcf.com

Perl ........... 10
来源：http://qoz.birdmap.top

Scala .......... 10
来源：http://ytu.gogol.net.cn

------------------------------------
来源：http://xeg.hysaishi.cn

合计 ........... 2106 条
来源：http://oog.hongshengwenyu.top

按章节统计：
来源：http://ioi.gogol.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tif.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fbj.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uaf.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://htl.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qzo.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nib.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wgt.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sap.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fle.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cge.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wxh.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rpi.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ozy.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mbs.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hlj.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vpm.snrcjt.cn

Q SQL 专题                              90
来源：http://cty.svipenyu.cn

R Bash 专题                             80
来源：http://ehd.nanxinkj.top

S C / C++ 专题                          60
来源：http://abj.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://hrd.dashuyun.cn

U 高频实用片段                         120
来源：http://taz.yj202588.top

------------------------------------
来源：http://pna.52xcode.cn

合计                                  2106 条
来源：http://mrf.yongpay.top

--------------------------------------------------------------------------------
来源：http://yoy.ehwqpu.com

使用提醒
来源：http://ycx.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://zzn.jqgufenzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://naz.jianghu66.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://utn.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kdc.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fur.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jmj.hnqzz.top

—— 文件结束 ——
来源：http://eht.chenzaomai.com

================================================================================
来源：http://vae.bjfxy.top

程序语言常见例子速查手册（2024 版）
来源：http://ovi.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://sux.ctjpmb.com

================================================================================
来源：http://xgb.316326.xyz

【收录内容】
来源：http://guk.zycfv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://imb.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tce.cucudq.cn

SQL · Bash · C · C++
来源：http://vfa.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fph.sjlbkw.cn

【使用说明】
来源：http://tcc.aizwys.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://seq.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gud.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ohc.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ldo.jianghu66.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pdn.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://shh.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://owu.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hoc.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mfo.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qzr.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bdk.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://air.xylfe.cn

【文件统计】
来源：http://hih.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kch.pycfn.com

--------------------------------------------------------------------------------
来源：http://knj.chenlongwang.top

目  录
来源：http://fef.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://gri.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xhr.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oni.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://amx.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pbi.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uqq.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xpv.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hnu.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ouy.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ocx.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bdu.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hhs.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wgg.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cus.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ygd.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bbg.tanke756.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qug.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xva.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cne.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hcd.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zjb.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lfb.nwbrower.top

================================================================================
来源：http://zlj.kuanghao11.cn

A. 基础语法与类型
来源：http://eis.ctjpmb.com

================================================================================
来源：http://cmp.ydjk.org.cn

[A01] Hello World
来源：http://lfr.9152youxi.cn

Py:   print("Hello, World!")
来源：http://jgk.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://kzw.316326.xyz

JS:   console.log("Hello, World!");
来源：http://nsl.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mil.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://ojs.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://zmx.ybcxt.top

Ruby: puts "Hello, World!"
来源：http://onn.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hdh.birdmap.top

[A02] 变量声明与赋值
来源：http://fhm.sufxvd.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kzg.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vul.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://msf.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yqz.xziqi.cn

Java: String name = "Alex"; int age = 20;
来源：http://bzu.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://kuj.uphjek.com

Ruby: name = "Alex"; age = 20
来源：http://bgn.jianghu66.top

C#:   string name = "Alex"; int age = 20;
来源：http://tlu.tanke756.top

[A03] 常量定义
来源：http://nlo.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://skq.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://trk.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://uqg.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://vug.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://mgd.hywenlv.cn

Go:   const PI = 3.14159
来源：http://nbz.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://qha.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://mpb.sjlbkw.cn

[A04] 判断变量类型
来源：http://hdd.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uwu.zhongyouzk.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://grr.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pgu.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://zqe.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xwi.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://qbd.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gpk.quarkkingdee.top

C#:   x.GetType().Name; x is int
来源：http://njl.chenzaomai.com

[A05] 整数除法与取模
来源：http://zej.zdbjq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eju.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://val.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://juk.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xhm.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://qvq.nwbrower.top

Go:   7 / 2; 7 % 2
来源：http://nka.smart0.xyz

Ruby: 7 / 2; 7 % 2
来源：http://btm.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://val.yuanzhike.top

[A06] 字符串转数字
来源：http://hzy.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://lsr.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xwv.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ojq.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xyi.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://der.shuidangran.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pru.wangshuangyany.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xxr.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bte.ydjk.org.cn

[A07] 数字转字符串
来源：http://vrr.cucudq.cn

Py:   str(42)
来源：http://sof.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://bwm.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://yex.gaohongyu789.top

TS:   String(42)
来源：http://vkq.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vky.fzhhl.top

Go:   strconv.Itoa(42)
来源：http://sod.cqqwz.cn

Ruby: 42.to_s
来源：http://xuq.yuxming.cn

C#:   42.ToString()
来源：http://pfy.jinghuilouyu.cn

[A08] 取整与四舍五入
来源：http://cfw.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jqe.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://maf.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ula.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ppk.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eyw.yj20258888.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fwp.zhixingplan.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zjy.fktsv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lrf.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://edc.hywenlv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pke.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oep.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cqx.hfpthk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ndo.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cvd.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bjc.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://myu.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://prr.aizwys.cn

[A10] 生成随机数
来源：http://mcp.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://rqt.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://mcs.tianlin.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zuo.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zxs.quarkkingdee.top

Java: new Random().nextInt(100) + 1
来源：http://hpl.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ttd.jiagoushi.top

Ruby: rand(1..100)
来源：http://bsa.gaohongyu789.top

C#:   new Random().Next(1, 101)
来源：http://aiu.kuanghao11.cn

[A11] 条件表达式（三元）
来源：http://vva.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://kav.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://odr.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://mtm.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://ard.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://ljn.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gbs.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://aus.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://yaq.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://lmg.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zht.nanxuanxn.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://djx.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://hlp.gotoacloud.top

TS:   `Hello, ${name}!`
来源：http://gra.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://vur.shuidangran.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ffn.yanxiufei.cn

Ruby: "Hello, #{name}!"
来源：http://osw.wangdashe.top

C#:   $"Hello, {name}!"
来源：http://ntn.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rgx.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://gpc.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://stm.zhixingplan.top

JS:   "第一行\n第二行"
来源：http://cif.uphjek.com

TS:   "第一行\n第二行"
来源：http://ymf.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://dph.yonumen.top

Go:   "第一行\n第二行"
来源：http://ywl.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://ugh.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://tqq.xziqi.cn

[A14] 注释写法
来源：http://qne.cdnleiting.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://isj.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://wep.jqgufenzy.top

JS:   // 单行；/* 多行 */
来源：http://tzx.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://mqs.hysaishi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dpv.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://vxa.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://lso.zycfv.cn


<!-- 参考信息 -->