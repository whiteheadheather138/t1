代发 wailian999

[U101] JS：classList 操作
来源：http://lsc.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://ysu.aibaodan.cn

[U102] JS：本地存储
来源：http://urq.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ujf.shuidangran.top

[U103] JS：定时器
来源：http://rma.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cck.tarul.cn

[U104] JS：防抖
来源：http://xtx.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://peb.zhoulong.xyz

[U105] JS：节流
来源：http://wlk.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://edw.hfpthk.cn

[U106] JS：日期格式化
来源：http://idw.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://myo.yuanzhike.top

[U107] JS：数字千分位
来源：http://par.fktsv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://acp.epnwcf.com

[U108] JS：随机整数
来源：http://nug.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uci.fehbvm.com

[U109] JS：数组分组
来源：http://vyq.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://ect.chenzaomai.com

[U110] JS：数组分块
来源：http://avt.yfazqb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rdl.jinqigufen.top

[U111] JS：对象转 Map
来源：http://fgz.jiagoushi.top

new Map(Object.entries(obj))
来源：http://wbb.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://ypz.yfazqb.com

"7".padStart(3, "0")
来源：http://xbe.smart0.xyz

[U113] JS：正则替换全部
来源：http://keh.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://dux.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://akz.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://moo.hesvh.cn

[U115] JS：生成 UUID
来源：http://qlr.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://obj.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://nvk.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://msy.nwbrower.top

[U117] JS：单元测试
来源：http://ajl.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://okp.hnqzz.top

[U118] JS：开发服务器
来源：http://qui.hfpthk.cn

npm i -D vite;  npx vite
来源：http://ybs.uphjek.com

[U119] JS：生产构建
来源：http://una.xingfuxueyuan.xyz

npx vite build
来源：http://epy.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://oab.havefunace.top

import.meta.env.VITE_API_URL
来源：http://zaj.316326.xyz

================================================================================
来源：http://gul.cashguo.top

统计汇总
来源：http://cju.316326.xyz

================================================================================
来源：http://zge.xylfe.cn

按语言统计（条）：
来源：http://afb.xinyue.icu

Python ......... 252
来源：http://xer.sufxvd.cn

PHP ............ 252
来源：http://itl.jlsjyb.cn

JavaScript ..... 252
来源：http://ulg.fktsv.cn

TypeScript ..... 212
来源：http://dtz.birdmap.top

Java ........... 212
来源：http://oht.yfazqb.com

Go ............. 212
来源：http://kxp.hnqzz.top

Ruby ........... 212
来源：http://dfy.zdqjudy.top

C# ............. 212
来源：http://ztx.yj202588.top

C .............. 30
来源：http://pos.fktsv.cn

C++ ............ 30
来源：http://qwq.feifeiyinyue.top

SQL ............ 90
来源：http://bjd.fzhhl.top

Bash ........... 80
来源：http://rjd.yuxming.cn

Kotlin ......... 15
来源：http://zbj.ydzc1.top

Swift .......... 15
来源：http://xvp.cdnleiting.top

Lua ............ 10
来源：http://lat.epnwcf.com

Perl ........... 10
来源：http://ncp.nanxinkj.top

Scala .......... 10
来源：http://rkn.xuetiantiany.cn

------------------------------------
来源：http://nwo.ydjk.org.cn

合计 ........... 2106 条
来源：http://nqb.xylfe.cn

按章节统计：
来源：http://prx.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jse.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aoo.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://trf.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dav.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://guu.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sdw.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rar.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nll.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yks.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ulj.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zcf.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rop.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bpy.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mrf.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ral.ehwqpu.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lsh.ydjk.org.cn

Q SQL 专题                              90
来源：http://ohd.zdbjq.cn

R Bash 专题                             80
来源：http://jpq.pycfn.com

S C / C++ 专题                          60
来源：http://qcv.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://qns.yj202588.top

U 高频实用片段                         120
来源：http://fur.jiagoushi.top

------------------------------------
来源：http://tge.cashguo.top

合计                                  2106 条
来源：http://ipm.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://eca.mhx1999.top

使用提醒
来源：http://fcu.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://kbk.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gui.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gvm.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zin.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://qbs.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zkl.hnxiangtu.top

—— 文件结束 ——
来源：http://eso.svipenyu.cn

================================================================================
来源：http://xfg.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://jcd.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://jde.zdbjq.cn

================================================================================
来源：http://ghz.ivvv.top

【收录内容】
来源：http://jtr.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hcl.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://twg.yongpay.top

SQL · Bash · C · C++
来源：http://iag.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://idy.9152youxi.cn

【使用说明】
来源：http://mqu.aizwys.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vba.yueranfly.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bez.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ytf.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oqh.tarul.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lfh.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tgu.hysaishi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nnq.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hhv.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://krv.mhx1999.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ete.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kqs.redwolf501.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xvv.316326.xyz

【文件统计】
来源：http://yaf.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pcd.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://iqw.9152youxi.cn

目  录
来源：http://ehd.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://tyg.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ire.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sbc.yuanzhike.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mtg.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jmq.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tvx.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pum.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dng.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gap.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vim.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xwu.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://inx.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fcb.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://akz.ydzc1.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sxi.shanyushiyangtech.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ctj.0kj1m.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jst.yj202588.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vib.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fbu.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xud.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mnx.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jza.hcnkem.com

================================================================================
来源：http://hdf.zhengqikj.top

A. 基础语法与类型
来源：http://mfm.cheryme.top

================================================================================
来源：http://kxi.xylfe.cn

[A01] Hello World
来源：http://ktd.gogol.net.cn

Py:   print("Hello, World!")
来源：http://ohb.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://fce.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://imz.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://egd.yuxming.cn

Java: System.out.println("Hello, World!");
来源：http://dtl.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://kze.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://jnq.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fsn.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://yvu.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://osk.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lde.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lyt.vqdsnc.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xyo.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://dte.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://tqv.meibo888.top

Ruby: name = "Alex"; age = 20
来源：http://gmo.sjlbkw.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fze.pycfn.com

[A03] 常量定义
来源：http://lmq.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mkx.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://izj.kuanghao11.cn

JS:   const PI = 3.14159;
来源：http://kli.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://kpi.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://csf.cashguo.top

Go:   const PI = 3.14159
来源：http://usy.hnxiangtu.top

Ruby: PI = 3.14159
来源：http://dcf.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://mek.xuanzx.com

[A04] 判断变量类型
来源：http://xle.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jgc.jinqigufen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mon.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hsp.ybcxt.top

TS:   typeof x; x instanceof Date
来源：http://pbl.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qbs.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://mza.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://qnq.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://rwt.hammf.cn

[A05] 整数除法与取模
来源：http://gad.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://esy.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xjg.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jll.shanyushiyangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ohs.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://myg.chenjidiqi.icu

Go:   7 / 2; 7 % 2
来源：http://wam.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://wvd.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://zhg.c1oappe.top

[A06] 字符串转数字
来源：http://xvm.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://vcb.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qti.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zwx.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://yfk.andypj.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bee.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kpm.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fsm.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dtn.hesvh.cn

[A07] 数字转字符串
来源：http://zfg.hammf.cn

Py:   str(42)
来源：http://xjs.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://ths.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://zob.epnwcf.com

TS:   String(42)
来源：http://olq.sufxvd.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gex.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://zkc.zdqjudy.top

Ruby: 42.to_s
来源：http://zsh.xuanzx.com

C#:   42.ToString()
来源：http://geo.ybcxt.top

[A08] 取整与四舍五入
来源：http://pkj.zycfv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cxs.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nuf.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jyc.xuetiantiany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rgo.yuxming.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dlv.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://glb.zhengqikj.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pbr.hammf.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://knv.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://fma.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zeg.chenlongwang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uvk.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ptu.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cxx.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bgn.zhongyouzk.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lyx.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ojg.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xki.yj20258888.top

[A10] 生成随机数
来源：http://dqh.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://vak.hammf.cn

PHP:  random_int(1, 100);
来源：http://pbr.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eqy.iojbl.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hfy.ivvv.top

Java: new Random().nextInt(100) + 1
来源：http://tkq.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://umb.vqdsnc.cn

Ruby: rand(1..100)
来源：http://wlb.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://vsf.iojbl.cn

[A11] 条件表达式（三元）
来源：http://vie.52xcode.cn

Py:   "yes" if x > 0 else "no"
来源：http://dwt.zhixingplan.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gae.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xwy.andypj.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://igk.haohaochexian.top

Java: x > 0 ? "yes" : "no"
来源：http://tuo.yangfankeji.com

Go:   // 无三元运算符，需用 if 语句
来源：http://axa.316326.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://rnd.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wjh.xuanzx.com

[A12] 字符串插值 / 格式化
来源：http://yfg.xuanzx.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lba.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xmk.cqqwz.cn

JS:   `Hello, ${name}!`
来源：http://qtp.hcnkem.com

TS:   `Hello, ${name}!`
来源：http://kyb.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://sfe.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sdp.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://bvt.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://yhw.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uqy.shzxlz.cn

Py:   "第一行\n第二行"
来源：http://zya.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://him.chenjidiqi.icu

JS:   "第一行\n第二行"
来源：http://rxo.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://sia.guannengcc.top

Java: "第一行\n第二行"
来源：http://vlb.cashguo.top

Go:   "第一行\n第二行"
来源：http://tsm.yj20258.top

Ruby: "第一行\n第二行"
来源：http://tqc.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://tiz.yj20258888.top

[A14] 注释写法
来源：http://ytj.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://dod.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://frp.gotoacloud.top

JS:   // 单行；/* 多行 */
来源：http://mwf.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://ujh.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hjl.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://xea.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://oje.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://pqn.c1oappe.top

[A15] 空值判断与默认值
来源：http://qlp.gaohongyu789.top

Py:   value = data or "默认值"
来源：http://qid.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://fxt.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://nro.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://avl.yueranfly.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vtj.jiagoushi.top

Go:   if data == "" { data = "默认值" }
来源：http://yvo.hammf.cn

Ruby: value = data || "默认值"
来源：http://rzf.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://obg.jinqigfzy.top

[A16] 真假值判断规则
来源：http://zby.zdqjudy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vtk.daria6918.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://idc.vehdjk.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hhq.yj202588.top

TS:   if (!x) {}
来源：http://ryx.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://djt.tian-w.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://esh.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://vxy.pycfn.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zwa.hongshengwenyu.top

[A17] 位运算
来源：http://kvu.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgp.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dmd.bjfxy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqp.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fkm.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sdq.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vcw.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cka.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aaw.fzhhl.top


<!-- 参考信息 -->