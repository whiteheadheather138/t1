代发 wailian999

[U101] JS：classList 操作
来源：http://vgd.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://rmd.xinyue.icu

[U102] JS：本地存储
来源：http://uvb.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jpc.aibaodan.cn

[U103] JS：定时器
来源：http://von.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hbn.andypj.xyz

[U104] JS：防抖
来源：http://vzb.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oyq.cucudq.cn

[U105] JS：节流
来源：http://kur.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://epv.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://thb.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fev.havefunace.top

[U107] JS：数字千分位
来源：http://juf.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mbc.0kj1m.cn

[U108] JS：随机整数
来源：http://rrw.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hub.pengpengdd.cyou

[U109] JS：数组分组
来源：http://bkk.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://wlz.jyoumei.cn

[U110] JS：数组分块
来源：http://zsj.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjr.fktsv.cn

[U111] JS：对象转 Map
来源：http://suf.yonumen.top

new Map(Object.entries(obj))
来源：http://fzq.yuanzhike.top

[U112] JS：字符串补位
来源：http://nfz.zhongyouzk.top

"7".padStart(3, "0")
来源：http://has.nanxinkj.top

[U113] JS：正则替换全部
来源：http://fnr.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://cxo.yfazqb.com

[U114] JS：JSON 深比较
来源：http://rbc.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://lja.yongpay.top

[U115] JS：生成 UUID
来源：http://ska.bjfxy.top

crypto.randomUUID()
来源：http://jzk.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://ygt.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://uoa.zycfv.cn

[U117] JS：单元测试
来源：http://kpz.yj202588.top

npm i -D vitest;  npx vitest
来源：http://avv.9152youxi.cn

[U118] JS：开发服务器
来源：http://bls.jiagoushi.top

npm i -D vite;  npx vite
来源：http://qve.xuetiantiany.cn

[U119] JS：生产构建
来源：http://yiw.chenzaomai.com

npx vite build
来源：http://uzp.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://unh.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://heo.hysaishi.cn

================================================================================
来源：http://meq.316326.xyz

统计汇总
来源：http://jqk.0kj1m.cn

================================================================================
来源：http://ztk.daxiang520.top

按语言统计（条）：
来源：http://rpe.yongpay.top

Python ......... 252
来源：http://uik.hongshengwenyu.top

PHP ............ 252
来源：http://hyn.daxiang520.top

JavaScript ..... 252
来源：http://mnz.yanxiufei.cn

TypeScript ..... 212
来源：http://lrv.shzxlz.cn

Java ........... 212
来源：http://vaa.zhengqikj.top

Go ............. 212
来源：http://qji.jinqigfzy.top

Ruby ........... 212
来源：http://dku.redwolf501.top

C# ............. 212
来源：http://hll.sweek.top

C .............. 30
来源：http://eio.dashuyun.cn

C++ ............ 30
来源：http://dum.quarkkingdee.top

SQL ............ 90
来源：http://lrh.shanyushiyangkeji.top

Bash ........... 80
来源：http://afb.yonumen.top

Kotlin ......... 15
来源：http://ilo.jyoumei.cn

Swift .......... 15
来源：http://ngk.haohaochexian.top

Lua ............ 10
来源：http://xrd.guannengcc.top

Perl ........... 10
来源：http://per.havefunace.top

Scala .......... 10
来源：http://qbk.tian-w.cn

------------------------------------
来源：http://dyj.zhixingplan.top

合计 ........... 2106 条
来源：http://uiq.jinqigfzy.top

按章节统计：
来源：http://mxw.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xii.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lox.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ack.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bnt.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gza.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tcf.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qxg.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iip.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ahd.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mrx.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://clo.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eqg.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zxw.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iis.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zhw.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spa.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://fkz.hesvh.cn

R Bash 专题                             80
来源：http://xpi.zhoulong.xyz

S C / C++ 专题                          60
来源：http://elr.jqgfzy.top

T 其他语言补充                          60
来源：http://bik.yfazqb.com

U 高频实用片段                         120
来源：http://ekz.hfpthk.cn

------------------------------------
来源：http://lsw.jinqigufen.top

合计                                  2106 条
来源：http://lcd.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://jah.sweek.top

使用提醒
来源：http://czo.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://ieq.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://smv.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hoy.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lqt.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mhu.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://atv.sweek.top

—— 文件结束 ——
来源：http://akd.cucudq.cn

================================================================================
来源：http://oog.dianchejie.cn

程序语言常见例子速查手册（2024 版）
来源：http://bhm.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://soe.cucudq.cn

================================================================================
来源：http://fcw.haohaochexian.top

【收录内容】
来源：http://rtz.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://hoe.hcnkem.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hkx.sufxvd.cn

SQL · Bash · C · C++
来源：http://jao.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hxd.jqgufenzy.top

【使用说明】
来源：http://bbw.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iam.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ubj.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mpe.hongshengwenyu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vei.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bbi.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aue.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xdf.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ajq.aizwys.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pgo.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pmy.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ppf.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ugz.bjfxy.top

【文件统计】
来源：http://fbh.kuanghao11.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xtc.nwbrower.top

--------------------------------------------------------------------------------
来源：http://uzx.9152youxi.cn

目  录
来源：http://fwg.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://qua.aibaodan.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kdi.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oea.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qyd.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mkm.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vbu.jlsjyb.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://enf.hcnkem.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mof.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kai.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://iwt.gzhubu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hcz.sufxvd.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bvk.aibaodan.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ooy.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cjf.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gwj.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xdt.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lip.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pfn.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rkf.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zuq.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zvb.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nbf.tanke756.top

================================================================================
来源：http://lvn.yueranfly.top

A. 基础语法与类型
来源：http://sht.chenzaomai.com

================================================================================
来源：http://wqq.feifeiyinyue.top

[A01] Hello World
来源：http://xoj.hammf.cn

Py:   print("Hello, World!")
来源：http://fek.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://fzh.meibo888.top

JS:   console.log("Hello, World!");
来源：http://ldj.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bom.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://wsg.xinyue.icu

Go:   fmt.Println("Hello, World!")
来源：http://ctr.cqqwz.cn

Ruby: puts "Hello, World!"
来源：http://ygq.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://grg.xinyue.icu

[A02] 变量声明与赋值
来源：http://rrj.zhiwuduotai.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lyw.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vhs.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://zae.hywenlv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oak.zhengqikj.top

Java: String name = "Alex"; int age = 20;
来源：http://nhj.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://oii.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://mmy.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://nmf.ehwqpu.com

[A03] 常量定义
来源：http://ppd.fktsv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vbp.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://rxv.jqgfzy.top

JS:   const PI = 3.14159;
来源：http://lqt.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://mwg.yj202588.top

Java: static final double PI = 3.14159;
来源：http://hfg.sxryk.cn

Go:   const PI = 3.14159
来源：http://nwu.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://dgn.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://dbj.wangdashe.top

[A04] 判断变量类型
来源：http://mtv.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://brd.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tdh.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://poo.pengpengdd.cyou

TS:   typeof x; x instanceof Date
来源：http://xau.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ddi.yongpay.top

Go:   reflect.TypeOf(x).Name()
来源：http://fmj.xuetiantiany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ame.jlsjyb.cn

C#:   x.GetType().Name; x is int
来源：http://xki.jqgufenzy.top

[A05] 整数除法与取模
来源：http://jof.yj20258.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pfr.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ygh.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rye.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kde.yongpay.top

Java: 7 / 2; 7 % 2
来源：http://haw.guannengcc.top

Go:   7 / 2; 7 % 2
来源：http://aik.316326.xyz

Ruby: 7 / 2; 7 % 2
来源：http://btq.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://myl.haohaochexian.top

[A06] 字符串转数字
来源：http://dhs.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://cpp.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lzu.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zxq.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://zgv.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pit.jianghu66.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rpm.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pvb.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pci.haohaochexian.top

[A07] 数字转字符串
来源：http://wzj.shuidangran.top

Py:   str(42)
来源：http://okd.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://vii.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://zvo.gzhubu.top

TS:   String(42)
来源：http://dxr.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dnw.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://ybv.gotoacloud.top

Ruby: 42.to_s
来源：http://ech.xziqi.cn

C#:   42.ToString()
来源：http://ezw.aibaodan.cn

[A08] 取整与四舍五入
来源：http://rwp.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iep.yuxming.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ltw.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iug.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ydd.ehwqpu.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ppy.yj20258.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tif.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yir.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://esq.guannengcc.top

[A09] 绝对值与最大最小值
来源：http://qpv.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hqb.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xfv.cucudq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://imw.aizwys.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jvw.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gdf.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qrh.haohaochexian.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cta.zhiwuduotai.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iqz.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://uqn.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://dop.sysykeji.top

PHP:  random_int(1, 100);
来源：http://ibc.cqqwz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cnd.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gpb.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://usx.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sfq.jiagoushi.top

Ruby: rand(1..100)
来源：http://ahf.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://dzc.mhx1999.top

[A11] 条件表达式（三元）
来源：http://kcj.yanxiufei.cn

Py:   "yes" if x > 0 else "no"
来源：http://vbf.ehwqpu.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://mql.ctjpmb.com

JS:   x > 0 ? "yes" : "no"
来源：http://ljy.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kav.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://dno.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kyn.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://lng.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://rcl.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://caj.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pjb.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mlb.jinghuilouyu.cn

JS:   `Hello, ${name}!`
来源：http://arr.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://nml.jyoumei.cn

Java: "Hello, %s!".formatted(name)
来源：http://prq.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eca.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://txe.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://wey.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hkx.xziqi.cn

Py:   "第一行\n第二行"
来源：http://xll.meibo888.top

PHP:  "第一行\n第二行"
来源：http://azu.fengsongda.top

JS:   "第一行\n第二行"
来源：http://omc.jyoumei.cn

TS:   "第一行\n第二行"
来源：http://bmh.zhengqikj.top

Java: "第一行\n第二行"
来源：http://ris.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://mtg.yongpay.top

Ruby: "第一行\n第二行"
来源：http://aim.shanyushiyangtech.top

C#:   "第一行\n第二行"
来源：http://tuf.shuidangran.top

[A14] 注释写法
来源：http://czg.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mbl.fengsongda.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://git.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://srs.0kj1m.cn

TS:   // 单行；/* 多行 */
来源：http://yyf.yj20258888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xox.yangfankeji.com

Go:   // 单行；/* 多行 */
来源：http://pkz.hesvh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xvm.tian-w.cn

C#:   // 单行；/* 多行 */
来源：http://ncm.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://kim.jinqigfzy.top

Py:   value = data or "默认值"
来源：http://xia.jiagoushi.top

PHP:  $value = $data ?? "默认值";
来源：http://vkx.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://dxb.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://drn.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wmi.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://alb.zycfv.cn

Ruby: value = data || "默认值"
来源：http://ryt.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://xsg.epnwcf.com

[A16] 真假值判断规则
来源：http://ivx.daxiang520.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qfx.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xrx.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zmz.cdnleiting.top

TS:   if (!x) {}
来源：http://ajo.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pen.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dlx.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://oqy.daria6918.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kub.zhijiandao.cn

[A17] 位运算
来源：http://wyr.daxiang520.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smr.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zcm.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uaq.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://reb.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://egr.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hwk.fehbvm.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://asz.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rss.daxiang520.top


<!-- 参考信息 -->