代发 wailian999

[U103] JS：定时器
来源：http://usd.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zkj.shangyingyoupin.top

[U104] JS：防抖
来源：http://hjp.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbl.guowangkeji.top

[U105] JS：节流
来源：http://ppu.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://egs.mhx1999.top

[U106] JS：日期格式化
来源：http://npi.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hrj.yj202588.top

[U107] JS：数字千分位
来源：http://kil.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ajv.ctjpmb.com

[U108] JS：随机整数
来源：http://fta.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jau.yuanzhike.top

[U109] JS：数组分组
来源：http://etc.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://wfh.9152youxi.cn

[U110] JS：数组分块
来源：http://rhc.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jto.guannengcc.top

[U111] JS：对象转 Map
来源：http://yzz.316326.xyz

new Map(Object.entries(obj))
来源：http://aik.gaohongyu789.top

[U112] JS：字符串补位
来源：http://gpu.dashuyun.cn

"7".padStart(3, "0")
来源：http://pdk.guannengcc.top

[U113] JS：正则替换全部
来源：http://zlo.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://hzi.yuxming.cn

[U114] JS：JSON 深比较
来源：http://ysp.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hdu.chenzaomai.com

[U115] JS：生成 UUID
来源：http://ijg.yuxming.cn

crypto.randomUUID()
来源：http://jpa.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://pgo.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://ayb.jqgfzy.top

[U117] JS：单元测试
来源：http://tmf.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://eji.yj202588.top

[U118] JS：开发服务器
来源：http://dyo.chenlongwang.top

npm i -D vite;  npx vite
来源：http://mei.dashuyun.cn

[U119] JS：生产构建
来源：http://ilo.xinyue.icu

npx vite build
来源：http://fxy.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://tvy.uphjek.com

import.meta.env.VITE_API_URL
来源：http://cyi.yj20258.top

================================================================================
来源：http://rmr.xinyue.icu

统计汇总
来源：http://qwg.dashuyun.cn

================================================================================
来源：http://ziz.tian-w.cn

按语言统计（条）：
来源：http://cdw.zycfv.cn

Python ......... 252
来源：http://guq.gogol.net.cn

PHP ............ 252
来源：http://why.zhijiandao.cn

JavaScript ..... 252
来源：http://cwe.svipenyu.cn

TypeScript ..... 212
来源：http://uup.zdbjq.cn

Java ........... 212
来源：http://jwy.feifeiyinyue.top

Go ............. 212
来源：http://iuy.fzhhl.top

Ruby ........... 212
来源：http://xms.tanke756.top

C# ............. 212
来源：http://kjn.xuanzx.com

C .............. 30
来源：http://bti.yvedp.cn

C++ ............ 30
来源：http://gid.zhengqikj.top

SQL ............ 90
来源：http://vdi.cucudq.cn

Bash ........... 80
来源：http://ovy.tianlin.xyz

Kotlin ......... 15
来源：http://hpp.chenzaomai.com

Swift .......... 15
来源：http://qbj.tianlin.xyz

Lua ............ 10
来源：http://fzw.haohaochexian.top

Perl ........... 10
来源：http://eom.snrcjt.cn

Scala .......... 10
来源：http://gdn.tianlin.xyz

------------------------------------
来源：http://vjo.xziqi.cn

合计 ........... 2106 条
来源：http://kar.chenlongwang.top

按章节统计：
来源：http://izx.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tyn.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uyc.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vas.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cfv.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pcf.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sbj.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xty.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nzt.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xwa.ydzc1.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://clw.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nvb.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oxv.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tdd.fengsongda.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://moj.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ike.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ase.hfpthk.cn

Q SQL 专题                              90
来源：http://rcq.nanxuanxn.top

R Bash 专题                             80
来源：http://dkp.yongpay.top

S C / C++ 专题                          60
来源：http://wjm.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://nzm.cashguo.top

U 高频实用片段                         120
来源：http://iio.gogol.net.cn

------------------------------------
来源：http://exu.bbcook.cn

合计                                  2106 条
来源：http://tzq.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://und.epnwcf.com

使用提醒
来源：http://nrg.iojbl.cn

--------------------------------------------------------------------------------
来源：http://txo.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oie.ywan-chungtsiang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ztj.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ofr.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jwg.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cgk.fzhhl.top

—— 文件结束 ——
来源：http://qfb.xylfe.cn

================================================================================
来源：http://iod.meibo888.top

程序语言常见例子速查手册（2024 版）
来源：http://cyq.yuxming.cn

Common Programming Examples Cheat Book
来源：http://meb.ivvv.top

================================================================================
来源：http://gxh.fzhhl.top

【收录内容】
来源：http://rzk.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ksn.yueranfly.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://frg.0kj1m.cn

SQL · Bash · C · C++
来源：http://spe.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hof.zhixingplan.top

【使用说明】
来源：http://fud.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://egs.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xmy.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://meq.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tfp.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fmp.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gwc.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rnx.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://urw.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rgg.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rcv.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sds.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mwg.yj20258.top

【文件统计】
来源：http://bux.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pre.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://wyt.xziqi.cn

目  录
来源：http://ueo.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://aoa.sxryk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jrt.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://alz.kuanghao11.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uze.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ymn.c1oappe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://swj.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://str.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gud.yonumen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pmq.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xza.daria6918.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lox.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nou.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hav.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yvy.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vkv.jinghuilouyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hii.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqs.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gtc.daxiang520.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xif.kuanghao11.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://chs.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://imy.snrcjt.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://evt.vehdjk.com

================================================================================
来源：http://eiy.svipenyu.cn

A. 基础语法与类型
来源：http://lwz.wangdashe.top

================================================================================
来源：http://pbt.xinyue.icu

[A01] Hello World
来源：http://bfj.ivvv.top

Py:   print("Hello, World!")
来源：http://fuk.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://din.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://qwg.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lit.epnwcf.com

Java: System.out.println("Hello, World!");
来源：http://ehy.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://kin.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://gga.hywenlv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ajz.cheryme.top

[A02] 变量声明与赋值
来源：http://gko.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iao.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://att.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mwb.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oxw.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://fmt.zhoulong.xyz

Go:   name := "Alex"; age := 20
来源：http://bqy.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://pid.xuetiantiany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jrf.fengsongda.top

[A03] 常量定义
来源：http://ywi.xylfe.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://irk.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://now.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://jhg.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://qnu.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://sqz.ctjpmb.com

Go:   const PI = 3.14159
来源：http://yxd.sysykeji.top

Ruby: PI = 3.14159
来源：http://gbb.smart0.xyz

C#:   const double PI = 3.14159;
来源：http://kgw.hnxiangtu.top

[A04] 判断变量类型
来源：http://oja.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gaq.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pju.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dkf.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://edt.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xfq.tanke756.top

Go:   reflect.TypeOf(x).Name()
来源：http://mep.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qws.daria6918.cn

C#:   x.GetType().Name; x is int
来源：http://kyf.ehwqpu.com

[A05] 整数除法与取模
来源：http://hvi.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rlh.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nmg.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://abn.tarul.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ouy.zhongyouzk.top

Java: 7 / 2; 7 % 2
来源：http://ftb.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://cks.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://tvp.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://kcc.zhoulong.xyz

[A06] 字符串转数字
来源：http://gfn.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://hhn.zhoulong.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yfw.ydjk.org.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tgc.cheryme.top

TS:   parseInt("42", 10); Number("42")
来源：http://nfx.jinyuanbaomall.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://luo.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tyx.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ixh.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://guq.kuanghao11.cn

[A07] 数字转字符串
来源：http://oyf.hcnkem.com

Py:   str(42)
来源：http://thj.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://sbg.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://pvp.bbcook.cn

TS:   String(42)
来源：http://amq.zycfv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kyk.cashguo.top

Go:   strconv.Itoa(42)
来源：http://qmo.c1oappe.top

Ruby: 42.to_s
来源：http://blh.chenzaomai.com

C#:   42.ToString()
来源：http://vmr.wangshuangyany.cn

[A08] 取整与四舍五入
来源：http://ave.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://riy.feifeiyinyue.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ned.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nso.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hiz.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rnn.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yuj.birdmap.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://opy.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mxz.nwbrower.top

[A09] 绝对值与最大最小值
来源：http://who.zycfv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ila.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aql.jqgufenzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lgb.guannengcc.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qzp.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hcm.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://olq.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kkc.mhx1999.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mvg.dashuyun.cn

[A10] 生成随机数
来源：http://lcb.pengpengdd.cyou

Py:   import random; random.randint(1, 100)
来源：http://uub.daria6918.cn

PHP:  random_int(1, 100);
来源：http://cbl.guannengcc.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://moh.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dat.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://hol.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qjl.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://egk.cqqwz.cn

C#:   new Random().Next(1, 101)
来源：http://rsa.316326.xyz

[A11] 条件表达式（三元）
来源：http://vqa.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://qvb.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://cqc.yj20258.top

JS:   x > 0 ? "yes" : "no"
来源：http://jua.quarkkingdee.top

TS:   x > 0 ? "yes" : "no"
来源：http://vhm.jyoumei.cn

Java: x > 0 ? "yes" : "no"
来源：http://zzb.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wxn.yanxiufei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mhb.zhaomingkeji.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://pmp.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://swi.ppjwa.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wnk.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qoj.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://qnr.tanke756.top

TS:   `Hello, ${name}!`
来源：http://ujd.sjlbkw.cn

Java: "Hello, %s!".formatted(name)
来源：http://isk.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qup.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://rsc.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://qxu.sysykeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lcu.redwolf501.top

Py:   "第一行\n第二行"
来源：http://vic.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://eiz.nanxinkj.top

JS:   "第一行\n第二行"
来源：http://mzl.fktsv.cn

TS:   "第一行\n第二行"
来源：http://tpj.sjlbkw.cn

Java: "第一行\n第二行"
来源：http://ann.redwolf501.top

Go:   "第一行\n第二行"
来源：http://dvl.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://akn.daxiang520.top

C#:   "第一行\n第二行"
来源：http://cdq.hnqzz.top

[A14] 注释写法
来源：http://ayz.tianlin.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://skp.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yub.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://cgw.jinghuilouyu.cn

TS:   // 单行；/* 多行 */
来源：http://kyf.ctjpmb.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jpk.havefunace.top

Go:   // 单行；/* 多行 */
来源：http://xmb.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://ywm.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://teo.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://gua.yangfankeji.com

Py:   value = data or "默认值"
来源：http://crw.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://yzi.snrcjt.cn

JS:   const value = data ?? "默认值";
来源：http://gnb.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://ldz.c1oappe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fsc.jinqigfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://hfq.gaohongyu789.top

Ruby: value = data || "默认值"
来源：http://clz.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://ays.yueranfly.top

[A16] 真假值判断规则
来源：http://jit.uphjek.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mlk.jianghu66.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ird.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gja.fengsongda.top

TS:   if (!x) {}
来源：http://uie.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iaa.yj20258888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eua.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://zwz.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yix.fktsv.cn

[A17] 位运算
来源：http://wyo.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bzi.nanxuanxn.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yyk.jqgufenzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wdd.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wrb.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttv.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://byz.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nwa.hongshengwenyu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://abv.wangdashe.top

[A18] 字符与 ASCII 码互转
来源：http://gvh.tarul.cn

Py:   ord("A"); chr(65)
来源：http://ayo.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://dps.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://udx.shanyushiyangtech.top


<!-- 参考信息 -->