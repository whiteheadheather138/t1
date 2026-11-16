代发 wailian999

[U99] JS：事件监听
来源：http://ndv.ybcxt.top

el.addEventListener("click", e => {})
来源：http://hfb.cucudq.cn

[U100] JS：DOM 查询
来源：http://wma.sxryk.cn

document.querySelector(".item")
来源：http://elb.0kj1m.cn

[U101] JS：classList 操作
来源：http://zxn.ctjpmb.com

el.classList.toggle("active")
来源：http://pmh.hywenlv.cn

[U102] JS：本地存储
来源：http://gaf.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://msw.sysykeji.top

[U103] JS：定时器
来源：http://wju.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sdx.jqgfzy.top

[U104] JS：防抖
来源：http://hlu.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhl.smart0.xyz

[U105] JS：节流
来源：http://ehc.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wic.meibo888.top

[U106] JS：日期格式化
来源：http://pui.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lve.andypj.xyz

[U107] JS：数字千分位
来源：http://usl.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ajx.yanxiufei.cn

[U108] JS：随机整数
来源：http://gcv.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://clu.snrcjt.cn

[U109] JS：数组分组
来源：http://kdu.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://mrl.dianchejie.cn

[U110] JS：数组分块
来源：http://idk.yfazqb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dov.0kj1m.cn

[U111] JS：对象转 Map
来源：http://tsq.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://wdl.hesvh.cn

[U112] JS：字符串补位
来源：http://btq.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://urm.yueranfly.top

[U113] JS：正则替换全部
来源：http://bql.birdmap.top

s.replaceAll("a", "b")
来源：http://xue.xylfe.cn

[U114] JS：JSON 深比较
来源：http://fyl.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://aoj.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://elg.ybcxt.top

crypto.randomUUID()
来源：http://vfg.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://hma.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://cej.svipenyu.cn

[U117] JS：单元测试
来源：http://whh.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://ckk.ppjwa.cn

[U118] JS：开发服务器
来源：http://ykm.sysykeji.top

npm i -D vite;  npx vite
来源：http://hfh.xylfe.cn

[U119] JS：生产构建
来源：http://wtq.tanke756.top

npx vite build
来源：http://tmy.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://jgl.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://mft.yueranfly.top

================================================================================
来源：http://irz.jlsjyb.cn

统计汇总
来源：http://ult.fanxiaobao.xyz

================================================================================
来源：http://tyd.mhx1999.top

按语言统计（条）：
来源：http://gpv.tanke756.top

Python ......... 252
来源：http://xar.uphjek.com

PHP ............ 252
来源：http://yrw.chenjidiqi.icu

JavaScript ..... 252
来源：http://puf.fehbvm.com

TypeScript ..... 212
来源：http://ipc.52xcode.cn

Java ........... 212
来源：http://wax.tian-w.cn

Go ............. 212
来源：http://mgd.xuanzx.com

Ruby ........... 212
来源：http://frq.vqdsnc.cn

C# ............. 212
来源：http://lfj.chenjidiqi.icu

C .............. 30
来源：http://ypb.feifeiyinyue.top

C++ ............ 30
来源：http://yxh.yonumen.top

SQL ............ 90
来源：http://lps.cashguo.top

Bash ........... 80
来源：http://wzi.316326.xyz

Kotlin ......... 15
来源：http://bak.kuanghao11.cn

Swift .......... 15
来源：http://bps.yanxiufei.cn

Lua ............ 10
来源：http://fdp.quarkkingdee.top

Perl ........... 10
来源：http://vha.sjlbkw.cn

Scala .......... 10
来源：http://acv.hammf.cn

------------------------------------
来源：http://icp.jinqigfzy.top

合计 ........... 2106 条
来源：http://qlj.xingfuxueyuan.xyz

按章节统计：
来源：http://rnj.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pxq.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qfg.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wbh.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ssk.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jng.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://onc.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fhw.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qsz.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ywt.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jxs.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lvg.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lgt.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dox.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pja.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bxk.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mbi.fktsv.cn

Q SQL 专题                              90
来源：http://shj.fanxiaobao.xyz

R Bash 专题                             80
来源：http://wlm.xylfe.cn

S C / C++ 专题                          60
来源：http://btw.aibaodan.cn

T 其他语言补充                          60
来源：http://ipj.ctjpmb.com

U 高频实用片段                         120
来源：http://nbi.zhoulong.xyz

------------------------------------
来源：http://mlg.dashuyun.cn

合计                                  2106 条
来源：http://ryj.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://rgb.daria6918.cn

使用提醒
来源：http://ynv.guannengcc.top

--------------------------------------------------------------------------------
来源：http://dpj.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cgw.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mav.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kxi.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://djm.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qeq.bbcook.cn

—— 文件结束 ——
来源：http://jup.fzhhl.top

================================================================================
来源：http://aie.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://jca.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://mme.yj20258888.top

================================================================================
来源：http://zmq.birdmap.top

【收录内容】
来源：http://sma.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kag.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hpo.sufxvd.cn

SQL · Bash · C · C++
来源：http://txf.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zni.ybcxt.top

【使用说明】
来源：http://ayv.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hej.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wex.feifeiyinyue.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://njl.uphjek.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cmw.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://oqd.sxryk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sxj.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jro.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jmt.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fxz.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://quy.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kre.wangdashe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qxw.snrcjt.cn

【文件统计】
来源：http://qta.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iyl.smart0.xyz

--------------------------------------------------------------------------------
来源：http://eap.zhoulong.xyz

目  录
来源：http://ldw.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://ufs.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zpe.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dfv.hnqzz.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yqw.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lhk.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ycx.ctjpmb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cdm.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tcp.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bjy.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ncr.hywenlv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kil.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yyz.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cnp.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nqy.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ikr.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dxp.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kfj.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lkn.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://enl.hnxiangtu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://loj.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mgy.gzhubu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qkg.tanke756.top

================================================================================
来源：http://ate.shanyushiyangtech.top

A. 基础语法与类型
来源：http://xfh.cucudq.cn

================================================================================
来源：http://rcl.hysaishi.cn

[A01] Hello World
来源：http://cnj.gzhubu.top

Py:   print("Hello, World!")
来源：http://hjm.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://ags.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://qbr.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rji.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://dqn.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://xzt.shangyingyoupin.top

Ruby: puts "Hello, World!"
来源：http://rkb.jinyuanbaomall.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aoz.fzhhl.top

[A02] 变量声明与赋值
来源：http://zjq.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://syl.cheryme.top

PHP:  $name = "Alex"; $age = 20;
来源：http://skr.hesvh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mxy.dianchejie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gxy.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://msw.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://csk.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://nid.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ifv.jinqigufen.top

[A03] 常量定义
来源：http://pzp.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zdy.wangshuangyany.cn

PHP:  const PI = 3.14159;
来源：http://xqx.tarul.cn

JS:   const PI = 3.14159;
来源：http://hrw.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://vfm.xziqi.cn

Java: static final double PI = 3.14159;
来源：http://oqa.hysaishi.cn

Go:   const PI = 3.14159
来源：http://zmw.svipenyu.cn

Ruby: PI = 3.14159
来源：http://tgs.pycfn.com

C#:   const double PI = 3.14159;
来源：http://nbm.fktsv.cn

[A04] 判断变量类型
来源：http://bfg.jinqigfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lfq.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://syo.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mhl.daxiang520.top

TS:   typeof x; x instanceof Date
来源：http://jlh.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zmk.yongpay.top

Go:   reflect.TypeOf(x).Name()
来源：http://bye.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zft.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://uje.ydzc1.top

[A05] 整数除法与取模
来源：http://qsi.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xjz.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://luq.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fyr.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lia.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://kjl.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://xgs.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://sha.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://bjs.epnwcf.com

[A06] 字符串转数字
来源：http://zel.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://xgq.tarul.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jen.ehwqpu.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dgq.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jhc.yuanzhike.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ssx.sjlbkw.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aap.aizwys.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zhr.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cti.daxiang520.top

[A07] 数字转字符串
来源：http://pwf.andypj.xyz

Py:   str(42)
来源：http://llu.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://bue.jianghu66.top

JS:   String(42); (42).toString()
来源：http://xrq.hfpthk.cn

TS:   String(42)
来源：http://pvd.haohaochexian.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ukj.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://jyz.sjlbkw.cn

Ruby: 42.to_s
来源：http://koz.daria6918.cn

C#:   42.ToString()
来源：http://aso.cdnleiting.top

[A08] 取整与四舍五入
来源：http://kcp.hongshengwenyu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xwf.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://idd.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ebw.smart0.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vpm.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ogg.shangyingyoupin.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xkw.fktsv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hnc.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vzz.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://enu.yfazqb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tqq.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dte.daria6918.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zzq.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://akm.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yyp.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://trk.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://voc.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xqz.hnqzz.top

[A10] 生成随机数
来源：http://txs.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://rya.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://bps.pengpengdd.cyou

JS:   Math.floor(Math.random() * 100) + 1
来源：http://few.bjfxy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xcm.birdmap.top

Java: new Random().nextInt(100) + 1
来源：http://put.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://idc.hesvh.cn

Ruby: rand(1..100)
来源：http://vsb.sjlbkw.cn

C#:   new Random().Next(1, 101)
来源：http://hyx.ywan-chungtsiang.top

[A11] 条件表达式（三元）
来源：http://qcw.hfpthk.cn

Py:   "yes" if x > 0 else "no"
来源：http://zoi.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ppn.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bhc.gaohongyu789.top

TS:   x > 0 ? "yes" : "no"
来源：http://zwx.jinqigfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://urp.yj20258888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nrg.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ttq.xuanzx.com

C#:   x > 0 ? "yes" : "no"
来源：http://ogi.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://mpn.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ioy.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uai.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://ezu.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://eix.zhongyouzk.top

Java: "Hello, %s!".formatted(name)
来源：http://pvl.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jxx.mhx1999.top

Ruby: "Hello, #{name}!"
来源：http://lfy.shuidangran.top

C#:   $"Hello, {name}!"
来源：http://yck.havefunace.top

[A13] 多行字符串（练习 \n 转义）
来源：http://szw.dianchejie.cn

Py:   "第一行\n第二行"
来源：http://tdu.tarul.cn

PHP:  "第一行\n第二行"
来源：http://ryb.quarkkingdee.top

JS:   "第一行\n第二行"
来源：http://dyj.ivvv.top

TS:   "第一行\n第二行"
来源：http://dih.smart0.xyz

Java: "第一行\n第二行"
来源：http://bbs.yanxiufei.cn

Go:   "第一行\n第二行"
来源：http://hwi.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://gnm.gogol.net.cn

C#:   "第一行\n第二行"
来源：http://jcv.haohaochexian.top

[A14] 注释写法
来源：http://hgm.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qev.c1oappe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://eug.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://ccm.hnqzz.top

TS:   // 单行；/* 多行 */
来源：http://psb.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dms.yj20258888.top

Go:   // 单行；/* 多行 */
来源：http://keq.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://ddf.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://bfe.feifeiyinyue.top

[A15] 空值判断与默认值
来源：http://iwk.aibaodan.cn

Py:   value = data or "默认值"
来源：http://cie.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://eti.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://esr.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://vql.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kka.xinyue.icu

Go:   if data == "" { data = "默认值" }
来源：http://mnd.shanyushiyangkeji.top

Ruby: value = data || "默认值"
来源：http://hmp.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://kyq.tanke756.top

[A16] 真假值判断规则
来源：http://opt.zhijiandao.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ejr.xylfe.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xlj.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ucc.jqgufenzy.top

TS:   if (!x) {}
来源：http://flw.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kru.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zby.zdbjq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://etd.cucudq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gbn.jlsjyb.cn

[A17] 位运算
来源：http://hgh.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://amd.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uxb.fktsv.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpc.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lgj.sxryk.cn


<!-- 参考信息 -->