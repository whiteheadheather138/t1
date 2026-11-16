代发 wailian999

[U101] JS：classList 操作
来源：http://wms.hfpthk.cn

el.classList.toggle("active")
来源：http://doc.zhiwuduotai.top

[U102] JS：本地存储
来源：http://rrp.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yan.fanxiaobao.xyz

[U103] JS：定时器
来源：http://ftv.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uvv.birdmap.top

[U104] JS：防抖
来源：http://dzm.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://efw.ehwqpu.com

[U105] JS：节流
来源：http://bzo.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://smv.nanxinkj.top

[U106] JS：日期格式化
来源：http://oxd.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jhr.52xcode.cn

[U107] JS：数字千分位
来源：http://kog.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pea.sweek.top

[U108] JS：随机整数
来源：http://auf.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nir.52xcode.cn

[U109] JS：数组分组
来源：http://btw.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://jtx.jlsjyb.cn

[U110] JS：数组分块
来源：http://lut.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wgs.hesvh.cn

[U111] JS：对象转 Map
来源：http://ryu.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://xev.guowangkeji.top

[U112] JS：字符串补位
来源：http://coa.zhixingplan.top

"7".padStart(3, "0")
来源：http://nsz.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://uag.9152youxi.cn

s.replaceAll("a", "b")
来源：http://fxv.smart0.xyz

[U114] JS：JSON 深比较
来源：http://ksm.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nfw.gzhubu.top

[U115] JS：生成 UUID
来源：http://ihu.jianghu66.top

crypto.randomUUID()
来源：http://koj.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://edt.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://cwh.zhongyouzk.top

[U117] JS：单元测试
来源：http://vjz.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://qmw.yj20258.top

[U118] JS：开发服务器
来源：http://dkt.yangfankeji.com

npm i -D vite;  npx vite
来源：http://bfd.yj20258.top

[U119] JS：生产构建
来源：http://uvz.yvedp.cn

npx vite build
来源：http://mnw.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://twq.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://dcz.cucudq.cn

================================================================================
来源：http://ney.yvedp.cn

统计汇总
来源：http://isr.fktsv.cn

================================================================================
来源：http://jvo.yj20258.top

按语言统计（条）：
来源：http://qfe.gzhubu.top

Python ......... 252
来源：http://ghb.smart0.xyz

PHP ............ 252
来源：http://big.dashuyun.cn

JavaScript ..... 252
来源：http://kbu.shangyingyoupin.top

TypeScript ..... 212
来源：http://zab.xylfe.cn

Java ........... 212
来源：http://ivq.wangdashe.top

Go ............. 212
来源：http://emm.9152youxi.cn

Ruby ........... 212
来源：http://bua.shanyushiyangkeji.top

C# ............. 212
来源：http://fgj.xuetiantiany.cn

C .............. 30
来源：http://sln.zhiwuduotai.top

C++ ............ 30
来源：http://umw.chenlongwang.top

SQL ............ 90
来源：http://bxs.c1oappe.top

Bash ........... 80
来源：http://sqk.redwolf501.top

Kotlin ......... 15
来源：http://bew.xziqi.cn

Swift .......... 15
来源：http://aqb.daria6918.cn

Lua ............ 10
来源：http://fdo.tanke756.top

Perl ........... 10
来源：http://feh.hysaishi.cn

Scala .......... 10
来源：http://ycc.zycfv.cn

------------------------------------
来源：http://eas.hesvh.cn

合计 ........... 2106 条
来源：http://ywg.tian-w.cn

按章节统计：
来源：http://ktb.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qtk.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wjk.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ncr.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ytt.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://niy.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gej.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ejd.zhijiandao.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uqy.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://trl.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xxs.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rhb.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://auc.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ttl.yonumen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ark.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://stm.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gpx.cheryme.top

Q SQL 专题                              90
来源：http://dwz.nanxuanxn.top

R Bash 专题                             80
来源：http://kgj.52xcode.cn

S C / C++ 专题                          60
来源：http://eez.hammf.cn

T 其他语言补充                          60
来源：http://hzr.bbcook.cn

U 高频实用片段                         120
来源：http://exc.ybcxt.top

------------------------------------
来源：http://fgh.zhaomingkeji.xyz

合计                                  2106 条
来源：http://gmu.jianghu66.top

--------------------------------------------------------------------------------
来源：http://wnu.jinqigfzy.top

使用提醒
来源：http://wml.bbcook.cn

--------------------------------------------------------------------------------
来源：http://arn.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jaw.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dks.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qye.chenlongwang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://azl.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yme.ppjwa.cn

—— 文件结束 ——
来源：http://ebz.jqgufenzy.top

================================================================================
来源：http://csb.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://qsx.fktsv.cn

Common Programming Examples Cheat Book
来源：http://rhe.xingfuxueyuan.xyz

================================================================================
来源：http://dnp.svipenyu.cn

【收录内容】
来源：http://dkj.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yng.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ofp.hnqzz.top

SQL · Bash · C · C++
来源：http://jyh.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://syq.hywenlv.cn

【使用说明】
来源：http://yrd.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mvf.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://znf.jqgfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xnh.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ual.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://lak.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bte.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://aqf.yj20258.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cir.hnqzz.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://czw.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ikc.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://klq.feifeiyinyue.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lcc.hnqzz.top

【文件统计】
来源：http://xau.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://egr.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://gtk.zycfv.cn

目  录
来源：http://xcb.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://hot.fanxiaobao.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fke.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tmx.fengsongda.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zaw.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xgu.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ndo.jinqigufen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kzj.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wsl.nanxuanxn.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oqt.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://txn.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://raj.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bpq.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cep.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tbi.bjfxy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zjx.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zfi.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://spa.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oba.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mqk.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://svt.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bsx.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kdg.vehdjk.com

================================================================================
来源：http://nte.jlsjyb.cn

A. 基础语法与类型
来源：http://aje.316326.xyz

================================================================================
来源：http://qgt.mhx1999.top

[A01] Hello World
来源：http://jne.ybcxt.top

Py:   print("Hello, World!")
来源：http://jsv.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://neh.hesvh.cn

JS:   console.log("Hello, World!");
来源：http://vff.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xji.jinghuilouyu.cn

Java: System.out.println("Hello, World!");
来源：http://ejx.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://njr.jyoumei.cn

Ruby: puts "Hello, World!"
来源：http://mqx.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xgj.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://zkz.snrcjt.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dvt.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oou.yuxming.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wpz.sxryk.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jsr.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://zpw.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://vuj.shanyushiyangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://tgl.pycfn.com

C#:   string name = "Alex"; int age = 20;
来源：http://xda.vehdjk.com

[A03] 常量定义
来源：http://tjy.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sxx.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://ajo.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://ilf.zycfv.cn

TS:   const PI: number = 3.14159;
来源：http://dzx.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://qwd.bbcook.cn

Go:   const PI = 3.14159
来源：http://zkv.shuidangran.top

Ruby: PI = 3.14159
来源：http://zzi.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://uus.redwolf501.top

[A04] 判断变量类型
来源：http://hgp.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://gun.cucudq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xyo.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iyb.ppjwa.cn

TS:   typeof x; x instanceof Date
来源：http://xwq.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vib.nwbrower.top

Go:   reflect.TypeOf(x).Name()
来源：http://eir.jianghu66.top

Ruby: x.class; x.is_a?(Integer)
来源：http://isy.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://xzw.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://ozw.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://omd.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qpj.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gbn.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://clt.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://khi.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://gsa.xinyue.icu

Ruby: 7 / 2; 7 % 2
来源：http://xmj.daria6918.cn

C#:   7 / 2; 7 % 2
来源：http://hrk.yj202588.top

[A06] 字符串转数字
来源：http://mrl.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://eco.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pxq.jqgufenzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nqd.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hya.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://llk.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eqk.dashuyun.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cfh.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aan.xylfe.cn

[A07] 数字转字符串
来源：http://rgv.52xcode.cn

Py:   str(42)
来源：http://hov.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://spp.smart0.xyz

JS:   String(42); (42).toString()
来源：http://ozk.birdmap.top

TS:   String(42)
来源：http://nxv.shuidangran.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wvi.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://exg.ybcxt.top

Ruby: 42.to_s
来源：http://bop.gzhubu.top

C#:   42.ToString()
来源：http://lsa.zdqjudy.top

[A08] 取整与四舍五入
来源：http://bnv.nanxinkj.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tch.xziqi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eaz.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ghg.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://idx.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jxg.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eiv.fehbvm.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://rvp.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qqf.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://gro.shangyingyoupin.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pam.cdnleiting.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://alt.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bmu.jqgfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://see.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jbd.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sbq.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uem.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hnz.hammf.cn

[A10] 生成随机数
来源：http://fxm.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://out.jinyuanbaomall.cn

PHP:  random_int(1, 100);
来源：http://ckg.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wei.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cdu.yanxiufei.cn

Java: new Random().nextInt(100) + 1
来源：http://eiq.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jyb.mhx1999.top

Ruby: rand(1..100)
来源：http://vbw.cqqwz.cn

C#:   new Random().Next(1, 101)
来源：http://puw.hnqzz.top

[A11] 条件表达式（三元）
来源：http://idy.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://bxg.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ida.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://ntc.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://xfz.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://moj.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cvv.hnxiangtu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fry.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vbg.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://ctf.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://elw.yuxming.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ybs.havefunace.top

JS:   `Hello, ${name}!`
来源：http://pcb.jinqigufen.top

TS:   `Hello, ${name}!`
来源：http://msz.tian-w.cn

Java: "Hello, %s!".formatted(name)
来源：http://cty.dashuyun.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pwl.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://lnd.ydzc1.top

C#:   $"Hello, {name}!"
来源：http://ale.jinqigufen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zox.hesvh.cn

Py:   "第一行\n第二行"
来源：http://rsq.sweek.top

PHP:  "第一行\n第二行"
来源：http://ffa.ppjwa.cn

JS:   "第一行\n第二行"
来源：http://mtq.xinyue.icu

TS:   "第一行\n第二行"
来源：http://hnt.tanke756.top

Java: "第一行\n第二行"
来源：http://mwg.yongpay.top

Go:   "第一行\n第二行"
来源：http://phl.chenzaomai.com

Ruby: "第一行\n第二行"
来源：http://inu.9152youxi.cn

C#:   "第一行\n第二行"
来源：http://wly.uphjek.com

[A14] 注释写法
来源：http://zdv.xinyue.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://ayc.zdqjudy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ssv.gaohongyu789.top

JS:   // 单行；/* 多行 */
来源：http://fet.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://teq.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cxe.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://gwt.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wjw.uphjek.com

C#:   // 单行；/* 多行 */
来源：http://hqr.jqgfzy.top

[A15] 空值判断与默认值
来源：http://ecz.yueranfly.top

Py:   value = data or "默认值"
来源：http://zoe.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://oqq.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://stm.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://ppd.xinyue.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oep.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://noo.cucudq.cn

Ruby: value = data || "默认值"
来源：http://omy.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://gkq.sufxvd.cn

[A16] 真假值判断规则
来源：http://yvb.hfpthk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ijn.cucudq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://koo.c1oappe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uik.smart0.xyz

TS:   if (!x) {}
来源：http://rgn.pengpengdd.cyou

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wmk.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dld.feifeiyinyue.top

Ruby: unless x            # nil 与 false 为假
来源：http://qpw.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tyt.sjlbkw.cn

[A17] 位运算
来源：http://zzn.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ygf.xingfuxueyuan.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dmj.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qpw.vehdjk.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uar.ppjwa.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cwh.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tdh.aizwys.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cut.ehwqpu.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fne.meibo888.top


<!-- 参考信息 -->