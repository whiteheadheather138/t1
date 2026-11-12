代发 wailian999

[U105] JS：节流
来源：http://ieh.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gqr.gaohongyu789.top

[U106] JS：日期格式化
来源：http://bhy.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fhf.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://wdl.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lxh.yuanzhike.top

[U108] JS：随机整数
来源：http://oub.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jcr.jiagoushi.top

[U109] JS：数组分组
来源：http://dqg.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://sfb.quarkkingdee.top

[U110] JS：数组分块
来源：http://bam.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xuu.ydzc1.top

[U111] JS：对象转 Map
来源：http://afm.yongpay.top

new Map(Object.entries(obj))
来源：http://qkg.shuidangran.top

[U112] JS：字符串补位
来源：http://fji.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://kwb.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://qmn.bjfxy.top

s.replaceAll("a", "b")
来源：http://tyv.yfazqb.com

[U114] JS：JSON 深比较
来源：http://qmb.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gua.ybcxt.top

[U115] JS：生成 UUID
来源：http://nwt.cucudq.cn

crypto.randomUUID()
来源：http://sby.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://zpl.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://teu.sysykeji.top

[U117] JS：单元测试
来源：http://uax.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://mur.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://yxw.cqqwz.cn

npm i -D vite;  npx vite
来源：http://qsw.zhoulong.xyz

[U119] JS：生产构建
来源：http://ped.shuidangran.top

npx vite build
来源：http://xiw.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://isi.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://qyw.cdnleiting.top

================================================================================
来源：http://ifb.smart0.xyz

统计汇总
来源：http://gko.guannengcc.top

================================================================================
来源：http://ofo.c1oappe.top

按语言统计（条）：
来源：http://zby.xziqi.cn

Python ......... 252
来源：http://otq.yj20258888.top

PHP ............ 252
来源：http://rcq.hnxiangtu.top

JavaScript ..... 252
来源：http://uvu.ehwqpu.com

TypeScript ..... 212
来源：http://xef.zdqjudy.top

Java ........... 212
来源：http://fao.hcnkem.com

Go ............. 212
来源：http://uhk.jqgfzy.top

Ruby ........... 212
来源：http://hhh.hongshengwenyu.top

C# ............. 212
来源：http://aqo.gzhubu.top

C .............. 30
来源：http://wwf.jqgufenzy.top

C++ ............ 30
来源：http://xod.ywan-chungtsiang.top

SQL ............ 90
来源：http://yei.hnqzz.top

Bash ........... 80
来源：http://nmf.ppjwa.cn

Kotlin ......... 15
来源：http://tij.haohaochexian.top

Swift .......... 15
来源：http://vvs.yueranfly.top

Lua ............ 10
来源：http://ccd.yonumen.top

Perl ........... 10
来源：http://urr.zdbjq.cn

Scala .......... 10
来源：http://nll.xuetiantiany.cn

------------------------------------
来源：http://rzp.gaohongyu789.top

合计 ........... 2106 条
来源：http://tby.hcnkem.com

按章节统计：
来源：http://hcw.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kig.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gmw.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ntf.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eyn.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rks.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bch.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cyc.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fuv.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lsa.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cmh.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iwg.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kui.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jit.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rpx.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fho.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oki.9152youxi.cn

Q SQL 专题                              90
来源：http://cmt.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://ulq.yangfankeji.com

S C / C++ 专题                          60
来源：http://hds.ybcxt.top

T 其他语言补充                          60
来源：http://tpn.uphjek.com

U 高频实用片段                         120
来源：http://ltm.aibaodan.cn

------------------------------------
来源：http://goz.shanyushiyangkeji.top

合计                                  2106 条
来源：http://bsx.hesvh.cn

--------------------------------------------------------------------------------
来源：http://tth.tarul.cn

使用提醒
来源：http://xrz.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://jmx.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oaz.uphjek.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aja.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ktd.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ecq.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ijr.shanyushiyangtech.top

—— 文件结束 ——
来源：http://zxc.yvedp.cn

================================================================================
来源：http://ahg.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://alp.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://jny.jqgufenzy.top

================================================================================
来源：http://fkk.daxiang520.top

【收录内容】
来源：http://qin.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yiu.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lwe.0kj1m.cn

SQL · Bash · C · C++
来源：http://ekk.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dxb.ybcxt.top

【使用说明】
来源：http://eua.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xza.xuetiantiany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nre.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xwk.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://imx.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fzk.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qpx.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://loo.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jtv.yj20258888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pqc.fehbvm.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ipr.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xvo.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gsz.yuanzhike.top

【文件统计】
来源：http://rem.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ick.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://fop.fzhhl.top

目  录
来源：http://pkq.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://qky.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vqo.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iup.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kvj.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uwr.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xfy.zhiwuduotai.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://flm.chenzaomai.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wkx.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qdt.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wwn.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yxq.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://one.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bdt.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kkl.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zfy.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://crp.zhijiandao.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dac.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tqk.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://idw.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vzc.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ztv.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://njv.jiagoushi.top

================================================================================
来源：http://aaj.yanxiufei.cn

A. 基础语法与类型
来源：http://hvs.xziqi.cn

================================================================================
来源：http://iox.shangyingyoupin.top

[A01] Hello World
来源：http://ahl.wangdashe.top

Py:   print("Hello, World!")
来源：http://syv.cheryme.top

PHP:  echo "Hello, World!";
来源：http://tbk.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://etg.wangdashe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zng.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://nas.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://rim.zhongyouzk.top

Ruby: puts "Hello, World!"
来源：http://cdv.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zci.aizwys.cn

[A02] 变量声明与赋值
来源：http://fdz.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wjp.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pwm.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gfe.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bgb.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://zkm.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://owj.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://bsp.fzhhl.top

C#:   string name = "Alex"; int age = 20;
来源：http://rsw.haohaochexian.top

[A03] 常量定义
来源：http://ajf.zhiwuduotai.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pyi.chenlongwang.top

PHP:  const PI = 3.14159;
来源：http://twm.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://xju.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://zvf.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://sud.ydzc1.top

Go:   const PI = 3.14159
来源：http://tyg.cheryme.top

Ruby: PI = 3.14159
来源：http://qmp.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://cxe.sufxvd.cn

[A04] 判断变量类型
来源：http://gwb.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xka.52xcode.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yxb.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ixn.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://ezx.uphjek.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vhs.316326.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://orn.andypj.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ehc.yj20258888.top

C#:   x.GetType().Name; x is int
来源：http://khi.ehwqpu.com

[A05] 整数除法与取模
来源：http://eop.zdbjq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bpr.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://mtm.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bbb.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://axd.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://plf.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://kbt.mhx1999.top

Ruby: 7 / 2; 7 % 2
来源：http://nhu.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://dgs.smart0.xyz

[A06] 字符串转数字
来源：http://ozc.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://oag.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://btz.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wqv.sufxvd.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qns.cashguo.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jqh.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vsu.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gbx.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ekh.zhiwuduotai.top

[A07] 数字转字符串
来源：http://dkp.sufxvd.cn

Py:   str(42)
来源：http://qxu.wangshuangyany.cn

PHP:  (string) 42; strval(42)
来源：http://txu.ivvv.top

JS:   String(42); (42).toString()
来源：http://akz.feifeiyinyue.top

TS:   String(42)
来源：http://qdh.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qxn.yvedp.cn

Go:   strconv.Itoa(42)
来源：http://qad.ppjwa.cn

Ruby: 42.to_s
来源：http://dhn.yfazqb.com

C#:   42.ToString()
来源：http://xbk.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://ncq.jianghu66.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ncr.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://llf.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tvj.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mjo.cucudq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://klt.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://odj.hongshengwenyu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tiu.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://low.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://lcv.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qjf.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://svd.ybcxt.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xfp.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tie.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://epm.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ejg.chenlongwang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xlk.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ros.yuxming.cn

[A10] 生成随机数
来源：http://wlb.pycfn.com

Py:   import random; random.randint(1, 100)
来源：http://zcd.feifeiyinyue.top

PHP:  random_int(1, 100);
来源：http://yto.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pkd.cashguo.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hne.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://pns.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://joq.yanxiufei.cn

Ruby: rand(1..100)
来源：http://ges.xingfuxueyuan.xyz

C#:   new Random().Next(1, 101)
来源：http://dko.ydzc1.top

[A11] 条件表达式（三元）
来源：http://xfd.yongpay.top

Py:   "yes" if x > 0 else "no"
来源：http://okj.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rot.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://lts.yuxming.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iev.zycfv.cn

Java: x > 0 ? "yes" : "no"
来源：http://tlo.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ubu.epnwcf.com

Ruby: x > 0 ? "yes" : "no"
来源：http://oiw.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eky.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://phd.yj202588.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rkr.shanyushiyangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sqc.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://jrt.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://miq.fktsv.cn

Java: "Hello, %s!".formatted(name)
来源：http://bos.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wnl.jqgfzy.top

Ruby: "Hello, #{name}!"
来源：http://twx.guannengcc.top

C#:   $"Hello, {name}!"
来源：http://zic.0kj1m.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://icu.tarul.cn

Py:   "第一行\n第二行"
来源：http://egh.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://pbw.yj20258888.top

JS:   "第一行\n第二行"
来源：http://jrb.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://aly.sjlbkw.cn

Java: "第一行\n第二行"
来源：http://vtd.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://itx.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://czg.redwolf501.top

C#:   "第一行\n第二行"
来源：http://bjq.xingfuxueyuan.xyz

[A14] 注释写法
来源：http://cop.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nzw.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tsx.pycfn.com

JS:   // 单行；/* 多行 */
来源：http://mgm.chenjidiqi.icu

TS:   // 单行；/* 多行 */
来源：http://qwz.zdqjudy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bur.xuetiantiany.cn

Go:   // 单行；/* 多行 */
来源：http://xij.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rzw.jinqigfzy.top

C#:   // 单行；/* 多行 */
来源：http://ung.jyoumei.cn

[A15] 空值判断与默认值
来源：http://ksv.hnxiangtu.top

Py:   value = data or "默认值"
来源：http://omj.zhixingplan.top

PHP:  $value = $data ?? "默认值";
来源：http://tnw.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://qun.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://zfh.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://exm.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://oea.hnqzz.top

Ruby: value = data || "默认值"
来源：http://mkv.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://epc.bjfxy.top

[A16] 真假值判断规则
来源：http://bwu.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ify.ctjpmb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://huz.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sfb.bjfxy.top

TS:   if (!x) {}
来源：http://snw.havefunace.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gwj.xingfuxueyuan.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wpv.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rge.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dlx.yj202588.top

[A17] 位运算
来源：http://jbt.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zdb.daxiang520.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mby.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jgt.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ysk.sufxvd.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cms.yuxming.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yuk.hysaishi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gja.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulf.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://lkx.ydjk.org.cn

Py:   ord("A"); chr(65)
来源：http://ods.havefunace.top

PHP:  ord("A"); chr(65)
来源：http://gzs.ybcxt.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eiz.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xms.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://aht.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yxh.quarkkingdee.top

Ruby: "A".ord; 65.chr
来源：http://zwi.iojbl.cn


<!-- 参考信息 -->