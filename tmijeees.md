代发 wailian999

[U103] JS：定时器
来源：http://gzh.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xkd.yangfankeji.com

[U104] JS：防抖
来源：http://aqc.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryk.guannengcc.top

[U105] JS：节流
来源：http://dqx.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ktg.yj20258888.top

[U106] JS：日期格式化
来源：http://grx.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://haz.ywan-chungtsiang.top

[U107] JS：数字千分位
来源：http://vbu.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rko.zhaomingkeji.xyz

[U108] JS：随机整数
来源：http://wwp.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bad.vqdsnc.cn

[U109] JS：数组分组
来源：http://izl.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://jdi.yj20258.top

[U110] JS：数组分块
来源：http://iyo.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gug.yj20258888.top

[U111] JS：对象转 Map
来源：http://iib.316326.xyz

new Map(Object.entries(obj))
来源：http://iun.vehdjk.com

[U112] JS：字符串补位
来源：http://cab.snrcjt.cn

"7".padStart(3, "0")
来源：http://wnb.cqqwz.cn

[U113] JS：正则替换全部
来源：http://zpl.cheryme.top

s.replaceAll("a", "b")
来源：http://jrm.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://wew.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tfp.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://xzj.ydzc1.top

crypto.randomUUID()
来源：http://zlz.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://qab.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://vwj.yj20258888.top

[U117] JS：单元测试
来源：http://qeu.yj202588.top

npm i -D vitest;  npx vitest
来源：http://ozs.zdqjudy.top

[U118] JS：开发服务器
来源：http://tel.ivvv.top

npm i -D vite;  npx vite
来源：http://uzr.guannengcc.top

[U119] JS：生产构建
来源：http://hrj.316326.xyz

npx vite build
来源：http://wzd.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://mhy.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://wok.nwbrower.top

================================================================================
来源：http://vgp.sufxvd.cn

统计汇总
来源：http://spf.jqgfzy.top

================================================================================
来源：http://rgm.aizwys.cn

按语言统计（条）：
来源：http://vou.shuidangran.top

Python ......... 252
来源：http://tes.zdbjq.cn

PHP ............ 252
来源：http://xxi.zhiwuduotai.top

JavaScript ..... 252
来源：http://qrn.daria6918.cn

TypeScript ..... 212
来源：http://vtr.xziqi.cn

Java ........... 212
来源：http://xvw.hesvh.cn

Go ............. 212
来源：http://jsy.shanyushiyangtech.top

Ruby ........... 212
来源：http://odn.ppjwa.cn

C# ............. 212
来源：http://qbx.ywan-chungtsiang.top

C .............. 30
来源：http://rdm.shangyingyoupin.top

C++ ............ 30
来源：http://xpw.bbcook.cn

SQL ............ 90
来源：http://dnv.ivvv.top

Bash ........... 80
来源：http://nja.andypj.xyz

Kotlin ......... 15
来源：http://niu.hnxiangtu.top

Swift .......... 15
来源：http://sae.316326.xyz

Lua ............ 10
来源：http://umy.9152youxi.cn

Perl ........... 10
来源：http://jtr.yuxming.cn

Scala .......... 10
来源：http://pvb.0kj1m.cn

------------------------------------
来源：http://orf.chenlongwang.top

合计 ........... 2106 条
来源：http://jep.gotoacloud.top

按章节统计：
来源：http://mnj.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rqv.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tyq.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wpn.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nwq.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eeg.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://imi.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://exm.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zxr.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xlg.sxryk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dfv.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ngo.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nzr.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ctx.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dxf.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wcv.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://feu.hnqzz.top

Q SQL 专题                              90
来源：http://gtj.sxryk.cn

R Bash 专题                             80
来源：http://ncs.guannengcc.top

S C / C++ 专题                          60
来源：http://nrx.gogol.net.cn

T 其他语言补充                          60
来源：http://zog.cucudq.cn

U 高频实用片段                         120
来源：http://ptg.snrcjt.cn

------------------------------------
来源：http://arb.andypj.xyz

合计                                  2106 条
来源：http://syl.tanke756.top

--------------------------------------------------------------------------------
来源：http://mvx.yanxiufei.cn

使用提醒
来源：http://sxo.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://qku.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rdd.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dzu.yj20258888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uta.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://afc.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ses.316326.xyz

—— 文件结束 ——
来源：http://zhz.yongpay.top

================================================================================
来源：http://dao.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://lnw.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://ijn.xuetiantiany.cn

================================================================================
来源：http://trm.hnxiangtu.top

【收录内容】
来源：http://tul.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ctv.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wbj.daria6918.cn

SQL · Bash · C · C++
来源：http://rid.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://svy.cucudq.cn

【使用说明】
来源：http://czh.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hrs.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tpn.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vax.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rwi.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xze.fengsongda.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ffb.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://swx.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dsv.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://npn.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://glt.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pul.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sfg.fzhhl.top

【文件统计】
来源：http://zkn.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lou.gzhubu.top

--------------------------------------------------------------------------------
来源：http://mzq.feifeiyinyue.top

目  录
来源：http://jiq.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://dyh.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lmq.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tft.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vry.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mzy.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dte.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nns.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vxl.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qzb.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qne.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rlj.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://enf.chenlongwang.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dxg.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dhu.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jvt.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rfr.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ehl.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kvt.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ccc.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zii.yongpay.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ezk.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ftk.jianghu66.top

================================================================================
来源：http://mfn.snrcjt.cn

A. 基础语法与类型
来源：http://dzi.fanxiaobao.xyz

================================================================================
来源：http://ajj.hfpthk.cn

[A01] Hello World
来源：http://ivd.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://grr.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://qpx.yuanzhike.top

JS:   console.log("Hello, World!");
来源：http://sme.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xuz.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://gmt.yj202588.top

Go:   fmt.Println("Hello, World!")
来源：http://kwu.havefunace.top

Ruby: puts "Hello, World!"
来源：http://mnc.smart0.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://vde.shangyingyoupin.top

[A02] 变量声明与赋值
来源：http://pia.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dvp.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ouo.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://maf.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://orq.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://xeu.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://fmw.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://wbf.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://iho.jqgfzy.top

[A03] 常量定义
来源：http://dql.jqgufenzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hgi.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://ecj.yj20258888.top

JS:   const PI = 3.14159;
来源：http://tan.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://ezb.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://aqg.jinqigufen.top

Go:   const PI = 3.14159
来源：http://nul.haohaochexian.top

Ruby: PI = 3.14159
来源：http://frb.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://yje.gzhubu.top

[A04] 判断变量类型
来源：http://kdw.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ucx.fzhhl.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://abu.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ztz.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://zlc.tanke756.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tyu.epnwcf.com

Go:   reflect.TypeOf(x).Name()
来源：http://bmp.shzxlz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://aog.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://hnr.andypj.xyz

[A05] 整数除法与取模
来源：http://tih.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ybe.jiagoushi.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://flq.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://por.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lvh.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://hfi.guowangkeji.top

Go:   7 / 2; 7 % 2
来源：http://ctg.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://fbr.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://tfu.hammf.cn

[A06] 字符串转数字
来源：http://kik.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://ycx.ctjpmb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tpu.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ecd.jlsjyb.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pzi.svipenyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://flg.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nuz.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ims.guannengcc.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mto.nwbrower.top

[A07] 数字转字符串
来源：http://tvb.yvedp.cn

Py:   str(42)
来源：http://yqh.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://dff.nwbrower.top

JS:   String(42); (42).toString()
来源：http://xly.vehdjk.com

TS:   String(42)
来源：http://tnd.zhaomingkeji.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://zjm.hysaishi.cn

Go:   strconv.Itoa(42)
来源：http://qid.52xcode.cn

Ruby: 42.to_s
来源：http://yly.guannengcc.top

C#:   42.ToString()
来源：http://nfn.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://deh.fktsv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zzn.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blr.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zpa.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ncf.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oow.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tuj.tarul.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hhu.fengsongda.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ajq.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://jvm.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zqz.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ryn.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ais.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iec.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cxp.yanxiufei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://opn.yj202588.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qiv.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wna.havefunace.top

[A10] 生成随机数
来源：http://cfe.zycfv.cn

Py:   import random; random.randint(1, 100)
来源：http://iby.xziqi.cn

PHP:  random_int(1, 100);
来源：http://fhq.yvedp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lcc.fengsongda.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tkd.xziqi.cn

Java: new Random().nextInt(100) + 1
来源：http://guu.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hdz.aibaodan.cn

Ruby: rand(1..100)
来源：http://vli.ybcxt.top

C#:   new Random().Next(1, 101)
来源：http://mxj.shzxlz.cn

[A11] 条件表达式（三元）
来源：http://hxw.jqgfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://uib.xuanzx.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://opn.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://zsk.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://smg.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://kyg.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ato.zdqjudy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ybr.ehwqpu.com

C#:   x > 0 ? "yes" : "no"
来源：http://kzb.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://lat.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vvf.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sda.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://bio.tarul.cn

TS:   `Hello, ${name}!`
来源：http://uro.yj20258888.top

Java: "Hello, %s!".formatted(name)
来源：http://jbr.xingfuxueyuan.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hyx.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://gxl.fanxiaobao.xyz

C#:   $"Hello, {name}!"
来源：http://oni.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wxr.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://grp.cqqwz.cn

PHP:  "第一行\n第二行"
来源：http://lyg.yonumen.top

JS:   "第一行\n第二行"
来源：http://itn.c1oappe.top

TS:   "第一行\n第二行"
来源：http://rci.sysykeji.top

Java: "第一行\n第二行"
来源：http://ivd.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://bhh.sweek.top

Ruby: "第一行\n第二行"
来源：http://lxi.dashuyun.cn

C#:   "第一行\n第二行"
来源：http://kep.ydjk.org.cn

[A14] 注释写法
来源：http://wid.zhoulong.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://jnf.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://niu.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://mbv.jinqigfzy.top

TS:   // 单行；/* 多行 */
来源：http://jgd.yj20258.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lno.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://qje.tarul.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bhw.nwbrower.top

C#:   // 单行；/* 多行 */
来源：http://mvs.xziqi.cn

[A15] 空值判断与默认值
来源：http://njl.zdqjudy.top

Py:   value = data or "默认值"
来源：http://pyz.guannengcc.top

PHP:  $value = $data ?? "默认值";
来源：http://yfw.ywan-chungtsiang.top

JS:   const value = data ?? "默认值";
来源：http://xky.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://kpg.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fnl.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://num.9152youxi.cn

Ruby: value = data || "默认值"
来源：http://gqd.gzhubu.top

C#:   var value = data ?? "默认值";
来源：http://xzj.jiagoushi.top

[A16] 真假值判断规则
来源：http://zjr.xingfuxueyuan.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jhd.feifeiyinyue.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://trj.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rgp.hysaishi.cn

TS:   if (!x) {}
来源：http://prf.chenjidiqi.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://twm.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uyk.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://cku.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aqr.cashguo.top

[A17] 位运算
来源：http://lvy.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vbv.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ebg.zhongyouzk.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srb.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://msk.shzxlz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qex.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wgk.yvedp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlo.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://liv.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://kby.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://vxm.ehwqpu.com

PHP:  ord("A"); chr(65)
来源：http://vje.svipenyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dcv.bjfxy.top


<!-- 参考信息 -->