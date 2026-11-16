代发 wailian999

[U101] JS：classList 操作
来源：http://gkx.shangyingyoupin.top

el.classList.toggle("active")
来源：http://vqq.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://ckm.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ucf.yonumen.top

[U103] JS：定时器
来源：http://ufh.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qqz.daria6918.cn

[U104] JS：防抖
来源：http://xxs.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rqn.feifeiyinyue.top

[U105] JS：节流
来源：http://vog.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ptd.gogol.net.cn

[U106] JS：日期格式化
来源：http://esd.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gax.tian-w.cn

[U107] JS：数字千分位
来源：http://cee.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jgj.ctjpmb.com

[U108] JS：随机整数
来源：http://pmm.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dme.hammf.cn

[U109] JS：数组分组
来源：http://niz.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://wgn.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://idl.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kko.guowangkeji.top

[U111] JS：对象转 Map
来源：http://snw.birdmap.top

new Map(Object.entries(obj))
来源：http://kxw.xziqi.cn

[U112] JS：字符串补位
来源：http://iak.guowangkeji.top

"7".padStart(3, "0")
来源：http://esg.epnwcf.com

[U113] JS：正则替换全部
来源：http://jax.chenlongwang.top

s.replaceAll("a", "b")
来源：http://shf.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://zjs.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://otu.chenlongwang.top

[U115] JS：生成 UUID
来源：http://dqj.yueranfly.top

crypto.randomUUID()
来源：http://kaw.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://ynq.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://npk.zhengqikj.top

[U117] JS：单元测试
来源：http://lyb.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://klr.daxiang520.top

[U118] JS：开发服务器
来源：http://uxb.gogol.net.cn

npm i -D vite;  npx vite
来源：http://tgt.c1oappe.top

[U119] JS：生产构建
来源：http://lsx.zhijiandao.cn

npx vite build
来源：http://wkw.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://azb.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://ico.shzxlz.cn

================================================================================
来源：http://vvv.uphjek.com

统计汇总
来源：http://fvk.ctjpmb.com

================================================================================
来源：http://xhu.xinyue.icu

按语言统计（条）：
来源：http://joc.epnwcf.com

Python ......... 252
来源：http://paj.yuxming.cn

PHP ............ 252
来源：http://pln.cheryme.top

JavaScript ..... 252
来源：http://yfd.cashguo.top

TypeScript ..... 212
来源：http://dzy.guannengcc.top

Java ........... 212
来源：http://wyd.tarul.cn

Go ............. 212
来源：http://uif.snrcjt.cn

Ruby ........... 212
来源：http://sey.tarul.cn

C# ............. 212
来源：http://ygx.hongshengwenyu.top

C .............. 30
来源：http://xym.nanxinkj.top

C++ ............ 30
来源：http://lvj.fehbvm.com

SQL ............ 90
来源：http://tus.chenjidiqi.icu

Bash ........... 80
来源：http://goq.316326.xyz

Kotlin ......... 15
来源：http://uwz.sysykeji.top

Swift .......... 15
来源：http://tar.fanxiaobao.xyz

Lua ............ 10
来源：http://pbq.ehwqpu.com

Perl ........... 10
来源：http://vmm.fehbvm.com

Scala .......... 10
来源：http://xhk.shangyingyoupin.top

------------------------------------
来源：http://zza.wangshuangyany.cn

合计 ........... 2106 条
来源：http://mny.jinghuilouyu.cn

按章节统计：
来源：http://xry.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ewu.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tpl.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bte.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cww.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hax.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://giu.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://slw.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hay.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zsf.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ixq.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ivv.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://svr.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yzg.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qvz.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wjt.guowangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dto.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://mfo.yfazqb.com

R Bash 专题                             80
来源：http://eto.jlsjyb.cn

S C / C++ 专题                          60
来源：http://owq.yj20258888.top

T 其他语言补充                          60
来源：http://vaq.yanxiufei.cn

U 高频实用片段                         120
来源：http://jxn.vqdsnc.cn

------------------------------------
来源：http://qoj.52xcode.cn

合计                                  2106 条
来源：http://wox.hesvh.cn

--------------------------------------------------------------------------------
来源：http://euy.andypj.xyz

使用提醒
来源：http://ugw.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://pny.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kpx.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://svb.wangshuangyany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qnm.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rzq.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vjw.hnxiangtu.top

—— 文件结束 ——
来源：http://kst.shzxlz.cn

================================================================================
来源：http://jbd.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://rco.epnwcf.com

Common Programming Examples Cheat Book
来源：http://fgv.xinyue.icu

================================================================================
来源：http://hiw.nanxuanxn.top

【收录内容】
来源：http://end.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tdp.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kxf.quarkkingdee.top

SQL · Bash · C · C++
来源：http://hbf.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://anf.9152youxi.cn

【使用说明】
来源：http://nqo.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ocs.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wjy.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://heq.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wkd.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hcx.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ptn.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fny.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gul.jqgufenzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://njd.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wmd.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://brw.cucudq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jcr.shangyingyoupin.top

【文件统计】
来源：http://mpj.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rhv.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://kqo.tianlin.xyz

目  录
来源：http://djs.tarul.cn

--------------------------------------------------------------------------------
来源：http://dcm.yuanzhike.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bpg.yuxming.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dhb.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bve.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gst.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zee.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pqh.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mwd.fktsv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nnn.bbcook.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tef.meibo888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eiw.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lif.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zrc.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fvi.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://phc.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wpy.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zan.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ane.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://qcw.pycfn.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rxh.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dvh.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://enm.cucudq.cn

================================================================================
来源：http://llx.cheryme.top

A. 基础语法与类型
来源：http://mcd.smart0.xyz

================================================================================
来源：http://gwj.feifeiyinyue.top

[A01] Hello World
来源：http://peh.nwbrower.top

Py:   print("Hello, World!")
来源：http://zlf.hfpthk.cn

PHP:  echo "Hello, World!";
来源：http://bzo.cheryme.top

JS:   console.log("Hello, World!");
来源：http://cck.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oxh.52xcode.cn

Java: System.out.println("Hello, World!");
来源：http://alp.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://nqm.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://ehb.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://psr.zhengqikj.top

[A02] 变量声明与赋值
来源：http://dbu.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mnl.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cet.yj20258888.top

JS:   let name = "Alex"; const age = 20;
来源：http://clr.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://prm.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://fos.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://ovc.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://iqi.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bka.zhixingplan.top

[A03] 常量定义
来源：http://pgf.yvedp.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iup.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://mki.aizwys.cn

JS:   const PI = 3.14159;
来源：http://xcs.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://clm.meibo888.top

Java: static final double PI = 3.14159;
来源：http://eix.tianlin.xyz

Go:   const PI = 3.14159
来源：http://pqf.hysaishi.cn

Ruby: PI = 3.14159
来源：http://jsr.ivvv.top

C#:   const double PI = 3.14159;
来源：http://hio.tianlin.xyz

[A04] 判断变量类型
来源：http://ntz.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jyf.xuetiantiany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://izu.ppjwa.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fwb.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://pbe.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://alc.meibo888.top

Go:   reflect.TypeOf(x).Name()
来源：http://dcq.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yqq.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://sea.aibaodan.cn

[A05] 整数除法与取模
来源：http://oyk.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://snl.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ohe.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vlr.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hhr.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://zch.nanxuanxn.top

Go:   7 / 2; 7 % 2
来源：http://mam.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://ppe.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://hfa.hfpthk.cn

[A06] 字符串转数字
来源：http://yqv.cheryme.top

Py:   int("42"); float("3.14")
来源：http://tho.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rdr.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://crb.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://txg.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kpd.zhaomingkeji.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mrd.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gat.aizwys.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hsb.gzhubu.top

[A07] 数字转字符串
来源：http://ltb.xziqi.cn

Py:   str(42)
来源：http://ezr.zdbjq.cn

PHP:  (string) 42; strval(42)
来源：http://qsq.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://ogq.yuxming.cn

TS:   String(42)
来源：http://soq.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ncx.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://lcs.aizwys.cn

Ruby: 42.to_s
来源：http://xrh.aizwys.cn

C#:   42.ToString()
来源：http://axq.dashuyun.cn

[A08] 取整与四舍五入
来源：http://apo.52xcode.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ngs.jianghu66.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xdv.tarul.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uwa.yfazqb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kza.wangdashe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://egy.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ryl.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vla.0kj1m.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://edd.birdmap.top

[A09] 绝对值与最大最小值
来源：http://zfj.shuidangran.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ysh.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bqc.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://shw.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hqd.jinyuanbaomall.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mob.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yje.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ctv.nwbrower.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vpd.gaohongyu789.top

[A10] 生成随机数
来源：http://ykw.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://plc.jyoumei.cn

PHP:  random_int(1, 100);
来源：http://quc.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pvk.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jbc.cheryme.top

Java: new Random().nextInt(100) + 1
来源：http://ule.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ygw.yueranfly.top

Ruby: rand(1..100)
来源：http://wpb.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://vnq.zhaomingkeji.xyz

[A11] 条件表达式（三元）
来源：http://zlg.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://zbn.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bgd.jianghu66.top

JS:   x > 0 ? "yes" : "no"
来源：http://upg.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://azd.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://bjh.zhijiandao.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bzx.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://klr.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://rlq.fktsv.cn

[A12] 字符串插值 / 格式化
来源：http://fah.yongpay.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rsc.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tfd.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://jqs.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://bqj.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://yfg.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jey.jinqigfzy.top

Ruby: "Hello, #{name}!"
来源：http://rnc.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://hbl.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://ueu.hammf.cn

Py:   "第一行\n第二行"
来源：http://tai.shuidangran.top

PHP:  "第一行\n第二行"
来源：http://uua.epnwcf.com

JS:   "第一行\n第二行"
来源：http://zfc.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://hub.shangyingyoupin.top

Java: "第一行\n第二行"
来源：http://xgv.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://mwx.redwolf501.top

Ruby: "第一行\n第二行"
来源：http://fdh.shuidangran.top

C#:   "第一行\n第二行"
来源：http://yvp.jlsjyb.cn

[A14] 注释写法
来源：http://gyb.daria6918.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xue.wangdashe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ozp.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://upz.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://spx.fzhhl.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dfw.quarkkingdee.top

Go:   // 单行；/* 多行 */
来源：http://wdx.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://cjl.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://yus.yj20258888.top

[A15] 空值判断与默认值
来源：http://vxh.mhx1999.top

Py:   value = data or "默认值"
来源：http://qew.haohaochexian.top

PHP:  $value = $data ?? "默认值";
来源：http://vbb.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://roi.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://acv.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nko.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://tby.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://zok.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://rzo.kuanghao11.cn

[A16] 真假值判断规则
来源：http://sux.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ljd.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hus.hywenlv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://afh.tianlin.xyz

TS:   if (!x) {}
来源：http://jyu.jiagoushi.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fwb.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hxk.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://pzb.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sqy.quarkkingdee.top

[A17] 位运算
来源：http://jrn.jinqigufen.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ecd.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ahi.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://leq.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kqf.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jox.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bob.ctjpmb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nsh.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nbb.vqdsnc.cn


<!-- 参考信息 -->