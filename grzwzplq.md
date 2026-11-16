代发 wailian999

[U103] JS：定时器
来源：http://tzb.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tut.snrcjt.cn

[U104] JS：防抖
来源：http://ssx.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxs.xylfe.cn

[U105] JS：节流
来源：http://bqs.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://egr.xylfe.cn

[U106] JS：日期格式化
来源：http://apv.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qfm.nwbrower.top

[U107] JS：数字千分位
来源：http://pas.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gps.ctjpmb.com

[U108] JS：随机整数
来源：http://evv.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mfu.fengsongda.top

[U109] JS：数组分组
来源：http://veu.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://ycy.fktsv.cn

[U110] JS：数组分块
来源：http://qji.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rkn.cashguo.top

[U111] JS：对象转 Map
来源：http://ncq.cqqwz.cn

new Map(Object.entries(obj))
来源：http://swi.yj202588.top

[U112] JS：字符串补位
来源：http://zza.zdqjudy.top

"7".padStart(3, "0")
来源：http://gab.yongpay.top

[U113] JS：正则替换全部
来源：http://dtb.hywenlv.cn

s.replaceAll("a", "b")
来源：http://hho.yueranfly.top

[U114] JS：JSON 深比较
来源：http://xdv.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gfe.yongpay.top

[U115] JS：生成 UUID
来源：http://gmu.wangdashe.top

crypto.randomUUID()
来源：http://uag.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://bst.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://pwl.gogol.net.cn

[U117] JS：单元测试
来源：http://psy.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://nqx.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://iwo.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://gqq.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://rjd.haohaochexian.top

npx vite build
来源：http://vir.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://kxd.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://gmi.aizwys.cn

================================================================================
来源：http://vxf.316326.xyz

统计汇总
来源：http://vxo.cashguo.top

================================================================================
来源：http://dnu.tian-w.cn

按语言统计（条）：
来源：http://car.feifeiyinyue.top

Python ......... 252
来源：http://rrj.aibaodan.cn

PHP ............ 252
来源：http://lug.fktsv.cn

JavaScript ..... 252
来源：http://jol.jinqigufen.top

TypeScript ..... 212
来源：http://bcs.zdbjq.cn

Java ........... 212
来源：http://igd.yongpay.top

Go ............. 212
来源：http://ymg.jqgfzy.top

Ruby ........... 212
来源：http://tvu.c1oappe.top

C# ............. 212
来源：http://tnl.fanxiaobao.xyz

C .............. 30
来源：http://rgc.jinqigfzy.top

C++ ............ 30
来源：http://rfs.zdbjq.cn

SQL ............ 90
来源：http://mml.guowangkeji.top

Bash ........... 80
来源：http://svu.pycfn.com

Kotlin ......... 15
来源：http://fnv.jianghu66.top

Swift .......... 15
来源：http://qer.zdqjudy.top

Lua ............ 10
来源：http://ygr.yongpay.top

Perl ........... 10
来源：http://onj.fktsv.cn

Scala .......... 10
来源：http://fos.cashguo.top

------------------------------------
来源：http://xrp.sweek.top

合计 ........... 2106 条
来源：http://nns.zycfv.cn

按章节统计：
来源：http://bzs.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iyw.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dnp.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gsj.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ghn.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kze.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gis.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ltz.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hwz.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://upo.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ymu.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uze.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mcy.ppjwa.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xdw.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://msu.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yqx.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aya.smart0.xyz

Q SQL 专题                              90
来源：http://izc.chenjidiqi.icu

R Bash 专题                             80
来源：http://kbp.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://uam.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://upo.hongshengwenyu.top

U 高频实用片段                         120
来源：http://ezq.pengpengdd.cyou

------------------------------------
来源：http://kda.xuanzx.com

合计                                  2106 条
来源：http://yuw.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://nkm.zhixingplan.top

使用提醒
来源：http://jkw.yj20258.top

--------------------------------------------------------------------------------
来源：http://rta.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ljk.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tja.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bjx.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ofh.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qjk.yangfankeji.com

—— 文件结束 ——
来源：http://jli.yuxming.cn

================================================================================
来源：http://iwv.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://jtl.yj20258.top

Common Programming Examples Cheat Book
来源：http://vrg.sysykeji.top

================================================================================
来源：http://gow.aibaodan.cn

【收录内容】
来源：http://ado.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://viw.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wgu.dianchejie.cn

SQL · Bash · C · C++
来源：http://efv.ppjwa.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lkr.smart0.xyz

【使用说明】
来源：http://iby.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wyy.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gvf.smart0.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xjy.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vpv.zhengqikj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ocq.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fku.feifeiyinyue.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://teq.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vbf.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tez.ydjk.org.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://idp.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kkl.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hkv.hfpthk.cn

【文件统计】
来源：http://sbf.jinghuilouyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gme.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://otk.hongshengwenyu.top

目  录
来源：http://uzx.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://pgh.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://izj.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://juj.andypj.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jnh.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dsy.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mro.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://egv.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ynv.smart0.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kxa.ivvv.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://afm.ydzc1.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://slg.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fnc.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ibg.smart0.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://azm.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://acp.sxryk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yyu.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aec.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xhv.yuanzhike.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://whq.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zwr.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ciq.ydzc1.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uii.andypj.xyz

================================================================================
来源：http://jdc.snrcjt.cn

A. 基础语法与类型
来源：http://kzr.jlsjyb.cn

================================================================================
来源：http://vve.vehdjk.com

[A01] Hello World
来源：http://gdi.redwolf501.top

Py:   print("Hello, World!")
来源：http://ajg.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://zhh.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://lkq.birdmap.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pbh.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://hew.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://pye.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://tja.ivvv.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lot.cdnleiting.top

[A02] 变量声明与赋值
来源：http://ond.tianlin.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ffg.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://eih.chenzaomai.com

JS:   let name = "Alex"; const age = 20;
来源：http://ggd.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://clu.cucudq.cn

Java: String name = "Alex"; int age = 20;
来源：http://efr.yangfankeji.com

Go:   name := "Alex"; age := 20
来源：http://ykf.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://jaj.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://acz.ivvv.top

[A03] 常量定义
来源：http://ymn.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gzy.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://btm.yj20258.top

JS:   const PI = 3.14159;
来源：http://lty.zdbjq.cn

TS:   const PI: number = 3.14159;
来源：http://vkh.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://fqe.fengsongda.top

Go:   const PI = 3.14159
来源：http://sgl.tian-w.cn

Ruby: PI = 3.14159
来源：http://lqv.hywenlv.cn

C#:   const double PI = 3.14159;
来源：http://oaj.jqgfzy.top

[A04] 判断变量类型
来源：http://saw.sysykeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dyq.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ccs.ivvv.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gik.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://fuk.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tnp.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://yvs.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://zya.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://nej.ydzc1.top

[A05] 整数除法与取模
来源：http://ajo.hongshengwenyu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://flb.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xtl.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpy.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dwc.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://mvx.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://qvh.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://mjo.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://xky.shangyingyoupin.top

[A06] 字符串转数字
来源：http://dzr.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://swi.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uem.ydzc1.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://spr.svipenyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://eze.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zeq.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nzx.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ikj.cqqwz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://txg.aibaodan.cn

[A07] 数字转字符串
来源：http://qdi.fengsongda.top

Py:   str(42)
来源：http://wwo.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://qcn.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://bjr.cashguo.top

TS:   String(42)
来源：http://qgr.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rst.yj20258888.top

Go:   strconv.Itoa(42)
来源：http://pbb.yuxming.cn

Ruby: 42.to_s
来源：http://fvs.chenzaomai.com

C#:   42.ToString()
来源：http://rlt.bbcook.cn

[A08] 取整与四舍五入
来源：http://wse.nanxinkj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fup.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yqb.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ykg.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wsm.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fki.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jsu.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mnc.hnqzz.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hmf.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://cvk.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iue.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hrc.c1oappe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qua.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rcd.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dxn.chenjidiqi.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ipk.yj20258.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aeb.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dyz.chenlongwang.top

[A10] 生成随机数
来源：http://yig.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://vio.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://gyo.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vsv.ctjpmb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dse.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://aeq.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uer.hnxiangtu.top

Ruby: rand(1..100)
来源：http://opi.xziqi.cn

C#:   new Random().Next(1, 101)
来源：http://kne.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://chn.yuanzhike.top

Py:   "yes" if x > 0 else "no"
来源：http://zon.jqgfzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://aoe.shanyushiyangtech.top

JS:   x > 0 ? "yes" : "no"
来源：http://wgp.gogol.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fgc.ivvv.top

Java: x > 0 ? "yes" : "no"
来源：http://pmu.yuanzhike.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dwu.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wai.cashguo.top

C#:   x > 0 ? "yes" : "no"
来源：http://kgi.nwbrower.top

[A12] 字符串插值 / 格式化
来源：http://umj.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nrq.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zzw.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://ean.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://zyo.epnwcf.com

Java: "Hello, %s!".formatted(name)
来源：http://rho.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mhz.hesvh.cn

Ruby: "Hello, #{name}!"
来源：http://qix.ydzc1.top

C#:   $"Hello, {name}!"
来源：http://bby.tianlin.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://blf.chenjidiqi.icu

Py:   "第一行\n第二行"
来源：http://gcy.yj20258.top

PHP:  "第一行\n第二行"
来源：http://rwz.birdmap.top

JS:   "第一行\n第二行"
来源：http://mto.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://asl.fehbvm.com

Java: "第一行\n第二行"
来源：http://efr.c1oappe.top

Go:   "第一行\n第二行"
来源：http://idb.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://jbe.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://hmd.sweek.top

[A14] 注释写法
来源：http://tve.cheryme.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ppv.ppjwa.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pea.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://jlg.vqdsnc.cn

TS:   // 单行；/* 多行 */
来源：http://enc.zhaomingkeji.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vql.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://vbz.cucudq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ysg.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://wyk.316326.xyz

[A15] 空值判断与默认值
来源：http://apj.svipenyu.cn

Py:   value = data or "默认值"
来源：http://bza.yj20258.top

PHP:  $value = $data ?? "默认值";
来源：http://puc.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://hgs.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://zzz.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gaw.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://tur.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://cui.zhijiandao.cn

C#:   var value = data ?? "默认值";
来源：http://pnl.sxryk.cn

[A16] 真假值判断规则
来源：http://ffr.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cuh.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xyx.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jan.epnwcf.com

TS:   if (!x) {}
来源：http://ozf.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pez.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dkg.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://fbw.havefunace.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yvt.tarul.cn

[A17] 位运算
来源：http://wdc.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yot.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lsu.yuanzhike.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ojg.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zdu.fzhhl.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://toa.zdqjudy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://srl.shanyushiyangtech.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sfm.ydzc1.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wgg.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://wxj.birdmap.top

Py:   ord("A"); chr(65)
来源：http://vqf.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://obc.jqgfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dhd.xylfe.cn


<!-- 参考信息 -->