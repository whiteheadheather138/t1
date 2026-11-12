代发 wailian999

[U101] JS：classList 操作
来源：http://abt.jlsjyb.cn

el.classList.toggle("active")
来源：http://cyb.birdmap.top

[U102] JS：本地存储
来源：http://qrd.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://toc.cheryme.top

[U103] JS：定时器
来源：http://ydi.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jjn.yuxming.cn

[U104] JS：防抖
来源：http://ghh.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lae.wangdashe.top

[U105] JS：节流
来源：http://mjs.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lsq.vehdjk.com

[U106] JS：日期格式化
来源：http://ott.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mmn.zycfv.cn

[U107] JS：数字千分位
来源：http://cwf.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sva.hesvh.cn

[U108] JS：随机整数
来源：http://hgj.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hmx.shangyingyoupin.top

[U109] JS：数组分组
来源：http://bdu.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://yba.fehbvm.com

[U110] JS：数组分块
来源：http://xzd.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lho.sysykeji.top

[U111] JS：对象转 Map
来源：http://lza.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://hmg.tian-w.cn

[U112] JS：字符串补位
来源：http://gqi.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://iqd.andypj.xyz

[U113] JS：正则替换全部
来源：http://teq.yvedp.cn

s.replaceAll("a", "b")
来源：http://aqf.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://dkk.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://muk.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://pef.meibo888.top

crypto.randomUUID()
来源：http://gwf.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://teg.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://zsc.yanxiufei.cn

[U117] JS：单元测试
来源：http://sce.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://ixv.hnqzz.top

[U118] JS：开发服务器
来源：http://irb.yvedp.cn

npm i -D vite;  npx vite
来源：http://ysr.hysaishi.cn

[U119] JS：生产构建
来源：http://auw.hnxiangtu.top

npx vite build
来源：http://fjf.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://erp.birdmap.top

import.meta.env.VITE_API_URL
来源：http://bhy.kuanghao11.cn

================================================================================
来源：http://tgl.shangyingyoupin.top

统计汇总
来源：http://gqv.jinqigfzy.top

================================================================================
来源：http://nbo.zhongyouzk.top

按语言统计（条）：
来源：http://okw.9152youxi.cn

Python ......... 252
来源：http://kux.hcnkem.com

PHP ............ 252
来源：http://ixv.sysykeji.top

JavaScript ..... 252
来源：http://gtu.wangdashe.top

TypeScript ..... 212
来源：http://xxy.ctjpmb.com

Java ........... 212
来源：http://nqz.mhx1999.top

Go ............. 212
来源：http://elw.fzhhl.top

Ruby ........... 212
来源：http://kwx.cdnleiting.top

C# ............. 212
来源：http://noy.yuxming.cn

C .............. 30
来源：http://ibq.zhaomingkeji.xyz

C++ ............ 30
来源：http://lww.cashguo.top

SQL ............ 90
来源：http://una.pycfn.com

Bash ........... 80
来源：http://plr.birdmap.top

Kotlin ......... 15
来源：http://xao.gaohongyu789.top

Swift .......... 15
来源：http://oiq.fzhhl.top

Lua ............ 10
来源：http://ban.jinqigfzy.top

Perl ........... 10
来源：http://mpn.gogol.net.cn

Scala .......... 10
来源：http://vmt.jlsjyb.cn

------------------------------------
来源：http://jlp.316326.xyz

合计 ........... 2106 条
来源：http://thn.cdnleiting.top

按章节统计：
来源：http://ccs.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://crs.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ojq.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ikd.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bqd.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zcz.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://urm.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wph.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cdm.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lov.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ltc.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hhf.redwolf501.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://foa.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aww.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tkw.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://elg.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jvl.ydzc1.top

Q SQL 专题                              90
来源：http://zap.hnxiangtu.top

R Bash 专题                             80
来源：http://fur.zhijiandao.cn

S C / C++ 专题                          60
来源：http://ycx.yongpay.top

T 其他语言补充                          60
来源：http://ikp.nwbrower.top

U 高频实用片段                         120
来源：http://snc.gzhubu.top

------------------------------------
来源：http://yoy.gzhubu.top

合计                                  2106 条
来源：http://duh.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://bjo.shzxlz.cn

使用提醒
来源：http://oxt.yonumen.top

--------------------------------------------------------------------------------
来源：http://mkl.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bcb.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kbl.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rip.hammf.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nab.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pye.snrcjt.cn

—— 文件结束 ——
来源：http://oie.redwolf501.top

================================================================================
来源：http://xhx.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://qgz.bbcook.cn

Common Programming Examples Cheat Book
来源：http://czn.cucudq.cn

================================================================================
来源：http://ydr.xylfe.cn

【收录内容】
来源：http://mgp.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://dgz.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sxu.c1oappe.top

SQL · Bash · C · C++
来源：http://avt.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qhy.ybcxt.top

【使用说明】
来源：http://elo.hywenlv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://luf.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sal.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bkz.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ydr.hfpthk.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://llf.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pvh.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qwr.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://klo.guowangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xyz.yonumen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cgl.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jpm.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uxb.zhiwuduotai.top

【文件统计】
来源：http://nke.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kqh.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ipx.yfazqb.com

目  录
来源：http://hqj.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://aup.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dpe.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://szp.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ufg.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rmv.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dwz.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aug.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sru.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uvi.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kxy.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://den.gaohongyu789.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ogm.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sni.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jhr.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kth.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ubk.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://geo.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jfu.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ztf.shangyingyoupin.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qib.hywenlv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fwa.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://luv.xziqi.cn

================================================================================
来源：http://rfd.cqqwz.cn

A. 基础语法与类型
来源：http://pvu.jinyuanbaomall.cn

================================================================================
来源：http://kpr.ppjwa.cn

[A01] Hello World
来源：http://azq.cheryme.top

Py:   print("Hello, World!")
来源：http://vnd.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://vie.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://whq.feifeiyinyue.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ukt.shanyushiyangtech.top

Java: System.out.println("Hello, World!");
来源：http://wqj.hysaishi.cn

Go:   fmt.Println("Hello, World!")
来源：http://qye.cqqwz.cn

Ruby: puts "Hello, World!"
来源：http://jji.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://udj.316326.xyz

[A02] 变量声明与赋值
来源：http://oni.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dmg.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://taw.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://iku.zhixingplan.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ypq.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://xov.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://jwu.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://wxc.nanxinkj.top

C#:   string name = "Alex"; int age = 20;
来源：http://jbq.yanxiufei.cn

[A03] 常量定义
来源：http://fxi.shzxlz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qmq.yj20258.top

PHP:  const PI = 3.14159;
来源：http://jyk.yongpay.top

JS:   const PI = 3.14159;
来源：http://tbt.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://zmx.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://ott.haohaochexian.top

Go:   const PI = 3.14159
来源：http://tpc.pycfn.com

Ruby: PI = 3.14159
来源：http://wuu.sysykeji.top

C#:   const double PI = 3.14159;
来源：http://jty.havefunace.top

[A04] 判断变量类型
来源：http://ibk.sysykeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gwz.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://icz.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bpb.fktsv.cn

TS:   typeof x; x instanceof Date
来源：http://fsv.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ulu.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://lrg.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://vfq.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://vac.shzxlz.cn

[A05] 整数除法与取模
来源：http://iae.hcnkem.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hob.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vib.aizwys.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vkp.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gfc.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://kev.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://hly.jinyuanbaomall.cn

Ruby: 7 / 2; 7 % 2
来源：http://kix.c1oappe.top

C#:   7 / 2; 7 % 2
来源：http://teo.nwbrower.top

[A06] 字符串转数字
来源：http://usk.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://lmx.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dby.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oyt.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://mwi.redwolf501.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bxq.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tgz.wangdashe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zoj.shanyushiyangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://con.uphjek.com

[A07] 数字转字符串
来源：http://jhl.ywan-chungtsiang.top

Py:   str(42)
来源：http://ihb.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://ych.andypj.xyz

JS:   String(42); (42).toString()
来源：http://ymy.hnqzz.top

TS:   String(42)
来源：http://qhw.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pwm.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://lsg.jinqigufen.top

Ruby: 42.to_s
来源：http://afr.mhx1999.top

C#:   42.ToString()
来源：http://rmo.dianchejie.cn

[A08] 取整与四舍五入
来源：http://yuq.hcnkem.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xna.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://umc.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://euf.bjfxy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://amm.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sou.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iga.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://whe.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dus.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://jkm.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nxt.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://djd.ehwqpu.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eaa.hywenlv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xdd.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xio.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://slj.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cns.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qdd.tian-w.cn

[A10] 生成随机数
来源：http://zvz.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://zio.fzhhl.top

PHP:  random_int(1, 100);
来源：http://uuq.cheryme.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bcl.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tzs.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://aow.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ljd.316326.xyz

Ruby: rand(1..100)
来源：http://vbz.guannengcc.top

C#:   new Random().Next(1, 101)
来源：http://hux.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://eip.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://qxh.epnwcf.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://swu.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://anp.zdqjudy.top

TS:   x > 0 ? "yes" : "no"
来源：http://vyu.jinyuanbaomall.cn

Java: x > 0 ? "yes" : "no"
来源：http://wvk.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mwr.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://utp.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://wol.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://qkx.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qwd.ywan-chungtsiang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xka.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://zyt.mhx1999.top

TS:   `Hello, ${name}!`
来源：http://rtl.epnwcf.com

Java: "Hello, %s!".formatted(name)
来源：http://qne.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zrk.pengpengdd.cyou

Ruby: "Hello, #{name}!"
来源：http://lpj.jianghu66.top

C#:   $"Hello, {name}!"
来源：http://eve.havefunace.top

[A13] 多行字符串（练习 \n 转义）
来源：http://whw.zhoulong.xyz

Py:   "第一行\n第二行"
来源：http://gtg.fzhhl.top

PHP:  "第一行\n第二行"
来源：http://foa.hnxiangtu.top

JS:   "第一行\n第二行"
来源：http://wtx.yj20258.top

TS:   "第一行\n第二行"
来源：http://wls.yvedp.cn

Java: "第一行\n第二行"
来源：http://odk.yueranfly.top

Go:   "第一行\n第二行"
来源：http://klg.uphjek.com

Ruby: "第一行\n第二行"
来源：http://nrr.ydzc1.top

C#:   "第一行\n第二行"
来源：http://ntd.svipenyu.cn

[A14] 注释写法
来源：http://rug.yongpay.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ruy.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pvg.nanxinkj.top

JS:   // 单行；/* 多行 */
来源：http://pvj.ppjwa.cn

TS:   // 单行；/* 多行 */
来源：http://kow.havefunace.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qko.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://tiq.tarul.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dkm.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://bbv.tian-w.cn

[A15] 空值判断与默认值
来源：http://rqw.gogol.net.cn

Py:   value = data or "默认值"
来源：http://tqb.dianchejie.cn

PHP:  $value = $data ?? "默认值";
来源：http://pie.xingfuxueyuan.xyz

JS:   const value = data ?? "默认值";
来源：http://ehd.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://vne.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vhi.jinqigufen.top

Go:   if data == "" { data = "默认值" }
来源：http://spa.zhongyouzk.top

Ruby: value = data || "默认值"
来源：http://emm.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://buz.tianlin.xyz

[A16] 真假值判断规则
来源：http://igo.nanxinkj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zdb.hongshengwenyu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eaq.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ino.hcnkem.com

TS:   if (!x) {}
来源：http://wwc.jinqigfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nkr.meibo888.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://opp.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gff.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qaj.aizwys.cn

[A17] 位运算
来源：http://ezn.zhaomingkeji.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nuz.hfpthk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gzg.daria6918.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hhz.redwolf501.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hxq.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rez.hysaishi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tke.jqgfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://amc.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttn.jinqigufen.top


<!-- 参考信息 -->