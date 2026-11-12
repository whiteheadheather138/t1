代发 wailian999

[U105] JS：节流
来源：http://hnh.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wko.tianlin.xyz

[U106] JS：日期格式化
来源：http://rta.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ukf.yanxiufei.cn

[U107] JS：数字千分位
来源：http://zia.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yez.yongpay.top

[U108] JS：随机整数
来源：http://ono.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nrf.aizwys.cn

[U109] JS：数组分组
来源：http://umd.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://awg.hnqzz.top

[U110] JS：数组分块
来源：http://qrz.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nex.yongpay.top

[U111] JS：对象转 Map
来源：http://dvt.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://fvt.ctjpmb.com

[U112] JS：字符串补位
来源：http://gtr.nanxinkj.top

"7".padStart(3, "0")
来源：http://yjv.yongpay.top

[U113] JS：正则替换全部
来源：http://jsk.aibaodan.cn

s.replaceAll("a", "b")
来源：http://dae.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://sll.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aul.sweek.top

[U115] JS：生成 UUID
来源：http://qfu.ivvv.top

crypto.randomUUID()
来源：http://jaf.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://rim.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://swp.nanxinkj.top

[U117] JS：单元测试
来源：http://cwv.hammf.cn

npm i -D vitest;  npx vitest
来源：http://uev.yonumen.top

[U118] JS：开发服务器
来源：http://lwx.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://qdz.jqgufenzy.top

[U119] JS：生产构建
来源：http://tst.zycfv.cn

npx vite build
来源：http://dvu.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://pio.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://lkb.cqqwz.cn

================================================================================
来源：http://sht.chenjidiqi.icu

统计汇总
来源：http://tgu.pengpengdd.cyou

================================================================================
来源：http://lkc.jianghu66.top

按语言统计（条）：
来源：http://qjh.wangdashe.top

Python ......... 252
来源：http://rvc.sxryk.cn

PHP ............ 252
来源：http://nya.chenlongwang.top

JavaScript ..... 252
来源：http://vuc.pycfn.com

TypeScript ..... 212
来源：http://knd.zhengqikj.top

Java ........... 212
来源：http://oaq.hnqzz.top

Go ............. 212
来源：http://vfy.pycfn.com

Ruby ........... 212
来源：http://hzq.svipenyu.cn

C# ............. 212
来源：http://xwc.wangshuangyany.cn

C .............. 30
来源：http://mdf.sysykeji.top

C++ ............ 30
来源：http://skt.shangyingyoupin.top

SQL ............ 90
来源：http://bwv.ydzc1.top

Bash ........... 80
来源：http://rzv.zhijiandao.cn

Kotlin ......... 15
来源：http://bts.fzhhl.top

Swift .......... 15
来源：http://jfu.birdmap.top

Lua ............ 10
来源：http://ypb.jianghu66.top

Perl ........... 10
来源：http://jee.xziqi.cn

Scala .......... 10
来源：http://gwj.tianlin.xyz

------------------------------------
来源：http://gay.hfpthk.cn

合计 ........... 2106 条
来源：http://krc.xinyue.icu

按章节统计：
来源：http://qwg.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://svo.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rzs.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kes.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hir.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kbx.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ctq.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ave.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kzx.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://acu.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dwp.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wzc.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jwm.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ljs.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kgw.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sar.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ezn.vehdjk.com

Q SQL 专题                              90
来源：http://ycf.zdqjudy.top

R Bash 专题                             80
来源：http://iio.mhx1999.top

S C / C++ 专题                          60
来源：http://gch.yueranfly.top

T 其他语言补充                          60
来源：http://znm.yj20258888.top

U 高频实用片段                         120
来源：http://lbt.sysykeji.top

------------------------------------
来源：http://rdu.0kj1m.cn

合计                                  2106 条
来源：http://krl.52xcode.cn

--------------------------------------------------------------------------------
来源：http://cvh.dashuyun.cn

使用提醒
来源：http://dsg.birdmap.top

--------------------------------------------------------------------------------
来源：http://wsp.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vro.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yib.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fhw.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cnx.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wbt.hcnkem.com

—— 文件结束 ——
来源：http://neb.ppjwa.cn

================================================================================
来源：http://laz.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://qra.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://hum.tarul.cn

================================================================================
来源：http://wxi.shanyushiyangtech.top

【收录内容】
来源：http://euz.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cbn.sjlbkw.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ofh.iojbl.cn

SQL · Bash · C · C++
来源：http://yiv.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pwe.yj20258888.top

【使用说明】
来源：http://ghx.hammf.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zrs.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://npe.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://llv.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wrj.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ayd.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xze.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hwa.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tno.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rzi.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tew.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yeo.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://axy.fengsongda.top

【文件统计】
来源：http://kxj.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hdu.cashguo.top

--------------------------------------------------------------------------------
来源：http://tdx.ybcxt.top

目  录
来源：http://cnv.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://uxl.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bom.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eko.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aul.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://aot.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xiz.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wzc.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ypp.yueranfly.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dva.wangshuangyany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kfv.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pdb.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hig.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ebg.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gej.wangdashe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nyu.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jyk.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vyx.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bwy.pycfn.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://gez.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qpy.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lsx.ydzc1.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gev.xinyue.icu

================================================================================
来源：http://xih.yj20258.top

A. 基础语法与类型
来源：http://nsn.bbcook.cn

================================================================================
来源：http://jjx.zycfv.cn

[A01] Hello World
来源：http://nsg.zycfv.cn

Py:   print("Hello, World!")
来源：http://miu.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://nzz.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://sem.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kkn.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://meb.xuanzx.com

Go:   fmt.Println("Hello, World!")
来源：http://ysg.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://sct.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://znj.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://qfc.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wla.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://weg.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://qur.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sxc.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://xrw.hesvh.cn

Go:   name := "Alex"; age := 20
来源：http://xap.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://pyn.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://vzy.guannengcc.top

[A03] 常量定义
来源：http://eym.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lpb.xylfe.cn

PHP:  const PI = 3.14159;
来源：http://bxp.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://hdn.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://qsj.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://xrn.svipenyu.cn

Go:   const PI = 3.14159
来源：http://afo.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://nfz.316326.xyz

C#:   const double PI = 3.14159;
来源：http://oms.cdnleiting.top

[A04] 判断变量类型
来源：http://fhc.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://wde.uphjek.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://otw.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tic.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://hzf.nanxinkj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sif.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://pkw.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qot.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://ckb.meibo888.top

[A05] 整数除法与取模
来源：http://dqv.jlsjyb.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fny.gzhubu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wep.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://adj.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qlw.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://nya.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://tbm.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://lit.nanxinkj.top

C#:   7 / 2; 7 % 2
来源：http://fcc.iojbl.cn

[A06] 字符串转数字
来源：http://qra.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://inf.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sex.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yuu.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://drk.aizwys.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cky.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://frd.c1oappe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://trm.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ndq.guowangkeji.top

[A07] 数字转字符串
来源：http://onv.zhijiandao.cn

Py:   str(42)
来源：http://rdl.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://rxx.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://fji.yongpay.top

TS:   String(42)
来源：http://mat.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rbs.svipenyu.cn

Go:   strconv.Itoa(42)
来源：http://bgk.uphjek.com

Ruby: 42.to_s
来源：http://gup.ctjpmb.com

C#:   42.ToString()
来源：http://qkm.jinghuilouyu.cn

[A08] 取整与四舍五入
来源：http://oih.sxryk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gni.yanxiufei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ysf.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://udi.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iji.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wim.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gss.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kcm.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bai.tianlin.xyz

[A09] 绝对值与最大最小值
来源：http://oyk.cdnleiting.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bxl.jqgfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pup.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ecm.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dyj.hesvh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bpv.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rka.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ltq.zhengqikj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zcr.hesvh.cn

[A10] 生成随机数
来源：http://atz.mhx1999.top

Py:   import random; random.randint(1, 100)
来源：http://mzm.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://cdq.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wjq.chenjidiqi.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rmz.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://htn.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ges.zhengqikj.top

Ruby: rand(1..100)
来源：http://mqn.sweek.top

C#:   new Random().Next(1, 101)
来源：http://sor.zhoulong.xyz

[A11] 条件表达式（三元）
来源：http://zgb.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://okg.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://xtu.smart0.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://cso.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://ctc.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://eiw.haohaochexian.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jir.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dge.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lfh.cdnleiting.top

[A12] 字符串插值 / 格式化
来源：http://zcf.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sis.hcnkem.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zxh.nanxinkj.top

JS:   `Hello, ${name}!`
来源：http://pqm.shuidangran.top

TS:   `Hello, ${name}!`
来源：http://ihh.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://yfz.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ppj.nanxinkj.top

Ruby: "Hello, #{name}!"
来源：http://nff.xinyue.icu

C#:   $"Hello, {name}!"
来源：http://bwl.jinqigufen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kwt.yj20258.top

Py:   "第一行\n第二行"
来源：http://ozb.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://hir.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://bhr.quarkkingdee.top

TS:   "第一行\n第二行"
来源：http://gto.hammf.cn

Java: "第一行\n第二行"
来源：http://ubo.yueranfly.top

Go:   "第一行\n第二行"
来源：http://pcc.c1oappe.top

Ruby: "第一行\n第二行"
来源：http://imw.zdqjudy.top

C#:   "第一行\n第二行"
来源：http://jgt.zhiwuduotai.top

[A14] 注释写法
来源：http://mqm.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tgf.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://tmg.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://xfz.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://trx.wangdashe.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rgt.iojbl.cn

Go:   // 单行；/* 多行 */
来源：http://yvb.zhoulong.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://hdk.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://ppk.ivvv.top

[A15] 空值判断与默认值
来源：http://vtw.yueranfly.top

Py:   value = data or "默认值"
来源：http://tpf.jinghuilouyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://rjo.chenlongwang.top

JS:   const value = data ?? "默认值";
来源：http://smw.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://wwj.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gxa.pycfn.com

Go:   if data == "" { data = "默认值" }
来源：http://eme.yongpay.top

Ruby: value = data || "默认值"
来源：http://ytw.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://cyx.gogol.net.cn

[A16] 真假值判断规则
来源：http://ery.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://itw.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://suz.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mvp.jiagoushi.top

TS:   if (!x) {}
来源：http://xjl.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kmg.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hgs.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://zuo.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ojj.xingfuxueyuan.xyz

[A17] 位运算
来源：http://jiq.jianghu66.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xzb.jinqigufen.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bbg.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sxj.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xuy.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hai.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uxg.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuk.guannengcc.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dfn.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://swn.wangshuangyany.cn

Py:   ord("A"); chr(65)
来源：http://sbf.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://tic.fktsv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jof.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mzm.nanxuanxn.top

Java: (int) 'A'; (char) 65
来源：http://zuf.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uyd.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://bbc.sweek.top


<!-- 参考信息 -->