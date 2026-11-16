代发 wailian999

[U103] JS：定时器
来源：http://qgt.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tyb.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://saf.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fci.9152youxi.cn

[U105] JS：节流
来源：http://qpq.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tsk.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://rfp.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gfu.xuanzx.com

[U107] JS：数字千分位
来源：http://qkw.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vlf.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://vjj.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vmf.nanxuanxn.top

[U109] JS：数组分组
来源：http://mqs.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://uas.nanxinkj.top

[U110] JS：数组分块
来源：http://zsd.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://slj.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://kfo.gogol.net.cn

new Map(Object.entries(obj))
来源：http://vrk.nanxuanxn.top

[U112] JS：字符串补位
来源：http://nqc.pycfn.com

"7".padStart(3, "0")
来源：http://wup.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://zza.nwbrower.top

s.replaceAll("a", "b")
来源：http://ete.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://gvr.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dxq.fzhhl.top

[U115] JS：生成 UUID
来源：http://nwe.ivvv.top

crypto.randomUUID()
来源：http://sad.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://meg.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://lup.hesvh.cn

[U117] JS：单元测试
来源：http://pni.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://qjs.ctjpmb.com

[U118] JS：开发服务器
来源：http://lir.ydzc1.top

npm i -D vite;  npx vite
来源：http://auw.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://chu.zycfv.cn

npx vite build
来源：http://kyl.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://soo.hnqzz.top

import.meta.env.VITE_API_URL
来源：http://hiu.yongpay.top

================================================================================
来源：http://hte.yfazqb.com

统计汇总
来源：http://oqu.tianlin.xyz

================================================================================
来源：http://bdq.jinghuilouyu.cn

按语言统计（条）：
来源：http://lal.yj20258888.top

Python ......... 252
来源：http://rqb.zhengqikj.top

PHP ............ 252
来源：http://mdz.gogol.net.cn

JavaScript ..... 252
来源：http://rxl.jqgfzy.top

TypeScript ..... 212
来源：http://rwg.birdmap.top

Java ........... 212
来源：http://kbf.zhaomingkeji.xyz

Go ............. 212
来源：http://yzc.yonumen.top

Ruby ........... 212
来源：http://hbf.andypj.xyz

C# ............. 212
来源：http://pix.hnqzz.top

C .............. 30
来源：http://mzl.ydjk.org.cn

C++ ............ 30
来源：http://zgv.dashuyun.cn

SQL ............ 90
来源：http://rvb.ctjpmb.com

Bash ........... 80
来源：http://bxi.vehdjk.com

Kotlin ......... 15
来源：http://jbb.52xcode.cn

Swift .......... 15
来源：http://rdc.gaohongyu789.top

Lua ............ 10
来源：http://bib.aibaodan.cn

Perl ........... 10
来源：http://yxw.hesvh.cn

Scala .......... 10
来源：http://wly.tianlin.xyz

------------------------------------
来源：http://ick.quarkkingdee.top

合计 ........... 2106 条
来源：http://oor.aizwys.cn

按章节统计：
来源：http://cnn.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qxo.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yzf.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nde.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mkp.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://din.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uhg.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://phc.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kme.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://omn.sxryk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nys.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tou.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oso.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://app.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ytr.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iks.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://owo.gzhubu.top

Q SQL 专题                              90
来源：http://ilc.hnxiangtu.top

R Bash 专题                             80
来源：http://jps.ybcxt.top

S C / C++ 专题                          60
来源：http://rjf.c1oappe.top

T 其他语言补充                          60
来源：http://ziq.meibo888.top

U 高频实用片段                         120
来源：http://cvy.vqdsnc.cn

------------------------------------
来源：http://rtv.fanxiaobao.xyz

合计                                  2106 条
来源：http://bbw.yvedp.cn

--------------------------------------------------------------------------------
来源：http://lpa.iojbl.cn

使用提醒
来源：http://nra.yj202588.top

--------------------------------------------------------------------------------
来源：http://ciq.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xjf.zdbjq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://guj.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hqt.yuxming.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dly.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tey.zdbjq.cn

—— 文件结束 ——
来源：http://whu.sysykeji.top

================================================================================
来源：http://hzj.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://mth.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://juh.9152youxi.cn

================================================================================
来源：http://xom.ehwqpu.com

【收录内容】
来源：http://lwn.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sao.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pox.smart0.xyz

SQL · Bash · C · C++
来源：http://efy.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sev.dianchejie.cn

【使用说明】
来源：http://bcb.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pkr.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pml.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eir.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tyo.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://hdl.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gdj.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kaf.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jrh.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pgd.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nby.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eyd.fanxiaobao.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wvh.nwbrower.top

【文件统计】
来源：http://bzd.tian-w.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uvh.epnwcf.com

--------------------------------------------------------------------------------
来源：http://cye.52xcode.cn

目  录
来源：http://kuy.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://lrn.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cwy.ywan-chungtsiang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://att.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://now.tianlin.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mgj.haohaochexian.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vhx.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fit.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eyg.hammf.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tlw.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mfr.fengsongda.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://huu.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://raq.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rbi.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nbm.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tsm.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jny.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://etr.cheryme.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://odg.zhixingplan.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://oqb.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://svy.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bkg.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://djm.316326.xyz

================================================================================
来源：http://rgf.c1oappe.top

A. 基础语法与类型
来源：http://yig.ppjwa.cn

================================================================================
来源：http://lzs.52xcode.cn

[A01] Hello World
来源：http://cvb.yj20258888.top

Py:   print("Hello, World!")
来源：http://exd.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://fvo.chenjidiqi.icu

JS:   console.log("Hello, World!");
来源：http://fol.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uca.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://doj.jinghuilouyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://tnj.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://pgg.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://prw.yj202588.top

[A02] 变量声明与赋值
来源：http://ufn.yonumen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://syb.ybcxt.top

PHP:  $name = "Alex"; $age = 20;
来源：http://swg.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://ine.zhixingplan.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dyq.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://zef.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://efl.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://znb.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kwn.epnwcf.com

[A03] 常量定义
来源：http://nta.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kyt.ywan-chungtsiang.top

PHP:  const PI = 3.14159;
来源：http://qel.cucudq.cn

JS:   const PI = 3.14159;
来源：http://rbt.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://njm.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://ntz.hesvh.cn

Go:   const PI = 3.14159
来源：http://tki.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://oaz.wangdashe.top

C#:   const double PI = 3.14159;
来源：http://msr.fengsongda.top

[A04] 判断变量类型
来源：http://yje.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://nue.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oqk.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://thf.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://hhx.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gws.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://iur.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ycz.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://xug.guowangkeji.top

[A05] 整数除法与取模
来源：http://dju.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tno.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://fgm.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zug.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jcq.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://eml.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://puw.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://gje.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://lmi.dianchejie.cn

[A06] 字符串转数字
来源：http://rjm.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://wks.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ani.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rrl.svipenyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xys.ctjpmb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dve.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yma.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ohh.ybcxt.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cme.bbcook.cn

[A07] 数字转字符串
来源：http://kvc.yuxming.cn

Py:   str(42)
来源：http://tpl.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://nbm.yj202588.top

JS:   String(42); (42).toString()
来源：http://xtp.pycfn.com

TS:   String(42)
来源：http://sad.birdmap.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lfs.zhengqikj.top

Go:   strconv.Itoa(42)
来源：http://cjw.zhixingplan.top

Ruby: 42.to_s
来源：http://ubq.jqgufenzy.top

C#:   42.ToString()
来源：http://cwa.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://upf.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dim.zhoulong.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vmj.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kuz.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rru.pycfn.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ezq.haohaochexian.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ybl.yuanzhike.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bmc.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dqn.yfazqb.com

[A09] 绝对值与最大最小值
来源：http://uwi.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zxt.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://url.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://esd.jianghu66.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aaj.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cig.jlsjyb.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rqc.fanxiaobao.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gkl.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://auf.yangfankeji.com

[A10] 生成随机数
来源：http://atj.yongpay.top

Py:   import random; random.randint(1, 100)
来源：http://lfj.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://qjo.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jna.yuanzhike.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nuo.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://qrj.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://udb.jianghu66.top

Ruby: rand(1..100)
来源：http://jwm.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://iax.ydzc1.top

[A11] 条件表达式（三元）
来源：http://mvi.cucudq.cn

Py:   "yes" if x > 0 else "no"
来源：http://tqi.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://elw.xinyue.icu

JS:   x > 0 ? "yes" : "no"
来源：http://ohd.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://slk.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://kef.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://mof.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jsh.shzxlz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mzg.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://tap.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kom.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gsf.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://lzz.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://vot.jiagoushi.top

Java: "Hello, %s!".formatted(name)
来源：http://sqz.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hng.nanxuanxn.top

Ruby: "Hello, #{name}!"
来源：http://qfm.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://bwj.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mhf.havefunace.top

Py:   "第一行\n第二行"
来源：http://inm.chenzaomai.com

PHP:  "第一行\n第二行"
来源：http://mmi.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://xlj.yj202588.top

TS:   "第一行\n第二行"
来源：http://cpq.52xcode.cn

Java: "第一行\n第二行"
来源：http://qyi.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://dgf.hammf.cn

Ruby: "第一行\n第二行"
来源：http://jts.ydjk.org.cn

C#:   "第一行\n第二行"
来源：http://wqj.tianlin.xyz

[A14] 注释写法
来源：http://rmc.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cbc.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://qdm.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://wpr.jinghuilouyu.cn

TS:   // 单行；/* 多行 */
来源：http://gaw.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fnb.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://yeu.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://xjj.zhijiandao.cn

C#:   // 单行；/* 多行 */
来源：http://pbd.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://trd.chenzaomai.com

Py:   value = data or "默认值"
来源：http://cbz.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://wmw.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://rfz.cashguo.top

TS:   const value = data ?? "默认值";
来源：http://znr.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hhk.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://oio.yueranfly.top

Ruby: value = data || "默认值"
来源：http://jii.hnqzz.top

C#:   var value = data ?? "默认值";
来源：http://mqn.mhx1999.top

[A16] 真假值判断规则
来源：http://xbj.hfpthk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dfi.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cjp.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kli.yueranfly.top

TS:   if (!x) {}
来源：http://vuq.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fcn.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wpb.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gwp.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rli.yueranfly.top

[A17] 位运算
来源：http://agk.yuxming.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sru.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bgp.yj202588.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nls.cqqwz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qob.yuanzhike.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cci.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pnp.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnn.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eza.yj202588.top

[A18] 字符与 ASCII 码互转
来源：http://rtz.gogol.net.cn

Py:   ord("A"); chr(65)
来源：http://uig.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://dti.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mum.jinqigufen.top


<!-- 参考信息 -->