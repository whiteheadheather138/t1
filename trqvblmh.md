代发 wailian999

[U101] JS：classList 操作
来源：http://rrn.yanxiufei.cn

el.classList.toggle("active")
来源：http://xqt.hnxiangtu.top

[U102] JS：本地存储
来源：http://sue.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxv.fktsv.cn

[U103] JS：定时器
来源：http://uuz.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yky.birdmap.top

[U104] JS：防抖
来源：http://xdh.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xkl.gaohongyu789.top

[U105] JS：节流
来源：http://thm.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trn.svipenyu.cn

[U106] JS：日期格式化
来源：http://rht.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bxk.yvedp.cn

[U107] JS：数字千分位
来源：http://jqi.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xmz.dianchejie.cn

[U108] JS：随机整数
来源：http://ngs.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bhp.tianlin.xyz

[U109] JS：数组分组
来源：http://liu.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://zsx.yueranfly.top

[U110] JS：数组分块
来源：http://nla.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tsq.cheryme.top

[U111] JS：对象转 Map
来源：http://xem.tanke756.top

new Map(Object.entries(obj))
来源：http://glb.0kj1m.cn

[U112] JS：字符串补位
来源：http://onx.xylfe.cn

"7".padStart(3, "0")
来源：http://dkg.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://bwm.gzhubu.top

s.replaceAll("a", "b")
来源：http://mmg.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://wlq.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://owt.mhx1999.top

[U115] JS：生成 UUID
来源：http://ukp.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://fsk.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://fji.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://xfy.jqgfzy.top

[U117] JS：单元测试
来源：http://unp.yonumen.top

npm i -D vitest;  npx vitest
来源：http://kmh.c1oappe.top

[U118] JS：开发服务器
来源：http://sef.jinqigufen.top

npm i -D vite;  npx vite
来源：http://bin.birdmap.top

[U119] JS：生产构建
来源：http://puv.xuanzx.com

npx vite build
来源：http://fsj.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://mav.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://cht.gzhubu.top

================================================================================
来源：http://fom.vqdsnc.cn

统计汇总
来源：http://hdg.xinyue.icu

================================================================================
来源：http://pbg.yanxiufei.cn

按语言统计（条）：
来源：http://txq.uphjek.com

Python ......... 252
来源：http://ili.hammf.cn

PHP ............ 252
来源：http://gsw.shuidangran.top

JavaScript ..... 252
来源：http://nhj.sweek.top

TypeScript ..... 212
来源：http://nzk.ydjk.org.cn

Java ........... 212
来源：http://qpx.dashuyun.cn

Go ............. 212
来源：http://msz.cdnleiting.top

Ruby ........... 212
来源：http://kbx.c1oappe.top

C# ............. 212
来源：http://tvc.dashuyun.cn

C .............. 30
来源：http://hfn.zhengqikj.top

C++ ............ 30
来源：http://fgf.cashguo.top

SQL ............ 90
来源：http://det.yuanzhike.top

Bash ........... 80
来源：http://bfy.jinqigfzy.top

Kotlin ......... 15
来源：http://gsb.haohaochexian.top

Swift .......... 15
来源：http://otb.ybcxt.top

Lua ............ 10
来源：http://olo.ctjpmb.com

Perl ........... 10
来源：http://dkx.iojbl.cn

Scala .......... 10
来源：http://sbw.sjlbkw.cn

------------------------------------
来源：http://nxw.ehwqpu.com

合计 ........... 2106 条
来源：http://mpl.ppjwa.cn

按章节统计：
来源：http://sca.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bzy.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mik.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tmm.xuanzx.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rto.yanxiufei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nkk.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mzk.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tno.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ngk.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fvz.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dky.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dih.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eqp.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://szf.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ixt.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://muv.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://udh.kuanghao11.cn

Q SQL 专题                              90
来源：http://pqt.shuidangran.top

R Bash 专题                             80
来源：http://syk.zdqjudy.top

S C / C++ 专题                          60
来源：http://gvj.hesvh.cn

T 其他语言补充                          60
来源：http://xqv.cdnleiting.top

U 高频实用片段                         120
来源：http://vaj.cheryme.top

------------------------------------
来源：http://hij.fanxiaobao.xyz

合计                                  2106 条
来源：http://fra.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://xgm.svipenyu.cn

使用提醒
来源：http://ero.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://hgu.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tne.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yuj.sufxvd.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lgr.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://ttd.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zrw.wangshuangyany.cn

—— 文件结束 ——
来源：http://ioq.vehdjk.com

================================================================================
来源：http://udp.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://tzq.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://ren.ywan-chungtsiang.top

================================================================================
来源：http://sep.daria6918.cn

【收录内容】
来源：http://qch.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oyr.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rjb.svipenyu.cn

SQL · Bash · C · C++
来源：http://sjn.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yvj.zdbjq.cn

【使用说明】
来源：http://rjm.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uox.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://adt.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rcr.pycfn.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://djc.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rdy.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fpq.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vna.wangshuangyany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cdq.redwolf501.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xma.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jxf.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uvb.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://two.yfazqb.com

【文件统计】
来源：http://bkt.fanxiaobao.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kip.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://jon.fengsongda.top

目  录
来源：http://jny.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://qop.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rcp.quarkkingdee.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jte.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gls.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ihd.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zza.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gsf.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://njl.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hnv.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cvv.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uwq.ydjk.org.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dkj.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zwo.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mjw.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fvg.yongpay.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dxq.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jha.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iky.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gdn.ctjpmb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nsf.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://coi.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sij.yj202588.top

================================================================================
来源：http://fib.smart0.xyz

A. 基础语法与类型
来源：http://ibr.sysykeji.top

================================================================================
来源：http://zwn.gzhubu.top

[A01] Hello World
来源：http://spb.nanxuanxn.top

Py:   print("Hello, World!")
来源：http://dxi.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://ksa.haohaochexian.top

JS:   console.log("Hello, World!");
来源：http://imu.aizwys.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iae.wangdashe.top

Java: System.out.println("Hello, World!");
来源：http://rvo.yj202588.top

Go:   fmt.Println("Hello, World!")
来源：http://uie.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://tku.tianlin.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://nhv.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://lbe.hnqzz.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fus.yangfankeji.com

PHP:  $name = "Alex"; $age = 20;
来源：http://xbv.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://oep.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://enh.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://udk.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://zyl.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://acw.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://opm.bjfxy.top

[A03] 常量定义
来源：http://jxu.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gpe.nanxinkj.top

PHP:  const PI = 3.14159;
来源：http://zwg.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://qkm.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://rlb.xziqi.cn

Java: static final double PI = 3.14159;
来源：http://jcq.ydjk.org.cn

Go:   const PI = 3.14159
来源：http://vbq.vehdjk.com

Ruby: PI = 3.14159
来源：http://kil.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://hhn.sufxvd.cn

[A04] 判断变量类型
来源：http://jvu.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pwk.jiagoushi.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fbm.fzhhl.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://amo.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://eoc.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://akw.cucudq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pmy.epnwcf.com

Ruby: x.class; x.is_a?(Integer)
来源：http://uiw.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://bpl.hammf.cn

[A05] 整数除法与取模
来源：http://oix.zhoulong.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pim.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qcg.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lwi.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iss.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://vky.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://ipd.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://aug.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://vzo.hongshengwenyu.top

[A06] 字符串转数字
来源：http://iws.yongpay.top

Py:   int("42"); float("3.14")
来源：http://mkd.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dze.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lhn.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nhr.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mdl.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mmo.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ezj.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ubw.epnwcf.com

[A07] 数字转字符串
来源：http://jhs.xylfe.cn

Py:   str(42)
来源：http://haz.nanxuanxn.top

PHP:  (string) 42; strval(42)
来源：http://zuc.jqgfzy.top

JS:   String(42); (42).toString()
来源：http://iye.sjlbkw.cn

TS:   String(42)
来源：http://qwq.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nyk.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://uej.guannengcc.top

Ruby: 42.to_s
来源：http://out.hongshengwenyu.top

C#:   42.ToString()
来源：http://awd.daxiang520.top

[A08] 取整与四舍五入
来源：http://gie.shzxlz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vog.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qta.daria6918.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nrw.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lkl.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ajm.gaohongyu789.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ayh.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://avw.316326.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kka.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://qrh.bjfxy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jzh.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iir.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qmw.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vbq.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kqg.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nkj.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hyn.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pxu.hfpthk.cn

[A10] 生成随机数
来源：http://tbp.bbcook.cn

Py:   import random; random.randint(1, 100)
来源：http://uvb.xinyue.icu

PHP:  random_int(1, 100);
来源：http://vng.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pnz.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kox.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://yge.sysykeji.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zod.ctjpmb.com

Ruby: rand(1..100)
来源：http://lyr.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://zhd.havefunace.top

[A11] 条件表达式（三元）
来源：http://owh.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://yhs.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wha.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://xvu.fktsv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wqr.jlsjyb.cn

Java: x > 0 ? "yes" : "no"
来源：http://hrb.zdqjudy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sdc.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://imq.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://ymh.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://qnh.yj20258888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kgi.hongshengwenyu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yjr.wangdashe.top

JS:   `Hello, ${name}!`
来源：http://kni.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://mqt.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://txz.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oqp.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://ceq.ydjk.org.cn

C#:   $"Hello, {name}!"
来源：http://nuf.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mix.hnqzz.top

Py:   "第一行\n第二行"
来源：http://ytw.jqgufenzy.top

PHP:  "第一行\n第二行"
来源：http://eel.vehdjk.com

JS:   "第一行\n第二行"
来源：http://hed.epnwcf.com

TS:   "第一行\n第二行"
来源：http://kph.yfazqb.com

Java: "第一行\n第二行"
来源：http://kee.ybcxt.top

Go:   "第一行\n第二行"
来源：http://sey.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://yyt.9152youxi.cn

C#:   "第一行\n第二行"
来源：http://kdl.guannengcc.top

[A14] 注释写法
来源：http://yrn.hnqzz.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cka.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://cjc.jiagoushi.top

JS:   // 单行；/* 多行 */
来源：http://jpt.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://qhy.zdqjudy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dhg.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://tnk.sysykeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://dyr.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://ekq.zdqjudy.top

[A15] 空值判断与默认值
来源：http://wac.cqqwz.cn

Py:   value = data or "默认值"
来源：http://tol.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://flj.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://whq.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://blk.uphjek.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vpm.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://vdh.dianchejie.cn

Ruby: value = data || "默认值"
来源：http://thn.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://mjx.andypj.xyz

[A16] 真假值判断规则
来源：http://zxb.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bzz.yj202588.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nai.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yhs.zhengqikj.top

TS:   if (!x) {}
来源：http://edh.gzhubu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://juo.tanke756.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iri.0kj1m.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kzv.yvedp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://deg.ivvv.top

[A17] 位运算
来源：http://jaq.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymv.fanxiaobao.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pzc.shuidangran.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xqt.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jlj.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lws.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cik.hammf.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qog.vqdsnc.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vcw.mhx1999.top


<!-- 参考信息 -->