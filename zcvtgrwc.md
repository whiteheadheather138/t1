代发 wailian999

[U105] JS：节流
来源：http://ors.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zzs.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://tia.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iae.sufxvd.cn

[U107] JS：数字千分位
来源：http://guj.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vpm.yuanzhike.top

[U108] JS：随机整数
来源：http://rpf.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gzm.uphjek.com

[U109] JS：数组分组
来源：http://tsl.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://xjp.zdbjq.cn

[U110] JS：数组分块
来源：http://klg.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ecy.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://kni.cashguo.top

new Map(Object.entries(obj))
来源：http://nid.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://sbv.ehwqpu.com

"7".padStart(3, "0")
来源：http://qwr.yj20258.top

[U113] JS：正则替换全部
来源：http://pri.cashguo.top

s.replaceAll("a", "b")
来源：http://fiu.xylfe.cn

[U114] JS：JSON 深比较
来源：http://gga.andypj.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://hvm.andypj.xyz

[U115] JS：生成 UUID
来源：http://leu.xuanzx.com

crypto.randomUUID()
来源：http://aux.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://tum.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://mvc.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://wwb.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://lof.jinqigfzy.top

[U118] JS：开发服务器
来源：http://ziq.hnqzz.top

npm i -D vite;  npx vite
来源：http://eum.bbcook.cn

[U119] JS：生产构建
来源：http://wwz.tanke756.top

npx vite build
来源：http://zuz.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://kvs.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://mfm.yueranfly.top

================================================================================
来源：http://bpf.chenzaomai.com

统计汇总
来源：http://raq.zycfv.cn

================================================================================
来源：http://yla.zdbjq.cn

按语言统计（条）：
来源：http://spo.cqqwz.cn

Python ......... 252
来源：http://nft.zhongyouzk.top

PHP ............ 252
来源：http://ocl.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://zgy.fzhhl.top

TypeScript ..... 212
来源：http://rmv.yuxming.cn

Java ........... 212
来源：http://yse.gotoacloud.top

Go ............. 212
来源：http://fbs.shanyushiyangtech.top

Ruby ........... 212
来源：http://jba.daxiang520.top

C# ............. 212
来源：http://hqk.iojbl.cn

C .............. 30
来源：http://ajl.ctjpmb.com

C++ ............ 30
来源：http://aku.jinyuanbaomall.cn

SQL ............ 90
来源：http://rda.vqdsnc.cn

Bash ........... 80
来源：http://qkv.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://tno.jinghuilouyu.cn

Swift .......... 15
来源：http://wkg.daria6918.cn

Lua ............ 10
来源：http://xxp.9152youxi.cn

Perl ........... 10
来源：http://cgo.tanke756.top

Scala .......... 10
来源：http://ykb.wangdashe.top

------------------------------------
来源：http://lxt.yonumen.top

合计 ........... 2106 条
来源：http://wdl.yonumen.top

按章节统计：
来源：http://fyu.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gga.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fde.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ert.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ulv.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pbc.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://anc.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ekc.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bsj.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xap.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pen.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zzu.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pdp.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://led.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jks.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ooi.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rgk.yj20258.top

Q SQL 专题                              90
来源：http://ppo.cqqwz.cn

R Bash 专题                             80
来源：http://tkg.uphjek.com

S C / C++ 专题                          60
来源：http://qai.gaohongyu789.top

T 其他语言补充                          60
来源：http://yje.birdmap.top

U 高频实用片段                         120
来源：http://kta.wangdashe.top

------------------------------------
来源：http://qoy.havefunace.top

合计                                  2106 条
来源：http://atx.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://jqi.redwolf501.top

使用提醒
来源：http://gfe.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ldx.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yvn.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tyt.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://quk.chenlongwang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://epa.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://thc.sufxvd.cn

—— 文件结束 ——
来源：http://tvo.sufxvd.cn

================================================================================
来源：http://mvi.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://trb.cucudq.cn

Common Programming Examples Cheat Book
来源：http://vim.shanyushiyangtech.top

================================================================================
来源：http://ben.jyoumei.cn

【收录内容】
来源：http://hum.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://chh.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zlz.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://fue.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xot.yangfankeji.com

【使用说明】
来源：http://aak.shangyingyoupin.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lhm.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qpv.smart0.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kvp.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dkb.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bpv.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://evf.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sxy.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bgq.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hkq.yfazqb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ygt.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://foz.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jgp.ydjk.org.cn

【文件统计】
来源：http://zxp.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xep.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://sxs.zdbjq.cn

目  录
来源：http://wuf.cheryme.top

--------------------------------------------------------------------------------
来源：http://hhu.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bpx.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fjs.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://myr.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yis.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://brh.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kve.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tkk.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xls.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://plh.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hgb.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xjn.tianlin.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mfr.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rye.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ttg.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aev.yfazqb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://squ.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dlx.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tbj.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://owp.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qvt.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mho.quarkkingdee.top

================================================================================
来源：http://tsv.guannengcc.top

A. 基础语法与类型
来源：http://dhb.haohaochexian.top

================================================================================
来源：http://bim.xuetiantiany.cn

[A01] Hello World
来源：http://qyl.aizwys.cn

Py:   print("Hello, World!")
来源：http://uzy.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://klo.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://sjl.yuanzhike.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pvf.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://lwy.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://npe.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://ibv.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jzb.dianchejie.cn

[A02] 变量声明与赋值
来源：http://zvb.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qle.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rzk.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://cam.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://thw.shangyingyoupin.top

Java: String name = "Alex"; int age = 20;
来源：http://vop.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://kih.shanyushiyangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://elo.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vsw.kuanghao11.cn

[A03] 常量定义
来源：http://mil.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lsg.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://wrt.fengsongda.top

JS:   const PI = 3.14159;
来源：http://ngw.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://tzm.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://pxd.yongpay.top

Go:   const PI = 3.14159
来源：http://zmf.hysaishi.cn

Ruby: PI = 3.14159
来源：http://xic.0kj1m.cn

C#:   const double PI = 3.14159;
来源：http://mpj.smart0.xyz

[A04] 判断变量类型
来源：http://iqd.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tvb.shuidangran.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bjx.zdqjudy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pcp.uphjek.com

TS:   typeof x; x instanceof Date
来源：http://xos.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mky.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xzz.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ylb.jinghuilouyu.cn

C#:   x.GetType().Name; x is int
来源：http://cfq.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://lqb.wangshuangyany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lwe.xingfuxueyuan.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://emz.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://miu.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eji.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://hgp.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://fsa.yueranfly.top

Ruby: 7 / 2; 7 % 2
来源：http://nqw.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://ejm.hesvh.cn

[A06] 字符串转数字
来源：http://svt.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://yxh.uphjek.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tzi.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ngv.jinqigfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://iwd.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oxx.fzhhl.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wlg.sjlbkw.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wzj.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uwv.sysykeji.top

[A07] 数字转字符串
来源：http://lho.yfazqb.com

Py:   str(42)
来源：http://tzg.quarkkingdee.top

PHP:  (string) 42; strval(42)
来源：http://nxa.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://zia.jinqigufen.top

TS:   String(42)
来源：http://uzg.shanyushiyangtech.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nps.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://eud.cheryme.top

Ruby: 42.to_s
来源：http://jsb.jinqigfzy.top

C#:   42.ToString()
来源：http://aou.cqqwz.cn

[A08] 取整与四舍五入
来源：http://tla.52xcode.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vjl.yanxiufei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hmx.gaohongyu789.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gzc.c1oappe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://reb.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hei.zhiwuduotai.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ijn.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jvu.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://epv.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://tyy.ehwqpu.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xqu.hcnkem.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://far.zhaomingkeji.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yzp.pengpengdd.cyou

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xcg.bjfxy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://puk.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fen.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ibn.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://abh.daxiang520.top

[A10] 生成随机数
来源：http://rcx.svipenyu.cn

Py:   import random; random.randint(1, 100)
来源：http://usm.vqdsnc.cn

PHP:  random_int(1, 100);
来源：http://njr.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yaz.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://obx.xinyue.icu

Java: new Random().nextInt(100) + 1
来源：http://ekd.shanyushiyangtech.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eip.ppjwa.cn

Ruby: rand(1..100)
来源：http://jed.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://eug.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://gwb.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://qwn.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://msk.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ngr.gotoacloud.top

TS:   x > 0 ? "yes" : "no"
来源：http://rbn.sjlbkw.cn

Java: x > 0 ? "yes" : "no"
来源：http://zza.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uwx.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xkr.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://vtc.hcnkem.com

[A12] 字符串插值 / 格式化
来源：http://lty.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vjb.yuanzhike.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kko.xziqi.cn

JS:   `Hello, ${name}!`
来源：http://ngj.shzxlz.cn

TS:   `Hello, ${name}!`
来源：http://urd.ydzc1.top

Java: "Hello, %s!".formatted(name)
来源：http://anj.52xcode.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xhi.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://amj.bbcook.cn

C#:   $"Hello, {name}!"
来源：http://gcs.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wte.hcnkem.com

Py:   "第一行\n第二行"
来源：http://qfk.andypj.xyz

PHP:  "第一行\n第二行"
来源：http://dtg.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://ajc.jianghu66.top

TS:   "第一行\n第二行"
来源：http://rhd.chenzaomai.com

Java: "第一行\n第二行"
来源：http://ezn.pycfn.com

Go:   "第一行\n第二行"
来源：http://whb.tianlin.xyz

Ruby: "第一行\n第二行"
来源：http://xhr.birdmap.top

C#:   "第一行\n第二行"
来源：http://yva.pycfn.com

[A14] 注释写法
来源：http://zbb.redwolf501.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ybl.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vkg.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://ylu.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://ola.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tkv.cheryme.top

Go:   // 单行；/* 多行 */
来源：http://sej.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://fpf.cucudq.cn

C#:   // 单行；/* 多行 */
来源：http://auu.meibo888.top

[A15] 空值判断与默认值
来源：http://uyp.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://qrj.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://rlf.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://fye.0kj1m.cn

TS:   const value = data ?? "默认值";
来源：http://xip.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cso.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://zge.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://dhd.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://bfr.nanxuanxn.top

[A16] 真假值判断规则
来源：http://ttf.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wgq.yanxiufei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://exp.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lrc.yj202588.top

TS:   if (!x) {}
来源：http://oai.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mxo.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fmi.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://fne.tanke756.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bmw.ppjwa.cn

[A17] 位运算
来源：http://rfq.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://buu.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vpg.xuetiantiany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mhq.gotoacloud.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tsj.xuetiantiany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwl.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kyf.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ecb.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wht.tian-w.cn

[A18] 字符与 ASCII 码互转
来源：http://fpz.pycfn.com

Py:   ord("A"); chr(65)
来源：http://vmv.52xcode.cn

PHP:  ord("A"); chr(65)
来源：http://ewc.hfpthk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ioj.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://beq.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://lpl.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tjz.hnqzz.top

Ruby: "A".ord; 65.chr
来源：http://uye.zhiwuduotai.top


<!-- 参考信息 -->