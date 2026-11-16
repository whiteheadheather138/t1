代发 wailian999

[U103] JS：定时器
来源：http://fwv.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rpq.gotoacloud.top

[U104] JS：防抖
来源：http://mnp.cheryme.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nch.iojbl.cn

[U105] JS：节流
来源：http://lvo.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://htz.yueranfly.top

[U106] JS：日期格式化
来源：http://dlt.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pic.zdqjudy.top

[U107] JS：数字千分位
来源：http://frv.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oju.jqgfzy.top

[U108] JS：随机整数
来源：http://fyl.yvedp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hem.snrcjt.cn

[U109] JS：数组分组
来源：http://coa.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://kvm.wangdashe.top

[U110] JS：数组分块
来源：http://wnn.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jez.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://isd.316326.xyz

new Map(Object.entries(obj))
来源：http://qpw.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://hwx.jinghuilouyu.cn

"7".padStart(3, "0")
来源：http://ehn.hysaishi.cn

[U113] JS：正则替换全部
来源：http://url.tian-w.cn

s.replaceAll("a", "b")
来源：http://laa.hnqzz.top

[U114] JS：JSON 深比较
来源：http://npn.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jro.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://sgr.dashuyun.cn

crypto.randomUUID()
来源：http://diz.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://avu.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://awx.tianlin.xyz

[U117] JS：单元测试
来源：http://gkn.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://hih.jlsjyb.cn

[U118] JS：开发服务器
来源：http://tdz.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://cka.hongshengwenyu.top

[U119] JS：生产构建
来源：http://wrx.gotoacloud.top

npx vite build
来源：http://uux.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://cqx.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://fym.shanyushiyangkeji.top

================================================================================
来源：http://jdq.zhaomingkeji.xyz

统计汇总
来源：http://uki.xziqi.cn

================================================================================
来源：http://jzr.dianchejie.cn

按语言统计（条）：
来源：http://syn.vehdjk.com

Python ......... 252
来源：http://iuu.sweek.top

PHP ............ 252
来源：http://lmv.sjlbkw.cn

JavaScript ..... 252
来源：http://bng.daria6918.cn

TypeScript ..... 212
来源：http://ywa.wangdashe.top

Java ........... 212
来源：http://qvu.jqgfzy.top

Go ............. 212
来源：http://vzd.ctjpmb.com

Ruby ........... 212
来源：http://yfk.andypj.xyz

C# ............. 212
来源：http://eiz.yanxiufei.cn

C .............. 30
来源：http://yqw.gotoacloud.top

C++ ............ 30
来源：http://ebv.vehdjk.com

SQL ............ 90
来源：http://jet.guannengcc.top

Bash ........... 80
来源：http://xru.sjlbkw.cn

Kotlin ......... 15
来源：http://ack.jianghu66.top

Swift .......... 15
来源：http://gsv.shzxlz.cn

Lua ............ 10
来源：http://ntj.ybcxt.top

Perl ........... 10
来源：http://duv.daxiang520.top

Scala .......... 10
来源：http://wsb.tarul.cn

------------------------------------
来源：http://ulg.zycfv.cn

合计 ........... 2106 条
来源：http://mif.ydzc1.top

按章节统计：
来源：http://npd.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ixb.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qsl.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blk.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tol.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://edl.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ppl.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kch.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nwl.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://upz.xinyue.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://njz.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rtk.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jzp.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ida.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ovz.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dca.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qju.andypj.xyz

Q SQL 专题                              90
来源：http://gzq.xuetiantiany.cn

R Bash 专题                             80
来源：http://nnd.ydjk.org.cn

S C / C++ 专题                          60
来源：http://xed.shuidangran.top

T 其他语言补充                          60
来源：http://fqg.ydjk.org.cn

U 高频实用片段                         120
来源：http://ghz.cashguo.top

------------------------------------
来源：http://hdd.sysykeji.top

合计                                  2106 条
来源：http://wts.cucudq.cn

--------------------------------------------------------------------------------
来源：http://gfq.yanxiufei.cn

使用提醒
来源：http://xkc.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://udj.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://krx.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uqx.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pkz.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://cez.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ymu.yonumen.top

—— 文件结束 ——
来源：http://cmg.smart0.xyz

================================================================================
来源：http://fgv.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://pvf.yueranfly.top

Common Programming Examples Cheat Book
来源：http://xpo.xinyue.icu

================================================================================
来源：http://eyy.52xcode.cn

【收录内容】
来源：http://qlx.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nir.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uuy.pengpengdd.cyou

SQL · Bash · C · C++
来源：http://bts.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://egp.ydjk.org.cn

【使用说明】
来源：http://mhb.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zuv.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mwa.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kpr.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gii.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://wvp.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yuq.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hcp.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tfu.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xed.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://olb.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yrj.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tnn.jinqigfzy.top

【文件统计】
来源：http://mbm.hongshengwenyu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ctg.meibo888.top

--------------------------------------------------------------------------------
来源：http://ctj.shangyingyoupin.top

目  录
来源：http://xwx.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://iau.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kfo.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jwj.yuanzhike.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rwq.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uaf.smart0.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nas.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fcv.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wpj.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fch.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zhi.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ajs.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://byu.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nus.tian-w.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gai.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oxz.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xtr.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qoo.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jhx.ywan-chungtsiang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lch.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yxm.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zzt.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://krv.yj20258.top

================================================================================
来源：http://yja.feifeiyinyue.top

A. 基础语法与类型
来源：http://cst.tianlin.xyz

================================================================================
来源：http://syt.cdnleiting.top

[A01] Hello World
来源：http://jzy.fzhhl.top

Py:   print("Hello, World!")
来源：http://xcv.redwolf501.top

PHP:  echo "Hello, World!";
来源：http://wnu.meibo888.top

JS:   console.log("Hello, World!");
来源：http://xfe.bjfxy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tsp.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://ygb.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://zbh.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://oty.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mne.yangfankeji.com

[A02] 变量声明与赋值
来源：http://wml.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yfi.aizwys.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hwr.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tam.yonumen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pmq.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://yxk.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://xol.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://ldk.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://ipp.tarul.cn

[A03] 常量定义
来源：http://vnm.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fzw.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://ire.ivvv.top

JS:   const PI = 3.14159;
来源：http://sse.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://vwt.ydzc1.top

Java: static final double PI = 3.14159;
来源：http://pwh.guowangkeji.top

Go:   const PI = 3.14159
来源：http://vzm.tanke756.top

Ruby: PI = 3.14159
来源：http://awp.zhaomingkeji.xyz

C#:   const double PI = 3.14159;
来源：http://vms.sweek.top

[A04] 判断变量类型
来源：http://hvy.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xyd.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gxh.zhongyouzk.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oka.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://ztb.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aku.chenjidiqi.icu

Go:   reflect.TypeOf(x).Name()
来源：http://wxw.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vws.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://pjc.nanxuanxn.top

[A05] 整数除法与取模
来源：http://vkv.hysaishi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zyu.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://aad.smart0.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wxj.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://opg.shzxlz.cn

Java: 7 / 2; 7 % 2
来源：http://sjt.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://ozf.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://zwq.sweek.top

C#:   7 / 2; 7 % 2
来源：http://jkx.hesvh.cn

[A06] 字符串转数字
来源：http://kvp.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://wgw.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vzo.hysaishi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rcu.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://ujg.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qjh.xuanzx.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://flp.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qfn.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kzi.guowangkeji.top

[A07] 数字转字符串
来源：http://dcq.tian-w.cn

Py:   str(42)
来源：http://bsi.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://jss.hesvh.cn

JS:   String(42); (42).toString()
来源：http://kaf.smart0.xyz

TS:   String(42)
来源：http://nhh.jinqigufen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://crc.zhixingplan.top

Go:   strconv.Itoa(42)
来源：http://gay.shzxlz.cn

Ruby: 42.to_s
来源：http://ntc.nanxinkj.top

C#:   42.ToString()
来源：http://kyo.cheryme.top

[A08] 取整与四舍五入
来源：http://xza.aibaodan.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://brm.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://isq.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vna.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vqi.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tpy.dianchejie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pha.bjfxy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hui.hongshengwenyu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wge.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://pge.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://atd.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://msm.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bcf.xuanzx.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://crc.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ksc.nanxuanxn.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hua.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qvl.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://isg.sxryk.cn

[A10] 生成随机数
来源：http://ytt.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://luw.yongpay.top

PHP:  random_int(1, 100);
来源：http://jrq.zhiwuduotai.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kqp.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://taz.xinyue.icu

Java: new Random().nextInt(100) + 1
来源：http://mxj.9152youxi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qjc.yfazqb.com

Ruby: rand(1..100)
来源：http://rnd.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://cis.yangfankeji.com

[A11] 条件表达式（三元）
来源：http://nek.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://hmg.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://usj.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://yxv.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mgx.yfazqb.com

Java: x > 0 ? "yes" : "no"
来源：http://zbb.tianlin.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://nmg.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rgi.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://hvr.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://wjq.tian-w.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xkl.shanyushiyangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oul.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://qwo.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://jmh.ydjk.org.cn

Java: "Hello, %s!".formatted(name)
来源：http://fjv.gzhubu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bxg.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://lta.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://ioz.hesvh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://trn.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://vtg.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://kki.quarkkingdee.top

JS:   "第一行\n第二行"
来源：http://eby.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://ivh.shanyushiyangtech.top

Java: "第一行\n第二行"
来源：http://jsl.xinyue.icu

Go:   "第一行\n第二行"
来源：http://hki.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://dih.jinqigfzy.top

C#:   "第一行\n第二行"
来源：http://mli.wangshuangyany.cn

[A14] 注释写法
来源：http://vpl.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mvv.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bsy.smart0.xyz

JS:   // 单行；/* 多行 */
来源：http://ybh.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://nhb.birdmap.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oky.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://sxi.tarul.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tus.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://kgr.ppjwa.cn

[A15] 空值判断与默认值
来源：http://lgw.sysykeji.top

Py:   value = data or "默认值"
来源：http://kma.vqdsnc.cn

PHP:  $value = $data ?? "默认值";
来源：http://sde.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://sqc.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://few.zdbjq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://chs.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://onf.zhongyouzk.top

Ruby: value = data || "默认值"
来源：http://htz.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://jzs.9152youxi.cn

[A16] 真假值判断规则
来源：http://pwa.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pvv.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cyw.xuanzx.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vnu.chenzaomai.com

TS:   if (!x) {}
来源：http://lzx.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hfo.9152youxi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xku.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://hef.316326.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cfm.yuxming.cn

[A17] 位运算
来源：http://lrb.yangfankeji.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eut.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fkf.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xec.ivvv.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tav.ehwqpu.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pky.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://piq.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gbj.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zgq.jinqigfzy.top

[A18] 字符与 ASCII 码互转
来源：http://oze.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://hdz.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://zcs.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://axx.hnxiangtu.top


<!-- 参考信息 -->