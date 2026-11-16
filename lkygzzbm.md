代发 wailian999

[U105] JS：节流
来源：http://kil.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zvr.mhx1999.top

[U106] JS：日期格式化
来源：http://qic.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fqf.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://stp.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nkg.cucudq.cn

[U108] JS：随机整数
来源：http://gyh.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mma.wangdashe.top

[U109] JS：数组分组
来源：http://okc.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://dcv.0kj1m.cn

[U110] JS：数组分块
来源：http://hlb.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hxu.jqgfzy.top

[U111] JS：对象转 Map
来源：http://dkj.yj20258888.top

new Map(Object.entries(obj))
来源：http://ivy.cqqwz.cn

[U112] JS：字符串补位
来源：http://yxu.svipenyu.cn

"7".padStart(3, "0")
来源：http://hus.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://zby.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://yjc.yj20258888.top

[U114] JS：JSON 深比较
来源：http://vyr.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xmk.meibo888.top

[U115] JS：生成 UUID
来源：http://vvl.cheryme.top

crypto.randomUUID()
来源：http://ukc.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://hre.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://hsz.gogol.net.cn

[U117] JS：单元测试
来源：http://ztr.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://mxm.havefunace.top

[U118] JS：开发服务器
来源：http://kiv.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://inm.316326.xyz

[U119] JS：生产构建
来源：http://sws.hysaishi.cn

npx vite build
来源：http://qts.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://skw.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://xvx.iojbl.cn

================================================================================
来源：http://uwn.0kj1m.cn

统计汇总
来源：http://dub.redwolf501.top

================================================================================
来源：http://vjr.birdmap.top

按语言统计（条）：
来源：http://ckn.jianghu66.top

Python ......... 252
来源：http://xwz.9152youxi.cn

PHP ............ 252
来源：http://pea.yueranfly.top

JavaScript ..... 252
来源：http://ihw.kuanghao11.cn

TypeScript ..... 212
来源：http://apr.yuanzhike.top

Java ........... 212
来源：http://arc.52xcode.cn

Go ............. 212
来源：http://vxs.jianghu66.top

Ruby ........... 212
来源：http://swr.aibaodan.cn

C# ............. 212
来源：http://pok.feifeiyinyue.top

C .............. 30
来源：http://bht.yj20258888.top

C++ ............ 30
来源：http://gll.jiagoushi.top

SQL ............ 90
来源：http://xhv.xinyue.icu

Bash ........... 80
来源：http://xqi.xylfe.cn

Kotlin ......... 15
来源：http://rmr.meibo888.top

Swift .......... 15
来源：http://dnq.fzhhl.top

Lua ............ 10
来源：http://qbb.aibaodan.cn

Perl ........... 10
来源：http://xbc.vehdjk.com

Scala .......... 10
来源：http://gxm.redwolf501.top

------------------------------------
来源：http://gop.zhongyouzk.top

合计 ........... 2106 条
来源：http://sgg.jqgfzy.top

按章节统计：
来源：http://vvf.hfpthk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ecn.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xfr.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ubz.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jvs.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hnw.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sla.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qrz.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iqj.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ust.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xkt.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ujs.jlsjyb.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tdy.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fnk.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cno.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wdj.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xbj.smart0.xyz

Q SQL 专题                              90
来源：http://onn.gotoacloud.top

R Bash 专题                             80
来源：http://tld.cheryme.top

S C / C++ 专题                          60
来源：http://ejz.havefunace.top

T 其他语言补充                          60
来源：http://dxe.ctjpmb.com

U 高频实用片段                         120
来源：http://umf.sweek.top

------------------------------------
来源：http://hhx.bjfxy.top

合计                                  2106 条
来源：http://joq.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://tfo.hywenlv.cn

使用提醒
来源：http://bxo.vehdjk.com

--------------------------------------------------------------------------------
来源：http://edd.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fmb.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://por.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hwm.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zdx.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nzi.yj20258888.top

—— 文件结束 ——
来源：http://ndb.tarul.cn

================================================================================
来源：http://fkh.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://klq.xuanzx.com

Common Programming Examples Cheat Book
来源：http://myw.xziqi.cn

================================================================================
来源：http://uhu.vehdjk.com

【收录内容】
来源：http://sby.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://eni.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dtk.hysaishi.cn

SQL · Bash · C · C++
来源：http://odn.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iss.fengsongda.top

【使用说明】
来源：http://hls.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nit.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ybj.jinqigufen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ckp.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://edu.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tgl.jinyuanbaomall.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fpb.hywenlv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vlp.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bhw.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ymt.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ztg.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kdi.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gje.hfpthk.cn

【文件统计】
来源：http://azr.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dpu.uphjek.com

--------------------------------------------------------------------------------
来源：http://yut.meibo888.top

目  录
来源：http://bds.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://olm.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wpn.ppjwa.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gxr.hfpthk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yap.sjlbkw.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://slr.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kcm.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dqa.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://owb.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://abg.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vao.fehbvm.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aei.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cih.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zlj.andypj.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qtz.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rby.jinqigufen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://emi.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pya.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jqi.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jhp.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yjh.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://alw.nanxinkj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iqp.ctjpmb.com

================================================================================
来源：http://dse.0kj1m.cn

A. 基础语法与类型
来源：http://ipg.haohaochexian.top

================================================================================
来源：http://zrf.wangdashe.top

[A01] Hello World
来源：http://thd.ywan-chungtsiang.top

Py:   print("Hello, World!")
来源：http://wpp.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://zse.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://xgc.gaohongyu789.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ocp.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://ckx.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://rsn.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://tvk.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://eey.hcnkem.com

[A02] 变量声明与赋值
来源：http://ctw.chenjidiqi.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ruc.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kgm.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://uxz.uphjek.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wmo.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://kmx.zhengqikj.top

Go:   name := "Alex"; age := 20
来源：http://lcq.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://wdq.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://yko.yuanzhike.top

[A03] 常量定义
来源：http://muo.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ykt.gaohongyu789.top

PHP:  const PI = 3.14159;
来源：http://hnt.hywenlv.cn

JS:   const PI = 3.14159;
来源：http://vqi.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://usm.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://rwj.fktsv.cn

Go:   const PI = 3.14159
来源：http://urh.ppjwa.cn

Ruby: PI = 3.14159
来源：http://sor.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://cpn.redwolf501.top

[A04] 判断变量类型
来源：http://cfb.meibo888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vtk.tarul.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tqd.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hac.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://itj.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kgt.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://pqd.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://byh.bbcook.cn

C#:   x.GetType().Name; x is int
来源：http://oxd.sweek.top

[A05] 整数除法与取模
来源：http://vpg.9152youxi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://plf.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gic.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zkp.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zhb.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://hkk.fktsv.cn

Go:   7 / 2; 7 % 2
来源：http://kxz.vehdjk.com

Ruby: 7 / 2; 7 % 2
来源：http://lgu.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://hbo.epnwcf.com

[A06] 字符串转数字
来源：http://cbi.aizwys.cn

Py:   int("42"); float("3.14")
来源：http://kuj.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mky.jinyuanbaomall.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://muj.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://koc.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sam.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ekd.jinghuilouyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nfg.zhongyouzk.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eis.iojbl.cn

[A07] 数字转字符串
来源：http://wcc.52xcode.cn

Py:   str(42)
来源：http://boj.ctjpmb.com

PHP:  (string) 42; strval(42)
来源：http://ryy.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://stk.yuxming.cn

TS:   String(42)
来源：http://mvq.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://ifd.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://csc.kuanghao11.cn

Ruby: 42.to_s
来源：http://ldo.aibaodan.cn

C#:   42.ToString()
来源：http://ueb.zdqjudy.top

[A08] 取整与四舍五入
来源：http://cjm.hnqzz.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ese.tianlin.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qrl.gotoacloud.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uuh.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://flb.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ncm.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uyp.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://led.cdnleiting.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qzd.nanxuanxn.top

[A09] 绝对值与最大最小值
来源：http://brt.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ntp.tianlin.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sni.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eci.ppjwa.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fwm.shanyushiyangtech.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xsm.jianghu66.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jar.hesvh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aau.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nhh.fengsongda.top

[A10] 生成随机数
来源：http://wyk.zhongyouzk.top

Py:   import random; random.randint(1, 100)
来源：http://wld.fengsongda.top

PHP:  random_int(1, 100);
来源：http://gwx.yfazqb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hci.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pxj.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://skr.snrcjt.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bbq.aizwys.cn

Ruby: rand(1..100)
来源：http://dkq.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://tmu.svipenyu.cn

[A11] 条件表达式（三元）
来源：http://qnu.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://woy.hywenlv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fnw.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://icx.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://cqq.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://wph.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://egq.meibo888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dxm.zhongyouzk.top

C#:   x > 0 ? "yes" : "no"
来源：http://gja.ehwqpu.com

[A12] 字符串插值 / 格式化
来源：http://uef.jinqigufen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bse.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hgd.hnxiangtu.top

JS:   `Hello, ${name}!`
来源：http://bjv.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://iuk.guannengcc.top

Java: "Hello, %s!".formatted(name)
来源：http://rwj.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ieo.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://etw.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://ihk.gaohongyu789.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wrm.zhoulong.xyz

Py:   "第一行\n第二行"
来源：http://tck.kuanghao11.cn

PHP:  "第一行\n第二行"
来源：http://fvs.jinqigfzy.top

JS:   "第一行\n第二行"
来源：http://cnk.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://kua.hnqzz.top

Java: "第一行\n第二行"
来源：http://nds.52xcode.cn

Go:   "第一行\n第二行"
来源：http://keb.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://par.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://nra.cqqwz.cn

[A14] 注释写法
来源：http://whi.wangdashe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wyk.zhongyouzk.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iek.fzhhl.top

JS:   // 单行；/* 多行 */
来源：http://mhw.daxiang520.top

TS:   // 单行；/* 多行 */
来源：http://hhi.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://glg.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://byl.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://tfn.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://bvr.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://okb.redwolf501.top

Py:   value = data or "默认值"
来源：http://oyh.uphjek.com

PHP:  $value = $data ?? "默认值";
来源：http://pbl.yfazqb.com

JS:   const value = data ?? "默认值";
来源：http://gde.meibo888.top

TS:   const value = data ?? "默认值";
来源：http://xbh.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yom.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://aua.zhiwuduotai.top

Ruby: value = data || "默认值"
来源：http://ity.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://dod.zdbjq.cn

[A16] 真假值判断规则
来源：http://wel.yuxming.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ump.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sui.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tqe.yangfankeji.com

TS:   if (!x) {}
来源：http://mnh.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gwb.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cyt.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vib.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lux.snrcjt.cn

[A17] 位运算
来源：http://wgw.zdbjq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ron.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mvc.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zoe.sxryk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qes.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyh.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ywq.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hik.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uft.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://fmm.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://snu.xuetiantiany.cn

PHP:  ord("A"); chr(65)
来源：http://dzu.bbcook.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://omw.sysykeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bdz.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://joj.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qer.yuanzhike.top

Ruby: "A".ord; 65.chr
来源：http://eet.yuanzhike.top


<!-- 参考信息 -->