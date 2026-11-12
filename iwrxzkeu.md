代发 wailian999

[U103] JS：定时器
来源：http://ftk.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aif.sysykeji.top

[U104] JS：防抖
来源：http://ell.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewk.ppjwa.cn

[U105] JS：节流
来源：http://pjt.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fsd.gotoacloud.top

[U106] JS：日期格式化
来源：http://dkm.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hnp.yj20258.top

[U107] JS：数字千分位
来源：http://ecg.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uqt.aibaodan.cn

[U108] JS：随机整数
来源：http://giw.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uie.jinqigfzy.top

[U109] JS：数组分组
来源：http://bdw.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://rol.tian-w.cn

[U110] JS：数组分块
来源：http://nns.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mhu.yangfankeji.com

[U111] JS：对象转 Map
来源：http://kvk.316326.xyz

new Map(Object.entries(obj))
来源：http://ysm.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://edn.quarkkingdee.top

"7".padStart(3, "0")
来源：http://jly.c1oappe.top

[U113] JS：正则替换全部
来源：http://pvs.chenzaomai.com

s.replaceAll("a", "b")
来源：http://bgp.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://lgh.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dxh.hesvh.cn

[U115] JS：生成 UUID
来源：http://hep.xuanzx.com

crypto.randomUUID()
来源：http://lmd.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://ohz.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://mji.shangyingyoupin.top

[U117] JS：单元测试
来源：http://bjh.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://spw.daxiang520.top

[U118] JS：开发服务器
来源：http://jgi.jyoumei.cn

npm i -D vite;  npx vite
来源：http://wcn.xylfe.cn

[U119] JS：生产构建
来源：http://kpp.xziqi.cn

npx vite build
来源：http://qwt.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://xkx.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://gqx.jinyuanbaomall.cn

================================================================================
来源：http://uik.aizwys.cn

统计汇总
来源：http://qvf.xinyue.icu

================================================================================
来源：http://zjk.xuanzx.com

按语言统计（条）：
来源：http://hfx.316326.xyz

Python ......... 252
来源：http://hwg.kuanghao11.cn

PHP ............ 252
来源：http://yso.yangfankeji.com

JavaScript ..... 252
来源：http://rle.epnwcf.com

TypeScript ..... 212
来源：http://rgf.wangshuangyany.cn

Java ........... 212
来源：http://nkn.zhijiandao.cn

Go ............. 212
来源：http://hgg.ivvv.top

Ruby ........... 212
来源：http://tdg.hywenlv.cn

C# ............. 212
来源：http://tmc.nanxuanxn.top

C .............. 30
来源：http://pdl.hammf.cn

C++ ............ 30
来源：http://qau.sysykeji.top

SQL ............ 90
来源：http://efc.havefunace.top

Bash ........... 80
来源：http://tgs.pycfn.com

Kotlin ......... 15
来源：http://eeb.0kj1m.cn

Swift .......... 15
来源：http://cwv.0kj1m.cn

Lua ............ 10
来源：http://iog.yueranfly.top

Perl ........... 10
来源：http://dsf.shanyushiyangtech.top

Scala .......... 10
来源：http://dvh.c1oappe.top

------------------------------------
来源：http://sli.tanke756.top

合计 ........... 2106 条
来源：http://zcp.daria6918.cn

按章节统计：
来源：http://jsm.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gde.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dbf.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fqn.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qhr.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pvk.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jej.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bej.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hvh.yfazqb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kzt.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wwc.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mni.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vkk.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gzq.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kgf.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yzp.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cvo.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://sze.yangfankeji.com

R Bash 专题                             80
来源：http://leo.snrcjt.cn

S C / C++ 专题                          60
来源：http://vjv.uphjek.com

T 其他语言补充                          60
来源：http://vfu.nanxinkj.top

U 高频实用片段                         120
来源：http://yfb.yj20258888.top

------------------------------------
来源：http://xlv.xuanzx.com

合计                                  2106 条
来源：http://jdr.yonumen.top

--------------------------------------------------------------------------------
来源：http://gxx.52xcode.cn

使用提醒
来源：http://nqs.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://qvo.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://slp.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://his.andypj.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mld.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oar.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dsa.wangshuangyany.cn

—— 文件结束 ——
来源：http://vbe.shuidangran.top

================================================================================
来源：http://xja.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://mai.ydzc1.top

Common Programming Examples Cheat Book
来源：http://who.chenlongwang.top

================================================================================
来源：http://obs.hesvh.cn

【收录内容】
来源：http://tdi.kuanghao11.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lke.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gwn.ybcxt.top

SQL · Bash · C · C++
来源：http://pcu.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jan.fehbvm.com

【使用说明】
来源：http://zhm.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hhd.hfpthk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://leo.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bow.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://svu.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://loi.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rzn.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hes.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://srd.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zmi.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lom.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ilg.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lrq.quarkkingdee.top

【文件统计】
来源：http://zdu.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ukg.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://lkc.kuanghao11.cn

目  录
来源：http://uqb.xziqi.cn

--------------------------------------------------------------------------------
来源：http://sws.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rmt.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://njy.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://urv.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xay.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fty.xingfuxueyuan.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cvc.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cqk.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://frj.chenlongwang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mlh.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tft.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mhy.nanxinkj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rxj.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://svr.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jos.pengpengdd.cyou

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qrc.hammf.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pqq.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ntz.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://icn.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qef.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ojz.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bkf.zhongyouzk.top

================================================================================
来源：http://vfe.cucudq.cn

A. 基础语法与类型
来源：http://bti.chenlongwang.top

================================================================================
来源：http://srk.yonumen.top

[A01] Hello World
来源：http://gcs.cqqwz.cn

Py:   print("Hello, World!")
来源：http://ned.tanke756.top

PHP:  echo "Hello, World!";
来源：http://tbg.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://pff.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xiv.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://bzg.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://zwk.andypj.xyz

Ruby: puts "Hello, World!"
来源：http://fwj.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kng.epnwcf.com

[A02] 变量声明与赋值
来源：http://lqz.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yxk.zhijiandao.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bna.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://lpl.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wpl.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://pqt.zhoulong.xyz

Go:   name := "Alex"; age := 20
来源：http://rve.c1oappe.top

Ruby: name = "Alex"; age = 20
来源：http://qaw.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://gqw.nanxuanxn.top

[A03] 常量定义
来源：http://zgf.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vdt.havefunace.top

PHP:  const PI = 3.14159;
来源：http://afl.haohaochexian.top

JS:   const PI = 3.14159;
来源：http://boi.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://jzq.shzxlz.cn

Java: static final double PI = 3.14159;
来源：http://pzw.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://dzz.9152youxi.cn

Ruby: PI = 3.14159
来源：http://xgh.yj202588.top

C#:   const double PI = 3.14159;
来源：http://cdd.shzxlz.cn

[A04] 判断变量类型
来源：http://ypc.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bpf.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zdf.guannengcc.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://evy.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://sfa.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kuv.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://aet.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qlq.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://ewn.xuanzx.com

[A05] 整数除法与取模
来源：http://pag.c1oappe.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://akz.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xki.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uzo.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://toy.yvedp.cn

Java: 7 / 2; 7 % 2
来源：http://dys.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://jfu.guowangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://uob.gzhubu.top

C#:   7 / 2; 7 % 2
来源：http://zaa.ivvv.top

[A06] 字符串转数字
来源：http://thc.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://nch.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lag.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sug.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://wjq.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bme.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aia.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kgs.nwbrower.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nra.nanxinkj.top

[A07] 数字转字符串
来源：http://hly.shuidangran.top

Py:   str(42)
来源：http://ftz.gotoacloud.top

PHP:  (string) 42; strval(42)
来源：http://wve.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://hhn.hysaishi.cn

TS:   String(42)
来源：http://fdr.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fks.wangdashe.top

Go:   strconv.Itoa(42)
来源：http://ixb.sjlbkw.cn

Ruby: 42.to_s
来源：http://hvb.gotoacloud.top

C#:   42.ToString()
来源：http://xgk.svipenyu.cn

[A08] 取整与四舍五入
来源：http://mgc.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://efp.sysykeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dbq.jinghuilouyu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rvr.yfazqb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pvc.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mrj.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rfq.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nhb.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jgm.pycfn.com

[A09] 绝对值与最大最小值
来源：http://xkh.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hde.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ltw.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zlf.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qik.ctjpmb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://snl.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pyj.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wen.yj20258.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blc.andypj.xyz

[A10] 生成随机数
来源：http://glz.jiagoushi.top

Py:   import random; random.randint(1, 100)
来源：http://zgw.mhx1999.top

PHP:  random_int(1, 100);
来源：http://orj.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lcc.shzxlz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ftq.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://fgr.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yto.cashguo.top

Ruby: rand(1..100)
来源：http://nck.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://shk.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://jgp.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://hwn.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vnw.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pdu.guannengcc.top

TS:   x > 0 ? "yes" : "no"
来源：http://oru.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://uow.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fxn.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://uyg.fengsongda.top

C#:   x > 0 ? "yes" : "no"
来源：http://nto.nwbrower.top

[A12] 字符串插值 / 格式化
来源：http://epn.ivvv.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vbl.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wfn.yongpay.top

JS:   `Hello, ${name}!`
来源：http://fsn.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://apj.aizwys.cn

Java: "Hello, %s!".formatted(name)
来源：http://dxf.sweek.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cdz.ywan-chungtsiang.top

Ruby: "Hello, #{name}!"
来源：http://onc.tianlin.xyz

C#:   $"Hello, {name}!"
来源：http://rkn.yvedp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kdo.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://dpj.ppjwa.cn

PHP:  "第一行\n第二行"
来源：http://vrv.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://wzo.gzhubu.top

TS:   "第一行\n第二行"
来源：http://usa.guowangkeji.top

Java: "第一行\n第二行"
来源：http://pqv.xinyue.icu

Go:   "第一行\n第二行"
来源：http://jka.sufxvd.cn

Ruby: "第一行\n第二行"
来源：http://qkc.ywan-chungtsiang.top

C#:   "第一行\n第二行"
来源：http://fwy.yueranfly.top

[A14] 注释写法
来源：http://pnu.gotoacloud.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tey.sxryk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vng.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://wqf.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://uqm.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cqk.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://vmr.tarul.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rkf.zycfv.cn

C#:   // 单行；/* 多行 */
来源：http://uxz.feifeiyinyue.top

[A15] 空值判断与默认值
来源：http://tfd.zdqjudy.top

Py:   value = data or "默认值"
来源：http://wgm.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://rhz.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://etw.epnwcf.com

TS:   const value = data ?? "默认值";
来源：http://yhu.zhaomingkeji.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zcr.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://zmp.sweek.top

Ruby: value = data || "默认值"
来源：http://aos.sufxvd.cn

C#:   var value = data ?? "默认值";
来源：http://xoy.jinyuanbaomall.cn

[A16] 真假值判断规则
来源：http://prx.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fgl.ctjpmb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jwq.yj20258.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rsc.yvedp.cn

TS:   if (!x) {}
来源：http://ywh.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rmh.ywan-chungtsiang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yuv.jlsjyb.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qqy.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://obr.gogol.net.cn

[A17] 位运算
来源：http://jrf.chenlongwang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://loi.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kdr.xuetiantiany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oyb.pycfn.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://icm.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szz.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hnm.pycfn.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afj.shangyingyoupin.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aeq.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://vsy.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://wsp.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://byh.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://alk.mhx1999.top


<!-- 参考信息 -->