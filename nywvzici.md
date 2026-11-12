代发 wailian999

[U103] JS：定时器
来源：http://yip.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gbn.cdnleiting.top

[U104] JS：防抖
来源：http://own.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgk.nwbrower.top

[U105] JS：节流
来源：http://hal.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ujw.vqdsnc.cn

[U106] JS：日期格式化
来源：http://nub.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zff.fktsv.cn

[U107] JS：数字千分位
来源：http://phu.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pyl.yonumen.top

[U108] JS：随机整数
来源：http://hje.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zjb.jinqigfzy.top

[U109] JS：数组分组
来源：http://xji.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://xyu.andypj.xyz

[U110] JS：数组分块
来源：http://amr.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sfs.fzhhl.top

[U111] JS：对象转 Map
来源：http://you.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://wry.0kj1m.cn

[U112] JS：字符串补位
来源：http://fpw.aibaodan.cn

"7".padStart(3, "0")
来源：http://mtf.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://nhj.yuxming.cn

s.replaceAll("a", "b")
来源：http://toj.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://pcs.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qei.vehdjk.com

[U115] JS：生成 UUID
来源：http://dvx.uphjek.com

crypto.randomUUID()
来源：http://pqc.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://cmk.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://fdd.xziqi.cn

[U117] JS：单元测试
来源：http://irx.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://sgg.shuidangran.top

[U118] JS：开发服务器
来源：http://cft.jianghu66.top

npm i -D vite;  npx vite
来源：http://fkq.gotoacloud.top

[U119] JS：生产构建
来源：http://ati.svipenyu.cn

npx vite build
来源：http://xuo.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://vdy.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://ocy.ywan-chungtsiang.top

================================================================================
来源：http://ifk.zhengqikj.top

统计汇总
来源：http://fnm.birdmap.top

================================================================================
来源：http://ucq.yanxiufei.cn

按语言统计（条）：
来源：http://tcg.tianlin.xyz

Python ......... 252
来源：http://ixa.tian-w.cn

PHP ............ 252
来源：http://lnh.vqdsnc.cn

JavaScript ..... 252
来源：http://dzz.hfpthk.cn

TypeScript ..... 212
来源：http://myq.guannengcc.top

Java ........... 212
来源：http://iwp.yueranfly.top

Go ............. 212
来源：http://bmz.fktsv.cn

Ruby ........... 212
来源：http://lkc.epnwcf.com

C# ............. 212
来源：http://mtj.svipenyu.cn

C .............. 30
来源：http://xxp.hfpthk.cn

C++ ............ 30
来源：http://jel.epnwcf.com

SQL ............ 90
来源：http://kaz.quarkkingdee.top

Bash ........... 80
来源：http://fad.pycfn.com

Kotlin ......... 15
来源：http://azt.aizwys.cn

Swift .......... 15
来源：http://rzr.fktsv.cn

Lua ............ 10
来源：http://alx.jinghuilouyu.cn

Perl ........... 10
来源：http://lmj.bjfxy.top

Scala .......... 10
来源：http://caa.epnwcf.com

------------------------------------
来源：http://tfc.nwbrower.top

合计 ........... 2106 条
来源：http://vcu.jlsjyb.cn

按章节统计：
来源：http://jgd.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gge.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tks.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://txb.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mkd.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dzn.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gzu.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qoy.cdnleiting.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qzy.fktsv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lsy.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zsu.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://czp.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://agd.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hsc.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aiy.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xzc.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lmw.jqgfzy.top

Q SQL 专题                              90
来源：http://yeb.xinyue.icu

R Bash 专题                             80
来源：http://ggn.hywenlv.cn

S C / C++ 专题                          60
来源：http://ilk.316326.xyz

T 其他语言补充                          60
来源：http://xws.hfpthk.cn

U 高频实用片段                         120
来源：http://ihv.kuanghao11.cn

------------------------------------
来源：http://fqq.ybcxt.top

合计                                  2106 条
来源：http://ypl.fzhhl.top

--------------------------------------------------------------------------------
来源：http://aaz.zhongyouzk.top

使用提醒
来源：http://oam.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://ykx.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zme.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yyg.shangyingyoupin.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mpq.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rhu.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xac.dianchejie.cn

—— 文件结束 ——
来源：http://lbh.jiagoushi.top

================================================================================
来源：http://jny.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://niv.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://msu.hesvh.cn

================================================================================
来源：http://sll.hfpthk.cn

【收录内容】
来源：http://vbb.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jgr.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xve.svipenyu.cn

SQL · Bash · C · C++
来源：http://fvh.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nci.daria6918.cn

【使用说明】
来源：http://idp.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://paq.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cba.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qxq.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xbc.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gbd.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ttu.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xsh.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://noe.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://reb.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://upr.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pdb.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://crc.shanyushiyangkeji.top

【文件统计】
来源：http://rgs.gaohongyu789.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://huz.gzhubu.top

--------------------------------------------------------------------------------
来源：http://zbb.jqgufenzy.top

目  录
来源：http://gci.316326.xyz

--------------------------------------------------------------------------------
来源：http://tdp.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://drw.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gfo.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lsx.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pqr.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qia.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yyq.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yfy.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jvt.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://scn.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ruw.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fwq.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iuu.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://axu.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ulg.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gsd.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jyl.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://igo.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tss.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vva.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://map.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ylq.hywenlv.cn

================================================================================
来源：http://fji.vehdjk.com

A. 基础语法与类型
来源：http://qua.shanyushiyangkeji.top

================================================================================
来源：http://buf.jinqigufen.top

[A01] Hello World
来源：http://omf.birdmap.top

Py:   print("Hello, World!")
来源：http://yiq.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://rco.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://uhc.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://daf.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://nfq.aibaodan.cn

Go:   fmt.Println("Hello, World!")
来源：http://plg.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://qls.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wgi.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://gsw.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lhc.xingfuxueyuan.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://wdm.yueranfly.top

JS:   let name = "Alex"; const age = 20;
来源：http://vbz.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bny.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://kto.hammf.cn

Go:   name := "Alex"; age := 20
来源：http://hsz.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://ajf.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://bzg.jyoumei.cn

[A03] 常量定义
来源：http://dag.hywenlv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gtd.yj20258888.top

PHP:  const PI = 3.14159;
来源：http://vpj.wangdashe.top

JS:   const PI = 3.14159;
来源：http://cau.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://jig.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://ody.gogol.net.cn

Go:   const PI = 3.14159
来源：http://ukz.xylfe.cn

Ruby: PI = 3.14159
来源：http://ffv.jinqigfzy.top

C#:   const double PI = 3.14159;
来源：http://zlk.meibo888.top

[A04] 判断变量类型
来源：http://ofi.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ttq.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dbr.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xld.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://kus.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://joh.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://ujp.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://kqe.c1oappe.top

C#:   x.GetType().Name; x is int
来源：http://jfw.yuxming.cn

[A05] 整数除法与取模
来源：http://nxk.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pkn.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gst.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hfa.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xcw.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://lrr.jinyuanbaomall.cn

Go:   7 / 2; 7 % 2
来源：http://kwq.ivvv.top

Ruby: 7 / 2; 7 % 2
来源：http://rij.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://ckp.tian-w.cn

[A06] 字符串转数字
来源：http://cwc.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://sqw.daria6918.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kyr.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zrv.nanxuanxn.top

TS:   parseInt("42", 10); Number("42")
来源：http://rie.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nhh.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pei.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://byq.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vzr.9152youxi.cn

[A07] 数字转字符串
来源：http://kki.aizwys.cn

Py:   str(42)
来源：http://qpn.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://std.tanke756.top

JS:   String(42); (42).toString()
来源：http://qve.kuanghao11.cn

TS:   String(42)
来源：http://sbv.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vpp.ydzc1.top

Go:   strconv.Itoa(42)
来源：http://ttx.vehdjk.com

Ruby: 42.to_s
来源：http://rhy.quarkkingdee.top

C#:   42.ToString()
来源：http://zxd.vehdjk.com

[A08] 取整与四舍五入
来源：http://ips.pengpengdd.cyou

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sqn.bjfxy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://djj.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wbw.uphjek.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fyr.jyoumei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nut.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mqs.pycfn.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://yuf.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pll.ehwqpu.com

[A09] 绝对值与最大最小值
来源：http://tdm.hnxiangtu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fkp.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hax.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kqj.fehbvm.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fci.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bdi.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fzs.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yuf.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ilb.zhaomingkeji.xyz

[A10] 生成随机数
来源：http://jid.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://fgo.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://cvq.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ryz.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zfc.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://ysx.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://otw.zycfv.cn

Ruby: rand(1..100)
来源：http://syp.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://lnl.yj20258888.top

[A11] 条件表达式（三元）
来源：http://anf.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://xxv.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://muz.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://mut.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://tvg.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://sxw.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zdi.ehwqpu.com

Ruby: x > 0 ? "yes" : "no"
来源：http://czm.316326.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://pcf.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://vvg.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ozw.yj20258888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xte.zhengqikj.top

JS:   `Hello, ${name}!`
来源：http://odw.xingfuxueyuan.xyz

TS:   `Hello, ${name}!`
来源：http://nxs.dashuyun.cn

Java: "Hello, %s!".formatted(name)
来源：http://lof.mhx1999.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dnz.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://kta.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://ddw.cucudq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jpd.yangfankeji.com

Py:   "第一行\n第二行"
来源：http://xsn.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://dpt.ivvv.top

JS:   "第一行\n第二行"
来源：http://vgr.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://muv.svipenyu.cn

Java: "第一行\n第二行"
来源：http://rwj.yangfankeji.com

Go:   "第一行\n第二行"
来源：http://rfd.meibo888.top

Ruby: "第一行\n第二行"
来源：http://tgc.aizwys.cn

C#:   "第一行\n第二行"
来源：http://jsg.fktsv.cn

[A14] 注释写法
来源：http://eyj.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://soo.gzhubu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pxx.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://rcp.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://wyl.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://weo.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://yrf.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://sgd.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://zit.yangfankeji.com

[A15] 空值判断与默认值
来源：http://vmz.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://lza.jyoumei.cn

PHP:  $value = $data ?? "默认值";
来源：http://jga.svipenyu.cn

JS:   const value = data ?? "默认值";
来源：http://oxm.birdmap.top

TS:   const value = data ?? "默认值";
来源：http://lyf.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ddd.fktsv.cn

Go:   if data == "" { data = "默认值" }
来源：http://fsn.guannengcc.top

Ruby: value = data || "默认值"
来源：http://jkc.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://kjt.tarul.cn

[A16] 真假值判断规则
来源：http://gis.yueranfly.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://omt.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bze.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dkn.hnqzz.top

TS:   if (!x) {}
来源：http://une.316326.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://can.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cgb.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://wtj.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zma.andypj.xyz

[A17] 位运算
来源：http://apn.jqgufenzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rfg.jinqigfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ryj.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmn.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zjg.jianghu66.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgu.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yvg.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bsu.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdy.wangdashe.top

[A18] 字符与 ASCII 码互转
来源：http://ytp.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://oen.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://pxa.snrcjt.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vvl.vehdjk.com


<!-- 参考信息 -->