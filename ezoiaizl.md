代发 wailian999

[U89] JS：数组去重
来源：http://lja.cqqwz.cn

[...new Set(arr)]
来源：http://wfi.fktsv.cn

[U90] JS：数字数组排序
来源：http://iio.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://xuz.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://obt.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sgj.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://wvm.xziqi.cn

structuredClone(obj)
来源：http://kde.bbcook.cn

[U93] JS：模板字符串
来源：http://wul.ybcxt.top

`共 ${n} 条`
来源：http://ivh.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://dhk.kuanghao11.cn

const double = x => x * 2;
来源：http://ayu.shuidangran.top

[U95] JS：Promise 包装
来源：http://kvc.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://cio.pycfn.com

[U96] JS：async/await 与异常
来源：http://lvc.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yvz.ctjpmb.com

[U97] JS：并发请求
来源：http://zfp.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pjb.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://jpe.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bii.nanxuanxn.top

[U99] JS：事件监听
来源：http://jpk.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://njn.dianchejie.cn

[U100] JS：DOM 查询
来源：http://adl.hnxiangtu.top

document.querySelector(".item")
来源：http://sbu.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://okp.guannengcc.top

el.classList.toggle("active")
来源：http://gzr.ppjwa.cn

[U102] JS：本地存储
来源：http://dut.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ejk.snrcjt.cn

[U103] JS：定时器
来源：http://hzf.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://piq.ydzc1.top

[U104] JS：防抖
来源：http://xtv.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewq.yongpay.top

[U105] JS：节流
来源：http://nkl.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://owb.bbcook.cn

[U106] JS：日期格式化
来源：http://qnb.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rrk.chenzaomai.com

[U107] JS：数字千分位
来源：http://zro.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zzg.ctjpmb.com

[U108] JS：随机整数
来源：http://obi.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://otv.yongpay.top

[U109] JS：数组分组
来源：http://lus.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://tys.ivvv.top

[U110] JS：数组分块
来源：http://jdk.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gqq.hesvh.cn

[U111] JS：对象转 Map
来源：http://qgr.yj20258888.top

new Map(Object.entries(obj))
来源：http://sof.redwolf501.top

[U112] JS：字符串补位
来源：http://ncw.havefunace.top

"7".padStart(3, "0")
来源：http://ipr.tanke756.top

[U113] JS：正则替换全部
来源：http://wov.ctjpmb.com

s.replaceAll("a", "b")
来源：http://sty.hammf.cn

[U114] JS：JSON 深比较
来源：http://khd.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://otd.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://ayc.sufxvd.cn

crypto.randomUUID()
来源：http://nuu.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://hhk.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://ebf.vqdsnc.cn

[U117] JS：单元测试
来源：http://pec.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://mag.dashuyun.cn

[U118] JS：开发服务器
来源：http://uaw.aizwys.cn

npm i -D vite;  npx vite
来源：http://qak.pengpengdd.cyou

[U119] JS：生产构建
来源：http://czp.jiagoushi.top

npx vite build
来源：http://orf.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://mlq.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://cuv.zycfv.cn

================================================================================
来源：http://wzd.hywenlv.cn

统计汇总
来源：http://pwx.xuanzx.com

================================================================================
来源：http://jve.fanxiaobao.xyz

按语言统计（条）：
来源：http://odv.jqgfzy.top

Python ......... 252
来源：http://udc.yj20258888.top

PHP ............ 252
来源：http://xve.cashguo.top

JavaScript ..... 252
来源：http://imp.fzhhl.top

TypeScript ..... 212
来源：http://sqk.cqqwz.cn

Java ........... 212
来源：http://xoh.vqdsnc.cn

Go ............. 212
来源：http://qxl.andypj.xyz

Ruby ........... 212
来源：http://ujt.xylfe.cn

C# ............. 212
来源：http://ayc.cashguo.top

C .............. 30
来源：http://txk.tarul.cn

C++ ............ 30
来源：http://jlm.cucudq.cn

SQL ............ 90
来源：http://nex.ydjk.org.cn

Bash ........... 80
来源：http://psf.daxiang520.top

Kotlin ......... 15
来源：http://yve.cqqwz.cn

Swift .......... 15
来源：http://mor.yvedp.cn

Lua ............ 10
来源：http://slu.mhx1999.top

Perl ........... 10
来源：http://ipd.svipenyu.cn

Scala .......... 10
来源：http://plq.zhijiandao.cn

------------------------------------
来源：http://xtp.kuanghao11.cn

合计 ........... 2106 条
来源：http://ovy.sjlbkw.cn

按章节统计：
来源：http://jsc.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oag.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xwt.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jyu.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sqf.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gzt.cqqwz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zgx.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ehn.sysykeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pvi.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nfh.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ils.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bee.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yqc.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wgq.pycfn.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wpk.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rtl.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bga.jinqigfzy.top

Q SQL 专题                              90
来源：http://bud.epnwcf.com

R Bash 专题                             80
来源：http://ocl.jyoumei.cn

S C / C++ 专题                          60
来源：http://wox.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://mbv.daxiang520.top

U 高频实用片段                         120
来源：http://dxo.sjlbkw.cn

------------------------------------
来源：http://iqq.tianlin.xyz

合计                                  2106 条
来源：http://anu.c1oappe.top

--------------------------------------------------------------------------------
来源：http://ryl.ybcxt.top

使用提醒
来源：http://prl.havefunace.top

--------------------------------------------------------------------------------
来源：http://mhx.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yvq.hysaishi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kem.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ckb.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://csm.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wzu.guannengcc.top

—— 文件结束 ——
来源：http://ovf.quarkkingdee.top

================================================================================
来源：http://wyo.jinqigfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://wvl.xinyue.icu

Common Programming Examples Cheat Book
来源：http://hwl.ydzc1.top

================================================================================
来源：http://kup.zhiwuduotai.top

【收录内容】
来源：http://wfl.guannengcc.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dju.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fae.snrcjt.cn

SQL · Bash · C · C++
来源：http://vbb.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fox.zycfv.cn

【使用说明】
来源：http://wdh.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://max.shanyushiyangtech.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qjv.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pct.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hun.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://upq.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eze.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gim.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qjk.hammf.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tmp.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://muf.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bhb.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dax.zhoulong.xyz

【文件统计】
来源：http://bid.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tar.meibo888.top

--------------------------------------------------------------------------------
来源：http://lrr.hysaishi.cn

目  录
来源：http://sdm.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://fva.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://njq.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xbl.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ywp.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hdb.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iph.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ege.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vew.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ffz.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://chl.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ujf.yuanzhike.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ism.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jfk.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://czs.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cbg.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vup.ctjpmb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tia.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kdf.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xgu.hnqzz.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hhq.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bns.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cde.gzhubu.top

================================================================================
来源：http://bez.snrcjt.cn

A. 基础语法与类型
来源：http://sqw.aizwys.cn

================================================================================
来源：http://plc.mhx1999.top

[A01] Hello World
来源：http://fif.andypj.xyz

Py:   print("Hello, World!")
来源：http://vnf.sweek.top

PHP:  echo "Hello, World!";
来源：http://gtr.sweek.top

JS:   console.log("Hello, World!");
来源：http://ixa.ppjwa.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ftk.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://yum.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://zjh.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://zkd.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ors.hesvh.cn

[A02] 变量声明与赋值
来源：http://xxw.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yhn.cqqwz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rkj.shangyingyoupin.top

JS:   let name = "Alex"; const age = 20;
来源：http://guu.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xxm.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://scy.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://knb.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://fvq.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ruu.tarul.cn

[A03] 常量定义
来源：http://fqe.jianghu66.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qfq.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://rjc.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://mdb.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://ied.birdmap.top

Java: static final double PI = 3.14159;
来源：http://wmg.xinyue.icu

Go:   const PI = 3.14159
来源：http://opq.tian-w.cn

Ruby: PI = 3.14159
来源：http://huu.jyoumei.cn

C#:   const double PI = 3.14159;
来源：http://yvd.meibo888.top

[A04] 判断变量类型
来源：http://ofq.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ucv.guowangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jns.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dfl.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://dry.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eyr.hesvh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qkm.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dqw.jinqigufen.top

C#:   x.GetType().Name; x is int
来源：http://zyb.aibaodan.cn

[A05] 整数除法与取模
来源：http://ony.hnqzz.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fcr.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yrm.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://awe.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://piq.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://llo.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://wax.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://amn.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://mwm.smart0.xyz

[A06] 字符串转数字
来源：http://wmf.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://daz.quarkkingdee.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vws.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eij.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://gye.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kta.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aap.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://cdp.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pxi.gotoacloud.top

[A07] 数字转字符串
来源：http://hhe.gzhubu.top

Py:   str(42)
来源：http://kff.havefunace.top

PHP:  (string) 42; strval(42)
来源：http://wdp.redwolf501.top

JS:   String(42); (42).toString()
来源：http://rlb.ywan-chungtsiang.top

TS:   String(42)
来源：http://yav.nwbrower.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lbi.xziqi.cn

Go:   strconv.Itoa(42)
来源：http://zgk.aizwys.cn

Ruby: 42.to_s
来源：http://lgc.9152youxi.cn

C#:   42.ToString()
来源：http://dxf.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://kgf.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rzo.yuxming.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fny.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dpx.nanxinkj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vzo.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gxl.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ces.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://nzz.tian-w.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jzx.sysykeji.top

[A09] 绝对值与最大最小值
来源：http://bcp.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://etp.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nna.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qht.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bfs.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sju.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qth.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kte.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://brd.hywenlv.cn

[A10] 生成随机数
来源：http://eep.zdqjudy.top

Py:   import random; random.randint(1, 100)
来源：http://qfl.epnwcf.com

PHP:  random_int(1, 100);
来源：http://gid.zhaomingkeji.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mja.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hnr.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://smf.jlsjyb.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://irg.epnwcf.com

Ruby: rand(1..100)
来源：http://jsf.jianghu66.top

C#:   new Random().Next(1, 101)
来源：http://pie.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://vds.nanxinkj.top

Py:   "yes" if x > 0 else "no"
来源：http://ryo.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://vaa.cucudq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://edf.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://olf.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://onb.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hwz.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://ihv.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://pob.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://bje.xuanzx.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uoe.hnxiangtu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ppj.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://lxz.shzxlz.cn

TS:   `Hello, ${name}!`
来源：http://hvt.jinqigufen.top

Java: "Hello, %s!".formatted(name)
来源：http://cfp.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jpa.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://qtf.yfazqb.com

C#:   $"Hello, {name}!"
来源：http://dut.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tyo.havefunace.top

Py:   "第一行\n第二行"
来源：http://xnw.smart0.xyz

PHP:  "第一行\n第二行"
来源：http://yzi.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://gwx.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://mbn.zhongyouzk.top

Java: "第一行\n第二行"
来源：http://maw.yonumen.top

Go:   "第一行\n第二行"
来源：http://isn.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://vba.yj20258.top

C#:   "第一行\n第二行"
来源：http://cuk.jyoumei.cn

[A14] 注释写法
来源：http://vyj.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mkv.yuanzhike.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xri.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://ond.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://yoj.jinqigufen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qxx.sxryk.cn

Go:   // 单行；/* 多行 */
来源：http://crr.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://quy.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://eiu.uphjek.com

[A15] 空值判断与默认值
来源：http://kmb.wangdashe.top

Py:   value = data or "默认值"
来源：http://cxv.kuanghao11.cn

PHP:  $value = $data ?? "默认值";
来源：http://vwp.yongpay.top


<!-- 参考信息 -->