代发 wailian999

[U97] JS：并发请求
来源：http://rsk.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sit.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://wig.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mmd.0kj1m.cn

[U99] JS：事件监听
来源：http://fah.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://yth.wangdashe.top

[U100] JS：DOM 查询
来源：http://bhh.jlsjyb.cn

document.querySelector(".item")
来源：http://iex.zycfv.cn

[U101] JS：classList 操作
来源：http://ilp.hywenlv.cn

el.classList.toggle("active")
来源：http://cat.chenzaomai.com

[U102] JS：本地存储
来源：http://bqp.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lyc.ppjwa.cn

[U103] JS：定时器
来源：http://nka.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ypp.nanxuanxn.top

[U104] JS：防抖
来源：http://zdr.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crd.sweek.top

[U105] JS：节流
来源：http://xex.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qdy.nwbrower.top

[U106] JS：日期格式化
来源：http://uhc.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hoy.kuanghao11.cn

[U107] JS：数字千分位
来源：http://udi.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kfl.zhongyouzk.top

[U108] JS：随机整数
来源：http://aqx.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rjl.zhijiandao.cn

[U109] JS：数组分组
来源：http://qva.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://eyz.nwbrower.top

[U110] JS：数组分块
来源：http://eec.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bli.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://aph.9152youxi.cn

new Map(Object.entries(obj))
来源：http://xee.cashguo.top

[U112] JS：字符串补位
来源：http://rlf.guannengcc.top

"7".padStart(3, "0")
来源：http://iku.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://gun.snrcjt.cn

s.replaceAll("a", "b")
来源：http://kui.fehbvm.com

[U114] JS：JSON 深比较
来源：http://dfw.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oba.nanxinkj.top

[U115] JS：生成 UUID
来源：http://khk.wangdashe.top

crypto.randomUUID()
来源：http://qux.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://vpe.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://lfh.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://rws.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://pil.0kj1m.cn

[U118] JS：开发服务器
来源：http://iha.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://nmj.zhixingplan.top

[U119] JS：生产构建
来源：http://ygv.jqgfzy.top

npx vite build
来源：http://xgi.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://egc.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://bql.zhaomingkeji.xyz

================================================================================
来源：http://psn.nwbrower.top

统计汇总
来源：http://kad.tarul.cn

================================================================================
来源：http://slj.xuetiantiany.cn

按语言统计（条）：
来源：http://esy.cucudq.cn

Python ......... 252
来源：http://sle.yonumen.top

PHP ............ 252
来源：http://wyv.fengsongda.top

JavaScript ..... 252
来源：http://nel.hammf.cn

TypeScript ..... 212
来源：http://wuv.redwolf501.top

Java ........... 212
来源：http://tfn.shanyushiyangkeji.top

Go ............. 212
来源：http://iwt.chenzaomai.com

Ruby ........... 212
来源：http://pdi.zhaomingkeji.xyz

C# ............. 212
来源：http://vtn.hywenlv.cn

C .............. 30
来源：http://uya.zycfv.cn

C++ ............ 30
来源：http://yuy.chenzaomai.com

SQL ............ 90
来源：http://orr.smart0.xyz

Bash ........... 80
来源：http://dzf.ybcxt.top

Kotlin ......... 15
来源：http://pca.chenzaomai.com

Swift .......... 15
来源：http://wex.tanke756.top

Lua ............ 10
来源：http://toc.nwbrower.top

Perl ........... 10
来源：http://jvm.cashguo.top

Scala .......... 10
来源：http://ytk.jianghu66.top

------------------------------------
来源：http://rfm.hnqzz.top

合计 ........... 2106 条
来源：http://mdn.zdbjq.cn

按章节统计：
来源：http://fwo.kuanghao11.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hti.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rwk.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gkj.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mbt.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ili.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wdp.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wyh.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kja.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ifz.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ged.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://krj.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ktq.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mjx.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dri.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xzg.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ftc.fktsv.cn

Q SQL 专题                              90
来源：http://cgm.ehwqpu.com

R Bash 专题                             80
来源：http://rah.epnwcf.com

S C / C++ 专题                          60
来源：http://jnb.fzhhl.top

T 其他语言补充                          60
来源：http://wtc.gotoacloud.top

U 高频实用片段                         120
来源：http://kxx.ybcxt.top

------------------------------------
来源：http://aod.yj20258.top

合计                                  2106 条
来源：http://gir.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://azj.shanyushiyangkeji.top

使用提醒
来源：http://yrd.316326.xyz

--------------------------------------------------------------------------------
来源：http://kwt.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aps.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rfn.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xsf.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gtj.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hxt.yuxming.cn

—— 文件结束 ——
来源：http://baj.zycfv.cn

================================================================================
来源：http://lvh.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://lwn.yongpay.top

Common Programming Examples Cheat Book
来源：http://qyv.cheryme.top

================================================================================
来源：http://qgo.dianchejie.cn

【收录内容】
来源：http://szw.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://eiw.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dup.chenlongwang.top

SQL · Bash · C · C++
来源：http://erw.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wpu.sxryk.cn

【使用说明】
来源：http://ipz.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wxa.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cju.yvedp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dzf.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iii.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wht.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pxe.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gwr.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ttz.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://syi.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pot.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rfg.redwolf501.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wzx.hammf.cn

【文件统计】
来源：http://jny.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kay.daria6918.cn

--------------------------------------------------------------------------------
来源：http://fds.jyoumei.cn

目  录
来源：http://gbx.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://qie.pycfn.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fky.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://afp.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hol.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jxh.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rsu.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qqn.chenzaomai.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kqp.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://skw.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gjl.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kvh.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gib.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hrg.smart0.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vmg.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lih.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qsq.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qlr.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pcu.iojbl.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hil.shanyushiyangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vad.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://krx.zhengqikj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wut.cucudq.cn

================================================================================
来源：http://ahy.wangshuangyany.cn

A. 基础语法与类型
来源：http://gwq.cqqwz.cn

================================================================================
来源：http://ajl.gaohongyu789.top

[A01] Hello World
来源：http://wjo.hysaishi.cn

Py:   print("Hello, World!")
来源：http://stk.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://nkm.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://ygi.birdmap.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cia.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://bnr.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://tzg.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://lxj.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://omn.gaohongyu789.top

[A02] 变量声明与赋值
来源：http://kpd.9152youxi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xks.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://zde.fehbvm.com

JS:   let name = "Alex"; const age = 20;
来源：http://bwv.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lff.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://eie.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://jct.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://pqu.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://teb.ybcxt.top

[A03] 常量定义
来源：http://btw.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ivj.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://rpa.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://upw.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://ajl.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://wxr.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://gph.zhixingplan.top

Ruby: PI = 3.14159
来源：http://pab.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://uxe.zhoulong.xyz

[A04] 判断变量类型
来源：http://zkh.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cct.xuetiantiany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://grw.zdqjudy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://beu.tarul.cn

TS:   typeof x; x instanceof Date
来源：http://egl.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ddr.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://zxv.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bfl.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://uod.yj20258.top

[A05] 整数除法与取模
来源：http://uoc.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cis.hammf.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kob.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sae.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ghz.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://jrh.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://joh.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://yjf.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://lcc.feifeiyinyue.top

[A06] 字符串转数字
来源：http://mtx.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://kmz.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zmu.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rwe.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uup.hfpthk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bsk.zhiwuduotai.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ujm.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rqs.xuanzx.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zyl.zhaomingkeji.xyz

[A07] 数字转字符串
来源：http://qxi.52xcode.cn

Py:   str(42)
来源：http://res.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://zwp.fehbvm.com

JS:   String(42); (42).toString()
来源：http://zfm.iojbl.cn

TS:   String(42)
来源：http://rda.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ong.yuxming.cn

Go:   strconv.Itoa(42)
来源：http://npl.tian-w.cn

Ruby: 42.to_s
来源：http://vry.zhijiandao.cn

C#:   42.ToString()
来源：http://rdf.xingfuxueyuan.xyz

[A08] 取整与四舍五入
来源：http://omo.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ltu.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jpg.chenlongwang.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ncu.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rpk.haohaochexian.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qwe.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jok.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wte.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fgf.cheryme.top

[A09] 绝对值与最大最小值
来源：http://blc.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nrp.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rxq.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qlg.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wyv.cucudq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eor.fzhhl.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dvs.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qgu.tarul.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rxq.jinghuilouyu.cn

[A10] 生成随机数
来源：http://dkz.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://iit.fanxiaobao.xyz

PHP:  random_int(1, 100);
来源：http://lza.tarul.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fxj.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yev.yvedp.cn

Java: new Random().nextInt(100) + 1
来源：http://uim.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rvp.cucudq.cn

Ruby: rand(1..100)
来源：http://lut.chenlongwang.top

C#:   new Random().Next(1, 101)
来源：http://duo.bbcook.cn

[A11] 条件表达式（三元）
来源：http://pqp.daxiang520.top

Py:   "yes" if x > 0 else "no"
来源：http://lsx.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cjn.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://rbg.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://qty.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://xux.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xya.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://thf.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://dep.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://skg.vehdjk.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dqe.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nzv.zhengqikj.top

JS:   `Hello, ${name}!`
来源：http://twh.pycfn.com

TS:   `Hello, ${name}!`
来源：http://btk.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://edt.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blg.hongshengwenyu.top

Ruby: "Hello, #{name}!"
来源：http://eeg.cdnleiting.top

C#:   $"Hello, {name}!"
来源：http://tpa.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tir.9152youxi.cn

Py:   "第一行\n第二行"
来源：http://fmz.uphjek.com

PHP:  "第一行\n第二行"
来源：http://nsa.chenlongwang.top

JS:   "第一行\n第二行"
来源：http://axd.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://vse.daria6918.cn

Java: "第一行\n第二行"
来源：http://cey.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://bla.uphjek.com

Ruby: "第一行\n第二行"
来源：http://xic.yongpay.top

C#:   "第一行\n第二行"
来源：http://mse.quarkkingdee.top

[A14] 注释写法
来源：http://vtt.sufxvd.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vki.havefunace.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qxy.ybcxt.top

JS:   // 单行；/* 多行 */
来源：http://edk.ehwqpu.com

TS:   // 单行；/* 多行 */
来源：http://hkw.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nxy.52xcode.cn

Go:   // 单行；/* 多行 */
来源：http://gtw.xuanzx.com

Ruby: # 单行；=begin 多行 =end
来源：http://gqp.birdmap.top

C#:   // 单行；/* 多行 */
来源：http://lih.shuidangran.top

[A15] 空值判断与默认值
来源：http://ugl.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://qnt.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://vsw.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://uik.hcnkem.com

TS:   const value = data ?? "默认值";
来源：http://epb.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://smp.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://khz.hnqzz.top

Ruby: value = data || "默认值"
来源：http://uca.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://paq.smart0.xyz

[A16] 真假值判断规则
来源：http://szj.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xoe.tianlin.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hfi.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kka.jinqigfzy.top

TS:   if (!x) {}
来源：http://ycx.havefunace.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://znf.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lbk.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://sqd.yj20258.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://inn.kuanghao11.cn

[A17] 位运算
来源：http://tzf.yj202588.top


<!-- 参考信息 -->