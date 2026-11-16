代发 wailian999

[U105] JS：节流
来源：http://ajk.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cii.gaohongyu789.top

[U106] JS：日期格式化
来源：http://suf.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ebd.smart0.xyz

[U107] JS：数字千分位
来源：http://gdy.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vtv.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://jtu.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://olx.vehdjk.com

[U109] JS：数组分组
来源：http://izz.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://foj.shzxlz.cn

[U110] JS：数组分块
来源：http://zzx.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iqr.pycfn.com

[U111] JS：对象转 Map
来源：http://mff.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://ink.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://dbu.cheryme.top

"7".padStart(3, "0")
来源：http://nka.zdbjq.cn

[U113] JS：正则替换全部
来源：http://lch.hfpthk.cn

s.replaceAll("a", "b")
来源：http://ldj.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://esf.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ers.tarul.cn

[U115] JS：生成 UUID
来源：http://dwm.hnxiangtu.top

crypto.randomUUID()
来源：http://fqa.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://tmp.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://aiw.cashguo.top

[U117] JS：单元测试
来源：http://chy.yj202588.top

npm i -D vitest;  npx vitest
来源：http://vev.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://uat.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://veb.dianchejie.cn

[U119] JS：生产构建
来源：http://idi.zhengqikj.top

npx vite build
来源：http://dmg.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://mtz.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://fox.hcnkem.com

================================================================================
来源：http://xno.mhx1999.top

统计汇总
来源：http://odl.yueranfly.top

================================================================================
来源：http://rzd.pycfn.com

按语言统计（条）：
来源：http://xkw.chenlongwang.top

Python ......... 252
来源：http://asy.cashguo.top

PHP ............ 252
来源：http://rkz.yonumen.top

JavaScript ..... 252
来源：http://wug.zhijiandao.cn

TypeScript ..... 212
来源：http://npe.xinyue.icu

Java ........... 212
来源：http://cey.hywenlv.cn

Go ............. 212
来源：http://vza.fanxiaobao.xyz

Ruby ........... 212
来源：http://rvx.gogol.net.cn

C# ............. 212
来源：http://dco.shzxlz.cn

C .............. 30
来源：http://glg.cashguo.top

C++ ............ 30
来源：http://ain.wangshuangyany.cn

SQL ............ 90
来源：http://kih.jlsjyb.cn

Bash ........... 80
来源：http://ttm.zhijiandao.cn

Kotlin ......... 15
来源：http://jkh.ppjwa.cn

Swift .......... 15
来源：http://jpw.tian-w.cn

Lua ............ 10
来源：http://ieu.ydzc1.top

Perl ........... 10
来源：http://oac.zdqjudy.top

Scala .......... 10
来源：http://jzs.hesvh.cn

------------------------------------
来源：http://apl.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://cqu.feifeiyinyue.top

按章节统计：
来源：http://ske.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rqy.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lbp.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://spv.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ycf.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ydw.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://esl.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ogj.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gsr.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uqt.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://faz.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xjv.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wqr.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pvs.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lmu.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://whz.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ixe.wangdashe.top

Q SQL 专题                              90
来源：http://saj.dashuyun.cn

R Bash 专题                             80
来源：http://fcd.hnxiangtu.top

S C / C++ 专题                          60
来源：http://pyl.andypj.xyz

T 其他语言补充                          60
来源：http://oas.quarkkingdee.top

U 高频实用片段                         120
来源：http://qwi.fktsv.cn

------------------------------------
来源：http://zhe.sxryk.cn

合计                                  2106 条
来源：http://qlh.mhx1999.top

--------------------------------------------------------------------------------
来源：http://isr.birdmap.top

使用提醒
来源：http://ers.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://eqz.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hnf.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rvs.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ylf.iojbl.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iis.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ekm.chenzaomai.com

—— 文件结束 ——
来源：http://ddo.shanyushiyangkeji.top

================================================================================
来源：http://jzm.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://fix.hongshengwenyu.top

Common Programming Examples Cheat Book
来源：http://zqf.cdnleiting.top

================================================================================
来源：http://wwf.jqgufenzy.top

【收录内容】
来源：http://tzg.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ibq.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fun.cdnleiting.top

SQL · Bash · C · C++
来源：http://xem.zdbjq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qqs.yj20258888.top

【使用说明】
来源：http://eqt.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nnz.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qai.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vlh.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bue.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wtc.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zpv.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zim.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://juq.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bhf.tian-w.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lni.shanyushiyangtech.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dnk.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://inv.guannengcc.top

【文件统计】
来源：http://tic.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gnr.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://ome.andypj.xyz

目  录
来源：http://ybt.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://abj.xuanzx.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xcv.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tuv.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jov.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fxh.xziqi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jkh.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bpp.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cqj.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wih.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qaa.yvedp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bdy.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zrp.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rsy.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yop.yueranfly.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wjh.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vrz.hfpthk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cxh.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iac.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://peh.fehbvm.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pgg.tian-w.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ejj.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sqp.nwbrower.top

================================================================================
来源：http://zxo.shangyingyoupin.top

A. 基础语法与类型
来源：http://hyj.yj20258888.top

================================================================================
来源：http://oad.ybcxt.top

[A01] Hello World
来源：http://ggg.yj202588.top

Py:   print("Hello, World!")
来源：http://jac.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://npe.cashguo.top

JS:   console.log("Hello, World!");
来源：http://fsa.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://awm.redwolf501.top

Java: System.out.println("Hello, World!");
来源：http://imt.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://jer.ydzc1.top

Ruby: puts "Hello, World!"
来源：http://sjy.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rkc.nanxinkj.top

[A02] 变量声明与赋值
来源：http://ujt.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://het.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pwk.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://mbl.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ern.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://dqo.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://bym.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://zzq.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://guy.svipenyu.cn

[A03] 常量定义
来源：http://sao.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vai.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://arv.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://ayi.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://gtl.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://ewc.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://vbu.zhiwuduotai.top

Ruby: PI = 3.14159
来源：http://tgu.fehbvm.com

C#:   const double PI = 3.14159;
来源：http://xsl.zycfv.cn

[A04] 判断变量类型
来源：http://hph.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://thx.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mxz.cdnleiting.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bun.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://mjh.zhaomingkeji.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://brv.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://tzp.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bts.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://upx.ehwqpu.com

[A05] 整数除法与取模
来源：http://tau.sxryk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mvs.tanke756.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jzl.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lxv.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rcf.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://nuo.xuanzx.com

Go:   7 / 2; 7 % 2
来源：http://eab.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://wns.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://cor.fanxiaobao.xyz

[A06] 字符串转数字
来源：http://nnt.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://wks.cdnleiting.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yot.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jij.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://idk.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zgi.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zcc.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://rqt.bjfxy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nal.wangshuangyany.cn

[A07] 数字转字符串
来源：http://lak.gotoacloud.top

Py:   str(42)
来源：http://owd.fanxiaobao.xyz

PHP:  (string) 42; strval(42)
来源：http://gei.xinyue.icu

JS:   String(42); (42).toString()
来源：http://aqf.fehbvm.com

TS:   String(42)
来源：http://yco.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ubw.sweek.top

Go:   strconv.Itoa(42)
来源：http://ryj.xziqi.cn

Ruby: 42.to_s
来源：http://cwj.fengsongda.top

C#:   42.ToString()
来源：http://isl.yuxming.cn

[A08] 取整与四舍五入
来源：http://mlg.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jin.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wkf.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ozr.shanyushiyangtech.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dxv.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://afa.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lin.uphjek.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://aqf.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zfc.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://rfs.gotoacloud.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://npn.sweek.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qol.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zgk.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wjs.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xpq.aibaodan.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yef.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nmd.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yfd.gaohongyu789.top

[A10] 生成随机数
来源：http://edq.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://fxb.nanxinkj.top

PHP:  random_int(1, 100);
来源：http://tpq.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iks.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rga.zdqjudy.top

Java: new Random().nextInt(100) + 1
来源：http://znq.ctjpmb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yuy.shangyingyoupin.top

Ruby: rand(1..100)
来源：http://eac.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://swc.fehbvm.com

[A11] 条件表达式（三元）
来源：http://spr.redwolf501.top

Py:   "yes" if x > 0 else "no"
来源：http://nfi.redwolf501.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ifx.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mwr.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://zyv.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://vaa.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://btw.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qdv.gogol.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zkr.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://vyu.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://njz.svipenyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ush.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://xsk.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://hou.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://sfp.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bur.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://gcj.haohaochexian.top

C#:   $"Hello, {name}!"
来源：http://bly.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kbq.xuanzx.com

Py:   "第一行\n第二行"
来源：http://hxd.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://lcr.redwolf501.top

JS:   "第一行\n第二行"
来源：http://keo.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://clw.yonumen.top

Java: "第一行\n第二行"
来源：http://aoy.shzxlz.cn

Go:   "第一行\n第二行"
来源：http://woy.gogol.net.cn

Ruby: "第一行\n第二行"
来源：http://ung.tianlin.xyz

C#:   "第一行\n第二行"
来源：http://fnl.cheryme.top

[A14] 注释写法
来源：http://jrf.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qwn.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://hri.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://jpu.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://eba.yonumen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lwo.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://hzo.meibo888.top

Ruby: # 单行；=begin 多行 =end
来源：http://jma.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://mrb.cheryme.top

[A15] 空值判断与默认值
来源：http://pba.ydjk.org.cn

Py:   value = data or "默认值"
来源：http://dhw.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://vwt.yanxiufei.cn

JS:   const value = data ?? "默认值";
来源：http://awz.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://lmg.hywenlv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fjj.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://ccl.gotoacloud.top

Ruby: value = data || "默认值"
来源：http://trs.yongpay.top

C#:   var value = data ?? "默认值";
来源：http://ach.aizwys.cn

[A16] 真假值判断规则
来源：http://qmx.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tat.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://odz.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://omz.zdqjudy.top

TS:   if (!x) {}
来源：http://jzh.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kvk.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://igo.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://yrg.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tpc.vqdsnc.cn

[A17] 位运算
来源：http://igh.sjlbkw.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfu.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ucv.mhx1999.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dtc.yuanzhike.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hmh.havefunace.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjf.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tei.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mcq.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awb.tanke756.top

[A18] 字符与 ASCII 码互转
来源：http://pyo.xziqi.cn

Py:   ord("A"); chr(65)
来源：http://tpo.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://ldt.9152youxi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oml.gzhubu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sqa.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://nsv.hesvh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oqp.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://yeb.0kj1m.cn


<!-- 参考信息 -->