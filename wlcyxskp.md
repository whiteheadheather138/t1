代发 wailian999

[U101] JS：classList 操作
来源：http://uwp.ybcxt.top

el.classList.toggle("active")
来源：http://hfb.cucudq.cn

[U102] JS：本地存储
来源：http://bgc.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wwh.xuetiantiany.cn

[U103] JS：定时器
来源：http://nmt.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hty.guannengcc.top

[U104] JS：防抖
来源：http://ohj.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wvl.xuetiantiany.cn

[U105] JS：节流
来源：http://bjc.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dhh.sjlbkw.cn

[U106] JS：日期格式化
来源：http://mrd.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fbq.yonumen.top

[U107] JS：数字千分位
来源：http://gvt.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wps.hesvh.cn

[U108] JS：随机整数
来源：http://clf.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xku.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://vhg.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://biw.xziqi.cn

[U110] JS：数组分块
来源：http://hbb.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ogy.ctjpmb.com

[U111] JS：对象转 Map
来源：http://xhz.xuanzx.com

new Map(Object.entries(obj))
来源：http://uet.smart0.xyz

[U112] JS：字符串补位
来源：http://xxd.xylfe.cn

"7".padStart(3, "0")
来源：http://oju.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://coh.shzxlz.cn

s.replaceAll("a", "b")
来源：http://mgl.nwbrower.top

[U114] JS：JSON 深比较
来源：http://eic.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gxe.tanke756.top

[U115] JS：生成 UUID
来源：http://fyj.pengpengdd.cyou

crypto.randomUUID()
来源：http://mzw.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://xzs.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://coj.jiagoushi.top

[U117] JS：单元测试
来源：http://wtd.hnqzz.top

npm i -D vitest;  npx vitest
来源：http://rcc.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://pgy.yuanzhike.top

npm i -D vite;  npx vite
来源：http://gvp.cheryme.top

[U119] JS：生产构建
来源：http://ccn.ydjk.org.cn

npx vite build
来源：http://rzn.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://eze.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://ynz.andypj.xyz

================================================================================
来源：http://gya.shangyingyoupin.top

统计汇总
来源：http://ete.jinyuanbaomall.cn

================================================================================
来源：http://qii.shanyushiyangtech.top

按语言统计（条）：
来源：http://ckd.xziqi.cn

Python ......... 252
来源：http://tzl.hongshengwenyu.top

PHP ............ 252
来源：http://iwc.wangshuangyany.cn

JavaScript ..... 252
来源：http://eml.jinghuilouyu.cn

TypeScript ..... 212
来源：http://pbw.ydzc1.top

Java ........... 212
来源：http://ara.jianghu66.top

Go ............. 212
来源：http://tdm.dashuyun.cn

Ruby ........... 212
来源：http://gbo.gaohongyu789.top

C# ............. 212
来源：http://ywo.sjlbkw.cn

C .............. 30
来源：http://bqz.havefunace.top

C++ ............ 30
来源：http://tvs.hfpthk.cn

SQL ............ 90
来源：http://gkd.svipenyu.cn

Bash ........... 80
来源：http://tfs.vqdsnc.cn

Kotlin ......... 15
来源：http://gow.fzhhl.top

Swift .......... 15
来源：http://xgi.hcnkem.com

Lua ............ 10
来源：http://elf.vehdjk.com

Perl ........... 10
来源：http://iax.hammf.cn

Scala .......... 10
来源：http://wjs.jqgfzy.top

------------------------------------
来源：http://lid.cheryme.top

合计 ........... 2106 条
来源：http://idk.yj20258888.top

按章节统计：
来源：http://yob.xziqi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vvo.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kfs.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bnt.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ycy.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://brt.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fde.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iob.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tjr.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tkm.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xty.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mpj.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ykx.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sfq.svipenyu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zkm.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vpx.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tdp.aibaodan.cn

Q SQL 专题                              90
来源：http://hgn.ehwqpu.com

R Bash 专题                             80
来源：http://osp.hammf.cn

S C / C++ 专题                          60
来源：http://dxd.jqgufenzy.top

T 其他语言补充                          60
来源：http://tvp.nwbrower.top

U 高频实用片段                         120
来源：http://zjx.sufxvd.cn

------------------------------------
来源：http://cec.epnwcf.com

合计                                  2106 条
来源：http://rpb.tian-w.cn

--------------------------------------------------------------------------------
来源：http://buz.hammf.cn

使用提醒
来源：http://vqq.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://zkr.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://flv.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sqw.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mzd.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://piv.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cjs.gotoacloud.top

—— 文件结束 ——
来源：http://rev.guowangkeji.top

================================================================================
来源：http://fne.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://zyu.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://wpr.yvedp.cn

================================================================================
来源：http://mug.daria6918.cn

【收录内容】
来源：http://uke.hfpthk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://njq.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sib.zhixingplan.top

SQL · Bash · C · C++
来源：http://ozs.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ybw.jyoumei.cn

【使用说明】
来源：http://bnd.jyoumei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://czo.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hpv.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qfy.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zit.yangfankeji.com

Bash:  Shell         C:     C             C++:   C++
来源：http://fns.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jhu.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rbs.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fln.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hmn.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ypr.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kyl.c1oappe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qyy.xuetiantiany.cn

【文件统计】
来源：http://bzi.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qqd.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://tmg.cucudq.cn

目  录
来源：http://dws.daxiang520.top

--------------------------------------------------------------------------------
来源：http://chm.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://csf.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xmx.jinqigfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qcm.shanyushiyangtech.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hzu.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ysh.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xlc.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://obf.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tuu.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://btl.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://njh.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://akw.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kqm.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fcr.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cnb.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hhv.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://htj.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gys.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zuf.haohaochexian.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vvq.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oxg.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bpj.shanyushiyangkeji.top

================================================================================
来源：http://tis.daria6918.cn

A. 基础语法与类型
来源：http://mmz.shangyingyoupin.top

================================================================================
来源：http://gug.ppjwa.cn

[A01] Hello World
来源：http://noe.ydzc1.top

Py:   print("Hello, World!")
来源：http://fla.jqgufenzy.top

PHP:  echo "Hello, World!";
来源：http://sor.fehbvm.com

JS:   console.log("Hello, World!");
来源：http://wss.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://piv.zhijiandao.cn

Java: System.out.println("Hello, World!");
来源：http://qan.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://fqb.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://ucg.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xkp.316326.xyz

[A02] 变量声明与赋值
来源：http://dtk.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jlq.ppjwa.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qfw.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jso.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mcw.yj20258.top

Java: String name = "Alex"; int age = 20;
来源：http://jhy.fengsongda.top

Go:   name := "Alex"; age := 20
来源：http://gmx.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://quu.sufxvd.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hzo.jinghuilouyu.cn

[A03] 常量定义
来源：http://uit.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sey.guowangkeji.top

PHP:  const PI = 3.14159;
来源：http://nrb.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://vvs.zhiwuduotai.top

TS:   const PI: number = 3.14159;
来源：http://kac.yj20258.top

Java: static final double PI = 3.14159;
来源：http://qjo.yj20258.top

Go:   const PI = 3.14159
来源：http://rar.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://zvs.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://dfv.nanxinkj.top

[A04] 判断变量类型
来源：http://lff.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tfd.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ogd.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://avp.quarkkingdee.top

TS:   typeof x; x instanceof Date
来源：http://pfs.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dbo.yongpay.top

Go:   reflect.TypeOf(x).Name()
来源：http://rfr.xinyue.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://ozr.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://rye.zdbjq.cn

[A05] 整数除法与取模
来源：http://iaa.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jlc.jqgfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nyg.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pda.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kql.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://oys.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://wph.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://blm.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://dsf.sweek.top

[A06] 字符串转数字
来源：http://ntc.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://tig.xuanzx.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oui.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vcv.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://uiy.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nvc.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cib.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rxm.guannengcc.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mia.ppjwa.cn

[A07] 数字转字符串
来源：http://vrf.redwolf501.top

Py:   str(42)
来源：http://lsu.sufxvd.cn

PHP:  (string) 42; strval(42)
来源：http://vfy.yongpay.top

JS:   String(42); (42).toString()
来源：http://eat.sxryk.cn

TS:   String(42)
来源：http://elo.pengpengdd.cyou

Java: String.valueOf(42); Integer.toString(42)
来源：http://blv.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://qhr.ydjk.org.cn

Ruby: 42.to_s
来源：http://swk.fzhhl.top

C#:   42.ToString()
来源：http://rda.sysykeji.top

[A08] 取整与四舍五入
来源：http://lvx.hcnkem.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nbt.yuanzhike.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vkh.yuanzhike.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wdp.zhongyouzk.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hlp.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://krt.ctjpmb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://klg.xinyue.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://pvh.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oev.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://ump.vqdsnc.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://udb.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iul.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wze.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pbo.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://khj.epnwcf.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fpi.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gro.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ium.meibo888.top

[A10] 生成随机数
来源：http://hzr.yuanzhike.top

Py:   import random; random.randint(1, 100)
来源：http://iol.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://ffy.zhiwuduotai.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fuu.sxryk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cvc.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://oew.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hdu.zhijiandao.cn

Ruby: rand(1..100)
来源：http://hao.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://gne.birdmap.top

[A11] 条件表达式（三元）
来源：http://wvf.hesvh.cn

Py:   "yes" if x > 0 else "no"
来源：http://qof.dashuyun.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ybo.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oaa.sweek.top

TS:   x > 0 ? "yes" : "no"
来源：http://agv.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://ett.yueranfly.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tct.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://oul.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://afg.jqgufenzy.top

[A12] 字符串插值 / 格式化
来源：http://eys.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sma.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dvq.jinqigufen.top

JS:   `Hello, ${name}!`
来源：http://ehz.mhx1999.top

TS:   `Hello, ${name}!`
来源：http://qar.hnqzz.top

Java: "Hello, %s!".formatted(name)
来源：http://tck.xuetiantiany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://coi.gzhubu.top

Ruby: "Hello, #{name}!"
来源：http://dxf.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://ixm.guannengcc.top

[A13] 多行字符串（练习 \n 转义）
来源：http://eqm.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://bdm.nanxinkj.top

PHP:  "第一行\n第二行"
来源：http://dbw.tanke756.top

JS:   "第一行\n第二行"
来源：http://qiq.yj20258888.top

TS:   "第一行\n第二行"
来源：http://pwo.hysaishi.cn

Java: "第一行\n第二行"
来源：http://ryf.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://rsq.c1oappe.top

Ruby: "第一行\n第二行"
来源：http://ufq.jlsjyb.cn

C#:   "第一行\n第二行"
来源：http://giz.nanxuanxn.top

[A14] 注释写法
来源：http://xny.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://dcx.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ijh.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://dcu.zdbjq.cn

TS:   // 单行；/* 多行 */
来源：http://kvv.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ecu.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://xdb.hnxiangtu.top

Ruby: # 单行；=begin 多行 =end
来源：http://fmb.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://git.jianghu66.top

[A15] 空值判断与默认值
来源：http://afa.cheryme.top

Py:   value = data or "默认值"
来源：http://mdp.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://ozq.xylfe.cn

JS:   const value = data ?? "默认值";
来源：http://uua.tarul.cn

TS:   const value = data ?? "默认值";
来源：http://xjw.kuanghao11.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ntg.tianlin.xyz

Go:   if data == "" { data = "默认值" }
来源：http://osc.havefunace.top

Ruby: value = data || "默认值"
来源：http://ufr.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://ytl.hysaishi.cn

[A16] 真假值判断规则
来源：http://xmi.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nay.316326.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://msl.bbcook.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sck.chenzaomai.com

TS:   if (!x) {}
来源：http://ohk.hywenlv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fxl.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xrl.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zvo.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://peu.xuetiantiany.cn

[A17] 位运算
来源：http://mmo.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcp.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cor.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlh.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hbq.tanke756.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ggo.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zvv.xuetiantiany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eju.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://itb.sweek.top


<!-- 参考信息 -->