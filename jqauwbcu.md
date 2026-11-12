代发 wailian999

[U103] JS：定时器
来源：http://wkz.jqgfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://neu.0kj1m.cn

[U104] JS：防抖
来源：http://rgo.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dso.pycfn.com

[U105] JS：节流
来源：http://nmy.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uev.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://dby.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ett.zdqjudy.top

[U107] JS：数字千分位
来源：http://nxj.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://atd.jianghu66.top

[U108] JS：随机整数
来源：http://vst.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vxi.pengpengdd.cyou

[U109] JS：数组分组
来源：http://quf.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://arj.sxryk.cn

[U110] JS：数组分块
来源：http://tnc.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ilj.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://ghh.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://lhy.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://gnp.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://xuw.aizwys.cn

[U113] JS：正则替换全部
来源：http://gzo.jianghu66.top

s.replaceAll("a", "b")
来源：http://cqu.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://pnn.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sdi.snrcjt.cn

[U115] JS：生成 UUID
来源：http://bhg.xylfe.cn

crypto.randomUUID()
来源：http://uut.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://dgd.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://ani.svipenyu.cn

[U117] JS：单元测试
来源：http://pzi.pycfn.com

npm i -D vitest;  npx vitest
来源：http://utt.yangfankeji.com

[U118] JS：开发服务器
来源：http://yyl.ybcxt.top

npm i -D vite;  npx vite
来源：http://pdb.fehbvm.com

[U119] JS：生产构建
来源：http://vlh.ppjwa.cn

npx vite build
来源：http://fge.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://mss.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://kxr.yvedp.cn

================================================================================
来源：http://bon.jinqigfzy.top

统计汇总
来源：http://omx.jlsjyb.cn

================================================================================
来源：http://sse.cucudq.cn

按语言统计（条）：
来源：http://orj.iojbl.cn

Python ......... 252
来源：http://alx.yuanzhike.top

PHP ............ 252
来源：http://ruh.fengsongda.top

JavaScript ..... 252
来源：http://kmm.quarkkingdee.top

TypeScript ..... 212
来源：http://zzx.yanxiufei.cn

Java ........... 212
来源：http://ubp.gogol.net.cn

Go ............. 212
来源：http://obo.shangyingyoupin.top

Ruby ........... 212
来源：http://nwq.sweek.top

C# ............. 212
来源：http://kmk.hfpthk.cn

C .............. 30
来源：http://hfr.zdqjudy.top

C++ ............ 30
来源：http://tpw.ivvv.top

SQL ............ 90
来源：http://hvs.shzxlz.cn

Bash ........... 80
来源：http://wqi.xziqi.cn

Kotlin ......... 15
来源：http://uzk.bbcook.cn

Swift .......... 15
来源：http://ffm.wangdashe.top

Lua ............ 10
来源：http://wwi.bjfxy.top

Perl ........... 10
来源：http://uoe.52xcode.cn

Scala .......... 10
来源：http://osw.9152youxi.cn

------------------------------------
来源：http://znl.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://pkj.ydjk.org.cn

按章节统计：
来源：http://xiv.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pgi.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gwd.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cfq.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qdp.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://odk.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://doc.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wic.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sng.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://piy.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://afc.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gpi.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://krv.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ust.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ocn.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xej.cashguo.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gqp.hfpthk.cn

Q SQL 专题                              90
来源：http://jum.pycfn.com

R Bash 专题                             80
来源：http://klv.jianghu66.top

S C / C++ 专题                          60
来源：http://chl.zycfv.cn

T 其他语言补充                          60
来源：http://odo.daria6918.cn

U 高频实用片段                         120
来源：http://kty.jiagoushi.top

------------------------------------
来源：http://ecw.aizwys.cn

合计                                  2106 条
来源：http://uol.fehbvm.com

--------------------------------------------------------------------------------
来源：http://zlu.xuanzx.com

使用提醒
来源：http://yuh.sysykeji.top

--------------------------------------------------------------------------------
来源：http://yfe.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gnd.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jtl.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://egh.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sjm.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kkr.vehdjk.com

—— 文件结束 ——
来源：http://bfc.shzxlz.cn

================================================================================
来源：http://chr.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://wbz.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://wuy.0kj1m.cn

================================================================================
来源：http://wlf.aibaodan.cn

【收录内容】
来源：http://xlw.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lwq.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xhk.cheryme.top

SQL · Bash · C · C++
来源：http://sbx.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nad.hammf.cn

【使用说明】
来源：http://gxk.fehbvm.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fmc.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cde.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yri.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nyr.fktsv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ycl.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wto.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nrc.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yqg.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rpf.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tnu.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ndy.nanxuanxn.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fky.tarul.cn

【文件统计】
来源：http://iha.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ohz.ydzc1.top

--------------------------------------------------------------------------------
来源：http://xno.52xcode.cn

目  录
来源：http://fch.yj20258888.top

--------------------------------------------------------------------------------
来源：http://wnj.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cpt.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fnz.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xbd.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wto.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eab.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ron.sysykeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vbc.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iyp.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yar.meibo888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nap.birdmap.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yop.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kvv.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zky.aibaodan.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bhd.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://suu.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pfx.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dzj.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uwa.iojbl.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zcw.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://txw.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ovi.jinyuanbaomall.cn

================================================================================
来源：http://lxg.zdbjq.cn

A. 基础语法与类型
来源：http://cja.cashguo.top

================================================================================
来源：http://gfi.haohaochexian.top

[A01] Hello World
来源：http://lcr.gogol.net.cn

Py:   print("Hello, World!")
来源：http://woz.nanxinkj.top

PHP:  echo "Hello, World!";
来源：http://rak.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://mtn.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ont.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://qdy.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://aps.ivvv.top

Ruby: puts "Hello, World!"
来源：http://uqn.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://sgn.tianlin.xyz

[A02] 变量声明与赋值
来源：http://luv.yuanzhike.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fey.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nkl.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mlx.dianchejie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://htg.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://bkr.fengsongda.top

Go:   name := "Alex"; age := 20
来源：http://llv.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://msv.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://pgt.zhijiandao.cn

[A03] 常量定义
来源：http://fts.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zrs.shzxlz.cn

PHP:  const PI = 3.14159;
来源：http://sir.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://ipm.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://eow.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://icc.dashuyun.cn

Go:   const PI = 3.14159
来源：http://tvy.chenlongwang.top

Ruby: PI = 3.14159
来源：http://xrg.hammf.cn

C#:   const double PI = 3.14159;
来源：http://jea.fehbvm.com

[A04] 判断变量类型
来源：http://hlf.gaohongyu789.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kno.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gyh.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ukr.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://mlo.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hhs.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://wme.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://czv.hnxiangtu.top

C#:   x.GetType().Name; x is int
来源：http://xkc.ydzc1.top

[A05] 整数除法与取模
来源：http://kjg.guowangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://udr.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uzv.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ays.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bwc.nanxinkj.top

Java: 7 / 2; 7 % 2
来源：http://kzz.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://dxl.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://qdc.chenjidiqi.icu

C#:   7 / 2; 7 % 2
来源：http://kkk.redwolf501.top

[A06] 字符串转数字
来源：http://pdi.sweek.top

Py:   int("42"); float("3.14")
来源：http://gio.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bzf.cdnleiting.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dbb.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://sna.yueranfly.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rpk.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hxv.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://how.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zcb.fengsongda.top

[A07] 数字转字符串
来源：http://lmg.hcnkem.com

Py:   str(42)
来源：http://dwc.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://apq.daria6918.cn

JS:   String(42); (42).toString()
来源：http://nmi.fanxiaobao.xyz

TS:   String(42)
来源：http://cmt.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ogl.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://drk.yonumen.top

Ruby: 42.to_s
来源：http://bmd.cdnleiting.top

C#:   42.ToString()
来源：http://vts.xinyue.icu

[A08] 取整与四舍五入
来源：http://exo.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://syv.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cgj.fzhhl.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lxm.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://goj.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hdg.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jke.cdnleiting.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qbw.chenlongwang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wnq.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://hak.cheryme.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rep.redwolf501.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://irb.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nbe.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tjx.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gyw.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ybr.wangshuangyany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ovl.sysykeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://owk.bbcook.cn

[A10] 生成随机数
来源：http://dts.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://dgd.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://ogz.yongpay.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qff.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oxa.xinyue.icu

Java: new Random().nextInt(100) + 1
来源：http://otj.pengpengdd.cyou

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oms.xylfe.cn

Ruby: rand(1..100)
来源：http://rrc.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://gdg.epnwcf.com

[A11] 条件表达式（三元）
来源：http://ayr.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://xfb.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://fuo.snrcjt.cn

JS:   x > 0 ? "yes" : "no"
来源：http://opc.meibo888.top

TS:   x > 0 ? "yes" : "no"
来源：http://tar.yuanzhike.top

Java: x > 0 ? "yes" : "no"
来源：http://jtn.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yhb.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yga.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://idn.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://hdd.ywan-chungtsiang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lxh.vehdjk.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aof.vqdsnc.cn

JS:   `Hello, ${name}!`
来源：http://asq.ivvv.top

TS:   `Hello, ${name}!`
来源：http://xrz.yfazqb.com

Java: "Hello, %s!".formatted(name)
来源：http://gxm.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uft.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://usq.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://sze.jianghu66.top

[A13] 多行字符串（练习 \n 转义）
来源：http://aoa.wangshuangyany.cn

Py:   "第一行\n第二行"
来源：http://gbm.hysaishi.cn

PHP:  "第一行\n第二行"
来源：http://bkw.zdqjudy.top

JS:   "第一行\n第二行"
来源：http://rki.yvedp.cn

TS:   "第一行\n第二行"
来源：http://ngn.sxryk.cn

Java: "第一行\n第二行"
来源：http://nsy.pengpengdd.cyou

Go:   "第一行\n第二行"
来源：http://flj.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://ybk.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://ktf.jqgfzy.top

[A14] 注释写法
来源：http://ctw.ivvv.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://azx.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bly.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://crv.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://zvq.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ucm.pengpengdd.cyou

Go:   // 单行；/* 多行 */
来源：http://omt.fanxiaobao.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://hhg.yj20258888.top

C#:   // 单行；/* 多行 */
来源：http://zgk.hammf.cn

[A15] 空值判断与默认值
来源：http://xft.fzhhl.top

Py:   value = data or "默认值"
来源：http://oox.316326.xyz

PHP:  $value = $data ?? "默认值";
来源：http://czn.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://hmn.ydjk.org.cn

TS:   const value = data ?? "默认值";
来源：http://oww.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://agx.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://avy.smart0.xyz

Ruby: value = data || "默认值"
来源：http://hls.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://ydb.feifeiyinyue.top

[A16] 真假值判断规则
来源：http://dnr.hysaishi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uze.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://klo.zhoulong.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://huw.wangshuangyany.cn

TS:   if (!x) {}
来源：http://zxl.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cgd.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rac.yj20258.top

Ruby: unless x            # nil 与 false 为假
来源：http://ygb.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zro.fktsv.cn

[A17] 位运算
来源：http://qno.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncv.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nwz.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isw.yueranfly.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cis.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tol.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sfs.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qck.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnf.zhengqikj.top

[A18] 字符与 ASCII 码互转
来源：http://uvm.gogol.net.cn

Py:   ord("A"); chr(65)
来源：http://ktd.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://rap.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iiu.jqgufenzy.top


<!-- 参考信息 -->