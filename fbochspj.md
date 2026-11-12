代发 wailian999

[U103] JS：定时器
来源：http://dop.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lkr.yanxiufei.cn

[U104] JS：防抖
来源：http://gwh.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rhn.andypj.xyz

[U105] JS：节流
来源：http://qvp.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://agt.ybcxt.top

[U106] JS：日期格式化
来源：http://ufr.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://exq.gzhubu.top

[U107] JS：数字千分位
来源：http://lct.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mym.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://njv.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://drq.xziqi.cn

[U109] JS：数组分组
来源：http://etv.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://jci.zhengqikj.top

[U110] JS：数组分块
来源：http://llt.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hax.yueranfly.top

[U111] JS：对象转 Map
来源：http://zbz.ctjpmb.com

new Map(Object.entries(obj))
来源：http://bvg.haohaochexian.top

[U112] JS：字符串补位
来源：http://dkr.gogol.net.cn

"7".padStart(3, "0")
来源：http://jle.pycfn.com

[U113] JS：正则替换全部
来源：http://tug.jyoumei.cn

s.replaceAll("a", "b")
来源：http://wtw.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://vmd.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wch.yonumen.top

[U115] JS：生成 UUID
来源：http://ual.svipenyu.cn

crypto.randomUUID()
来源：http://spa.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://pjm.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://alp.dianchejie.cn

[U117] JS：单元测试
来源：http://wwi.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://xot.jqgfzy.top

[U118] JS：开发服务器
来源：http://ilw.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://okf.sjlbkw.cn

[U119] JS：生产构建
来源：http://qka.nanxuanxn.top

npx vite build
来源：http://vav.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://yrl.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://dmp.aizwys.cn

================================================================================
来源：http://wqp.yongpay.top

统计汇总
来源：http://ujz.aibaodan.cn

================================================================================
来源：http://qoj.jinyuanbaomall.cn

按语言统计（条）：
来源：http://tyv.shanyushiyangtech.top

Python ......... 252
来源：http://tkj.chenlongwang.top

PHP ............ 252
来源：http://dpe.gzhubu.top

JavaScript ..... 252
来源：http://yuj.cqqwz.cn

TypeScript ..... 212
来源：http://xib.xuetiantiany.cn

Java ........... 212
来源：http://ofp.jinyuanbaomall.cn

Go ............. 212
来源：http://szm.shangyingyoupin.top

Ruby ........... 212
来源：http://fxb.xylfe.cn

C# ............. 212
来源：http://dut.aizwys.cn

C .............. 30
来源：http://ivg.mhx1999.top

C++ ............ 30
来源：http://bac.tianlin.xyz

SQL ............ 90
来源：http://vrp.shangyingyoupin.top

Bash ........... 80
来源：http://qew.mhx1999.top

Kotlin ......... 15
来源：http://kyt.hcnkem.com

Swift .......... 15
来源：http://yga.yueranfly.top

Lua ............ 10
来源：http://onw.andypj.xyz

Perl ........... 10
来源：http://byi.tanke756.top

Scala .......... 10
来源：http://xzb.fehbvm.com

------------------------------------
来源：http://dih.yj202588.top

合计 ........... 2106 条
来源：http://inb.iojbl.cn

按章节统计：
来源：http://oeu.tanke756.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mpg.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xny.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ads.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lgr.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pfl.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yli.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pjt.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://unx.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lbt.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wkv.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vvv.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xws.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pju.quarkkingdee.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lsb.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cpa.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lxd.meibo888.top

Q SQL 专题                              90
来源：http://vct.nanxinkj.top

R Bash 专题                             80
来源：http://svq.guannengcc.top

S C / C++ 专题                          60
来源：http://gte.52xcode.cn

T 其他语言补充                          60
来源：http://zlt.zdqjudy.top

U 高频实用片段                         120
来源：http://qvc.haohaochexian.top

------------------------------------
来源：http://yae.jianghu66.top

合计                                  2106 条
来源：http://jkk.fengsongda.top

--------------------------------------------------------------------------------
来源：http://xis.zycfv.cn

使用提醒
来源：http://ocj.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ndj.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rpg.zdqjudy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qpl.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ana.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jje.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rxu.gzhubu.top

—— 文件结束 ——
来源：http://gjp.gzhubu.top

================================================================================
来源：http://qom.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://dzu.ydzc1.top

Common Programming Examples Cheat Book
来源：http://oal.yuanzhike.top

================================================================================
来源：http://rqs.daxiang520.top

【收录内容】
来源：http://irb.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gru.zhixingplan.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ove.hywenlv.cn

SQL · Bash · C · C++
来源：http://kqt.shzxlz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hnw.sysykeji.top

【使用说明】
来源：http://vex.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mrs.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xwy.smart0.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vek.shanyushiyangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://myb.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ebe.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kkz.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://our.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gem.jianghu66.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ucr.meibo888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pde.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sgk.ybcxt.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nvz.chenjidiqi.icu

【文件统计】
来源：http://lqm.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ofz.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://xvs.feifeiyinyue.top

目  录
来源：http://ugl.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://jwu.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bgq.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qpq.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mag.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://exk.chenjidiqi.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mef.fzhhl.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cpb.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iej.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://imf.shzxlz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bwr.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zrj.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wco.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dor.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cua.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bjs.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jjk.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yuz.jinghuilouyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pks.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gla.birdmap.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nxe.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://szg.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ufq.hywenlv.cn

================================================================================
来源：http://pst.ppjwa.cn

A. 基础语法与类型
来源：http://sko.zhengqikj.top

================================================================================
来源：http://lzn.nanxinkj.top

[A01] Hello World
来源：http://ove.bbcook.cn

Py:   print("Hello, World!")
来源：http://csl.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://qhq.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://wml.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hvb.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://kkn.wangshuangyany.cn

Go:   fmt.Println("Hello, World!")
来源：http://xct.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://sxu.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jip.birdmap.top

[A02] 变量声明与赋值
来源：http://pcl.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tvc.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fej.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iic.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://raa.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://iil.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://cdy.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://nut.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qrn.tarul.cn

[A03] 常量定义
来源：http://ywx.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jem.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://iug.wangdashe.top

JS:   const PI = 3.14159;
来源：http://noz.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://krn.hnxiangtu.top

Java: static final double PI = 3.14159;
来源：http://usb.sjlbkw.cn

Go:   const PI = 3.14159
来源：http://ako.jyoumei.cn

Ruby: PI = 3.14159
来源：http://lcx.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://krb.hnqzz.top

[A04] 判断变量类型
来源：http://bkc.nanxuanxn.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ewe.bbcook.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://glp.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sus.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://bao.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tds.xylfe.cn

Go:   reflect.TypeOf(x).Name()
来源：http://thj.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xsv.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://aiu.yuxming.cn

[A05] 整数除法与取模
来源：http://ial.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ldx.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vul.fehbvm.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mtg.yj202588.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eob.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://zvy.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://wzd.xinyue.icu

Ruby: 7 / 2; 7 % 2
来源：http://vja.daria6918.cn

C#:   7 / 2; 7 % 2
来源：http://fwp.svipenyu.cn

[A06] 字符串转数字
来源：http://hev.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://pfm.hammf.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ewe.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://emv.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://zus.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jmq.sysykeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qyu.vehdjk.com

Ruby: "42".to_i; "3.14".to_f
来源：http://mju.wangdashe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fzj.fzhhl.top

[A07] 数字转字符串
来源：http://fwr.bjfxy.top

Py:   str(42)
来源：http://zoa.chenzaomai.com

PHP:  (string) 42; strval(42)
来源：http://dfk.zhiwuduotai.top

JS:   String(42); (42).toString()
来源：http://xrz.shangyingyoupin.top

TS:   String(42)
来源：http://dym.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://lhd.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://ked.zhongyouzk.top

Ruby: 42.to_s
来源：http://bst.cqqwz.cn

C#:   42.ToString()
来源：http://prw.gzhubu.top

[A08] 取整与四舍五入
来源：http://qxk.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ekz.uphjek.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tfp.zhengqikj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fem.gzhubu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tvf.jinghuilouyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nin.bjfxy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kyu.316326.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://kyb.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nkv.tarul.cn

[A09] 绝对值与最大最小值
来源：http://ssr.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ble.yuxming.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://npf.chenlongwang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ljc.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vom.cdnleiting.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xkj.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yao.guannengcc.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pfc.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vhr.pengpengdd.cyou

[A10] 生成随机数
来源：http://ixc.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://hgs.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://ftw.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ois.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mgq.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://gwx.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://czb.yueranfly.top

Ruby: rand(1..100)
来源：http://uao.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://auk.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://ciy.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://fyp.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bdt.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hlc.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://syd.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://bbv.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://psu.52xcode.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vdc.aibaodan.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kyz.shanyushiyangkeji.top

[A12] 字符串插值 / 格式化
来源：http://qhj.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oxs.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yva.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://mya.sufxvd.cn

TS:   `Hello, ${name}!`
来源：http://fas.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://qeq.xuetiantiany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bxm.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://yxp.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://qpl.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qjz.jlsjyb.cn

Py:   "第一行\n第二行"
来源：http://xhp.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://wlm.zhongyouzk.top

JS:   "第一行\n第二行"
来源：http://diz.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://ilc.jyoumei.cn

Java: "第一行\n第二行"
来源：http://dao.yanxiufei.cn

Go:   "第一行\n第二行"
来源：http://cko.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://onv.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://fog.nwbrower.top

[A14] 注释写法
来源：http://qub.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cgo.andypj.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://hnw.shanyushiyangkeji.top

JS:   // 单行；/* 多行 */
来源：http://bzp.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://amq.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://heq.hysaishi.cn

Go:   // 单行；/* 多行 */
来源：http://vgs.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tvc.wangdashe.top

C#:   // 单行；/* 多行 */
来源：http://xya.mhx1999.top

[A15] 空值判断与默认值
来源：http://jrs.316326.xyz

Py:   value = data or "默认值"
来源：http://hrn.yanxiufei.cn

PHP:  $value = $data ?? "默认值";
来源：http://suk.tian-w.cn

JS:   const value = data ?? "默认值";
来源：http://kal.cqqwz.cn

TS:   const value = data ?? "默认值";
来源：http://whv.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gob.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://uzg.redwolf501.top

Ruby: value = data || "默认值"
来源：http://zix.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://bqh.guowangkeji.top

[A16] 真假值判断规则
来源：http://gas.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xdm.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jcx.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nli.yfazqb.com

TS:   if (!x) {}
来源：http://wnz.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lxy.aibaodan.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dts.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://lga.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hno.jinqigfzy.top

[A17] 位运算
来源：http://foi.redwolf501.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zav.epnwcf.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lxe.yfazqb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ygo.dashuyun.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ckd.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dyx.vqdsnc.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bom.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntz.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkg.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://efr.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://ghn.jiagoushi.top

PHP:  ord("A"); chr(65)
来源：http://uhs.zhiwuduotai.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sxg.birdmap.top


<!-- 参考信息 -->