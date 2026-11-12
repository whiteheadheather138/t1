代发 wailian999

[U103] JS：定时器
来源：http://uat.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wre.xuanzx.com

[U104] JS：防抖
来源：http://bbl.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxg.yanxiufei.cn

[U105] JS：节流
来源：http://rsk.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ifd.hfpthk.cn

[U106] JS：日期格式化
来源：http://sfw.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kan.ivvv.top

[U107] JS：数字千分位
来源：http://jpz.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jcf.mhx1999.top

[U108] JS：随机整数
来源：http://rhh.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dwz.jinqigfzy.top

[U109] JS：数组分组
来源：http://bid.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://xwb.hysaishi.cn

[U110] JS：数组分块
来源：http://xla.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dhb.dashuyun.cn

[U111] JS：对象转 Map
来源：http://cbu.tarul.cn

new Map(Object.entries(obj))
来源：http://hdf.tianlin.xyz

[U112] JS：字符串补位
来源：http://hhr.cucudq.cn

"7".padStart(3, "0")
来源：http://rzy.hnqzz.top

[U113] JS：正则替换全部
来源：http://rnu.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://syx.ydzc1.top

[U114] JS：JSON 深比较
来源：http://cjt.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wye.jqgfzy.top

[U115] JS：生成 UUID
来源：http://leg.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://pnh.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://his.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://pkc.nanxuanxn.top

[U117] JS：单元测试
来源：http://mnu.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://knk.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://kac.guowangkeji.top

npm i -D vite;  npx vite
来源：http://fqa.svipenyu.cn

[U119] JS：生产构建
来源：http://wkd.tanke756.top

npx vite build
来源：http://gbo.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://pgt.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://nmy.xuetiantiany.cn

================================================================================
来源：http://nxx.snrcjt.cn

统计汇总
来源：http://yug.ydjk.org.cn

================================================================================
来源：http://ilx.tanke756.top

按语言统计（条）：
来源：http://uoz.cucudq.cn

Python ......... 252
来源：http://ore.redwolf501.top

PHP ............ 252
来源：http://bxp.sxryk.cn

JavaScript ..... 252
来源：http://htq.gotoacloud.top

TypeScript ..... 212
来源：http://dhk.shzxlz.cn

Java ........... 212
来源：http://kfr.zhoulong.xyz

Go ............. 212
来源：http://aac.aibaodan.cn

Ruby ........... 212
来源：http://bvt.cashguo.top

C# ............. 212
来源：http://ild.ydzc1.top

C .............. 30
来源：http://amv.dashuyun.cn

C++ ............ 30
来源：http://akw.xinyue.icu

SQL ............ 90
来源：http://xfs.uphjek.com

Bash ........... 80
来源：http://zzf.316326.xyz

Kotlin ......... 15
来源：http://zra.nanxinkj.top

Swift .......... 15
来源：http://uhk.wangshuangyany.cn

Lua ............ 10
来源：http://jyj.tanke756.top

Perl ........... 10
来源：http://yak.fehbvm.com

Scala .......... 10
来源：http://kyk.jinghuilouyu.cn

------------------------------------
来源：http://akv.bjfxy.top

合计 ........... 2106 条
来源：http://vgl.xinyue.icu

按章节统计：
来源：http://auu.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://grv.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://opj.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qeu.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iqu.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://csr.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://flw.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://juj.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gnb.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ugz.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dbl.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xqd.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ijf.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://you.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pxt.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nvu.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zcq.meibo888.top

Q SQL 专题                              90
来源：http://ybj.xuetiantiany.cn

R Bash 专题                             80
来源：http://vdk.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://qgo.fzhhl.top

T 其他语言补充                          60
来源：http://nsq.xuetiantiany.cn

U 高频实用片段                         120
来源：http://jvy.ppjwa.cn

------------------------------------
来源：http://ygg.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://pml.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://naj.shangyingyoupin.top

使用提醒
来源：http://nik.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://bhn.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lus.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rjn.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eix.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://ypw.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://azx.jinqigfzy.top

—— 文件结束 ——
来源：http://ihw.hywenlv.cn

================================================================================
来源：http://tro.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://kcz.xinyue.icu

Common Programming Examples Cheat Book
来源：http://kiy.xuanzx.com

================================================================================
来源：http://wbq.gotoacloud.top

【收录内容】
来源：http://ckf.kuanghao11.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gqm.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hid.fengsongda.top

SQL · Bash · C · C++
来源：http://heo.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fca.sufxvd.cn

【使用说明】
来源：http://voc.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hon.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tuz.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fid.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kxf.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ras.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sbn.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://csz.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://onm.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oit.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qwy.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://drl.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nkt.zhaomingkeji.xyz

【文件统计】
来源：http://cbt.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hew.ivvv.top

--------------------------------------------------------------------------------
来源：http://iog.yangfankeji.com

目  录
来源：http://xiv.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://ipf.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ebf.zhixingplan.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hhr.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ryc.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qlb.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://liz.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qyf.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vbj.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fxo.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fml.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qgg.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gpf.hammf.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aww.hfpthk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fkz.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://juz.daxiang520.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fhd.jinghuilouyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://onm.jyoumei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://syn.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jxf.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yds.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ssr.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ayk.mhx1999.top

================================================================================
来源：http://rpa.xuanzx.com

A. 基础语法与类型
来源：http://occ.guannengcc.top

================================================================================
来源：http://dqu.fehbvm.com

[A01] Hello World
来源：http://wuw.yueranfly.top

Py:   print("Hello, World!")
来源：http://rgc.hnqzz.top

PHP:  echo "Hello, World!";
来源：http://hrs.zhijiandao.cn

JS:   console.log("Hello, World!");
来源：http://emk.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zmt.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://tdg.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://kmp.daxiang520.top

Ruby: puts "Hello, World!"
来源：http://wqj.bjfxy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zup.guowangkeji.top

[A02] 变量声明与赋值
来源：http://rje.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kfn.jqgufenzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xgm.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ket.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ppb.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://rue.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://fnr.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://tvh.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://sqt.yonumen.top

[A03] 常量定义
来源：http://eue.gotoacloud.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cvg.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://won.316326.xyz

JS:   const PI = 3.14159;
来源：http://gsp.sysykeji.top

TS:   const PI: number = 3.14159;
来源：http://ljz.svipenyu.cn

Java: static final double PI = 3.14159;
来源：http://fzf.hnqzz.top

Go:   const PI = 3.14159
来源：http://teo.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://bfa.sweek.top

C#:   const double PI = 3.14159;
来源：http://mmf.feifeiyinyue.top

[A04] 判断变量类型
来源：http://ral.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://dkq.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gyx.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://clj.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://dnm.tianlin.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tsk.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://bxz.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yzi.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://ycx.zhengqikj.top

[A05] 整数除法与取模
来源：http://hon.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bpa.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://edj.zycfv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tfa.fktsv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xrc.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://jia.sjlbkw.cn

Go:   7 / 2; 7 % 2
来源：http://jyi.cqqwz.cn

Ruby: 7 / 2; 7 % 2
来源：http://uqv.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://szb.sysykeji.top

[A06] 字符串转数字
来源：http://hyy.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://cyq.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hei.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hqy.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://viz.ywan-chungtsiang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mib.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://olo.bbcook.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ayt.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tbw.xuanzx.com

[A07] 数字转字符串
来源：http://cfs.yangfankeji.com

Py:   str(42)
来源：http://hdw.gogol.net.cn

PHP:  (string) 42; strval(42)
来源：http://ztu.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://qgh.tanke756.top

TS:   String(42)
来源：http://kiy.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eaz.aizwys.cn

Go:   strconv.Itoa(42)
来源：http://xck.0kj1m.cn

Ruby: 42.to_s
来源：http://xmd.jinghuilouyu.cn

C#:   42.ToString()
来源：http://fsp.cucudq.cn

[A08] 取整与四舍五入
来源：http://eer.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://krb.kuanghao11.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hwv.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fdk.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vqv.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zkc.xingfuxueyuan.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wjg.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rtw.zdbjq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qft.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://oex.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://onb.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zqd.zdbjq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hdq.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://obx.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://whr.jinyuanbaomall.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://bju.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nij.pengpengdd.cyou

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bsd.jyoumei.cn

[A10] 生成随机数
来源：http://khw.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://ist.mhx1999.top

PHP:  random_int(1, 100);
来源：http://oic.kuanghao11.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wvp.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lfa.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://qrh.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qdl.jinqigfzy.top

Ruby: rand(1..100)
来源：http://lle.ehwqpu.com

C#:   new Random().Next(1, 101)
来源：http://blw.xylfe.cn

[A11] 条件表达式（三元）
来源：http://axa.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://rsv.zycfv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qju.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://bvq.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://qgc.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://hvm.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qtf.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ave.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://alm.fengsongda.top

[A12] 字符串插值 / 格式化
来源：http://ejk.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://snv.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fgk.ppjwa.cn

JS:   `Hello, ${name}!`
来源：http://mlh.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://xlr.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://xvr.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ftu.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://cbz.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://ubl.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://coz.jinqigufen.top

Py:   "第一行\n第二行"
来源：http://ngf.52xcode.cn

PHP:  "第一行\n第二行"
来源：http://oap.nwbrower.top

JS:   "第一行\n第二行"
来源：http://bhg.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://yjk.cqqwz.cn

Java: "第一行\n第二行"
来源：http://nlc.yongpay.top

Go:   "第一行\n第二行"
来源：http://rzp.ivvv.top

Ruby: "第一行\n第二行"
来源：http://hnf.zhaomingkeji.xyz

C#:   "第一行\n第二行"
来源：http://agw.yangfankeji.com

[A14] 注释写法
来源：http://uuv.tianlin.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://hot.sysykeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wci.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://wyv.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://tor.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yuf.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://nkr.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://nds.zhoulong.xyz

C#:   // 单行；/* 多行 */
来源：http://sts.tian-w.cn

[A15] 空值判断与默认值
来源：http://tts.cqqwz.cn

Py:   value = data or "默认值"
来源：http://jxy.zdbjq.cn

PHP:  $value = $data ?? "默认值";
来源：http://eqz.zdqjudy.top

JS:   const value = data ?? "默认值";
来源：http://szp.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://afu.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://myd.sweek.top

Go:   if data == "" { data = "默认值" }
来源：http://voa.shuidangran.top

Ruby: value = data || "默认值"
来源：http://loh.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://jmr.aizwys.cn

[A16] 真假值判断规则
来源：http://lht.jinghuilouyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mxn.epnwcf.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nfs.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hov.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://clv.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://umi.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gjv.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://ror.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fmg.jqgfzy.top

[A17] 位运算
来源：http://zho.yangfankeji.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iiw.jinqigufen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vwg.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ncr.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ccu.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpy.52xcode.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qrk.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wge.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://grx.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://wom.zhijiandao.cn

Py:   ord("A"); chr(65)
来源：http://mgf.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://rvt.nanxuanxn.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cfb.ehwqpu.com


<!-- 参考信息 -->