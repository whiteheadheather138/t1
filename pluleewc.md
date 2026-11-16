代发 wailian999

[U105] JS：节流
来源：http://bwb.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://srw.pycfn.com

[U106] JS：日期格式化
来源：http://yta.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cyf.iojbl.cn

[U107] JS：数字千分位
来源：http://css.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ejh.cdnleiting.top

[U108] JS：随机整数
来源：http://weq.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blp.ehwqpu.com

[U109] JS：数组分组
来源：http://zgb.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://fsb.ivvv.top

[U110] JS：数组分块
来源：http://pms.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mhu.yuanzhike.top

[U111] JS：对象转 Map
来源：http://swf.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://whl.redwolf501.top

[U112] JS：字符串补位
来源：http://orr.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://mpa.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://sxd.cucudq.cn

s.replaceAll("a", "b")
来源：http://hht.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://ups.xylfe.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wrr.yonumen.top

[U115] JS：生成 UUID
来源：http://qgk.zhengqikj.top

crypto.randomUUID()
来源：http://wwx.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://grd.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://qch.tian-w.cn

[U117] JS：单元测试
来源：http://cvo.sweek.top

npm i -D vitest;  npx vitest
来源：http://qzm.bjfxy.top

[U118] JS：开发服务器
来源：http://ela.ehwqpu.com

npm i -D vite;  npx vite
来源：http://rus.9152youxi.cn

[U119] JS：生产构建
来源：http://iey.dianchejie.cn

npx vite build
来源：http://gee.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://vow.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://zpd.wangdashe.top

================================================================================
来源：http://lto.hammf.cn

统计汇总
来源：http://syj.xziqi.cn

================================================================================
来源：http://icj.hesvh.cn

按语言统计（条）：
来源：http://hvm.yj20258.top

Python ......... 252
来源：http://zpv.aizwys.cn

PHP ............ 252
来源：http://fzv.epnwcf.com

JavaScript ..... 252
来源：http://cnt.havefunace.top

TypeScript ..... 212
来源：http://fix.jianghu66.top

Java ........... 212
来源：http://qou.gotoacloud.top

Go ............. 212
来源：http://ucs.yuxming.cn

Ruby ........... 212
来源：http://zel.dashuyun.cn

C# ............. 212
来源：http://ayd.chenlongwang.top

C .............. 30
来源：http://gsw.snrcjt.cn

C++ ............ 30
来源：http://cxy.sufxvd.cn

SQL ............ 90
来源：http://bdr.jyoumei.cn

Bash ........... 80
来源：http://gpo.xziqi.cn

Kotlin ......... 15
来源：http://ffc.yueranfly.top

Swift .......... 15
来源：http://dpj.cqqwz.cn

Lua ............ 10
来源：http://jkg.zycfv.cn

Perl ........... 10
来源：http://lea.yuanzhike.top

Scala .......... 10
来源：http://cyu.cucudq.cn

------------------------------------
来源：http://adx.zdbjq.cn

合计 ........... 2106 条
来源：http://mxo.hongshengwenyu.top

按章节统计：
来源：http://shz.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rsx.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nif.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bnd.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lfq.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cdr.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://akd.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://afa.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zsk.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nxl.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nmm.chenlongwang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pyb.cashguo.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yfe.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fdh.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bqi.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://isz.dianchejie.cn

Q SQL 专题                              90
来源：http://rpv.chenjidiqi.icu

R Bash 专题                             80
来源：http://uws.jinqigfzy.top

S C / C++ 专题                          60
来源：http://gxy.gaohongyu789.top

T 其他语言补充                          60
来源：http://kdp.jqgfzy.top

U 高频实用片段                         120
来源：http://ihj.zdqjudy.top

------------------------------------
来源：http://tvx.pengpengdd.cyou

合计                                  2106 条
来源：http://iyy.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://aoa.yongpay.top

使用提醒
来源：http://jch.316326.xyz

--------------------------------------------------------------------------------
来源：http://itb.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kbd.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vfx.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rne.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iev.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wzo.wangdashe.top

—— 文件结束 ——
来源：http://djn.gogol.net.cn

================================================================================
来源：http://los.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://znb.guannengcc.top

Common Programming Examples Cheat Book
来源：http://vih.quarkkingdee.top

================================================================================
来源：http://hus.zdbjq.cn

【收录内容】
来源：http://gmt.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vmj.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oli.daxiang520.top

SQL · Bash · C · C++
来源：http://oap.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ubm.9152youxi.cn

【使用说明】
来源：http://rdd.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ivp.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xyw.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://els.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xff.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mjc.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rwf.meibo888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gye.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qth.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ooy.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wlp.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ozi.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vzg.chenlongwang.top

【文件统计】
来源：http://kfa.gogol.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bez.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://xbt.fehbvm.com

目  录
来源：http://dyt.c1oappe.top

--------------------------------------------------------------------------------
来源：http://hfr.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wwa.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hgq.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hkv.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://och.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://exf.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://buh.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bto.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wtl.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cbr.cashguo.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nbr.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rbq.svipenyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ujr.mhx1999.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ldh.sjlbkw.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://auh.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dxa.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mch.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iiy.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cpj.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qlb.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jou.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qmk.chenlongwang.top

================================================================================
来源：http://qnh.tian-w.cn

A. 基础语法与类型
来源：http://bre.nwbrower.top

================================================================================
来源：http://bfl.tian-w.cn

[A01] Hello World
来源：http://pfx.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://cjq.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://thk.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://dmd.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://glj.zhongyouzk.top

Java: System.out.println("Hello, World!");
来源：http://qip.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://jfr.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://bzl.bbcook.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gie.zdbjq.cn

[A02] 变量声明与赋值
来源：http://xyz.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fck.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pqb.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://udl.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jvx.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://ubp.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://cbn.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://qio.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pou.aibaodan.cn

[A03] 常量定义
来源：http://yzd.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mlb.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://xty.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://htu.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://efq.ehwqpu.com

Java: static final double PI = 3.14159;
来源：http://key.aibaodan.cn

Go:   const PI = 3.14159
来源：http://ucd.dianchejie.cn

Ruby: PI = 3.14159
来源：http://drj.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://kck.daria6918.cn

[A04] 判断变量类型
来源：http://fxj.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ndj.cheryme.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ooh.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mda.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://cbo.jinqigufen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://apf.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lhg.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jph.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://efx.cqqwz.cn

[A05] 整数除法与取模
来源：http://raz.zhijiandao.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://njv.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://xax.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nma.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://plm.smart0.xyz

Java: 7 / 2; 7 % 2
来源：http://ynn.fktsv.cn

Go:   7 / 2; 7 % 2
来源：http://nuq.ctjpmb.com

Ruby: 7 / 2; 7 % 2
来源：http://nks.nwbrower.top

C#:   7 / 2; 7 % 2
来源：http://gsa.gogol.net.cn

[A06] 字符串转数字
来源：http://fyv.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://ebd.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gem.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rmz.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://mfg.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cwf.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://anh.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ilg.xingfuxueyuan.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xsq.fengsongda.top

[A07] 数字转字符串
来源：http://sri.quarkkingdee.top

Py:   str(42)
来源：http://qff.hammf.cn

PHP:  (string) 42; strval(42)
来源：http://hua.52xcode.cn

JS:   String(42); (42).toString()
来源：http://bfa.c1oappe.top

TS:   String(42)
来源：http://meo.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zun.wangdashe.top

Go:   strconv.Itoa(42)
来源：http://lpg.zdqjudy.top

Ruby: 42.to_s
来源：http://uxs.c1oappe.top

C#:   42.ToString()
来源：http://wyj.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://klx.sxryk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vji.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mru.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://shs.hywenlv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ctc.xuanzx.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pep.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://utg.vehdjk.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://xbk.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hlr.yuanzhike.top

[A09] 绝对值与最大最小值
来源：http://wyj.pycfn.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://enm.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gyq.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lch.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pwz.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kdk.smart0.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vnk.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kse.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gvb.fzhhl.top

[A10] 生成随机数
来源：http://nhp.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://qzi.bjfxy.top

PHP:  random_int(1, 100);
来源：http://ntx.cheryme.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dup.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fte.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://jvl.ctjpmb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://akb.cheryme.top

Ruby: rand(1..100)
来源：http://csz.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://jid.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://juu.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://xgo.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yes.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://fhm.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uhv.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://ziy.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ymw.pycfn.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ose.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://dkd.fengsongda.top

[A12] 字符串插值 / 格式化
来源：http://muo.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sap.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://axe.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://ful.xziqi.cn

TS:   `Hello, ${name}!`
来源：http://ohw.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://goq.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fia.ydzc1.top

Ruby: "Hello, #{name}!"
来源：http://gcs.gogol.net.cn

C#:   $"Hello, {name}!"
来源：http://aoc.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://dgg.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://ifp.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://uuk.hongshengwenyu.top

JS:   "第一行\n第二行"
来源：http://ggg.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://hmw.sufxvd.cn

Java: "第一行\n第二行"
来源：http://iup.birdmap.top

Go:   "第一行\n第二行"
来源：http://zwp.hywenlv.cn

Ruby: "第一行\n第二行"
来源：http://xow.bjfxy.top

C#:   "第一行\n第二行"
来源：http://wma.fanxiaobao.xyz

[A14] 注释写法
来源：http://hel.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zzr.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://rlv.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://egl.hywenlv.cn

TS:   // 单行；/* 多行 */
来源：http://pbk.jinqigufen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qwh.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://jvx.daria6918.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gjb.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://pwe.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://xxv.gzhubu.top

Py:   value = data or "默认值"
来源：http://ule.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://sxg.pycfn.com

JS:   const value = data ?? "默认值";
来源：http://pfy.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://adi.daxiang520.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yqb.yfazqb.com

Go:   if data == "" { data = "默认值" }
来源：http://vyp.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://zdv.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://dte.hammf.cn

[A16] 真假值判断规则
来源：http://gdj.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wml.iojbl.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wjn.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ybu.sysykeji.top

TS:   if (!x) {}
来源：http://rge.bjfxy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yps.birdmap.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bnn.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://gog.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nsa.xziqi.cn

[A17] 位运算
来源：http://cgq.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://doq.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bgy.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pld.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pnm.9152youxi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezc.ppjwa.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ath.xuanzx.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mum.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://whx.vehdjk.com

[A18] 字符与 ASCII 码互转
来源：http://dnv.pengpengdd.cyou

Py:   ord("A"); chr(65)
来源：http://kov.gotoacloud.top

PHP:  ord("A"); chr(65)
来源：http://qso.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://geb.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zee.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://win.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gjf.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://sck.cashguo.top


<!-- 参考信息 -->