代发 wailian999

[U103] JS：定时器
来源：http://mzq.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tod.hongshengwenyu.top

[U104] JS：防抖
来源：http://tvd.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dsy.chenzaomai.com

[U105] JS：节流
来源：http://ygd.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vdi.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://iok.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ypo.ivvv.top

[U107] JS：数字千分位
来源：http://rze.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ctg.daxiang520.top

[U108] JS：随机整数
来源：http://rht.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://amu.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://ega.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://ukb.fktsv.cn

[U110] JS：数组分块
来源：http://uud.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://obm.fehbvm.com

[U111] JS：对象转 Map
来源：http://dym.tarul.cn

new Map(Object.entries(obj))
来源：http://hnr.xziqi.cn

[U112] JS：字符串补位
来源：http://lsw.ybcxt.top

"7".padStart(3, "0")
来源：http://uag.ctjpmb.com

[U113] JS：正则替换全部
来源：http://kkr.fktsv.cn

s.replaceAll("a", "b")
来源：http://hkc.bjfxy.top

[U114] JS：JSON 深比较
来源：http://yxf.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rwa.chenlongwang.top

[U115] JS：生成 UUID
来源：http://tkv.xylfe.cn

crypto.randomUUID()
来源：http://zxq.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://nzs.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://kpk.wangshuangyany.cn

[U117] JS：单元测试
来源：http://jui.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://roo.cashguo.top

[U118] JS：开发服务器
来源：http://ary.hysaishi.cn

npm i -D vite;  npx vite
来源：http://lez.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://qtj.fzhhl.top

npx vite build
来源：http://zuo.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://rvl.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://deo.vqdsnc.cn

================================================================================
来源：http://lhs.gzhubu.top

统计汇总
来源：http://wsn.aizwys.cn

================================================================================
来源：http://gxe.zdqjudy.top

按语言统计（条）：
来源：http://iqm.smart0.xyz

Python ......... 252
来源：http://phd.zycfv.cn

PHP ............ 252
来源：http://pne.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://qfq.dianchejie.cn

TypeScript ..... 212
来源：http://ywo.yvedp.cn

Java ........... 212
来源：http://nql.yueranfly.top

Go ............. 212
来源：http://yxa.nanxuanxn.top

Ruby ........... 212
来源：http://hdp.0kj1m.cn

C# ............. 212
来源：http://ysw.nwbrower.top

C .............. 30
来源：http://tsk.yueranfly.top

C++ ............ 30
来源：http://gmw.nanxuanxn.top

SQL ............ 90
来源：http://rxk.zhiwuduotai.top

Bash ........... 80
来源：http://baw.epnwcf.com

Kotlin ......... 15
来源：http://cqx.jinqigufen.top

Swift .......... 15
来源：http://ijk.yangfankeji.com

Lua ............ 10
来源：http://mtr.havefunace.top

Perl ........... 10
来源：http://aee.yj20258.top

Scala .......... 10
来源：http://jzb.cashguo.top

------------------------------------
来源：http://caf.meibo888.top

合计 ........... 2106 条
来源：http://lbs.shanyushiyangkeji.top

按章节统计：
来源：http://bsz.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qec.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vtk.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zmj.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://shl.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bcp.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cmj.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wpc.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eiq.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://llr.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wnr.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ptw.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tps.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wod.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tzd.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hcj.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ycn.yvedp.cn

Q SQL 专题                              90
来源：http://itn.fengsongda.top

R Bash 专题                             80
来源：http://woh.ehwqpu.com

S C / C++ 专题                          60
来源：http://daz.bjfxy.top

T 其他语言补充                          60
来源：http://ola.9152youxi.cn

U 高频实用片段                         120
来源：http://vxk.c1oappe.top

------------------------------------
来源：http://exb.hongshengwenyu.top

合计                                  2106 条
来源：http://xxc.vehdjk.com

--------------------------------------------------------------------------------
来源：http://snb.vqdsnc.cn

使用提醒
来源：http://thy.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://jmh.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vfx.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://evi.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tts.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cep.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lay.ppjwa.cn

—— 文件结束 ——
来源：http://xrt.ctjpmb.com

================================================================================
来源：http://iwf.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://wwy.tarul.cn

Common Programming Examples Cheat Book
来源：http://xjw.vqdsnc.cn

================================================================================
来源：http://ufm.hnxiangtu.top

【收录内容】
来源：http://kqq.cashguo.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xlb.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xqx.cucudq.cn

SQL · Bash · C · C++
来源：http://vis.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dob.tianlin.xyz

【使用说明】
来源：http://pwg.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ylj.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qgr.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://acz.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rzd.jqgfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jwv.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yrw.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bla.hongshengwenyu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ohs.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kkc.cucudq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uqq.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dnr.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dep.jianghu66.top

【文件统计】
来源：http://drw.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cef.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://yah.hywenlv.cn

目  录
来源：http://wrq.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://fmh.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mor.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dzn.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dfn.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hll.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://guk.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vlk.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lsl.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hyk.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rvb.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xwe.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://aac.fzhhl.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wbh.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uct.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bdc.birdmap.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nxd.52xcode.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dih.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rfh.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kri.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://srd.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ksb.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oju.sjlbkw.cn

================================================================================
来源：http://ora.xuanzx.com

A. 基础语法与类型
来源：http://xhu.yueranfly.top

================================================================================
来源：http://pxf.chenjidiqi.icu

[A01] Hello World
来源：http://xfm.xylfe.cn

Py:   print("Hello, World!")
来源：http://hju.uphjek.com

PHP:  echo "Hello, World!";
来源：http://bro.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://wvs.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zoz.shanyushiyangkeji.top

Java: System.out.println("Hello, World!");
来源：http://mgr.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://lcc.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://xde.fengsongda.top

C#:   Console.WriteLine("Hello, World!");
来源：http://sob.smart0.xyz

[A02] 变量声明与赋值
来源：http://uli.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tge.guannengcc.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fiw.fengsongda.top

JS:   let name = "Alex"; const age = 20;
来源：http://cjj.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vzr.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://jxj.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://cwz.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://izh.jianghu66.top

C#:   string name = "Alex"; int age = 20;
来源：http://pii.sxryk.cn

[A03] 常量定义
来源：http://wzn.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qdu.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://mat.birdmap.top

JS:   const PI = 3.14159;
来源：http://xxr.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://dhv.ybcxt.top

Java: static final double PI = 3.14159;
来源：http://snl.zycfv.cn

Go:   const PI = 3.14159
来源：http://yns.meibo888.top

Ruby: PI = 3.14159
来源：http://wgw.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://blq.hfpthk.cn

[A04] 判断变量类型
来源：http://bkt.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://icj.sufxvd.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tnq.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fyb.hammf.cn

TS:   typeof x; x instanceof Date
来源：http://kzt.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bum.yfazqb.com

Go:   reflect.TypeOf(x).Name()
来源：http://xnn.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vkx.316326.xyz

C#:   x.GetType().Name; x is int
来源：http://mtr.pengpengdd.cyou

[A05] 整数除法与取模
来源：http://bzs.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://edi.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gxd.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lzd.shanyushiyangtech.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ezw.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://cmc.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://ciy.jqgfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://xod.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://mja.yuxming.cn

[A06] 字符串转数字
来源：http://kvg.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://ofu.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pgy.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bfn.gzhubu.top

TS:   parseInt("42", 10); Number("42")
来源：http://rvw.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://brs.c1oappe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xwc.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://znd.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vbj.jqgfzy.top

[A07] 数字转字符串
来源：http://anp.jinyuanbaomall.cn

Py:   str(42)
来源：http://vwd.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://gsq.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://gbi.xziqi.cn

TS:   String(42)
来源：http://ilr.yj20258888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://puk.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://cne.0kj1m.cn

Ruby: 42.to_s
来源：http://dzh.tanke756.top

C#:   42.ToString()
来源：http://tps.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://gtr.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://phh.jqgufenzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://htz.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wco.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://awr.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://byy.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lkb.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mae.52xcode.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xvz.cucudq.cn

[A09] 绝对值与最大最小值
来源：http://gsp.vqdsnc.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fla.daria6918.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ihv.guannengcc.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blp.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qox.chenlongwang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://emo.fehbvm.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://njx.feifeiyinyue.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fhe.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ggx.yueranfly.top

[A10] 生成随机数
来源：http://vli.wangdashe.top

Py:   import random; random.randint(1, 100)
来源：http://con.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://rxn.jlsjyb.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://olg.shzxlz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://twi.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://fzo.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cid.yj202588.top

Ruby: rand(1..100)
来源：http://tsu.jyoumei.cn

C#:   new Random().Next(1, 101)
来源：http://tqj.havefunace.top

[A11] 条件表达式（三元）
来源：http://tht.hcnkem.com

Py:   "yes" if x > 0 else "no"
来源：http://hpw.jlsjyb.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xet.daria6918.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jre.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://sqw.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://www.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://her.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ocx.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://dtg.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://ebg.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lcb.shuidangran.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yyn.ctjpmb.com

JS:   `Hello, ${name}!`
来源：http://wzp.cdnleiting.top

TS:   `Hello, ${name}!`
来源：http://upr.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://myc.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oik.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://qvp.uphjek.com

C#:   $"Hello, {name}!"
来源：http://dgs.sweek.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nen.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://oom.ppjwa.cn

PHP:  "第一行\n第二行"
来源：http://izb.chenzaomai.com

JS:   "第一行\n第二行"
来源：http://wyi.daria6918.cn

TS:   "第一行\n第二行"
来源：http://vhe.xylfe.cn

Java: "第一行\n第二行"
来源：http://fop.redwolf501.top

Go:   "第一行\n第二行"
来源：http://xjg.chenjidiqi.icu

Ruby: "第一行\n第二行"
来源：http://iyj.yonumen.top

C#:   "第一行\n第二行"
来源：http://luy.sysykeji.top

[A14] 注释写法
来源：http://vvo.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qfg.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dpb.zhoulong.xyz

JS:   // 单行；/* 多行 */
来源：http://vuy.hnxiangtu.top

TS:   // 单行；/* 多行 */
来源：http://miv.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ide.dashuyun.cn

Go:   // 单行；/* 多行 */
来源：http://lpt.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://tff.fzhhl.top

C#:   // 单行；/* 多行 */
来源：http://ror.hnxiangtu.top

[A15] 空值判断与默认值
来源：http://xvr.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://ngr.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://abf.0kj1m.cn

JS:   const value = data ?? "默认值";
来源：http://ooh.xylfe.cn

TS:   const value = data ?? "默认值";
来源：http://xtk.hnxiangtu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ovx.316326.xyz

Go:   if data == "" { data = "默认值" }
来源：http://ywk.yj20258888.top

Ruby: value = data || "默认值"
来源：http://ydl.hongshengwenyu.top

C#:   var value = data ?? "默认值";
来源：http://wbq.yvedp.cn

[A16] 真假值判断规则
来源：http://tnm.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qbv.cashguo.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pbc.chenlongwang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cxy.dianchejie.cn

TS:   if (!x) {}
来源：http://dwx.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cfj.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pbo.daxiang520.top

Ruby: unless x            # nil 与 false 为假
来源：http://wgp.gogol.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kvc.yuanzhike.top

[A17] 位运算
来源：http://hrx.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwx.snrcjt.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xkx.gaohongyu789.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyr.epnwcf.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tnl.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aeq.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kmo.meibo888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wfv.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvm.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://iod.gzhubu.top

Py:   ord("A"); chr(65)
来源：http://tlz.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://nul.fengsongda.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yhs.quarkkingdee.top


<!-- 参考信息 -->