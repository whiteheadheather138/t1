代发 wailian999

[U103] JS：定时器
来源：http://alb.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kvl.ybcxt.top

[U104] JS：防抖
来源：http://gjl.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://llc.cheryme.top

[U105] JS：节流
来源：http://cgl.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fdy.aibaodan.cn

[U106] JS：日期格式化
来源：http://qau.cheryme.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pzs.guannengcc.top

[U107] JS：数字千分位
来源：http://pkd.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wnv.zhongyouzk.top

[U108] JS：随机整数
来源：http://lhg.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xdf.xylfe.cn

[U109] JS：数组分组
来源：http://hfx.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://knv.zhongyouzk.top

[U110] JS：数组分块
来源：http://iyr.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ecz.havefunace.top

[U111] JS：对象转 Map
来源：http://sqx.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://fwp.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://cza.tian-w.cn

"7".padStart(3, "0")
来源：http://nsq.yuxming.cn

[U113] JS：正则替换全部
来源：http://mzl.jyoumei.cn

s.replaceAll("a", "b")
来源：http://ndx.ydzc1.top

[U114] JS：JSON 深比较
来源：http://jha.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tob.yanxiufei.cn

[U115] JS：生成 UUID
来源：http://zcr.hesvh.cn

crypto.randomUUID()
来源：http://enp.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://fmi.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://pgb.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://mnm.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://ywe.fzhhl.top

[U118] JS：开发服务器
来源：http://aan.zdqjudy.top

npm i -D vite;  npx vite
来源：http://cdi.52xcode.cn

[U119] JS：生产构建
来源：http://iep.tianlin.xyz

npx vite build
来源：http://hck.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://pxf.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://pmj.guowangkeji.top

================================================================================
来源：http://gjb.zhiwuduotai.top

统计汇总
来源：http://eie.yj20258.top

================================================================================
来源：http://siw.tianlin.xyz

按语言统计（条）：
来源：http://iry.jyoumei.cn

Python ......... 252
来源：http://veg.yj20258888.top

PHP ............ 252
来源：http://ypc.redwolf501.top

JavaScript ..... 252
来源：http://tzx.redwolf501.top

TypeScript ..... 212
来源：http://xke.yonumen.top

Java ........... 212
来源：http://czm.shanyushiyangkeji.top

Go ............. 212
来源：http://oeg.jlsjyb.cn

Ruby ........... 212
来源：http://qcp.fzhhl.top

C# ............. 212
来源：http://gls.shanyushiyangtech.top

C .............. 30
来源：http://cyd.yonumen.top

C++ ............ 30
来源：http://ixe.shuidangran.top

SQL ............ 90
来源：http://mtk.ydjk.org.cn

Bash ........... 80
来源：http://ski.smart0.xyz

Kotlin ......... 15
来源：http://jto.nwbrower.top

Swift .......... 15
来源：http://jxq.tian-w.cn

Lua ............ 10
来源：http://myv.hnqzz.top

Perl ........... 10
来源：http://uqa.ppjwa.cn

Scala .......... 10
来源：http://ell.zhengqikj.top

------------------------------------
来源：http://ynn.chenlongwang.top

合计 ........... 2106 条
来源：http://ywj.cdnleiting.top

按章节统计：
来源：http://qse.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oqv.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gbi.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://noc.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xcc.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nlr.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ftp.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wxv.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wbe.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zxn.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rte.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vvj.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://auh.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wml.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ssr.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hgf.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bhb.zhixingplan.top

Q SQL 专题                              90
来源：http://lww.fanxiaobao.xyz

R Bash 专题                             80
来源：http://tzx.hcnkem.com

S C / C++ 专题                          60
来源：http://kum.jiagoushi.top

T 其他语言补充                          60
来源：http://evf.havefunace.top

U 高频实用片段                         120
来源：http://kpn.gogol.net.cn

------------------------------------
来源：http://zan.zhongyouzk.top

合计                                  2106 条
来源：http://ynv.yueranfly.top

--------------------------------------------------------------------------------
来源：http://wmu.zhoulong.xyz

使用提醒
来源：http://glg.hcnkem.com

--------------------------------------------------------------------------------
来源：http://ava.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://euh.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jyk.xingfuxueyuan.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ave.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wgv.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uys.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://rvn.dianchejie.cn

================================================================================
来源：http://rcw.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://vex.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://mqo.ehwqpu.com

================================================================================
来源：http://aor.zdqjudy.top

【收录内容】
来源：http://lbw.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bvp.zhengqikj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uds.jiagoushi.top

SQL · Bash · C · C++
来源：http://bao.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://czi.yj202588.top

【使用说明】
来源：http://wjj.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xkx.bbcook.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hzs.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nec.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ywb.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tio.sweek.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gyg.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hbc.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iyz.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sjv.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kab.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://npl.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wtx.tian-w.cn

【文件统计】
来源：http://ueq.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sun.yuxming.cn

--------------------------------------------------------------------------------
来源：http://vqd.ydjk.org.cn

目  录
来源：http://bjf.andypj.xyz

--------------------------------------------------------------------------------
来源：http://sgi.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fml.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jqd.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ewe.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rlz.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dsf.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vmc.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kzt.xylfe.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hdq.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xvp.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pol.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aop.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wkg.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xae.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://erc.tian-w.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wdv.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wbk.zhaomingkeji.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ygy.yueranfly.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fhi.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aew.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xdr.yonumen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://toq.daria6918.cn

================================================================================
来源：http://dat.chenzaomai.com

A. 基础语法与类型
来源：http://ohp.yj20258888.top

================================================================================
来源：http://gzv.tanke756.top

[A01] Hello World
来源：http://qwq.sufxvd.cn

Py:   print("Hello, World!")
来源：http://yoj.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://irr.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://cfj.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tgz.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://feb.cheryme.top

Go:   fmt.Println("Hello, World!")
来源：http://qyz.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://pxj.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wzk.hywenlv.cn

[A02] 变量声明与赋值
来源：http://zvc.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qgj.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jos.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://oem.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pip.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://ctm.tian-w.cn

Go:   name := "Alex"; age := 20
来源：http://dic.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://icf.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ivh.jinqigufen.top

[A03] 常量定义
来源：http://ipf.sysykeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yug.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://ndd.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://eyg.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://yfo.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://odh.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://vzj.ybcxt.top

Ruby: PI = 3.14159
来源：http://sze.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://cuz.gzhubu.top

[A04] 判断变量类型
来源：http://wis.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://fuw.zhengqikj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kkd.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://siq.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://ils.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vcb.gaohongyu789.top

Go:   reflect.TypeOf(x).Name()
来源：http://dbw.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bxp.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://vap.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://iqb.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lhb.tarul.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://swl.birdmap.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ycv.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gen.cashguo.top

Java: 7 / 2; 7 % 2
来源：http://lop.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://scx.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://ayr.jiagoushi.top

C#:   7 / 2; 7 % 2
来源：http://vey.yonumen.top

[A06] 字符串转数字
来源：http://vto.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://iaa.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lmj.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hmx.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://xux.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gmc.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qgb.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://mll.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vmr.xylfe.cn

[A07] 数字转字符串
来源：http://wvf.zhijiandao.cn

Py:   str(42)
来源：http://ama.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://rfi.cqqwz.cn

JS:   String(42); (42).toString()
来源：http://xas.xylfe.cn

TS:   String(42)
来源：http://mca.ywan-chungtsiang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vez.zhijiandao.cn

Go:   strconv.Itoa(42)
来源：http://syx.jinqigufen.top

Ruby: 42.to_s
来源：http://hpz.guowangkeji.top

C#:   42.ToString()
来源：http://lvt.fzhhl.top

[A08] 取整与四舍五入
来源：http://xzh.yanxiufei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ocl.zhixingplan.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dyw.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rhl.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sdw.xziqi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://khp.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ybm.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://klj.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mlu.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://lnq.shangyingyoupin.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bgv.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://who.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yvy.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://phi.fengsongda.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xuc.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jyj.zhiwuduotai.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kuq.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xdk.tianlin.xyz

[A10] 生成随机数
来源：http://jfw.hcnkem.com

Py:   import random; random.randint(1, 100)
来源：http://gsn.jinghuilouyu.cn

PHP:  random_int(1, 100);
来源：http://bdx.smart0.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vvl.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aqm.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://sgv.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://drh.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://aqe.yuanzhike.top

C#:   new Random().Next(1, 101)
来源：http://lqk.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://veh.feifeiyinyue.top

Py:   "yes" if x > 0 else "no"
来源：http://bhg.chenjidiqi.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://fxr.zhoulong.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://yvv.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://mvc.nwbrower.top

Java: x > 0 ? "yes" : "no"
来源：http://vef.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cft.bjfxy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cqs.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eoi.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://tmc.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://anz.dashuyun.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hju.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://hcv.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://knw.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://icy.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xnp.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://omm.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://zpx.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zpt.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://zyi.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://rqr.yj20258888.top

JS:   "第一行\n第二行"
来源：http://igl.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://neo.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://ggr.xylfe.cn

Go:   "第一行\n第二行"
来源：http://zuv.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://org.jinqigufen.top

C#:   "第一行\n第二行"
来源：http://vmr.yueranfly.top

[A14] 注释写法
来源：http://fmc.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://drt.chenzaomai.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://cgs.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://cte.snrcjt.cn

TS:   // 单行；/* 多行 */
来源：http://tcw.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gec.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://qjy.snrcjt.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qdn.ivvv.top

C#:   // 单行；/* 多行 */
来源：http://mct.fzhhl.top

[A15] 空值判断与默认值
来源：http://eav.hnqzz.top

Py:   value = data or "默认值"
来源：http://apb.jinqigfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://diy.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://dfs.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://cks.ppjwa.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nil.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://rwz.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://xae.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://mpc.cdnleiting.top

[A16] 真假值判断规则
来源：http://fug.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jzr.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oti.yj20258888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gvp.zycfv.cn

TS:   if (!x) {}
来源：http://rcg.yj20258.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ehk.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mjg.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://wkc.yuanzhike.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tlw.aizwys.cn

[A17] 位运算
来源：http://cid.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://huv.feifeiyinyue.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vba.vqdsnc.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqs.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uox.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzp.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cct.guowangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dqj.aizwys.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://koc.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://fbv.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://ged.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://msy.zhengqikj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wde.hnqzz.top


<!-- 参考信息 -->