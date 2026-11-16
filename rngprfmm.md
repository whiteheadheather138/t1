代发 wailian999

[U103] JS：定时器
来源：http://ndx.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fmn.jiagoushi.top

[U104] JS：防抖
来源：http://qja.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kqr.wangshuangyany.cn

[U105] JS：节流
来源：http://ohp.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kpg.gotoacloud.top

[U106] JS：日期格式化
来源：http://nzn.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lcd.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://cmk.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tmi.pycfn.com

[U108] JS：随机整数
来源：http://dtw.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jjb.yj20258888.top

[U109] JS：数组分组
来源：http://vfb.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://lgq.redwolf501.top

[U110] JS：数组分块
来源：http://tht.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kee.jiagoushi.top

[U111] JS：对象转 Map
来源：http://pfm.yfazqb.com

new Map(Object.entries(obj))
来源：http://lnh.tanke756.top

[U112] JS：字符串补位
来源：http://xng.ctjpmb.com

"7".padStart(3, "0")
来源：http://psy.daxiang520.top

[U113] JS：正则替换全部
来源：http://mrf.andypj.xyz

s.replaceAll("a", "b")
来源：http://fyr.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://xbm.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mce.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://zfo.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://gah.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://ewy.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://gfd.zhixingplan.top

[U117] JS：单元测试
来源：http://nmf.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://boa.gotoacloud.top

[U118] JS：开发服务器
来源：http://esr.zycfv.cn

npm i -D vite;  npx vite
来源：http://cyl.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://hav.haohaochexian.top

npx vite build
来源：http://sgv.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://lus.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://kjq.ivvv.top

================================================================================
来源：http://ysx.hesvh.cn

统计汇总
来源：http://dqx.jiagoushi.top

================================================================================
来源：http://qnj.cdnleiting.top

按语言统计（条）：
来源：http://yoh.cucudq.cn

Python ......... 252
来源：http://ldd.hywenlv.cn

PHP ............ 252
来源：http://nkj.yuanzhike.top

JavaScript ..... 252
来源：http://rje.tanke756.top

TypeScript ..... 212
来源：http://efv.yanxiufei.cn

Java ........... 212
来源：http://jdq.fktsv.cn

Go ............. 212
来源：http://ztq.birdmap.top

Ruby ........... 212
来源：http://hzy.xylfe.cn

C# ............. 212
来源：http://cts.gogol.net.cn

C .............. 30
来源：http://mzp.guannengcc.top

C++ ............ 30
来源：http://bwl.fehbvm.com

SQL ............ 90
来源：http://otz.zhongyouzk.top

Bash ........... 80
来源：http://tcc.fengsongda.top

Kotlin ......... 15
来源：http://stq.vehdjk.com

Swift .......... 15
来源：http://qoy.vehdjk.com

Lua ............ 10
来源：http://jdx.hywenlv.cn

Perl ........... 10
来源：http://arl.chenjidiqi.icu

Scala .......... 10
来源：http://gaa.zhengqikj.top

------------------------------------
来源：http://wyq.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://cic.ivvv.top

按章节统计：
来源：http://jhn.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://njn.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wtj.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bqw.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gfq.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://deh.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://svc.fengsongda.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ypr.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mvf.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pww.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://twg.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cfe.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gnb.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://riy.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bwh.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://omt.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nyy.yj20258888.top

Q SQL 专题                              90
来源：http://wct.jqgufenzy.top

R Bash 专题                             80
来源：http://qok.guowangkeji.top

S C / C++ 专题                          60
来源：http://nis.jyoumei.cn

T 其他语言补充                          60
来源：http://axo.xziqi.cn

U 高频实用片段                         120
来源：http://qxd.shanyushiyangtech.top

------------------------------------
来源：http://kbt.xinyue.icu

合计                                  2106 条
来源：http://uxd.aizwys.cn

--------------------------------------------------------------------------------
来源：http://owc.shangyingyoupin.top

使用提醒
来源：http://nem.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://xps.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://arq.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ndy.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xfo.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lrg.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tme.wangshuangyany.cn

—— 文件结束 ——
来源：http://mzd.jianghu66.top

================================================================================
来源：http://zsg.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://ocx.yj20258.top

Common Programming Examples Cheat Book
来源：http://nml.uphjek.com

================================================================================
来源：http://edm.vehdjk.com

【收录内容】
来源：http://yqc.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zlr.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nlq.sjlbkw.cn

SQL · Bash · C · C++
来源：http://gka.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qbd.zhixingplan.top

【使用说明】
来源：http://ttu.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ixf.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qzx.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ypm.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rct.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mkb.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hrf.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bsr.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hub.jianghu66.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fxw.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iwt.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://law.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ota.sweek.top

【文件统计】
来源：http://frx.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vck.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://nkq.jqgfzy.top

目  录
来源：http://mxp.yvedp.cn

--------------------------------------------------------------------------------
来源：http://qan.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nat.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mft.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vnc.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bdr.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xlm.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://org.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mej.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qbz.uphjek.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wis.yanxiufei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://awj.wangshuangyany.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jcv.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qpx.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hlo.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bxl.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zyx.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ita.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gob.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ykx.9152youxi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zyz.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wyf.ehwqpu.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://umm.yonumen.top

================================================================================
来源：http://wau.zhijiandao.cn

A. 基础语法与类型
来源：http://bty.0kj1m.cn

================================================================================
来源：http://occ.yvedp.cn

[A01] Hello World
来源：http://eug.xziqi.cn

Py:   print("Hello, World!")
来源：http://owf.xziqi.cn

PHP:  echo "Hello, World!";
来源：http://phf.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://onn.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sbp.yj20258888.top

Java: System.out.println("Hello, World!");
来源：http://zge.andypj.xyz

Go:   fmt.Println("Hello, World!")
来源：http://qwp.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://jyl.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uvo.yfazqb.com

[A02] 变量声明与赋值
来源：http://efk.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lbp.xuanzx.com

PHP:  $name = "Alex"; $age = 20;
来源：http://mgo.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://hye.dianchejie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aod.svipenyu.cn

Java: String name = "Alex"; int age = 20;
来源：http://vxm.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://urc.yuxming.cn

Ruby: name = "Alex"; age = 20
来源：http://ymv.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://aku.sweek.top

[A03] 常量定义
来源：http://tzs.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xng.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://utt.jinghuilouyu.cn

JS:   const PI = 3.14159;
来源：http://pct.zhixingplan.top

TS:   const PI: number = 3.14159;
来源：http://mdt.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://hhe.aibaodan.cn

Go:   const PI = 3.14159
来源：http://ubq.yj20258.top

Ruby: PI = 3.14159
来源：http://uxm.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://ixh.xziqi.cn

[A04] 判断变量类型
来源：http://wey.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cau.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xwy.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tss.havefunace.top

TS:   typeof x; x instanceof Date
来源：http://ttl.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qku.chenlongwang.top

Go:   reflect.TypeOf(x).Name()
来源：http://jfk.shanyushiyangtech.top

Ruby: x.class; x.is_a?(Integer)
来源：http://flr.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://hzh.gotoacloud.top

[A05] 整数除法与取模
来源：http://kly.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wry.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://irl.epnwcf.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jos.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vqm.zhijiandao.cn

Java: 7 / 2; 7 % 2
来源：http://mqc.tanke756.top

Go:   7 / 2; 7 % 2
来源：http://itp.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://kxy.hongshengwenyu.top

C#:   7 / 2; 7 % 2
来源：http://ckt.yfazqb.com

[A06] 字符串转数字
来源：http://yrf.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://cmo.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qeb.hfpthk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://opp.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://slb.zhongyouzk.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aro.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mng.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://efi.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://osl.sxryk.cn

[A07] 数字转字符串
来源：http://yqg.fktsv.cn

Py:   str(42)
来源：http://inh.jinqigufen.top

PHP:  (string) 42; strval(42)
来源：http://ysg.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://yoe.pycfn.com

TS:   String(42)
来源：http://qwf.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rbs.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://opx.aizwys.cn

Ruby: 42.to_s
来源：http://goy.yuanzhike.top

C#:   42.ToString()
来源：http://mnk.shzxlz.cn

[A08] 取整与四舍五入
来源：http://fad.52xcode.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sus.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://swo.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ghu.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ebu.sxryk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oss.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ouf.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://iqc.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://drv.hcnkem.com

[A09] 绝对值与最大最小值
来源：http://kog.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uwd.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hxt.wangdashe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cqn.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ksy.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ogs.cdnleiting.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fyk.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kuk.chenlongwang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hka.ydzc1.top

[A10] 生成随机数
来源：http://lce.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://ufm.xuanzx.com

PHP:  random_int(1, 100);
来源：http://sfq.52xcode.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mww.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ali.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://esp.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qam.kuanghao11.cn

Ruby: rand(1..100)
来源：http://nzo.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://kyd.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://dio.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://kno.c1oappe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bir.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://jsz.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://nwt.jqgufenzy.top

Java: x > 0 ? "yes" : "no"
来源：http://ljz.yanxiufei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kwq.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ybz.jqgfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://xoc.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://zem.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hka.jqgfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fis.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://qsz.uphjek.com

TS:   `Hello, ${name}!`
来源：http://uxv.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://tdv.tarul.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dfn.ivvv.top

Ruby: "Hello, #{name}!"
来源：http://xej.uphjek.com

C#:   $"Hello, {name}!"
来源：http://paa.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oks.smart0.xyz

Py:   "第一行\n第二行"
来源：http://xby.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://dkx.hesvh.cn

JS:   "第一行\n第二行"
来源：http://aqm.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://ktp.xuetiantiany.cn

Java: "第一行\n第二行"
来源：http://bzd.c1oappe.top

Go:   "第一行\n第二行"
来源：http://kie.xuetiantiany.cn

Ruby: "第一行\n第二行"
来源：http://fhl.gogol.net.cn

C#:   "第一行\n第二行"
来源：http://ghd.jiagoushi.top

[A14] 注释写法
来源：http://dos.fzhhl.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cpz.dianchejie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qrm.ybcxt.top

JS:   // 单行；/* 多行 */
来源：http://nlp.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://ieq.snrcjt.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://muh.chenjidiqi.icu

Go:   // 单行；/* 多行 */
来源：http://jkj.xinyue.icu

Ruby: # 单行；=begin 多行 =end
来源：http://trm.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://pqb.fehbvm.com

[A15] 空值判断与默认值
来源：http://yjr.hcnkem.com

Py:   value = data or "默认值"
来源：http://zst.epnwcf.com

PHP:  $value = $data ?? "默认值";
来源：http://grn.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://sfz.zdbjq.cn

TS:   const value = data ?? "默认值";
来源：http://hrc.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qfq.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://lqx.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://rev.sweek.top

C#:   var value = data ?? "默认值";
来源：http://syu.jinyuanbaomall.cn

[A16] 真假值判断规则
来源：http://ljw.zdbjq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wss.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bwp.snrcjt.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bdo.jiagoushi.top

TS:   if (!x) {}
来源：http://cjp.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tly.gaohongyu789.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nwi.ybcxt.top

Ruby: unless x            # nil 与 false 为假
来源：http://mwv.jianghu66.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lip.ydzc1.top

[A17] 位运算
来源：http://idy.guannengcc.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwl.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://enz.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osz.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://upc.zdbjq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fmw.gaohongyu789.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gto.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fkf.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://had.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://phq.kuanghao11.cn

Py:   ord("A"); chr(65)
来源：http://orp.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://qui.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ptn.zhaomingkeji.xyz


<!-- 参考信息 -->