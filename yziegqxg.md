代发 wailian999

[U101] JS：classList 操作
来源：http://uoc.guowangkeji.top

el.classList.toggle("active")
来源：http://ueq.ehwqpu.com

[U102] JS：本地存储
来源：http://ddw.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mdu.feifeiyinyue.top

[U103] JS：定时器
来源：http://veu.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xbv.hywenlv.cn

[U104] JS：防抖
来源：http://lex.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvs.snrcjt.cn

[U105] JS：节流
来源：http://wpz.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gqb.fzhhl.top

[U106] JS：日期格式化
来源：http://idq.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://htj.nanxinkj.top

[U107] JS：数字千分位
来源：http://wuj.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yvu.chenlongwang.top

[U108] JS：随机整数
来源：http://pqw.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fxe.ehwqpu.com

[U109] JS：数组分组
来源：http://qjd.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://urm.tarul.cn

[U110] JS：数组分块
来源：http://vwm.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gmu.yj202588.top

[U111] JS：对象转 Map
来源：http://tsm.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://osm.fehbvm.com

[U112] JS：字符串补位
来源：http://wxd.ybcxt.top

"7".padStart(3, "0")
来源：http://dqn.yueranfly.top

[U113] JS：正则替换全部
来源：http://ibw.hammf.cn

s.replaceAll("a", "b")
来源：http://rox.hnqzz.top

[U114] JS：JSON 深比较
来源：http://hcq.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://var.cheryme.top

[U115] JS：生成 UUID
来源：http://mpb.ivvv.top

crypto.randomUUID()
来源：http://dfr.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://kti.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://smf.mhx1999.top

[U117] JS：单元测试
来源：http://yop.cheryme.top

npm i -D vitest;  npx vitest
来源：http://ggi.tianlin.xyz

[U118] JS：开发服务器
来源：http://awt.ctjpmb.com

npm i -D vite;  npx vite
来源：http://sbr.nanxinkj.top

[U119] JS：生产构建
来源：http://lks.hywenlv.cn

npx vite build
来源：http://tzp.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://uou.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://ean.yuanzhike.top

================================================================================
来源：http://jtx.nwbrower.top

统计汇总
来源：http://dvd.mhx1999.top

================================================================================
来源：http://sjg.sweek.top

按语言统计（条）：
来源：http://bic.xinyue.icu

Python ......... 252
来源：http://tab.ybcxt.top

PHP ............ 252
来源：http://gnc.cashguo.top

JavaScript ..... 252
来源：http://qru.kuanghao11.cn

TypeScript ..... 212
来源：http://nyg.mhx1999.top

Java ........... 212
来源：http://vrg.guannengcc.top

Go ............. 212
来源：http://afj.svipenyu.cn

Ruby ........... 212
来源：http://zgf.ctjpmb.com

C# ............. 212
来源：http://eva.jianghu66.top

C .............. 30
来源：http://jww.sweek.top

C++ ............ 30
来源：http://lpn.xuanzx.com

SQL ............ 90
来源：http://dbx.zhongyouzk.top

Bash ........... 80
来源：http://gkp.shanyushiyangtech.top

Kotlin ......... 15
来源：http://ezg.uphjek.com

Swift .......... 15
来源：http://sqw.316326.xyz

Lua ............ 10
来源：http://diw.zhongyouzk.top

Perl ........... 10
来源：http://jyg.jinqigfzy.top

Scala .......... 10
来源：http://ahm.fehbvm.com

------------------------------------
来源：http://agh.yvedp.cn

合计 ........... 2106 条
来源：http://jid.52xcode.cn

按章节统计：
来源：http://sfh.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dzk.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wbw.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wmi.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bfo.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oju.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://krl.daxiang520.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxl.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rot.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rfc.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tak.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dqr.pengpengdd.cyou

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fpy.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://icw.fengsongda.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jzy.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zoc.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ilt.zdbjq.cn

Q SQL 专题                              90
来源：http://vxk.jiagoushi.top

R Bash 专题                             80
来源：http://iue.sysykeji.top

S C / C++ 专题                          60
来源：http://fqk.yangfankeji.com

T 其他语言补充                          60
来源：http://mfq.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://gtr.xinyue.icu

------------------------------------
来源：http://nzb.52xcode.cn

合计                                  2106 条
来源：http://vyp.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://qyo.hcnkem.com

使用提醒
来源：http://ntr.aizwys.cn

--------------------------------------------------------------------------------
来源：http://kce.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fjl.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://phs.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fwy.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zss.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bha.hfpthk.cn

—— 文件结束 ——
来源：http://dlu.jinghuilouyu.cn

================================================================================
来源：http://ldk.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://djr.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://orz.zdbjq.cn

================================================================================
来源：http://wpz.yvedp.cn

【收录内容】
来源：http://ahe.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xjx.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pfl.ybcxt.top

SQL · Bash · C · C++
来源：http://zjf.xuetiantiany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fzj.hfpthk.cn

【使用说明】
来源：http://tnd.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iin.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mvp.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vti.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zvn.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jnb.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ict.shuidangran.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ouf.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gji.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://upk.ivvv.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mjn.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vtn.nwbrower.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qxu.aizwys.cn

【文件统计】
来源：http://rvu.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xdb.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://ksc.smart0.xyz

目  录
来源：http://mpf.fzhhl.top

--------------------------------------------------------------------------------
来源：http://dwj.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jti.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aqg.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mqt.ywan-chungtsiang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ejn.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vgw.havefunace.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lyh.tian-w.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://upc.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qsl.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wbi.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qya.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ozl.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wmh.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://obs.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wyw.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://syc.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://frm.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://npr.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://awa.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uqp.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nkl.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mag.xingfuxueyuan.xyz

================================================================================
来源：http://cxy.sweek.top

A. 基础语法与类型
来源：http://oqf.dianchejie.cn

================================================================================
来源：http://cnv.tarul.cn

[A01] Hello World
来源：http://nab.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://vsy.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://gqo.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://vul.chenzaomai.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://miy.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://kgq.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://pee.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://lbk.fktsv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://roa.shuidangran.top

[A02] 变量声明与赋值
来源：http://jti.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://exr.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uqq.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jze.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mqs.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://mcz.cqqwz.cn

Go:   name := "Alex"; age := 20
来源：http://sxi.tanke756.top

Ruby: name = "Alex"; age = 20
来源：http://gta.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://xuy.smart0.xyz

[A03] 常量定义
来源：http://ptc.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yjj.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://nvc.havefunace.top

JS:   const PI = 3.14159;
来源：http://khv.ppjwa.cn

TS:   const PI: number = 3.14159;
来源：http://uiy.guowangkeji.top

Java: static final double PI = 3.14159;
来源：http://wug.zhengqikj.top

Go:   const PI = 3.14159
来源：http://asz.bbcook.cn

Ruby: PI = 3.14159
来源：http://mlx.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://mys.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://tvw.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kjb.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lee.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ckw.hfpthk.cn

TS:   typeof x; x instanceof Date
来源：http://vtp.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cyb.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aod.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sui.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://ttn.zycfv.cn

[A05] 整数除法与取模
来源：http://wfv.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fri.tarul.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pdo.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sly.ywan-chungtsiang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tlb.shuidangran.top

Java: 7 / 2; 7 % 2
来源：http://mzc.yongpay.top

Go:   7 / 2; 7 % 2
来源：http://wso.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://qgc.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://pzb.tianlin.xyz

[A06] 字符串转数字
来源：http://oxe.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://ehp.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yqf.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tlv.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://hry.iojbl.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cog.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://thh.kuanghao11.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ibe.jinyuanbaomall.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kgy.xylfe.cn

[A07] 数字转字符串
来源：http://pyp.pengpengdd.cyou

Py:   str(42)
来源：http://ogv.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://xym.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://ujx.gotoacloud.top

TS:   String(42)
来源：http://fhr.cqqwz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eav.gzhubu.top

Go:   strconv.Itoa(42)
来源：http://dpt.xinyue.icu

Ruby: 42.to_s
来源：http://cvb.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://jhb.cheryme.top

[A08] 取整与四舍五入
来源：http://pmi.jqgfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wni.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nxm.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uyk.cucudq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gug.pycfn.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pco.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vyt.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mpm.yangfankeji.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pim.guowangkeji.top

[A09] 绝对值与最大最小值
来源：http://jhp.xinyue.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yko.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://igk.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://khl.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uql.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://djy.yuxming.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sat.hnqzz.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gto.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kem.aizwys.cn

[A10] 生成随机数
来源：http://hoh.gaohongyu789.top

Py:   import random; random.randint(1, 100)
来源：http://jfq.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://ert.xingfuxueyuan.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fxj.tarul.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gib.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://saz.bjfxy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fnn.gaohongyu789.top

Ruby: rand(1..100)
来源：http://oav.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://nxy.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://qmd.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://oju.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vve.ehwqpu.com

JS:   x > 0 ? "yes" : "no"
来源：http://fhv.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://ziu.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://oaa.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ajl.tianlin.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://zzz.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jpx.fanxiaobao.xyz

[A12] 字符串插值 / 格式化
来源：http://her.quarkkingdee.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kyb.nanxuanxn.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ovz.meibo888.top

JS:   `Hello, ${name}!`
来源：http://jkd.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://pgt.ydzc1.top

Java: "Hello, %s!".formatted(name)
来源：http://trk.andypj.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yrk.cucudq.cn

Ruby: "Hello, #{name}!"
来源：http://gps.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://ddr.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://iuk.aizwys.cn

Py:   "第一行\n第二行"
来源：http://ves.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://qqr.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://hyz.redwolf501.top

TS:   "第一行\n第二行"
来源：http://hlq.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://oke.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://rnt.hysaishi.cn

Ruby: "第一行\n第二行"
来源：http://gex.birdmap.top

C#:   "第一行\n第二行"
来源：http://amk.yueranfly.top

[A14] 注释写法
来源：http://ulh.52xcode.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://meg.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dzd.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://ypm.pengpengdd.cyou

TS:   // 单行；/* 多行 */
来源：http://ubi.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lbz.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://kmd.jlsjyb.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tui.fzhhl.top

C#:   // 单行；/* 多行 */
来源：http://gwb.xylfe.cn

[A15] 空值判断与默认值
来源：http://axs.havefunace.top

Py:   value = data or "默认值"
来源：http://gea.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://jwn.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://jwf.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://ghr.ivvv.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://juy.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://agi.jyoumei.cn

Ruby: value = data || "默认值"
来源：http://ola.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://gwx.zhiwuduotai.top

[A16] 真假值判断规则
来源：http://qix.ctjpmb.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qez.ywan-chungtsiang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jtx.hesvh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tkb.daria6918.cn

TS:   if (!x) {}
来源：http://rdv.fengsongda.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tbs.meibo888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pff.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://wof.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zrf.zdqjudy.top

[A17] 位运算
来源：http://zoj.pengpengdd.cyou

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnu.hnqzz.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gwh.kuanghao11.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzf.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nkh.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnq.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kkw.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://usu.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://akg.epnwcf.com


<!-- 参考信息 -->