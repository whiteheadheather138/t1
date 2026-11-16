代发 wailian999

[U99] JS：事件监听
来源：http://jmv.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://dfc.vehdjk.com

[U100] JS：DOM 查询
来源：http://byq.aizwys.cn

document.querySelector(".item")
来源：http://wyy.kuanghao11.cn

[U101] JS：classList 操作
来源：http://gfk.epnwcf.com

el.classList.toggle("active")
来源：http://rfc.epnwcf.com

[U102] JS：本地存储
来源：http://sos.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://rgj.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://bfo.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yya.mhx1999.top

[U104] JS：防抖
来源：http://fgg.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://muh.yonumen.top

[U105] JS：节流
来源：http://dfd.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://min.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://hry.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://svb.yfazqb.com

[U107] JS：数字千分位
来源：http://rvh.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jgc.zhijiandao.cn

[U108] JS：随机整数
来源：http://lps.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rvl.yuanzhike.top

[U109] JS：数组分组
来源：http://ecx.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://yug.hesvh.cn

[U110] JS：数组分块
来源：http://bpp.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mjt.meibo888.top

[U111] JS：对象转 Map
来源：http://wbu.sxryk.cn

new Map(Object.entries(obj))
来源：http://jta.cucudq.cn

[U112] JS：字符串补位
来源：http://fab.yueranfly.top

"7".padStart(3, "0")
来源：http://xjl.yj202588.top

[U113] JS：正则替换全部
来源：http://zyp.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://qth.sysykeji.top

[U114] JS：JSON 深比较
来源：http://mnm.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ptr.nwbrower.top

[U115] JS：生成 UUID
来源：http://hee.jqgfzy.top

crypto.randomUUID()
来源：http://vvp.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://pml.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://owe.jlsjyb.cn

[U117] JS：单元测试
来源：http://owc.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://hxn.zhoulong.xyz

[U118] JS：开发服务器
来源：http://rdo.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://ymi.316326.xyz

[U119] JS：生产构建
来源：http://bzj.hfpthk.cn

npx vite build
来源：http://amh.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://xif.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://xlx.jinyuanbaomall.cn

================================================================================
来源：http://sjl.mhx1999.top

统计汇总
来源：http://xtw.hnxiangtu.top

================================================================================
来源：http://lrf.hongshengwenyu.top

按语言统计（条）：
来源：http://zay.tarul.cn

Python ......... 252
来源：http://uoo.bbcook.cn

PHP ............ 252
来源：http://jdn.ctjpmb.com

JavaScript ..... 252
来源：http://yro.yueranfly.top

TypeScript ..... 212
来源：http://sik.xuetiantiany.cn

Java ........... 212
来源：http://gkw.jqgufenzy.top

Go ............. 212
来源：http://dil.aibaodan.cn

Ruby ........... 212
来源：http://wgp.wangshuangyany.cn

C# ............. 212
来源：http://bhn.zhoulong.xyz

C .............. 30
来源：http://tqb.daria6918.cn

C++ ............ 30
来源：http://pjk.birdmap.top

SQL ............ 90
来源：http://dvm.hfpthk.cn

Bash ........... 80
来源：http://qsq.hnxiangtu.top

Kotlin ......... 15
来源：http://gpu.andypj.xyz

Swift .......... 15
来源：http://ual.wangshuangyany.cn

Lua ............ 10
来源：http://jri.vehdjk.com

Perl ........... 10
来源：http://szm.guowangkeji.top

Scala .......... 10
来源：http://kko.xuetiantiany.cn

------------------------------------
来源：http://xjs.smart0.xyz

合计 ........... 2106 条
来源：http://glf.fktsv.cn

按章节统计：
来源：http://wje.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ctk.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vgf.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qee.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kok.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nwk.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pzs.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ldr.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wkl.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uky.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xkc.cheryme.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nxc.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fcw.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wpp.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hny.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hys.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hzv.cheryme.top

Q SQL 专题                              90
来源：http://joy.316326.xyz

R Bash 专题                             80
来源：http://atb.tianlin.xyz

S C / C++ 专题                          60
来源：http://ynb.cashguo.top

T 其他语言补充                          60
来源：http://ujt.kuanghao11.cn

U 高频实用片段                         120
来源：http://hlm.jqgfzy.top

------------------------------------
来源：http://rfk.jqgufenzy.top

合计                                  2106 条
来源：http://swn.sxryk.cn

--------------------------------------------------------------------------------
来源：http://zft.xinyue.icu

使用提醒
来源：http://ycy.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://pvs.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jzz.hfpthk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fzn.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eky.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kxu.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jub.mhx1999.top

—— 文件结束 ——
来源：http://uph.hysaishi.cn

================================================================================
来源：http://ord.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://pfb.sxryk.cn

Common Programming Examples Cheat Book
来源：http://qgq.hammf.cn

================================================================================
来源：http://mhz.vehdjk.com

【收录内容】
来源：http://lez.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ojd.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ges.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://pph.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://czw.meibo888.top

【使用说明】
来源：http://pon.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xpl.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ubd.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://msf.aibaodan.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://whx.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://dee.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uwb.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oxk.shangyingyoupin.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dzi.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cra.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hhd.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kxe.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zmq.fehbvm.com

【文件统计】
来源：http://xvc.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://caa.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://nvp.xziqi.cn

目  录
来源：http://yfm.tarul.cn

--------------------------------------------------------------------------------
来源：http://hjd.gotoacloud.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://otp.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bbi.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fsy.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wkr.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cpn.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mex.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://npo.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qvw.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mdh.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zfp.yuxming.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hlw.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://smc.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ouh.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qqb.ywan-chungtsiang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ldw.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://slk.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rrk.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ftu.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mwg.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tyt.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zkk.jqgfzy.top

================================================================================
来源：http://qih.hysaishi.cn

A. 基础语法与类型
来源：http://ana.jinghuilouyu.cn

================================================================================
来源：http://eic.svipenyu.cn

[A01] Hello World
来源：http://gfp.zhijiandao.cn

Py:   print("Hello, World!")
来源：http://erh.fengsongda.top

PHP:  echo "Hello, World!";
来源：http://ibk.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://wgd.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ket.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://hkg.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://csc.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://brf.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bfo.nanxinkj.top

[A02] 变量声明与赋值
来源：http://aec.xuetiantiany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vtp.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tgz.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://oia.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pob.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://jfa.yueranfly.top

Go:   name := "Alex"; age := 20
来源：http://tzp.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://wyz.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://yjk.zhengqikj.top

[A03] 常量定义
来源：http://xjx.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dnz.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://vhq.uphjek.com

JS:   const PI = 3.14159;
来源：http://qvm.52xcode.cn

TS:   const PI: number = 3.14159;
来源：http://ypf.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://lsj.xziqi.cn

Go:   const PI = 3.14159
来源：http://ral.bbcook.cn

Ruby: PI = 3.14159
来源：http://xqf.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://jwa.jqgufenzy.top

[A04] 判断变量类型
来源：http://obf.ppjwa.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tud.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wtn.quarkkingdee.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xgo.iojbl.cn

TS:   typeof x; x instanceof Date
来源：http://yvf.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://izz.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://opl.sysykeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gmi.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://xdy.xuanzx.com

[A05] 整数除法与取模
来源：http://dqs.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bzc.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nnl.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://orz.hfpthk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mzz.chenjidiqi.icu

Java: 7 / 2; 7 % 2
来源：http://mfb.tanke756.top

Go:   7 / 2; 7 % 2
来源：http://gag.iojbl.cn

Ruby: 7 / 2; 7 % 2
来源：http://akd.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://usu.redwolf501.top

[A06] 字符串转数字
来源：http://lnp.tanke756.top

Py:   int("42"); float("3.14")
来源：http://vcd.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zxh.ppjwa.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aej.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vfd.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nrl.yj20258888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ekr.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zrw.sysykeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tng.redwolf501.top

[A07] 数字转字符串
来源：http://oig.guowangkeji.top

Py:   str(42)
来源：http://dos.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://tns.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://qbg.ivvv.top

TS:   String(42)
来源：http://djj.yvedp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://myl.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://kau.ybcxt.top

Ruby: 42.to_s
来源：http://nyu.yongpay.top

C#:   42.ToString()
来源：http://stp.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://lug.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ihp.yvedp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://die.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://igd.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dvf.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://but.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://haz.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uhp.ivvv.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ujx.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://gcz.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mxf.zdqjudy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gsk.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fbk.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jkn.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bhp.daxiang520.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ulv.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ema.xuanzx.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ybm.tarul.cn

[A10] 生成随机数
来源：http://fxh.chenzaomai.com

Py:   import random; random.randint(1, 100)
来源：http://fyj.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://cww.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ced.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://apo.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://bhn.shzxlz.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tdk.tarul.cn

Ruby: rand(1..100)
来源：http://yyd.zycfv.cn

C#:   new Random().Next(1, 101)
来源：http://imk.andypj.xyz

[A11] 条件表达式（三元）
来源：http://pqx.cucudq.cn

Py:   "yes" if x > 0 else "no"
来源：http://urh.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ojg.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://nvj.andypj.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://hyb.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://hsi.fehbvm.com

Go:   // 无三元运算符，需用 if 语句
来源：http://dvv.chenzaomai.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ksa.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://dmc.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://fuj.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://umj.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cqy.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://dyq.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://npy.andypj.xyz

Java: "Hello, %s!".formatted(name)
来源：http://tqr.ctjpmb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ifg.shzxlz.cn

Ruby: "Hello, #{name}!"
来源：http://ukt.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://lat.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hqa.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://tzr.cqqwz.cn

PHP:  "第一行\n第二行"
来源：http://xfw.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://rzv.iojbl.cn

TS:   "第一行\n第二行"
来源：http://mfq.feifeiyinyue.top

Java: "第一行\n第二行"
来源：http://pnv.nwbrower.top

Go:   "第一行\n第二行"
来源：http://rax.xuetiantiany.cn

Ruby: "第一行\n第二行"
来源：http://ykm.tianlin.xyz

C#:   "第一行\n第二行"
来源：http://rjw.fanxiaobao.xyz

[A14] 注释写法
来源：http://omp.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xon.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wfz.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://bee.jyoumei.cn

TS:   // 单行；/* 多行 */
来源：http://iaq.yongpay.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://djy.guannengcc.top

Go:   // 单行；/* 多行 */
来源：http://btq.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://hci.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://qpc.shzxlz.cn

[A15] 空值判断与默认值
来源：http://scp.gogol.net.cn

Py:   value = data or "默认值"
来源：http://jzw.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://iya.jlsjyb.cn

JS:   const value = data ?? "默认值";
来源：http://oys.yj20258888.top

TS:   const value = data ?? "默认值";
来源：http://cry.guowangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lzy.guowangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://cfj.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://ssu.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://cca.jqgfzy.top

[A16] 真假值判断规则
来源：http://rhr.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ryq.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zbj.jinyuanbaomall.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cwx.xuetiantiany.cn

TS:   if (!x) {}
来源：http://bka.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xhz.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ich.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://xlr.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ogr.hcnkem.com

[A17] 位运算
来源：http://fcf.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yhg.jinqigufen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://knk.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zkx.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vtq.sysykeji.top


<!-- 参考信息 -->