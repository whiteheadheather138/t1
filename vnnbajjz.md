代发 wailian999

[U103] JS：定时器
来源：http://kyv.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vku.gotoacloud.top

[U104] JS：防抖
来源：http://sfp.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsn.ctjpmb.com

[U105] JS：节流
来源：http://lej.aizwys.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sul.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://smw.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fij.hnxiangtu.top

[U107] JS：数字千分位
来源：http://doh.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xmj.zhongyouzk.top

[U108] JS：随机整数
来源：http://mzl.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ewe.kuanghao11.cn

[U109] JS：数组分组
来源：http://pov.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://oaa.hesvh.cn

[U110] JS：数组分块
来源：http://ale.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qcy.zhixingplan.top

[U111] JS：对象转 Map
来源：http://ovf.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://sxx.aizwys.cn

[U112] JS：字符串补位
来源：http://xfk.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://zbf.jiagoushi.top

[U113] JS：正则替换全部
来源：http://jft.yj20258888.top

s.replaceAll("a", "b")
来源：http://rcm.ivvv.top

[U114] JS：JSON 深比较
来源：http://kra.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iqd.guowangkeji.top

[U115] JS：生成 UUID
来源：http://vap.shangyingyoupin.top

crypto.randomUUID()
来源：http://cbh.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://lnh.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://bwi.kuanghao11.cn

[U117] JS：单元测试
来源：http://pgh.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://izq.jiagoushi.top

[U118] JS：开发服务器
来源：http://vcb.hammf.cn

npm i -D vite;  npx vite
来源：http://lly.zhijiandao.cn

[U119] JS：生产构建
来源：http://mjg.fengsongda.top

npx vite build
来源：http://jds.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://yso.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://psi.ehwqpu.com

================================================================================
来源：http://czl.fktsv.cn

统计汇总
来源：http://shu.jyoumei.cn

================================================================================
来源：http://drt.sjlbkw.cn

按语言统计（条）：
来源：http://yzp.yj20258888.top

Python ......... 252
来源：http://ymg.52xcode.cn

PHP ............ 252
来源：http://rar.tarul.cn

JavaScript ..... 252
来源：http://naa.sysykeji.top

TypeScript ..... 212
来源：http://shq.tarul.cn

Java ........... 212
来源：http://dvl.birdmap.top

Go ............. 212
来源：http://aeg.dianchejie.cn

Ruby ........... 212
来源：http://lza.zdbjq.cn

C# ............. 212
来源：http://xnj.ydjk.org.cn

C .............. 30
来源：http://lpu.haohaochexian.top

C++ ............ 30
来源：http://fbv.tanke756.top

SQL ............ 90
来源：http://foz.dashuyun.cn

Bash ........... 80
来源：http://xki.zhengqikj.top

Kotlin ......... 15
来源：http://gns.zhiwuduotai.top

Swift .......... 15
来源：http://euu.svipenyu.cn

Lua ............ 10
来源：http://fpm.vqdsnc.cn

Perl ........... 10
来源：http://tdn.hnxiangtu.top

Scala .......... 10
来源：http://azr.feifeiyinyue.top

------------------------------------
来源：http://mnq.vehdjk.com

合计 ........... 2106 条
来源：http://xvx.yongpay.top

按章节统计：
来源：http://tqb.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nfz.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uzl.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jvz.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qec.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tco.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jqr.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rib.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vai.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kyj.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zkc.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://npq.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ula.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pur.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kwa.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rdd.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vrh.shzxlz.cn

Q SQL 专题                              90
来源：http://mzn.xuetiantiany.cn

R Bash 专题                             80
来源：http://etf.ydzc1.top

S C / C++ 专题                          60
来源：http://lwe.wangdashe.top

T 其他语言补充                          60
来源：http://csl.cdnleiting.top

U 高频实用片段                         120
来源：http://mwe.hfpthk.cn

------------------------------------
来源：http://xnh.jiagoushi.top

合计                                  2106 条
来源：http://bmc.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://nzd.zhengqikj.top

使用提醒
来源：http://sem.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://tlz.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yzf.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tto.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://woi.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mlj.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fwo.cucudq.cn

—— 文件结束 ——
来源：http://bsr.jinqigufen.top

================================================================================
来源：http://pan.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://oup.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://wrz.jinqigfzy.top

================================================================================
来源：http://zgi.zdbjq.cn

【收录内容】
来源：http://wwt.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jji.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ttb.jianghu66.top

SQL · Bash · C · C++
来源：http://taw.wangdashe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hsl.zhoulong.xyz

【使用说明】
来源：http://spb.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yma.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qnw.yj202588.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://esu.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oqw.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rrk.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dtg.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://awz.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nwg.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jrq.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uje.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vyq.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hmv.gaohongyu789.top

【文件统计】
来源：http://fih.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kgi.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://fis.cashguo.top

目  录
来源：http://aad.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://qoa.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pin.quarkkingdee.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jiw.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://prb.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lqg.cdnleiting.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kzu.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://woj.xinyue.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wjs.mhx1999.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jvl.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ibq.yueranfly.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eqk.tarul.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rjp.shanyushiyangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lgq.hongshengwenyu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hxs.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nwm.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zmt.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://thr.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sia.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://fzq.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mvl.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukd.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vqr.zhixingplan.top

================================================================================
来源：http://oje.fzhhl.top

A. 基础语法与类型
来源：http://jtd.gzhubu.top

================================================================================
来源：http://dyt.ybcxt.top

[A01] Hello World
来源：http://lmj.ppjwa.cn

Py:   print("Hello, World!")
来源：http://wjg.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://lpk.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://vbc.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vip.hesvh.cn

Java: System.out.println("Hello, World!");
来源：http://swl.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://cze.jinghuilouyu.cn

Ruby: puts "Hello, World!"
来源：http://ndj.xziqi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kbz.fehbvm.com

[A02] 变量声明与赋值
来源：http://fsl.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yxn.shanyushiyangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lpz.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://eaz.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mxa.yfazqb.com

Java: String name = "Alex"; int age = 20;
来源：http://adt.shangyingyoupin.top

Go:   name := "Alex"; age := 20
来源：http://rzq.snrcjt.cn

Ruby: name = "Alex"; age = 20
来源：http://dia.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://beo.zhengqikj.top

[A03] 常量定义
来源：http://aak.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qsp.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://gfn.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://dfr.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://hfd.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://yra.ivvv.top

Go:   const PI = 3.14159
来源：http://xnd.jiagoushi.top

Ruby: PI = 3.14159
来源：http://tpb.shzxlz.cn

C#:   const double PI = 3.14159;
来源：http://vyb.smart0.xyz

[A04] 判断变量类型
来源：http://wcc.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pub.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://muk.sxryk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kdw.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://suc.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cjg.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://unu.hfpthk.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vdn.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://sua.quarkkingdee.top

[A05] 整数除法与取模
来源：http://gup.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://typ.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://bpj.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ybu.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://txb.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://geq.zdqjudy.top

Go:   7 / 2; 7 % 2
来源：http://bxq.yuxming.cn

Ruby: 7 / 2; 7 % 2
来源：http://bsp.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://wdc.hcnkem.com

[A06] 字符串转数字
来源：http://fjk.havefunace.top

Py:   int("42"); float("3.14")
来源：http://wsz.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://llo.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ffz.ybcxt.top

TS:   parseInt("42", 10); Number("42")
来源：http://bry.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://glm.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ebe.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://huw.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nmi.guowangkeji.top

[A07] 数字转字符串
来源：http://dbn.fengsongda.top

Py:   str(42)
来源：http://bow.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://rkb.havefunace.top

JS:   String(42); (42).toString()
来源：http://zza.chenlongwang.top

TS:   String(42)
来源：http://whi.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xzf.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://kky.hammf.cn

Ruby: 42.to_s
来源：http://cey.guowangkeji.top

C#:   42.ToString()
来源：http://uzk.ydzc1.top

[A08] 取整与四舍五入
来源：http://uri.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vxd.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hii.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zvz.zhoulong.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yxa.pengpengdd.cyou

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dbx.yj20258.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://por.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ceg.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://alm.nwbrower.top

[A09] 绝对值与最大最小值
来源：http://buj.yj20258.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://thq.sufxvd.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ddb.xylfe.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ehi.hnqzz.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tge.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kfk.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qtm.sufxvd.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yoh.ctjpmb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kht.andypj.xyz

[A10] 生成随机数
来源：http://gro.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://ffa.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://wrp.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yom.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tsi.fengsongda.top

Java: new Random().nextInt(100) + 1
来源：http://fgb.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yln.yfazqb.com

Ruby: rand(1..100)
来源：http://qes.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://qxq.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://pql.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://clk.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xsp.xylfe.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ich.hfpthk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lsk.daria6918.cn

Java: x > 0 ? "yes" : "no"
来源：http://cfu.zhongyouzk.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ecf.yj20258888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hws.ywan-chungtsiang.top

C#:   x > 0 ? "yes" : "no"
来源：http://vzb.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://iou.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dxo.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xvb.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://iab.yj20258.top

TS:   `Hello, ${name}!`
来源：http://bzt.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://zaz.yangfankeji.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ooc.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://prl.yfazqb.com

C#:   $"Hello, {name}!"
来源：http://iwa.ehwqpu.com

[A13] 多行字符串（练习 \n 转义）
来源：http://hss.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://quj.zycfv.cn

PHP:  "第一行\n第二行"
来源：http://tpq.bjfxy.top

JS:   "第一行\n第二行"
来源：http://uvh.meibo888.top

TS:   "第一行\n第二行"
来源：http://tqw.shuidangran.top

Java: "第一行\n第二行"
来源：http://viw.tarul.cn

Go:   "第一行\n第二行"
来源：http://bta.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://vqm.zhiwuduotai.top

C#:   "第一行\n第二行"
来源：http://kox.zycfv.cn

[A14] 注释写法
来源：http://kyu.vehdjk.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://xjx.yanxiufei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rcl.tarul.cn

JS:   // 单行；/* 多行 */
来源：http://wlw.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://lwk.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://poe.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://siz.smart0.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://fak.jqgfzy.top

C#:   // 单行；/* 多行 */
来源：http://gch.yonumen.top

[A15] 空值判断与默认值
来源：http://uqs.hammf.cn

Py:   value = data or "默认值"
来源：http://bim.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://jjc.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://qpq.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://rqe.hnxiangtu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yso.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://til.yj20258.top

Ruby: value = data || "默认值"
来源：http://zct.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://mdu.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://hog.jinqigfzy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ktw.nwbrower.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jmn.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jsg.yongpay.top

TS:   if (!x) {}
来源：http://jgj.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ipe.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qun.shanyushiyangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://kjz.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zaw.zhiwuduotai.top

[A17] 位运算
来源：http://gtg.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://feh.jiagoushi.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yce.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kit.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kmr.yanxiufei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dve.cashguo.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dpp.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ehv.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyb.hnqzz.top

[A18] 字符与 ASCII 码互转
来源：http://voc.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://afs.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://rul.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jfm.hammf.cn


<!-- 参考信息 -->