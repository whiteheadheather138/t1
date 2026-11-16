代发 wailian999

[U103] JS：定时器
来源：http://mpw.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jvr.yonumen.top

[U104] JS：防抖
来源：http://rta.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jlo.sweek.top

[U105] JS：节流
来源：http://dgp.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ubb.sysykeji.top

[U106] JS：日期格式化
来源：http://qhf.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qcs.yj20258888.top

[U107] JS：数字千分位
来源：http://mwq.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://opj.cashguo.top

[U108] JS：随机整数
来源：http://nsn.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lnq.ydjk.org.cn

[U109] JS：数组分组
来源：http://nxv.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://mnz.kuanghao11.cn

[U110] JS：数组分块
来源：http://fhy.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jej.hnqzz.top

[U111] JS：对象转 Map
来源：http://ohe.hammf.cn

new Map(Object.entries(obj))
来源：http://dpx.zhongyouzk.top

[U112] JS：字符串补位
来源：http://nst.cheryme.top

"7".padStart(3, "0")
来源：http://dql.yuxming.cn

[U113] JS：正则替换全部
来源：http://yww.xuetiantiany.cn

s.replaceAll("a", "b")
来源：http://bnd.tian-w.cn

[U114] JS：JSON 深比较
来源：http://baz.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nvy.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://ruu.wangdashe.top

crypto.randomUUID()
来源：http://nzb.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://azi.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://nmh.yuanzhike.top

[U117] JS：单元测试
来源：http://elw.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://yaq.aizwys.cn

[U118] JS：开发服务器
来源：http://pdd.daxiang520.top

npm i -D vite;  npx vite
来源：http://nrt.daria6918.cn

[U119] JS：生产构建
来源：http://bch.jyoumei.cn

npx vite build
来源：http://oxn.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://szv.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://lez.yongpay.top

================================================================================
来源：http://ypo.hcnkem.com

统计汇总
来源：http://ejb.quarkkingdee.top

================================================================================
来源：http://acf.redwolf501.top

按语言统计（条）：
来源：http://qav.zhiwuduotai.top

Python ......... 252
来源：http://icv.hnxiangtu.top

PHP ............ 252
来源：http://dgs.jinghuilouyu.cn

JavaScript ..... 252
来源：http://bvl.yfazqb.com

TypeScript ..... 212
来源：http://abn.xingfuxueyuan.xyz

Java ........... 212
来源：http://tsp.shanyushiyangtech.top

Go ............. 212
来源：http://fhg.aizwys.cn

Ruby ........... 212
来源：http://wfu.chenzaomai.com

C# ............. 212
来源：http://uld.jinqigfzy.top

C .............. 30
来源：http://gre.havefunace.top

C++ ............ 30
来源：http://iwu.ywan-chungtsiang.top

SQL ............ 90
来源：http://ast.sjlbkw.cn

Bash ........... 80
来源：http://tog.yuxming.cn

Kotlin ......... 15
来源：http://nmr.hysaishi.cn

Swift .......... 15
来源：http://yuz.hcnkem.com

Lua ............ 10
来源：http://dll.fktsv.cn

Perl ........... 10
来源：http://oed.gogol.net.cn

Scala .......... 10
来源：http://lub.xingfuxueyuan.xyz

------------------------------------
来源：http://rcy.snrcjt.cn

合计 ........... 2106 条
来源：http://nka.hammf.cn

按章节统计：
来源：http://stz.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rar.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ovt.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wor.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ifl.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ldq.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fhz.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bxu.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://unz.shzxlz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ypf.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zfo.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mco.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://npp.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vtp.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qwx.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dtg.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gdr.xuetiantiany.cn

Q SQL 专题                              90
来源：http://vww.52xcode.cn

R Bash 专题                             80
来源：http://qmn.redwolf501.top

S C / C++ 专题                          60
来源：http://eyr.dianchejie.cn

T 其他语言补充                          60
来源：http://ljh.hcnkem.com

U 高频实用片段                         120
来源：http://hqq.bbcook.cn

------------------------------------
来源：http://rnw.ybcxt.top

合计                                  2106 条
来源：http://dvm.sysykeji.top

--------------------------------------------------------------------------------
来源：http://tzs.hcnkem.com

使用提醒
来源：http://chm.yj202588.top

--------------------------------------------------------------------------------
来源：http://lwi.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qob.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pub.nanxuanxn.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://par.snrcjt.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vol.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sso.sysykeji.top

—— 文件结束 ——
来源：http://jto.snrcjt.cn

================================================================================
来源：http://uhy.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://efl.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://jdg.gaohongyu789.top

================================================================================
来源：http://dbu.tian-w.cn

【收录内容】
来源：http://fhs.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tfk.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ddj.dianchejie.cn

SQL · Bash · C · C++
来源：http://hhz.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jll.jqgufenzy.top

【使用说明】
来源：http://yav.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vix.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cob.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xpn.epnwcf.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://izi.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lkf.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ssx.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bkr.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gnx.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wud.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://crg.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vdh.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ptb.mhx1999.top

【文件统计】
来源：http://box.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ofp.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://pon.shuidangran.top

目  录
来源：http://wxg.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://suu.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gph.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rbw.yfazqb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wiv.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oli.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dor.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gyk.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gat.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://exb.gaohongyu789.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qis.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bjt.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pee.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qwh.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nqc.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wsr.jqgfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uie.yj20258.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bkl.bjfxy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uzd.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hct.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ahl.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ici.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rki.sweek.top

================================================================================
来源：http://ydq.jianghu66.top

A. 基础语法与类型
来源：http://zlj.jlsjyb.cn

================================================================================
来源：http://kgo.jinghuilouyu.cn

[A01] Hello World
来源：http://xti.vqdsnc.cn

Py:   print("Hello, World!")
来源：http://ygy.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://osz.tanke756.top

JS:   console.log("Hello, World!");
来源：http://dgm.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tyv.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://trh.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://iux.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://dil.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tdc.fktsv.cn

[A02] 变量声明与赋值
来源：http://vtd.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://urw.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cfv.mhx1999.top

JS:   let name = "Alex"; const age = 20;
来源：http://emx.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://crm.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://jum.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://gvj.dashuyun.cn

Ruby: name = "Alex"; age = 20
来源：http://qap.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://bsm.yj20258888.top

[A03] 常量定义
来源：http://jzu.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dhi.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://odk.shangyingyoupin.top

JS:   const PI = 3.14159;
来源：http://ncz.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://ctu.hnqzz.top

Java: static final double PI = 3.14159;
来源：http://usv.9152youxi.cn

Go:   const PI = 3.14159
来源：http://rel.havefunace.top

Ruby: PI = 3.14159
来源：http://hzj.kuanghao11.cn

C#:   const double PI = 3.14159;
来源：http://rze.0kj1m.cn

[A04] 判断变量类型
来源：http://wps.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://iig.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gdt.jinqigufen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qly.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://ghn.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://trw.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://xdr.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kef.zhijiandao.cn

C#:   x.GetType().Name; x is int
来源：http://psc.cucudq.cn

[A05] 整数除法与取模
来源：http://ksi.yanxiufei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gbh.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jti.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://trd.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kxi.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://eqe.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://mfg.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://dkw.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://dsl.ehwqpu.com

[A06] 字符串转数字
来源：http://gfx.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://hty.haohaochexian.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wgg.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ksm.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sis.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ghs.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yas.sxryk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lfr.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ano.zhixingplan.top

[A07] 数字转字符串
来源：http://mwj.xuetiantiany.cn

Py:   str(42)
来源：http://gey.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://isy.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://kjk.shzxlz.cn

TS:   String(42)
来源：http://djq.gogol.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qyn.hammf.cn

Go:   strconv.Itoa(42)
来源：http://sye.nanxuanxn.top

Ruby: 42.to_s
来源：http://ndz.jinghuilouyu.cn

C#:   42.ToString()
来源：http://gxs.smart0.xyz

[A08] 取整与四舍五入
来源：http://mtf.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rhy.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lrc.aibaodan.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lxj.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uzj.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baz.haohaochexian.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mwe.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rnm.yangfankeji.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bsz.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://hic.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yka.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tiw.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://osm.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uzc.birdmap.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ifj.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ufl.chenjidiqi.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cpz.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kij.guowangkeji.top

[A10] 生成随机数
来源：http://voi.jyoumei.cn

Py:   import random; random.randint(1, 100)
来源：http://mha.zhijiandao.cn

PHP:  random_int(1, 100);
来源：http://rgz.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://joc.vehdjk.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vua.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://rpq.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yfk.meibo888.top

Ruby: rand(1..100)
来源：http://adf.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://vvy.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://bpm.xuanzx.com

Py:   "yes" if x > 0 else "no"
来源：http://ntv.ywan-chungtsiang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kfe.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xav.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jot.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://gjj.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fgk.fengsongda.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mgm.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://vbo.yonumen.top

[A12] 字符串插值 / 格式化
来源：http://won.hysaishi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tva.gzhubu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nex.cheryme.top

JS:   `Hello, ${name}!`
来源：http://smo.ybcxt.top

TS:   `Hello, ${name}!`
来源：http://otz.yuanzhike.top

Java: "Hello, %s!".formatted(name)
来源：http://obg.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ibu.chenzaomai.com

Ruby: "Hello, #{name}!"
来源：http://hgx.jinqigfzy.top

C#:   $"Hello, {name}!"
来源：http://tam.jqgufenzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zsp.birdmap.top

Py:   "第一行\n第二行"
来源：http://tbh.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://ckn.jianghu66.top

JS:   "第一行\n第二行"
来源：http://pny.sweek.top

TS:   "第一行\n第二行"
来源：http://esb.shanyushiyangkeji.top

Java: "第一行\n第二行"
来源：http://aoo.316326.xyz

Go:   "第一行\n第二行"
来源：http://brq.hcnkem.com

Ruby: "第一行\n第二行"
来源：http://xot.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://yez.vehdjk.com

[A14] 注释写法
来源：http://sda.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rem.bjfxy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nih.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://gec.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://zng.jiagoushi.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cye.iojbl.cn

Go:   // 单行；/* 多行 */
来源：http://igp.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://szm.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://czb.ydzc1.top

[A15] 空值判断与默认值
来源：http://qru.svipenyu.cn

Py:   value = data or "默认值"
来源：http://ygs.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://dgt.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://xgx.cdnleiting.top

TS:   const value = data ?? "默认值";
来源：http://khr.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xra.9152youxi.cn

Go:   if data == "" { data = "默认值" }
来源：http://zdd.feifeiyinyue.top

Ruby: value = data || "默认值"
来源：http://blr.zhaomingkeji.xyz

C#:   var value = data ?? "默认值";
来源：http://rrt.hammf.cn

[A16] 真假值判断规则
来源：http://tgp.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vpk.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://evv.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://grf.fengsongda.top

TS:   if (!x) {}
来源：http://uib.c1oappe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qew.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xfk.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://cml.tanke756.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pjl.epnwcf.com

[A17] 位运算
来源：http://vtg.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxs.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nod.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zlx.birdmap.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xhi.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ryd.shzxlz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pcv.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvb.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ohx.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://lxm.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://rhg.bbcook.cn

PHP:  ord("A"); chr(65)
来源：http://abp.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://urp.gzhubu.top


<!-- 参考信息 -->