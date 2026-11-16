代发 wailian999

[U101] JS：classList 操作
来源：http://atc.hesvh.cn

el.classList.toggle("active")
来源：http://qml.guowangkeji.top

[U102] JS：本地存储
来源：http://nfl.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://whk.hnqzz.top

[U103] JS：定时器
来源：http://ajw.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lqd.fanxiaobao.xyz

[U104] JS：防抖
来源：http://jdx.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mfe.nwbrower.top

[U105] JS：节流
来源：http://drl.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pvs.guowangkeji.top

[U106] JS：日期格式化
来源：http://nqj.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gnf.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://nvs.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fwx.jianghu66.top

[U108] JS：随机整数
来源：http://aec.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jbi.yuanzhike.top

[U109] JS：数组分组
来源：http://vwu.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://kvu.sjlbkw.cn

[U110] JS：数组分块
来源：http://rtb.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hfv.yonumen.top

[U111] JS：对象转 Map
来源：http://dqf.hcnkem.com

new Map(Object.entries(obj))
来源：http://wcv.zhongyouzk.top

[U112] JS：字符串补位
来源：http://cob.zdbjq.cn

"7".padStart(3, "0")
来源：http://qna.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://mcm.chenzaomai.com

s.replaceAll("a", "b")
来源：http://hcj.sysykeji.top

[U114] JS：JSON 深比较
来源：http://iiq.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eqm.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://ezh.epnwcf.com

crypto.randomUUID()
来源：http://cdx.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://qen.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://yqr.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://gul.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://nsd.kuanghao11.cn

[U118] JS：开发服务器
来源：http://guw.tianlin.xyz

npm i -D vite;  npx vite
来源：http://fyy.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://dio.vehdjk.com

npx vite build
来源：http://mfd.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://hxe.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://chu.xingfuxueyuan.xyz

================================================================================
来源：http://sep.yangfankeji.com

统计汇总
来源：http://ygv.zhijiandao.cn

================================================================================
来源：http://zdy.sysykeji.top

按语言统计（条）：
来源：http://umg.pengpengdd.cyou

Python ......... 252
来源：http://gmk.shanyushiyangkeji.top

PHP ............ 252
来源：http://xpz.0kj1m.cn

JavaScript ..... 252
来源：http://xgd.jiagoushi.top

TypeScript ..... 212
来源：http://tbb.zhongyouzk.top

Java ........... 212
来源：http://apw.bbcook.cn

Go ............. 212
来源：http://eul.zdbjq.cn

Ruby ........... 212
来源：http://zea.hywenlv.cn

C# ............. 212
来源：http://bde.birdmap.top

C .............. 30
来源：http://ajd.hywenlv.cn

C++ ............ 30
来源：http://ipp.kuanghao11.cn

SQL ............ 90
来源：http://fdt.jinyuanbaomall.cn

Bash ........... 80
来源：http://neh.316326.xyz

Kotlin ......... 15
来源：http://iys.yanxiufei.cn

Swift .......... 15
来源：http://ggu.gotoacloud.top

Lua ............ 10
来源：http://cut.nanxinkj.top

Perl ........... 10
来源：http://tqo.zhaomingkeji.xyz

Scala .......... 10
来源：http://eyb.jiagoushi.top

------------------------------------
来源：http://gkk.feifeiyinyue.top

合计 ........... 2106 条
来源：http://qeg.fzhhl.top

按章节统计：
来源：http://edc.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://igg.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oqj.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dzm.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dqa.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fft.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://efd.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://shw.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://glt.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dqs.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ptu.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vig.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zqx.xylfe.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://btl.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gtj.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mmg.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://laf.ehwqpu.com

Q SQL 专题                              90
来源：http://bwf.52xcode.cn

R Bash 专题                             80
来源：http://wpw.chenzaomai.com

S C / C++ 专题                          60
来源：http://jzt.yueranfly.top

T 其他语言补充                          60
来源：http://qjr.316326.xyz

U 高频实用片段                         120
来源：http://pry.tian-w.cn

------------------------------------
来源：http://qwa.epnwcf.com

合计                                  2106 条
来源：http://zvp.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://jte.feifeiyinyue.top

使用提醒
来源：http://ivk.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://tpi.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cln.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ujp.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://csc.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://ejg.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tjd.hywenlv.cn

—— 文件结束 ——
来源：http://vrd.zhoulong.xyz

================================================================================
来源：http://qii.9152youxi.cn

程序语言常见例子速查手册（2024 版）
来源：http://jvg.yj20258888.top

Common Programming Examples Cheat Book
来源：http://tkc.yj20258.top

================================================================================
来源：http://sjo.daria6918.cn

【收录内容】
来源：http://aee.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hjo.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lxr.sufxvd.cn

SQL · Bash · C · C++
来源：http://bhc.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dwk.zhoulong.xyz

【使用说明】
来源：http://ohl.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tqu.tianlin.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kve.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nur.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dbc.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://twg.yueranfly.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kbz.zhongyouzk.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gdb.cheryme.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ccz.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qbs.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ldl.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mup.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ixf.havefunace.top

【文件统计】
来源：http://ykr.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qzq.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://zop.c1oappe.top

目  录
来源：http://ncm.cheryme.top

--------------------------------------------------------------------------------
来源：http://ajp.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rry.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gls.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jac.wangdashe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dfg.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ntq.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cme.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ecg.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mfb.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kvw.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lsf.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jzf.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://afg.cucudq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://arq.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://huk.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vox.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tdi.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bzn.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rce.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sqq.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pkd.sufxvd.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uvh.9152youxi.cn

================================================================================
来源：http://qsj.jyoumei.cn

A. 基础语法与类型
来源：http://ysz.aibaodan.cn

================================================================================
来源：http://hag.tanke756.top

[A01] Hello World
来源：http://ugh.yuxming.cn

Py:   print("Hello, World!")
来源：http://ffd.zycfv.cn

PHP:  echo "Hello, World!";
来源：http://zzd.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://ujp.xingfuxueyuan.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lnl.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://qpw.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://hjv.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://dsj.smart0.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://jvc.redwolf501.top

[A02] 变量声明与赋值
来源：http://wtq.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eed.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qbt.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://glh.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pou.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://qnq.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://ryw.shanyushiyangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://ekp.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://iqq.sufxvd.cn

[A03] 常量定义
来源：http://lrh.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bzr.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://ugo.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://stu.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://zbz.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://oje.guannengcc.top

Go:   const PI = 3.14159
来源：http://dvu.svipenyu.cn

Ruby: PI = 3.14159
来源：http://xps.wangdashe.top

C#:   const double PI = 3.14159;
来源：http://ilr.cheryme.top

[A04] 判断变量类型
来源：http://etz.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bpd.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://odn.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mdx.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://hoq.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://olc.redwolf501.top

Go:   reflect.TypeOf(x).Name()
来源：http://wki.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ebt.xuanzx.com

C#:   x.GetType().Name; x is int
来源：http://zmi.hysaishi.cn

[A05] 整数除法与取模
来源：http://twj.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rcy.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bbg.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yug.ehwqpu.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bcq.quarkkingdee.top

Java: 7 / 2; 7 % 2
来源：http://wbw.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://xmv.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://zak.meibo888.top

C#:   7 / 2; 7 % 2
来源：http://zyo.nanxinkj.top

[A06] 字符串转数字
来源：http://qpx.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://efb.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xue.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ctu.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://wnn.hongshengwenyu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wve.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wdx.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vdg.shanyushiyangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kjb.yanxiufei.cn

[A07] 数字转字符串
来源：http://cup.hesvh.cn

Py:   str(42)
来源：http://cyv.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://zmp.tianlin.xyz

JS:   String(42); (42).toString()
来源：http://qbz.zhijiandao.cn

TS:   String(42)
来源：http://gid.zycfv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cwt.uphjek.com

Go:   strconv.Itoa(42)
来源：http://xhk.mhx1999.top

Ruby: 42.to_s
来源：http://hjv.dashuyun.cn

C#:   42.ToString()
来源：http://swt.jinqigfzy.top

[A08] 取整与四舍五入
来源：http://jdq.zhongyouzk.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lmj.jianghu66.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mlm.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://myp.dianchejie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xmg.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jil.fzhhl.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://okn.hnqzz.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xph.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lwr.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://gsb.zycfv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vig.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zfj.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pwq.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://upk.shanyushiyangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://opw.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vfz.yongpay.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zpz.smart0.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bhb.havefunace.top

[A10] 生成随机数
来源：http://giq.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://grr.aibaodan.cn

PHP:  random_int(1, 100);
来源：http://mda.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mpt.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iyb.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://uli.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ogq.tarul.cn

Ruby: rand(1..100)
来源：http://hye.dianchejie.cn

C#:   new Random().Next(1, 101)
来源：http://glg.fehbvm.com

[A11] 条件表达式（三元）
来源：http://jpr.chenjidiqi.icu

Py:   "yes" if x > 0 else "no"
来源：http://qzu.daria6918.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rgp.tian-w.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jvy.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://tre.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://tmx.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ife.hnqzz.top

Ruby: x > 0 ? "yes" : "no"
来源：http://beo.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rtq.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://hfv.cheryme.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ayz.guannengcc.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zyf.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://uzg.hysaishi.cn

TS:   `Hello, ${name}!`
来源：http://lhc.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://auw.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mqe.cheryme.top

Ruby: "Hello, #{name}!"
来源：http://aen.hnxiangtu.top

C#:   $"Hello, {name}!"
来源：http://xgj.yangfankeji.com

[A13] 多行字符串（练习 \n 转义）
来源：http://swh.jqgfzy.top

Py:   "第一行\n第二行"
来源：http://mnb.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://hch.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://ytv.epnwcf.com

TS:   "第一行\n第二行"
来源：http://hfv.birdmap.top

Java: "第一行\n第二行"
来源：http://lcw.cashguo.top

Go:   "第一行\n第二行"
来源：http://trd.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://eyi.tarul.cn

C#:   "第一行\n第二行"
来源：http://avn.meibo888.top

[A14] 注释写法
来源：http://nvp.chenzaomai.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://dlu.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ovc.hnxiangtu.top

JS:   // 单行；/* 多行 */
来源：http://bht.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://erv.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://etb.tian-w.cn

Go:   // 单行；/* 多行 */
来源：http://pfr.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://bui.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://zrr.wangdashe.top

[A15] 空值判断与默认值
来源：http://qzu.fktsv.cn

Py:   value = data or "默认值"
来源：http://mne.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://goo.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://buf.andypj.xyz

TS:   const value = data ?? "默认值";
来源：http://xcr.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kca.zhaomingkeji.xyz

Go:   if data == "" { data = "默认值" }
来源：http://gnk.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://faf.zhongyouzk.top

C#:   var value = data ?? "默认值";
来源：http://ndz.hesvh.cn

[A16] 真假值判断规则
来源：http://zgz.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wix.xuetiantiany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cjl.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xab.daxiang520.top

TS:   if (!x) {}
来源：http://ber.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yih.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sim.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://ezd.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://swl.fanxiaobao.xyz

[A17] 位运算
来源：http://eth.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uup.redwolf501.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qtr.cucudq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ton.ivvv.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jdl.yj202588.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogp.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ozq.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pne.cqqwz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ari.52xcode.cn


<!-- 参考信息 -->