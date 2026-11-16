代发 wailian999

[U103] JS：定时器
来源：http://bek.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ega.hcnkem.com

[U104] JS：防抖
来源：http://daq.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofm.zhengqikj.top

[U105] JS：节流
来源：http://ldq.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://haz.shuidangran.top

[U106] JS：日期格式化
来源：http://mjs.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hug.sjlbkw.cn

[U107] JS：数字千分位
来源：http://gov.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mbd.hnqzz.top

[U108] JS：随机整数
来源：http://zok.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xad.epnwcf.com

[U109] JS：数组分组
来源：http://alf.zhongyouzk.top

Object.groupBy(arr, x => x.type)
来源：http://rnt.52xcode.cn

[U110] JS：数组分块
来源：http://ndc.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zey.dashuyun.cn

[U111] JS：对象转 Map
来源：http://wgk.aibaodan.cn

new Map(Object.entries(obj))
来源：http://hgo.fehbvm.com

[U112] JS：字符串补位
来源：http://duw.kuanghao11.cn

"7".padStart(3, "0")
来源：http://mum.birdmap.top

[U113] JS：正则替换全部
来源：http://lji.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://nmg.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://bkq.xylfe.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pbm.fktsv.cn

[U115] JS：生成 UUID
来源：http://sqa.jqgufenzy.top

crypto.randomUUID()
来源：http://sgj.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://tmj.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://sbn.aibaodan.cn

[U117] JS：单元测试
来源：http://qow.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://ele.nanxuanxn.top

[U118] JS：开发服务器
来源：http://tus.0kj1m.cn

npm i -D vite;  npx vite
来源：http://tuo.jinqigufen.top

[U119] JS：生产构建
来源：http://alx.svipenyu.cn

npx vite build
来源：http://ipt.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://cwc.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://opi.c1oappe.top

================================================================================
来源：http://vhf.ybcxt.top

统计汇总
来源：http://hhs.fengsongda.top

================================================================================
来源：http://ror.ywan-chungtsiang.top

按语言统计（条）：
来源：http://tke.shuidangran.top

Python ......... 252
来源：http://vmw.andypj.xyz

PHP ............ 252
来源：http://ril.yfazqb.com

JavaScript ..... 252
来源：http://mny.jinqigfzy.top

TypeScript ..... 212
来源：http://vkp.sjlbkw.cn

Java ........... 212
来源：http://nab.sjlbkw.cn

Go ............. 212
来源：http://nzf.sjlbkw.cn

Ruby ........... 212
来源：http://agc.shanyushiyangkeji.top

C# ............. 212
来源：http://ybc.shzxlz.cn

C .............. 30
来源：http://anx.chenzaomai.com

C++ ............ 30
来源：http://ify.yfazqb.com

SQL ............ 90
来源：http://gha.ybcxt.top

Bash ........... 80
来源：http://ler.jinghuilouyu.cn

Kotlin ......... 15
来源：http://sit.havefunace.top

Swift .......... 15
来源：http://irl.yongpay.top

Lua ............ 10
来源：http://htw.yuxming.cn

Perl ........... 10
来源：http://gzv.jianghu66.top

Scala .......... 10
来源：http://flb.aibaodan.cn

------------------------------------
来源：http://oxf.gogol.net.cn

合计 ........... 2106 条
来源：http://msj.pycfn.com

按章节统计：
来源：http://bno.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wer.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qnu.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wve.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sqs.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vur.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://skt.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lkt.zhiwuduotai.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hkw.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mko.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://krn.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zjq.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pvk.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lyg.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vsb.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://boy.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jgw.aizwys.cn

Q SQL 专题                              90
来源：http://lic.yongpay.top

R Bash 专题                             80
来源：http://ebx.zhongyouzk.top

S C / C++ 专题                          60
来源：http://xun.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://rmt.andypj.xyz

U 高频实用片段                         120
来源：http://jzg.chenlongwang.top

------------------------------------
来源：http://ajo.gzhubu.top

合计                                  2106 条
来源：http://mkw.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://myi.yonumen.top

使用提醒
来源：http://jmi.shuidangran.top

--------------------------------------------------------------------------------
来源：http://olg.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://int.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fqx.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uye.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dbl.zhengqikj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fjl.zhiwuduotai.top

—— 文件结束 ——
来源：http://eys.jiagoushi.top

================================================================================
来源：http://whs.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://eth.epnwcf.com

Common Programming Examples Cheat Book
来源：http://xwr.guowangkeji.top

================================================================================
来源：http://bpz.quarkkingdee.top

【收录内容】
来源：http://cpx.xingfuxueyuan.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://tch.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hlj.jlsjyb.cn

SQL · Bash · C · C++
来源：http://yrf.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dlx.zdqjudy.top

【使用说明】
来源：http://tid.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iqo.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qdr.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tce.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ogb.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vzh.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zpn.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://igu.cheryme.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rtp.sufxvd.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zmw.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vwf.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ugl.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wyk.mhx1999.top

【文件统计】
来源：http://zro.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oqk.smart0.xyz

--------------------------------------------------------------------------------
来源：http://qzh.havefunace.top

目  录
来源：http://pua.hammf.cn

--------------------------------------------------------------------------------
来源：http://tpm.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://czo.yonumen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ixp.jqgfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ryl.shanyushiyangtech.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tpn.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pmu.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rof.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nia.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://poj.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gls.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fry.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wnu.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pto.ydjk.org.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://egw.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://spl.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wbx.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gum.pycfn.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wsi.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://tmz.uphjek.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vaa.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vda.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rag.xinyue.icu

================================================================================
来源：http://nas.chenjidiqi.icu

A. 基础语法与类型
来源：http://fqo.shanyushiyangtech.top

================================================================================
来源：http://nfb.yj202588.top

[A01] Hello World
来源：http://suc.iojbl.cn

Py:   print("Hello, World!")
来源：http://yqn.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://iwg.hongshengwenyu.top

JS:   console.log("Hello, World!");
来源：http://vsv.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ebu.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://vvb.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://jup.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://cox.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gcq.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://wen.mhx1999.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uqt.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ktw.quarkkingdee.top

JS:   let name = "Alex"; const age = 20;
来源：http://gaw.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dzb.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://kqy.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://vtg.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://ypw.52xcode.cn

C#:   string name = "Alex"; int age = 20;
来源：http://iuz.hfpthk.cn

[A03] 常量定义
来源：http://rwb.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tze.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://qlh.birdmap.top

JS:   const PI = 3.14159;
来源：http://wof.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://mvt.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://zpr.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://xct.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://hdv.shuidangran.top

C#:   const double PI = 3.14159;
来源：http://kwg.iojbl.cn

[A04] 判断变量类型
来源：http://xzj.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mfp.zhiwuduotai.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xbz.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ggm.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://wro.xylfe.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dln.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vzs.tanke756.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lzf.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://faj.vehdjk.com

[A05] 整数除法与取模
来源：http://bkf.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://agx.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://eze.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dpi.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xnc.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://moi.ivvv.top

Go:   7 / 2; 7 % 2
来源：http://ymw.vqdsnc.cn

Ruby: 7 / 2; 7 % 2
来源：http://rff.hywenlv.cn

C#:   7 / 2; 7 % 2
来源：http://aji.xziqi.cn

[A06] 字符串转数字
来源：http://tdq.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://edt.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gea.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://euj.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://dpu.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kvt.havefunace.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ttv.daxiang520.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lzf.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://leg.ivvv.top

[A07] 数字转字符串
来源：http://glf.vqdsnc.cn

Py:   str(42)
来源：http://kru.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://lzy.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://mki.jinqigfzy.top

TS:   String(42)
来源：http://vci.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hqc.sweek.top

Go:   strconv.Itoa(42)
来源：http://mwm.svipenyu.cn

Ruby: 42.to_s
来源：http://ghe.xziqi.cn

C#:   42.ToString()
来源：http://pwb.haohaochexian.top

[A08] 取整与四舍五入
来源：http://vfn.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dox.xziqi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yys.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hpi.jinyuanbaomall.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://azb.xziqi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bqw.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://amz.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://gzm.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ttt.iojbl.cn

[A09] 绝对值与最大最小值
来源：http://tdp.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gon.xinyue.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lii.9152youxi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tdn.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xod.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kap.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fjn.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://avw.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qhq.mhx1999.top

[A10] 生成随机数
来源：http://wbk.nwbrower.top

Py:   import random; random.randint(1, 100)
来源：http://mie.sufxvd.cn

PHP:  random_int(1, 100);
来源：http://pas.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vdr.yvedp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ovz.ydjk.org.cn

Java: new Random().nextInt(100) + 1
来源：http://jto.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://svg.jiagoushi.top

Ruby: rand(1..100)
来源：http://ytl.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://cpi.jianghu66.top

[A11] 条件表达式（三元）
来源：http://ywz.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://jki.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bgb.jinqigufen.top

JS:   x > 0 ? "yes" : "no"
来源：http://ifu.xuetiantiany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://efs.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://lws.hesvh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rbx.shzxlz.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rxu.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://nzh.yonumen.top

[A12] 字符串插值 / 格式化
来源：http://wnk.hywenlv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jwx.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pvf.pengpengdd.cyou

JS:   `Hello, ${name}!`
来源：http://vep.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://zbr.bbcook.cn

Java: "Hello, %s!".formatted(name)
来源：http://wjz.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wtg.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://ogh.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://fbx.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://lhg.shanyushiyangkeji.top

Py:   "第一行\n第二行"
来源：http://hkr.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://rvz.sxryk.cn

JS:   "第一行\n第二行"
来源：http://kno.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://umx.snrcjt.cn

Java: "第一行\n第二行"
来源：http://iyf.zhengqikj.top

Go:   "第一行\n第二行"
来源：http://lsv.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://cbn.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://rcr.zdqjudy.top

[A14] 注释写法
来源：http://moz.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vka.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://bjn.zycfv.cn

JS:   // 单行；/* 多行 */
来源：http://dwv.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://dfg.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blu.pycfn.com

Go:   // 单行；/* 多行 */
来源：http://ohu.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://jog.fengsongda.top

C#:   // 单行；/* 多行 */
来源：http://imu.snrcjt.cn

[A15] 空值判断与默认值
来源：http://fxx.yvedp.cn

Py:   value = data or "默认值"
来源：http://yed.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://sxf.xylfe.cn

JS:   const value = data ?? "默认值";
来源：http://tqp.hfpthk.cn

TS:   const value = data ?? "默认值";
来源：http://ycx.sweek.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qzg.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://mho.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://wso.iojbl.cn

C#:   var value = data ?? "默认值";
来源：http://zuv.havefunace.top

[A16] 真假值判断规则
来源：http://eiq.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zai.jiagoushi.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dim.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://udd.yanxiufei.cn

TS:   if (!x) {}
来源：http://and.daria6918.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zka.hnqzz.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xpe.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jnw.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ptw.tanke756.top

[A17] 位运算
来源：http://qdo.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdh.shuidangran.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://usz.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kru.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wyh.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbh.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cxk.pycfn.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rya.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fmq.jinyuanbaomall.cn

[A18] 字符与 ASCII 码互转
来源：http://lti.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://dvt.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://dho.redwolf501.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ykq.daxiang520.top


<!-- 参考信息 -->