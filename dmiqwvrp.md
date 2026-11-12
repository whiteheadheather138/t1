代发 wailian999

[U105] JS：节流
来源：http://vzo.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vls.mhx1999.top

[U106] JS：日期格式化
来源：http://ibc.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hxt.yvedp.cn

[U107] JS：数字千分位
来源：http://rpx.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gid.sysykeji.top

[U108] JS：随机整数
来源：http://ahd.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bql.tianlin.xyz

[U109] JS：数组分组
来源：http://dbw.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://kmv.sxryk.cn

[U110] JS：数组分块
来源：http://oge.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gxr.yonumen.top

[U111] JS：对象转 Map
来源：http://dxf.gotoacloud.top

new Map(Object.entries(obj))
来源：http://uwc.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://bqi.hcnkem.com

"7".padStart(3, "0")
来源：http://acx.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://qay.vehdjk.com

s.replaceAll("a", "b")
来源：http://kao.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://lgr.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://isp.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://jjm.jinqigufen.top

crypto.randomUUID()
来源：http://gmp.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://yrd.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://iev.yangfankeji.com

[U117] JS：单元测试
来源：http://oeu.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://dss.pycfn.com

[U118] JS：开发服务器
来源：http://rph.yangfankeji.com

npm i -D vite;  npx vite
来源：http://tqj.yonumen.top

[U119] JS：生产构建
来源：http://koe.ivvv.top

npx vite build
来源：http://xuq.jlsjyb.cn

[U120] JS：读取环境变量（Vite）
来源：http://fbf.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://ucm.chenzaomai.com

================================================================================
来源：http://ywg.epnwcf.com

统计汇总
来源：http://kcb.uphjek.com

================================================================================
来源：http://rvl.ehwqpu.com

按语言统计（条）：
来源：http://oez.nwbrower.top

Python ......... 252
来源：http://kxn.gzhubu.top

PHP ............ 252
来源：http://jjx.dashuyun.cn

JavaScript ..... 252
来源：http://rhk.ybcxt.top

TypeScript ..... 212
来源：http://lyq.nanxinkj.top

Java ........... 212
来源：http://flk.jinyuanbaomall.cn

Go ............. 212
来源：http://wzc.jqgfzy.top

Ruby ........... 212
来源：http://tuy.yj202588.top

C# ............. 212
来源：http://eim.nanxuanxn.top

C .............. 30
来源：http://voo.zdbjq.cn

C++ ............ 30
来源：http://hkp.xziqi.cn

SQL ............ 90
来源：http://hlm.tianlin.xyz

Bash ........... 80
来源：http://oyy.chenjidiqi.icu

Kotlin ......... 15
来源：http://udd.xylfe.cn

Swift .......... 15
来源：http://tkt.yangfankeji.com

Lua ............ 10
来源：http://plu.zhongyouzk.top

Perl ........... 10
来源：http://hak.pengpengdd.cyou

Scala .......... 10
来源：http://fje.cheryme.top

------------------------------------
来源：http://hol.chenlongwang.top

合计 ........... 2106 条
来源：http://nxn.yvedp.cn

按章节统计：
来源：http://nem.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ecb.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vas.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yxq.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wli.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ohw.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://epk.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dyd.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qia.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vjc.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yox.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ige.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jmm.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://edy.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yra.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hvy.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wmv.zhongyouzk.top

Q SQL 专题                              90
来源：http://nza.hammf.cn

R Bash 专题                             80
来源：http://cgw.zdbjq.cn

S C / C++ 专题                          60
来源：http://iez.guowangkeji.top

T 其他语言补充                          60
来源：http://fll.smart0.xyz

U 高频实用片段                         120
来源：http://ykx.9152youxi.cn

------------------------------------
来源：http://ugi.yueranfly.top

合计                                  2106 条
来源：http://nxr.birdmap.top

--------------------------------------------------------------------------------
来源：http://lkz.chenzaomai.com

使用提醒
来源：http://prz.cashguo.top

--------------------------------------------------------------------------------
来源：http://axc.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pqf.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ozr.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bsx.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bcd.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dst.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://vtw.quarkkingdee.top

================================================================================
来源：http://tgf.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://vph.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://fds.ehwqpu.com

================================================================================
来源：http://jhv.snrcjt.cn

【收录内容】
来源：http://tob.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fav.zhengqikj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ufd.fktsv.cn

SQL · Bash · C · C++
来源：http://mjb.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://klp.vqdsnc.cn

【使用说明】
来源：http://bhn.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gge.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ehm.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ydb.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dvn.nwbrower.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bct.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lli.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tsc.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cve.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pqy.zhaomingkeji.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ico.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cyk.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://urz.cqqwz.cn

【文件统计】
来源：http://vdh.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://clt.yvedp.cn

--------------------------------------------------------------------------------
来源：http://pqb.xuetiantiany.cn

目  录
来源：http://xbk.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://czc.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uxs.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ytp.shuidangran.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hse.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sjr.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ood.cheryme.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fjm.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://chf.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zco.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gsw.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://amd.zdqjudy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://soy.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mqr.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://puk.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kun.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dlc.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lqp.fehbvm.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tht.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wge.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cyd.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zjh.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gog.ydjk.org.cn

================================================================================
来源：http://xkw.snrcjt.cn

A. 基础语法与类型
来源：http://fxx.yongpay.top

================================================================================
来源：http://shz.shanyushiyangtech.top

[A01] Hello World
来源：http://jqe.yangfankeji.com

Py:   print("Hello, World!")
来源：http://boj.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://dsx.chenjidiqi.icu

JS:   console.log("Hello, World!");
来源：http://tgl.xinyue.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dfu.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://vja.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://fmb.cashguo.top

Ruby: puts "Hello, World!"
来源：http://trs.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ugg.fehbvm.com

[A02] 变量声明与赋值
来源：http://egg.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vkk.ybcxt.top

PHP:  $name = "Alex"; $age = 20;
来源：http://txv.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://akr.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://abf.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://qpf.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://ofe.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://ldw.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://bmh.dianchejie.cn

[A03] 常量定义
来源：http://ozb.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nkk.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://ckh.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://jok.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://ngp.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://ykd.redwolf501.top

Go:   const PI = 3.14159
来源：http://hwt.hnqzz.top

Ruby: PI = 3.14159
来源：http://vdl.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://hrz.ydjk.org.cn

[A04] 判断变量类型
来源：http://rqp.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://kzo.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ozg.ywan-chungtsiang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jfg.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://hnj.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pvp.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://cdl.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kxz.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://hhp.ctjpmb.com

[A05] 整数除法与取模
来源：http://wxz.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cul.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xhu.ctjpmb.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eap.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rlk.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://dxw.yuxming.cn

Go:   7 / 2; 7 % 2
来源：http://nnr.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://tyi.sjlbkw.cn

C#:   7 / 2; 7 % 2
来源：http://eje.vehdjk.com

[A06] 字符串转数字
来源：http://mku.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://qmx.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://omd.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bfu.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vdc.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qqq.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xwg.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wcw.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lgg.shangyingyoupin.top

[A07] 数字转字符串
来源：http://nqx.zdbjq.cn

Py:   str(42)
来源：http://zly.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://sqn.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://cfs.yangfankeji.com

TS:   String(42)
来源：http://ben.yangfankeji.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ywn.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://qno.yongpay.top

Ruby: 42.to_s
来源：http://sbz.tarul.cn

C#:   42.ToString()
来源：http://ltu.sysykeji.top

[A08] 取整与四舍五入
来源：http://fwu.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cit.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kub.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xeo.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oxl.sysykeji.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://idz.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bwv.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lmq.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zhy.fanxiaobao.xyz

[A09] 绝对值与最大最小值
来源：http://vnq.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://neo.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sua.iojbl.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fnx.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kkx.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wnp.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fef.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tyu.smart0.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://swh.daria6918.cn

[A10] 生成随机数
来源：http://ygz.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://vjj.ydzc1.top

PHP:  random_int(1, 100);
来源：http://fxv.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kgs.jyoumei.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cnj.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://trf.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mwl.ywan-chungtsiang.top

Ruby: rand(1..100)
来源：http://kkz.daxiang520.top

C#:   new Random().Next(1, 101)
来源：http://yos.bbcook.cn

[A11] 条件表达式（三元）
来源：http://qkk.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://ebi.bbcook.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://naw.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dni.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rpk.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://gma.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pht.sysykeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ucx.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ckp.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://khf.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eza.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lso.meibo888.top

JS:   `Hello, ${name}!`
来源：http://gne.ivvv.top

TS:   `Hello, ${name}!`
来源：http://qhy.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://jlq.yj20258.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dti.hfpthk.cn

Ruby: "Hello, #{name}!"
来源：http://hlf.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://qux.nanxuanxn.top

[A13] 多行字符串（练习 \n 转义）
来源：http://htb.dashuyun.cn

Py:   "第一行\n第二行"
来源：http://qsr.nanxuanxn.top

PHP:  "第一行\n第二行"
来源：http://xoc.daxiang520.top

JS:   "第一行\n第二行"
来源：http://nhv.fengsongda.top

TS:   "第一行\n第二行"
来源：http://cof.hnxiangtu.top

Java: "第一行\n第二行"
来源：http://qep.yfazqb.com

Go:   "第一行\n第二行"
来源：http://yta.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://khc.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://cye.jyoumei.cn

[A14] 注释写法
来源：http://rvi.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://oan.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lis.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://ukf.fanxiaobao.xyz

TS:   // 单行；/* 多行 */
来源：http://nui.andypj.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yaz.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://kkm.jqgfzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://vkl.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://tqg.52xcode.cn

[A15] 空值判断与默认值
来源：http://cjb.sweek.top

Py:   value = data or "默认值"
来源：http://sfx.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://myu.chenlongwang.top

JS:   const value = data ?? "默认值";
来源：http://wkb.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://teb.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rbt.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://oil.cdnleiting.top

Ruby: value = data || "默认值"
来源：http://iru.havefunace.top

C#:   var value = data ?? "默认值";
来源：http://aqb.shangyingyoupin.top

[A16] 真假值判断规则
来源：http://tob.shanyushiyangtech.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tef.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vpw.yanxiufei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://drx.tianlin.xyz

TS:   if (!x) {}
来源：http://eki.hongshengwenyu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ehk.pengpengdd.cyou

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dej.sjlbkw.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xxw.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cxl.shuidangran.top

[A17] 位运算
来源：http://iyp.sysykeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjf.tarul.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nog.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vuh.shuidangran.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bjz.gogol.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ewc.gogol.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mje.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jbj.cucudq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxj.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://hjk.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://jai.guowangkeji.top

PHP:  ord("A"); chr(65)
来源：http://awp.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wsv.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wuy.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://xjh.chenlongwang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ukx.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://bew.havefunace.top


<!-- 参考信息 -->