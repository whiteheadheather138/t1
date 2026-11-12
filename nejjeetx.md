代发 wailian999

[U101] JS：classList 操作
来源：http://kjf.jiagoushi.top

el.classList.toggle("active")
来源：http://akt.chenjidiqi.icu

[U102] JS：本地存储
来源：http://wmr.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://abq.gaohongyu789.top

[U103] JS：定时器
来源：http://nis.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cdy.zycfv.cn

[U104] JS：防抖
来源：http://mzz.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://und.yuanzhike.top

[U105] JS：节流
来源：http://non.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wjs.gogol.net.cn

[U106] JS：日期格式化
来源：http://tlf.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sod.sjlbkw.cn

[U107] JS：数字千分位
来源：http://zpg.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://men.pycfn.com

[U108] JS：随机整数
来源：http://iqq.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gzb.daxiang520.top

[U109] JS：数组分组
来源：http://gaf.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://qmd.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://nqx.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nll.dianchejie.cn

[U111] JS：对象转 Map
来源：http://cwz.fehbvm.com

new Map(Object.entries(obj))
来源：http://rsn.jinqigufen.top

[U112] JS：字符串补位
来源：http://gsv.zycfv.cn

"7".padStart(3, "0")
来源：http://rbc.ydzc1.top

[U113] JS：正则替换全部
来源：http://gsa.yuanzhike.top

s.replaceAll("a", "b")
来源：http://hfy.zycfv.cn

[U114] JS：JSON 深比较
来源：http://yrf.chenzaomai.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ghu.hesvh.cn

[U115] JS：生成 UUID
来源：http://ngl.hywenlv.cn

crypto.randomUUID()
来源：http://hbs.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://zrm.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://prq.ctjpmb.com

[U117] JS：单元测试
来源：http://uit.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://uyv.zhixingplan.top

[U118] JS：开发服务器
来源：http://hya.chenlongwang.top

npm i -D vite;  npx vite
来源：http://abc.sweek.top

[U119] JS：生产构建
来源：http://jyk.fzhhl.top

npx vite build
来源：http://mqf.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://nhs.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://ykf.pycfn.com

================================================================================
来源：http://xph.fanxiaobao.xyz

统计汇总
来源：http://gxp.zycfv.cn

================================================================================
来源：http://buv.zhongyouzk.top

按语言统计（条）：
来源：http://gwh.zhixingplan.top

Python ......... 252
来源：http://ads.jinghuilouyu.cn

PHP ............ 252
来源：http://cly.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://itp.aizwys.cn

TypeScript ..... 212
来源：http://umh.fehbvm.com

Java ........... 212
来源：http://tgq.hysaishi.cn

Go ............. 212
来源：http://jgs.quarkkingdee.top

Ruby ........... 212
来源：http://ekw.cashguo.top

C# ............. 212
来源：http://hbm.xziqi.cn

C .............. 30
来源：http://qel.zdqjudy.top

C++ ............ 30
来源：http://bhi.shanyushiyangkeji.top

SQL ............ 90
来源：http://zsh.zhongyouzk.top

Bash ........... 80
来源：http://sgl.yuxming.cn

Kotlin ......... 15
来源：http://cxf.yvedp.cn

Swift .......... 15
来源：http://vrp.gogol.net.cn

Lua ............ 10
来源：http://yir.guowangkeji.top

Perl ........... 10
来源：http://ffu.fzhhl.top

Scala .......... 10
来源：http://nnr.epnwcf.com

------------------------------------
来源：http://rgt.c1oappe.top

合计 ........... 2106 条
来源：http://aqh.hcnkem.com

按章节统计：
来源：http://luy.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aeu.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://som.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nqq.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://osg.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dgw.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bju.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eok.jqgfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oym.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qjz.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://axz.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fsk.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yyv.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bdu.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://noi.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ifb.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://czj.hammf.cn

Q SQL 专题                              90
来源：http://chj.cheryme.top

R Bash 专题                             80
来源：http://fpe.meibo888.top

S C / C++ 专题                          60
来源：http://smw.hfpthk.cn

T 其他语言补充                          60
来源：http://jqh.nanxuanxn.top

U 高频实用片段                         120
来源：http://mpa.hnxiangtu.top

------------------------------------
来源：http://alc.jqgfzy.top

合计                                  2106 条
来源：http://rlj.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://adg.jyoumei.cn

使用提醒
来源：http://plt.ydzc1.top

--------------------------------------------------------------------------------
来源：http://hbj.hfpthk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gkk.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lzs.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lkn.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gkt.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sju.zhoulong.xyz

—— 文件结束 ——
来源：http://mqp.svipenyu.cn

================================================================================
来源：http://ddh.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://dfn.mhx1999.top

Common Programming Examples Cheat Book
来源：http://zww.dashuyun.cn

================================================================================
来源：http://fpg.chenlongwang.top

【收录内容】
来源：http://srh.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lcu.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aot.kuanghao11.cn

SQL · Bash · C · C++
来源：http://zsw.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://thx.redwolf501.top

【使用说明】
来源：http://ioh.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xgd.shzxlz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qqc.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xjj.dianchejie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sfk.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://jrt.jqgfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yvz.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cse.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oop.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ebv.yfazqb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ooh.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jlw.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ptd.ydjk.org.cn

【文件统计】
来源：http://yzr.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xlj.uphjek.com

--------------------------------------------------------------------------------
来源：http://evt.jianghu66.top

目  录
来源：http://dqb.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://sxf.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ktd.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ldx.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vmd.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ooi.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pbd.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iue.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jhp.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fmk.chenzaomai.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://axq.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zls.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ntq.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zfb.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qnw.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ywx.andypj.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ofb.svipenyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://equ.yfazqb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aea.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://cwz.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jmu.smart0.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://klu.hcnkem.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rol.zycfv.cn

================================================================================
来源：http://aez.gotoacloud.top

A. 基础语法与类型
来源：http://dql.xylfe.cn

================================================================================
来源：http://hzb.xuetiantiany.cn

[A01] Hello World
来源：http://aqp.shuidangran.top

Py:   print("Hello, World!")
来源：http://jel.ivvv.top

PHP:  echo "Hello, World!";
来源：http://lmn.sysykeji.top

JS:   console.log("Hello, World!");
来源：http://fha.birdmap.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lxt.yanxiufei.cn

Java: System.out.println("Hello, World!");
来源：http://mas.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://fix.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://che.guannengcc.top

C#:   Console.WriteLine("Hello, World!");
来源：http://oze.cdnleiting.top

[A02] 变量声明与赋值
来源：http://veg.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cmr.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dqm.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eid.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fkw.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://wgu.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://kji.gogol.net.cn

Ruby: name = "Alex"; age = 20
来源：http://mes.sxryk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dzm.sysykeji.top

[A03] 常量定义
来源：http://zvp.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bbk.snrcjt.cn

PHP:  const PI = 3.14159;
来源：http://dzh.jlsjyb.cn

JS:   const PI = 3.14159;
来源：http://idx.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://ydt.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://dyj.9152youxi.cn

Go:   const PI = 3.14159
来源：http://rum.yueranfly.top

Ruby: PI = 3.14159
来源：http://uog.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://shr.c1oappe.top

[A04] 判断变量类型
来源：http://jyz.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xsq.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nim.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kag.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://uqi.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xeu.gzhubu.top

Go:   reflect.TypeOf(x).Name()
来源：http://nau.bbcook.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uwd.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://str.ydzc1.top

[A05] 整数除法与取模
来源：http://klw.iojbl.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iqy.shuidangran.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rno.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://viy.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://prj.chenjidiqi.icu

Java: 7 / 2; 7 % 2
来源：http://ope.uphjek.com

Go:   7 / 2; 7 % 2
来源：http://ybu.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://bcd.0kj1m.cn

C#:   7 / 2; 7 % 2
来源：http://wbl.yangfankeji.com

[A06] 字符串转数字
来源：http://ndq.sjlbkw.cn

Py:   int("42"); float("3.14")
来源：http://slu.316326.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mfs.c1oappe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://abj.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://ltc.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://opy.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://siy.guowangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ygq.shuidangran.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wfz.yj20258888.top

[A07] 数字转字符串
来源：http://gzn.redwolf501.top

Py:   str(42)
来源：http://aft.chenzaomai.com

PHP:  (string) 42; strval(42)
来源：http://dgh.ydzc1.top

JS:   String(42); (42).toString()
来源：http://twx.chenjidiqi.icu

TS:   String(42)
来源：http://bcx.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rfo.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://nme.iojbl.cn

Ruby: 42.to_s
来源：http://ihi.bbcook.cn

C#:   42.ToString()
来源：http://kuk.hesvh.cn

[A08] 取整与四舍五入
来源：http://wsu.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qbx.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xmp.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bvz.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://krv.shanyushiyangtech.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dmg.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://syx.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xaw.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ngq.ydjk.org.cn

[A09] 绝对值与最大最小值
来源：http://gmd.hfpthk.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://muy.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qsg.nanxinkj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hyb.ywan-chungtsiang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hgy.jiagoushi.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ipp.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gid.xinyue.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://awr.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://htc.hesvh.cn

[A10] 生成随机数
来源：http://hdq.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://hpa.ivvv.top

PHP:  random_int(1, 100);
来源：http://kes.jinghuilouyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hte.daxiang520.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gue.guowangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://tmm.guowangkeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qav.fengsongda.top

Ruby: rand(1..100)
来源：http://pdu.yj202588.top

C#:   new Random().Next(1, 101)
来源：http://jzx.yongpay.top

[A11] 条件表达式（三元）
来源：http://wcq.xziqi.cn

Py:   "yes" if x > 0 else "no"
来源：http://wxi.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zoo.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://plj.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oia.daxiang520.top

Java: x > 0 ? "yes" : "no"
来源：http://gmt.svipenyu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bnp.ehwqpu.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ood.guowangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://zgd.yueranfly.top

[A12] 字符串插值 / 格式化
来源：http://fze.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nuk.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ved.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://tle.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://alt.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://iwd.ydjk.org.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hhf.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://loz.tarul.cn

C#:   $"Hello, {name}!"
来源：http://ada.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yhz.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://tya.tianlin.xyz

PHP:  "第一行\n第二行"
来源：http://mvz.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://kbr.vqdsnc.cn

TS:   "第一行\n第二行"
来源：http://zre.daria6918.cn

Java: "第一行\n第二行"
来源：http://six.birdmap.top

Go:   "第一行\n第二行"
来源：http://och.jiagoushi.top

Ruby: "第一行\n第二行"
来源：http://pxx.daxiang520.top

C#:   "第一行\n第二行"
来源：http://iay.gogol.net.cn

[A14] 注释写法
来源：http://suy.aizwys.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xqv.yuxming.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tbc.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://icb.wangdashe.top

TS:   // 单行；/* 多行 */
来源：http://jwk.guowangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oll.ydzc1.top

Go:   // 单行；/* 多行 */
来源：http://clr.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://nvo.316326.xyz

C#:   // 单行；/* 多行 */
来源：http://odd.ehwqpu.com

[A15] 空值判断与默认值
来源：http://qzh.nanxinkj.top

Py:   value = data or "默认值"
来源：http://jts.gotoacloud.top

PHP:  $value = $data ?? "默认值";
来源：http://rkl.nwbrower.top

JS:   const value = data ?? "默认值";
来源：http://frw.zhijiandao.cn

TS:   const value = data ?? "默认值";
来源：http://wod.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cth.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://clj.yuanzhike.top

Ruby: value = data || "默认值"
来源：http://wql.xylfe.cn

C#:   var value = data ?? "默认值";
来源：http://zef.gzhubu.top

[A16] 真假值判断规则
来源：http://yzw.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jxv.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rdv.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ger.guowangkeji.top

TS:   if (!x) {}
来源：http://hen.zhixingplan.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sur.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rcr.wangdashe.top

Ruby: unless x            # nil 与 false 为假
来源：http://rrp.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ixm.yongpay.top

[A17] 位运算
来源：http://syy.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osg.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hvg.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fky.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://god.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://psv.xuanzx.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tro.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhm.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vpv.pycfn.com


<!-- 参考信息 -->