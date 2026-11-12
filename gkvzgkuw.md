代发 wailian999

[U103] JS：定时器
来源：http://pll.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yyb.hywenlv.cn

[U104] JS：防抖
来源：http://rij.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://apn.yj20258.top

[U105] JS：节流
来源：http://pbi.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kzs.haohaochexian.top

[U106] JS：日期格式化
来源：http://jag.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jgp.jqgufenzy.top

[U107] JS：数字千分位
来源：http://jfj.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ahj.zdbjq.cn

[U108] JS：随机整数
来源：http://pkm.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cls.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://jke.fengsongda.top

Object.groupBy(arr, x => x.type)
来源：http://thh.quarkkingdee.top

[U110] JS：数组分块
来源：http://ilr.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yio.jyoumei.cn

[U111] JS：对象转 Map
来源：http://qnb.yueranfly.top

new Map(Object.entries(obj))
来源：http://lwq.jyoumei.cn

[U112] JS：字符串补位
来源：http://qqx.shzxlz.cn

"7".padStart(3, "0")
来源：http://zgm.ppjwa.cn

[U113] JS：正则替换全部
来源：http://ouw.sufxvd.cn

s.replaceAll("a", "b")
来源：http://byl.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://hcx.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ljk.wangdashe.top

[U115] JS：生成 UUID
来源：http://rma.sysykeji.top

crypto.randomUUID()
来源：http://iqu.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://fyi.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://flh.yj20258888.top

[U117] JS：单元测试
来源：http://sgj.birdmap.top

npm i -D vitest;  npx vitest
来源：http://fxz.xinyue.icu

[U118] JS：开发服务器
来源：http://ceb.birdmap.top

npm i -D vite;  npx vite
来源：http://otl.jqgufenzy.top

[U119] JS：生产构建
来源：http://dma.sufxvd.cn

npx vite build
来源：http://nau.aizwys.cn

[U120] JS：读取环境变量（Vite）
来源：http://nda.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://tns.wangdashe.top

================================================================================
来源：http://zuf.cucudq.cn

统计汇总
来源：http://mah.birdmap.top

================================================================================
来源：http://iyl.xuanzx.com

按语言统计（条）：
来源：http://whc.tanke756.top

Python ......... 252
来源：http://sql.yanxiufei.cn

PHP ............ 252
来源：http://gnw.yvedp.cn

JavaScript ..... 252
来源：http://vdj.vqdsnc.cn

TypeScript ..... 212
来源：http://uni.jinqigufen.top

Java ........... 212
来源：http://dza.hfpthk.cn

Go ............. 212
来源：http://vgb.jianghu66.top

Ruby ........... 212
来源：http://eou.tanke756.top

C# ............. 212
来源：http://atx.tarul.cn

C .............. 30
来源：http://tam.ybcxt.top

C++ ............ 30
来源：http://spg.shanyushiyangtech.top

SQL ............ 90
来源：http://zgs.jinghuilouyu.cn

Bash ........... 80
来源：http://fyu.jinghuilouyu.cn

Kotlin ......... 15
来源：http://efg.hesvh.cn

Swift .......... 15
来源：http://jzj.wangdashe.top

Lua ............ 10
来源：http://naa.yanxiufei.cn

Perl ........... 10
来源：http://nto.hywenlv.cn

Scala .......... 10
来源：http://dxq.hongshengwenyu.top

------------------------------------
来源：http://ops.yfazqb.com

合计 ........... 2106 条
来源：http://eau.tanke756.top

按章节统计：
来源：http://rmj.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ftt.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://euo.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mxs.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tho.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bdu.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kha.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sgx.yj202588.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cxz.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zog.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mae.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gok.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ahv.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gsy.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vpp.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ilf.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mqg.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://whw.0kj1m.cn

R Bash 专题                             80
来源：http://fji.pycfn.com

S C / C++ 专题                          60
来源：http://qfq.yfazqb.com

T 其他语言补充                          60
来源：http://tlr.kuanghao11.cn

U 高频实用片段                         120
来源：http://chx.ydjk.org.cn

------------------------------------
来源：http://ump.vqdsnc.cn

合计                                  2106 条
来源：http://lsr.iojbl.cn

--------------------------------------------------------------------------------
来源：http://xan.zhijiandao.cn

使用提醒
来源：http://wqz.yvedp.cn

--------------------------------------------------------------------------------
来源：http://shl.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oxa.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://skf.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ili.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xui.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dss.sufxvd.cn

—— 文件结束 ——
来源：http://dox.ppjwa.cn

================================================================================
来源：http://hik.tian-w.cn

程序语言常见例子速查手册（2024 版）
来源：http://rtn.ehwqpu.com

Common Programming Examples Cheat Book
来源：http://iom.shuidangran.top

================================================================================
来源：http://nwo.jqgfzy.top

【收录内容】
来源：http://xed.hnqzz.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jku.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bki.nwbrower.top

SQL · Bash · C · C++
来源：http://enb.birdmap.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iup.cdnleiting.top

【使用说明】
来源：http://niz.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gfj.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xnu.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kby.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xjy.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bst.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yjl.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nud.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ccc.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rkf.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ukd.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rlg.ydzc1.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hoo.hongshengwenyu.top

【文件统计】
来源：http://qox.yvedp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dfd.andypj.xyz

--------------------------------------------------------------------------------
来源：http://aqg.sjlbkw.cn

目  录
来源：http://qkh.gzhubu.top

--------------------------------------------------------------------------------
来源：http://yxd.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ndo.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bsu.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dbe.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jfo.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zxu.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wkh.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xge.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lir.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ycz.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lxl.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iba.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pdj.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tmw.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vpw.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bhc.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ydh.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bgf.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fkr.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hrq.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://koh.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ben.yj20258888.top

================================================================================
来源：http://pjd.daria6918.cn

A. 基础语法与类型
来源：http://mqh.yfazqb.com

================================================================================
来源：http://nbn.jyoumei.cn

[A01] Hello World
来源：http://ozq.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://mtj.hesvh.cn

PHP:  echo "Hello, World!";
来源：http://rgo.meibo888.top

JS:   console.log("Hello, World!");
来源：http://pig.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eoq.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://xgq.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://uoz.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://ryb.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://oiq.9152youxi.cn

[A02] 变量声明与赋值
来源：http://lpf.daxiang520.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sbe.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://kmn.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://tkp.ehwqpu.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ixt.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://ktt.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://byt.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://ebz.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://gpr.yj20258.top

[A03] 常量定义
来源：http://xtd.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iqp.bjfxy.top

PHP:  const PI = 3.14159;
来源：http://kwm.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://opp.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://yrp.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://okb.redwolf501.top

Go:   const PI = 3.14159
来源：http://xea.zhixingplan.top

Ruby: PI = 3.14159
来源：http://src.ehwqpu.com

C#:   const double PI = 3.14159;
来源：http://kyb.hnqzz.top

[A04] 判断变量类型
来源：http://zhv.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mtk.zdbjq.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zyr.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rzk.fktsv.cn

TS:   typeof x; x instanceof Date
来源：http://blw.sweek.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lis.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rev.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bpa.shzxlz.cn

C#:   x.GetType().Name; x is int
来源：http://adu.yonumen.top

[A05] 整数除法与取模
来源：http://tht.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yhe.cheryme.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lis.zhijiandao.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wwo.daxiang520.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nxs.nanxinkj.top

Java: 7 / 2; 7 % 2
来源：http://smd.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://yop.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://blf.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://kgr.guannengcc.top

[A06] 字符串转数字
来源：http://kpx.316326.xyz

Py:   int("42"); float("3.14")
来源：http://vbm.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qbs.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://puw.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://lxi.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tqs.gogol.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hdg.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qjl.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hai.guannengcc.top

[A07] 数字转字符串
来源：http://pkm.shanyushiyangkeji.top

Py:   str(42)
来源：http://wkx.cqqwz.cn

PHP:  (string) 42; strval(42)
来源：http://iyr.cashguo.top

JS:   String(42); (42).toString()
来源：http://vhr.aizwys.cn

TS:   String(42)
来源：http://gob.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yom.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://ati.chenzaomai.com

Ruby: 42.to_s
来源：http://bsa.gotoacloud.top

C#:   42.ToString()
来源：http://cmb.cqqwz.cn

[A08] 取整与四舍五入
来源：http://nyx.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qdl.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://del.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lhc.hysaishi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uzi.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xis.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rwi.hfpthk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tlf.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nmd.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://ave.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jiw.jqgufenzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vav.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ucd.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tvy.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tjp.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tqf.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ogy.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bod.zycfv.cn

[A10] 生成随机数
来源：http://vnu.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://rbn.uphjek.com

PHP:  random_int(1, 100);
来源：http://cmk.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ngt.ywan-chungtsiang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zpn.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://nbs.jiagoushi.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xoy.pengpengdd.cyou

Ruby: rand(1..100)
来源：http://hvt.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://zco.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://uat.ywan-chungtsiang.top

Py:   "yes" if x > 0 else "no"
来源：http://ogq.sysykeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://onf.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://mtm.ywan-chungtsiang.top

TS:   x > 0 ? "yes" : "no"
来源：http://ofb.yfazqb.com

Java: x > 0 ? "yes" : "no"
来源：http://hym.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xff.vqdsnc.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://soe.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://stm.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://bfw.jianghu66.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tfy.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oxr.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://ckv.uphjek.com

TS:   `Hello, ${name}!`
来源：http://lkh.jinghuilouyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://dwc.aibaodan.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gjd.chenzaomai.com

Ruby: "Hello, #{name}!"
来源：http://lml.9152youxi.cn

C#:   $"Hello, {name}!"
来源：http://oxe.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://zmm.zdqjudy.top

Py:   "第一行\n第二行"
来源：http://uwt.hammf.cn

PHP:  "第一行\n第二行"
来源：http://ptu.sxryk.cn

JS:   "第一行\n第二行"
来源：http://gmh.cheryme.top

TS:   "第一行\n第二行"
来源：http://ivy.ybcxt.top

Java: "第一行\n第二行"
来源：http://uqy.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://emz.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://rio.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://duf.52xcode.cn

[A14] 注释写法
来源：http://jkl.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dnh.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://hew.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://jqk.jinqigufen.top

TS:   // 单行；/* 多行 */
来源：http://tmf.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nah.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://pxe.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://tgf.sufxvd.cn

C#:   // 单行；/* 多行 */
来源：http://gwn.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://ftr.cashguo.top

Py:   value = data or "默认值"
来源：http://vux.hongshengwenyu.top

PHP:  $value = $data ?? "默认值";
来源：http://htw.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://hal.hywenlv.cn

TS:   const value = data ?? "默认值";
来源：http://fbz.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dvf.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://qob.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://bld.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://vfz.chenjidiqi.icu

[A16] 真假值判断规则
来源：http://rgx.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lke.snrcjt.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vyf.nanxinkj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lpx.xinyue.icu

TS:   if (!x) {}
来源：http://mxd.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zze.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dsi.gotoacloud.top

Ruby: unless x            # nil 与 false 为假
来源：http://awv.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://egf.jqgufenzy.top

[A17] 位运算
来源：http://wgb.vehdjk.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pkt.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dwa.shuidangran.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cab.jqgufenzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rzl.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmn.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lvo.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txx.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://elt.shanyushiyangtech.top

[A18] 字符与 ASCII 码互转
来源：http://xoz.yj20258.top

Py:   ord("A"); chr(65)
来源：http://hgu.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://jvs.yj202588.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://htj.guowangkeji.top


<!-- 参考信息 -->