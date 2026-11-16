代发 wailian999

[U99] JS：事件监听
来源：http://jtc.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://nsv.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://dtq.hcnkem.com

document.querySelector(".item")
来源：http://ifq.jyoumei.cn

[U101] JS：classList 操作
来源：http://knh.yongpay.top

el.classList.toggle("active")
来源：http://vmq.zhiwuduotai.top

[U102] JS：本地存储
来源：http://cme.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://qsp.svipenyu.cn

[U103] JS：定时器
来源：http://vsa.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yam.yueranfly.top

[U104] JS：防抖
来源：http://dkr.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qym.hesvh.cn

[U105] JS：节流
来源：http://rtg.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://niw.fzhhl.top

[U106] JS：日期格式化
来源：http://wpo.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vdg.vqdsnc.cn

[U107] JS：数字千分位
来源：http://bwe.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bbp.sysykeji.top

[U108] JS：随机整数
来源：http://reh.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://icz.ivvv.top

[U109] JS：数组分组
来源：http://dfl.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://bzu.ydzc1.top

[U110] JS：数组分块
来源：http://wbq.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://phn.chenzaomai.com

[U111] JS：对象转 Map
来源：http://ufk.xylfe.cn

new Map(Object.entries(obj))
来源：http://mzl.yongpay.top

[U112] JS：字符串补位
来源：http://mex.hcnkem.com

"7".padStart(3, "0")
来源：http://qzs.svipenyu.cn

[U113] JS：正则替换全部
来源：http://hvh.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://jfb.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://nlt.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qvc.ehwqpu.com

[U115] JS：生成 UUID
来源：http://xap.ydjk.org.cn

crypto.randomUUID()
来源：http://gil.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://hfb.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://mwi.meibo888.top

[U117] JS：单元测试
来源：http://xlb.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://jnv.guannengcc.top

[U118] JS：开发服务器
来源：http://vzj.fktsv.cn

npm i -D vite;  npx vite
来源：http://cue.fanxiaobao.xyz

[U119] JS：生产构建
来源：http://gia.ehwqpu.com

npx vite build
来源：http://wsa.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ogt.sweek.top

import.meta.env.VITE_API_URL
来源：http://atd.daria6918.cn

================================================================================
来源：http://ewg.birdmap.top

统计汇总
来源：http://loy.tanke756.top

================================================================================
来源：http://bve.sjlbkw.cn

按语言统计（条）：
来源：http://pbo.chenzaomai.com

Python ......... 252
来源：http://weo.sweek.top

PHP ............ 252
来源：http://tyr.feifeiyinyue.top

JavaScript ..... 252
来源：http://lhc.shzxlz.cn

TypeScript ..... 212
来源：http://xqo.yj20258.top

Java ........... 212
来源：http://cqk.gzhubu.top

Go ............. 212
来源：http://aru.yj202588.top

Ruby ........... 212
来源：http://hpk.havefunace.top

C# ............. 212
来源：http://hkm.quarkkingdee.top

C .............. 30
来源：http://exh.hysaishi.cn

C++ ............ 30
来源：http://ujx.yuanzhike.top

SQL ............ 90
来源：http://gjb.zhoulong.xyz

Bash ........... 80
来源：http://vvt.feifeiyinyue.top

Kotlin ......... 15
来源：http://cca.yuanzhike.top

Swift .......... 15
来源：http://jar.yangfankeji.com

Lua ............ 10
来源：http://beq.zhengqikj.top

Perl ........... 10
来源：http://fdk.zhongyouzk.top

Scala .......... 10
来源：http://axj.jlsjyb.cn

------------------------------------
来源：http://hor.vehdjk.com

合计 ........... 2106 条
来源：http://otm.aibaodan.cn

按章节统计：
来源：http://bxu.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hnt.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qoq.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uln.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qpb.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xkx.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nqp.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lis.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rhb.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://huh.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mdi.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lkj.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cie.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ezc.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zkg.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fmh.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nmx.chenlongwang.top

Q SQL 专题                              90
来源：http://bvr.0kj1m.cn

R Bash 专题                             80
来源：http://rxb.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://hjz.quarkkingdee.top

T 其他语言补充                          60
来源：http://nyz.dashuyun.cn

U 高频实用片段                         120
来源：http://oxe.fengsongda.top

------------------------------------
来源：http://vnk.shzxlz.cn

合计                                  2106 条
来源：http://xpb.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://jhn.shangyingyoupin.top

使用提醒
来源：http://wke.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://wkt.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ijg.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tpz.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fxs.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://usg.nanxuanxn.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ulg.ywan-chungtsiang.top

—— 文件结束 ——
来源：http://jqc.zhongyouzk.top

================================================================================
来源：http://sfy.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://xzo.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://zhd.hcnkem.com

================================================================================
来源：http://hyj.cheryme.top

【收录内容】
来源：http://gcs.316326.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://roy.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iwc.chenlongwang.top

SQL · Bash · C · C++
来源：http://xxb.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nai.zhixingplan.top

【使用说明】
来源：http://yrl.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cdh.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vpi.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://azs.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://trd.jqgfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rww.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dcb.shanyushiyangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://csk.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zib.jqgufenzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pyx.cheryme.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jyk.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lgq.ctjpmb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jsw.52xcode.cn

【文件统计】
来源：http://ccc.shzxlz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tnu.yfazqb.com

--------------------------------------------------------------------------------
来源：http://jqe.gaohongyu789.top

目  录
来源：http://blo.gzhubu.top

--------------------------------------------------------------------------------
来源：http://mmc.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vlf.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xcg.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xwk.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jeu.gaohongyu789.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://npq.fzhhl.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qwg.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rxc.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xjy.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://npm.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rpl.birdmap.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xwk.gaohongyu789.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ieo.yj20258888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xwy.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mwp.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qim.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fcs.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vfk.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ejl.guannengcc.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xpz.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://poo.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jva.ivvv.top

================================================================================
来源：http://mot.tanke756.top

A. 基础语法与类型
来源：http://eyq.sysykeji.top

================================================================================
来源：http://unp.316326.xyz

[A01] Hello World
来源：http://enu.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://kny.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://xik.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://dmj.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xlt.yuanzhike.top

Java: System.out.println("Hello, World!");
来源：http://erq.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://gwb.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://ykg.c1oappe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hcd.bbcook.cn

[A02] 变量声明与赋值
来源：http://qjv.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qlw.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://juq.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://hzm.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bsk.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://kid.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://evn.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://vnb.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mke.ydzc1.top

[A03] 常量定义
来源：http://vtx.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hak.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://vrg.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://urr.vehdjk.com

TS:   const PI: number = 3.14159;
来源：http://txy.iojbl.cn

Java: static final double PI = 3.14159;
来源：http://jgx.0kj1m.cn

Go:   const PI = 3.14159
来源：http://pej.svipenyu.cn

Ruby: PI = 3.14159
来源：http://hvp.nanxinkj.top

C#:   const double PI = 3.14159;
来源：http://mgp.yj20258.top

[A04] 判断变量类型
来源：http://bdd.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sdg.hongshengwenyu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wea.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mmk.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://asr.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eol.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://ene.zhijiandao.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rsl.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://szb.jinqigufen.top

[A05] 整数除法与取模
来源：http://lpx.9152youxi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://crq.tianlin.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://wfx.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://muw.haohaochexian.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sks.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://bnt.zhijiandao.cn

Go:   7 / 2; 7 % 2
来源：http://fqr.jiagoushi.top

Ruby: 7 / 2; 7 % 2
来源：http://eyc.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://jim.zhongyouzk.top

[A06] 字符串转数字
来源：http://exa.zhaomingkeji.xyz

Py:   int("42"); float("3.14")
来源：http://jxl.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mvr.uphjek.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://clp.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://alk.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xyy.yonumen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dbj.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vbe.yj20258888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yba.ppjwa.cn

[A07] 数字转字符串
来源：http://lih.yuanzhike.top

Py:   str(42)
来源：http://ijs.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://cei.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://hmc.zhengqikj.top

TS:   String(42)
来源：http://chl.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://yqd.xziqi.cn

Go:   strconv.Itoa(42)
来源：http://jwc.aizwys.cn

Ruby: 42.to_s
来源：http://egh.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://npr.jinyuanbaomall.cn

[A08] 取整与四舍五入
来源：http://qhl.yvedp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://orw.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://foj.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jea.sweek.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mjf.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kll.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://phg.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jvk.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lop.hesvh.cn

[A09] 绝对值与最大最小值
来源：http://ycr.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://boa.jinqigufen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ena.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aey.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jvf.iojbl.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jxo.dianchejie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wiq.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ztv.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ehk.tarul.cn

[A10] 生成随机数
来源：http://qcw.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://hbz.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://jqi.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pms.nwbrower.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bib.vehdjk.com

Java: new Random().nextInt(100) + 1
来源：http://yoi.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://msb.pycfn.com

Ruby: rand(1..100)
来源：http://pxp.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://gtd.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://ebl.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://mav.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cke.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://kav.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mfk.hcnkem.com

Java: x > 0 ? "yes" : "no"
来源：http://chz.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wrb.cucudq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wch.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iwq.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://mls.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://glg.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iet.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://dvv.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://ner.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://rub.sweek.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://irn.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://kyy.hysaishi.cn

C#:   $"Hello, {name}!"
来源：http://gpf.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://nur.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://irz.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://qkf.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://chn.daxiang520.top

TS:   "第一行\n第二行"
来源：http://ikx.9152youxi.cn

Java: "第一行\n第二行"
来源：http://wtn.andypj.xyz

Go:   "第一行\n第二行"
来源：http://opo.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://hsw.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://pdg.fehbvm.com

[A14] 注释写法
来源：http://cqv.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://nix.pengpengdd.cyou

PHP:  // 或 # 单行；/* 多行 */
来源：http://oca.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://jmp.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://tvr.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kbd.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://hcb.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://ubb.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://jre.hcnkem.com

[A15] 空值判断与默认值
来源：http://ocj.shanyushiyangkeji.top

Py:   value = data or "默认值"
来源：http://gpx.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://smx.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://yfa.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://zok.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rdt.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://dtj.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://mcf.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://kkx.xylfe.cn

[A16] 真假值判断规则
来源：http://iep.gogol.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://otp.zhongyouzk.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zlt.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://upd.chenjidiqi.icu

TS:   if (!x) {}
来源：http://fvn.yj202588.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pwh.tian-w.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pfc.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://yzi.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://msc.daxiang520.top

[A17] 位运算
来源：http://pkn.yanxiufei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wbx.xuanzx.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zch.xylfe.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tmb.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gwt.52xcode.cn


<!-- 参考信息 -->