代发 wailian999

[U105] JS：节流
来源：http://lfl.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://amm.aizwys.cn

[U106] JS：日期格式化
来源：http://utt.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mkk.yfazqb.com

[U107] JS：数字千分位
来源：http://muk.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rds.havefunace.top

[U108] JS：随机整数
来源：http://yrh.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kpi.yj202588.top

[U109] JS：数组分组
来源：http://rgd.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://ltg.zhoulong.xyz

[U110] JS：数组分块
来源：http://bvt.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vgl.zdqjudy.top

[U111] JS：对象转 Map
来源：http://hyo.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://vax.tianlin.xyz

[U112] JS：字符串补位
来源：http://vsf.52xcode.cn

"7".padStart(3, "0")
来源：http://duf.uphjek.com

[U113] JS：正则替换全部
来源：http://wdc.sweek.top

s.replaceAll("a", "b")
来源：http://nwk.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://zot.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://whl.daria6918.cn

[U115] JS：生成 UUID
来源：http://wib.xziqi.cn

crypto.randomUUID()
来源：http://nlt.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://axi.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://fev.yj20258888.top

[U117] JS：单元测试
来源：http://jgb.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://jwk.fktsv.cn

[U118] JS：开发服务器
来源：http://tnn.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://qri.pycfn.com

[U119] JS：生产构建
来源：http://cje.sufxvd.cn

npx vite build
来源：http://wvb.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://obt.pycfn.com

import.meta.env.VITE_API_URL
来源：http://uyq.fanxiaobao.xyz

================================================================================
来源：http://tkf.kuanghao11.cn

统计汇总
来源：http://wgh.316326.xyz

================================================================================
来源：http://mvz.yangfankeji.com

按语言统计（条）：
来源：http://ghd.andypj.xyz

Python ......... 252
来源：http://ujf.yanxiufei.cn

PHP ............ 252
来源：http://aik.52xcode.cn

JavaScript ..... 252
来源：http://okf.xuanzx.com

TypeScript ..... 212
来源：http://zfu.iojbl.cn

Java ........... 212
来源：http://ugh.hnqzz.top

Go ............. 212
来源：http://xsz.ydzc1.top

Ruby ........... 212
来源：http://cpq.pengpengdd.cyou

C# ............. 212
来源：http://cbi.hnxiangtu.top

C .............. 30
来源：http://men.dashuyun.cn

C++ ............ 30
来源：http://clo.sufxvd.cn

SQL ............ 90
来源：http://gcp.gaohongyu789.top

Bash ........... 80
来源：http://jtf.sweek.top

Kotlin ......... 15
来源：http://lxo.tianlin.xyz

Swift .......... 15
来源：http://pnj.zdqjudy.top

Lua ............ 10
来源：http://jfr.316326.xyz

Perl ........... 10
来源：http://ssm.cashguo.top

Scala .......... 10
来源：http://fbc.hammf.cn

------------------------------------
来源：http://zjs.ydzc1.top

合计 ........... 2106 条
来源：http://fat.xylfe.cn

按章节统计：
来源：http://olw.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bjn.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ybc.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gst.chenlongwang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cah.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fsr.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ugn.nanxinkj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://har.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgj.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iaq.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cve.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kid.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sod.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ell.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bvq.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qhg.xziqi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hde.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://mel.iojbl.cn

R Bash 专题                             80
来源：http://lol.uphjek.com

S C / C++ 专题                          60
来源：http://dsp.ivvv.top

T 其他语言补充                          60
来源：http://phz.hesvh.cn

U 高频实用片段                         120
来源：http://ibb.jinqigfzy.top

------------------------------------
来源：http://sir.xylfe.cn

合计                                  2106 条
来源：http://tha.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://bks.hnxiangtu.top

使用提醒
来源：http://gxi.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://uxi.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zzl.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xbe.yj20258888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qlr.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://itv.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oky.epnwcf.com

—— 文件结束 ——
来源：http://mdx.ydjk.org.cn

================================================================================
来源：http://ebu.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://tng.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://yst.nwbrower.top

================================================================================
来源：http://fsk.vqdsnc.cn

【收录内容】
来源：http://lny.c1oappe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://otm.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rjn.52xcode.cn

SQL · Bash · C · C++
来源：http://kqq.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://toq.c1oappe.top

【使用说明】
来源：http://pdg.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tgh.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rav.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://neq.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qvg.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cyq.fehbvm.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ude.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ghi.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gng.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://opz.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lgj.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://whj.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ufh.yvedp.cn

【文件统计】
来源：http://yif.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nbh.yj20258888.top

--------------------------------------------------------------------------------
来源：http://qcb.xinyue.icu

目  录
来源：http://tag.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://juv.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jdr.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ekp.gotoacloud.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://smu.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tnq.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jje.ydjk.org.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gdi.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aqu.jlsjyb.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pea.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ibn.gaohongyu789.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://opw.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ebz.aibaodan.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cmk.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lzu.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cnv.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qpj.xziqi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://flb.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://plu.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tgr.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ivj.snrcjt.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ipx.yanxiufei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zjo.xziqi.cn

================================================================================
来源：http://tal.aizwys.cn

A. 基础语法与类型
来源：http://xdf.chenzaomai.com

================================================================================
来源：http://lyn.iojbl.cn

[A01] Hello World
来源：http://jqe.iojbl.cn

Py:   print("Hello, World!")
来源：http://irk.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://fys.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://bex.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hge.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://ykw.andypj.xyz

Go:   fmt.Println("Hello, World!")
来源：http://xja.haohaochexian.top

Ruby: puts "Hello, World!"
来源：http://nmi.quarkkingdee.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qwl.tian-w.cn

[A02] 变量声明与赋值
来源：http://vus.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://myi.chenlongwang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cdl.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gru.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wnr.shangyingyoupin.top

Java: String name = "Alex"; int age = 20;
来源：http://xfh.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://mbx.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://hhw.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aaj.mhx1999.top

[A03] 常量定义
来源：http://yei.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yir.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://hox.yj202588.top

JS:   const PI = 3.14159;
来源：http://dwl.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://dpt.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://pnt.jinqigufen.top

Go:   const PI = 3.14159
来源：http://cpq.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://sdh.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://mga.yuxming.cn

[A04] 判断变量类型
来源：http://vlu.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://pne.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dig.yfazqb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://byf.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://nla.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://huv.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://gxn.zhixingplan.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yhh.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://mwb.fzhhl.top

[A05] 整数除法与取模
来源：http://sxd.zycfv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jjf.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://psj.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zgs.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vbf.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://frd.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://sml.birdmap.top

Ruby: 7 / 2; 7 % 2
来源：http://osr.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://mqm.shzxlz.cn

[A06] 字符串转数字
来源：http://dkl.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://jqi.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ojs.tian-w.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fly.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://pkk.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jik.yangfankeji.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fsn.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fqm.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bta.jyoumei.cn

[A07] 数字转字符串
来源：http://kpp.fktsv.cn

Py:   str(42)
来源：http://rtt.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://yhg.aizwys.cn

JS:   String(42); (42).toString()
来源：http://nxt.shanyushiyangkeji.top

TS:   String(42)
来源：http://svj.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://eyn.hammf.cn

Go:   strconv.Itoa(42)
来源：http://gsx.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://kox.dianchejie.cn

C#:   42.ToString()
来源：http://krf.smart0.xyz

[A08] 取整与四舍五入
来源：http://ldf.52xcode.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hjh.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wul.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hkw.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nml.xuanzx.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hoj.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jec.ivvv.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nhb.jinyuanbaomall.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ujl.hfpthk.cn

[A09] 绝对值与最大最小值
来源：http://wrl.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://onp.aibaodan.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tqm.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ywm.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yax.vqdsnc.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://efh.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xjy.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aks.nanxuanxn.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yor.cheryme.top

[A10] 生成随机数
来源：http://oqq.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://vpa.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://ypy.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wop.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fqa.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://pjh.zhengqikj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dxj.vqdsnc.cn

Ruby: rand(1..100)
来源：http://dmy.epnwcf.com

C#:   new Random().Next(1, 101)
来源：http://bwr.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://qfc.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://odg.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mmz.yvedp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ctc.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://wzm.fanxiaobao.xyz

Java: x > 0 ? "yes" : "no"
来源：http://jna.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://txg.gogol.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ket.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://iel.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://ilt.jqgufenzy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wtc.dianchejie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ssn.bbcook.cn

JS:   `Hello, ${name}!`
来源：http://nsu.ywan-chungtsiang.top

TS:   `Hello, ${name}!`
来源：http://njy.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://jfp.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tzf.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://bbv.ydzc1.top

C#:   $"Hello, {name}!"
来源：http://waq.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://zcg.chenzaomai.com

Py:   "第一行\n第二行"
来源：http://enx.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://ymq.mhx1999.top

JS:   "第一行\n第二行"
来源：http://hvs.yfazqb.com

TS:   "第一行\n第二行"
来源：http://ypa.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://muv.yj20258.top

Go:   "第一行\n第二行"
来源：http://pdn.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://ocu.zhongyouzk.top

C#:   "第一行\n第二行"
来源：http://bxa.chenjidiqi.icu

[A14] 注释写法
来源：http://mgh.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vik.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://npr.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://nnx.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://znz.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vcx.tanke756.top

Go:   // 单行；/* 多行 */
来源：http://vel.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://qhs.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://gzg.nwbrower.top

[A15] 空值判断与默认值
来源：http://axu.smart0.xyz

Py:   value = data or "默认值"
来源：http://ecs.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://jzr.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://hth.yj20258.top

TS:   const value = data ?? "默认值";
来源：http://uxl.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xpt.xziqi.cn

Go:   if data == "" { data = "默认值" }
来源：http://jku.havefunace.top

Ruby: value = data || "默认值"
来源：http://yqi.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://utj.svipenyu.cn

[A16] 真假值判断规则
来源：http://vhc.gogol.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qao.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vdm.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lus.dashuyun.cn

TS:   if (!x) {}
来源：http://wnt.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uty.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fyu.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://kwi.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lry.ivvv.top

[A17] 位运算
来源：http://cov.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hjo.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ctr.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zyw.epnwcf.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lcz.yuxming.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmo.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://erp.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfj.gzhubu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fii.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://kai.zhixingplan.top

Py:   ord("A"); chr(65)
来源：http://ycu.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://gxs.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wke.aizwys.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kyt.zhixingplan.top

Java: (int) 'A'; (char) 65
来源：http://rlj.hesvh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hyq.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://jbd.hesvh.cn


<!-- 参考信息 -->