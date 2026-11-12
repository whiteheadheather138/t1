代发 wailian999

[U101] JS：classList 操作
来源：http://naf.0kj1m.cn

el.classList.toggle("active")
来源：http://soc.fengsongda.top

[U102] JS：本地存储
来源：http://zct.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://umi.snrcjt.cn

[U103] JS：定时器
来源：http://gyc.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oii.c1oappe.top

[U104] JS：防抖
来源：http://qtx.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdg.yanxiufei.cn

[U105] JS：节流
来源：http://kth.yueranfly.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cjp.smart0.xyz

[U106] JS：日期格式化
来源：http://vnt.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nan.quarkkingdee.top

[U107] JS：数字千分位
来源：http://ooe.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tls.zhixingplan.top

[U108] JS：随机整数
来源：http://huv.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bht.gotoacloud.top

[U109] JS：数组分组
来源：http://mkn.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://mzv.zhengqikj.top

[U110] JS：数组分块
来源：http://ibe.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qem.dianchejie.cn

[U111] JS：对象转 Map
来源：http://xer.bjfxy.top

new Map(Object.entries(obj))
来源：http://ysp.dianchejie.cn

[U112] JS：字符串补位
来源：http://fcu.yj20258.top

"7".padStart(3, "0")
来源：http://krx.smart0.xyz

[U113] JS：正则替换全部
来源：http://hja.havefunace.top

s.replaceAll("a", "b")
来源：http://mtj.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://vir.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oqv.zdbjq.cn

[U115] JS：生成 UUID
来源：http://ztw.yj202588.top

crypto.randomUUID()
来源：http://lkb.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://tnc.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://omm.cqqwz.cn

[U117] JS：单元测试
来源：http://wdi.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://tbc.mhx1999.top

[U118] JS：开发服务器
来源：http://wzy.hcnkem.com

npm i -D vite;  npx vite
来源：http://mqy.yj20258.top

[U119] JS：生产构建
来源：http://oom.316326.xyz

npx vite build
来源：http://qhf.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://ugr.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://xmg.meibo888.top

================================================================================
来源：http://ecp.gotoacloud.top

统计汇总
来源：http://fwa.yj20258.top

================================================================================
来源：http://pez.bjfxy.top

按语言统计（条）：
来源：http://xvp.cdnleiting.top

Python ......... 252
来源：http://dhp.fengsongda.top

PHP ............ 252
来源：http://cuq.feifeiyinyue.top

JavaScript ..... 252
来源：http://hwu.chenzaomai.com

TypeScript ..... 212
来源：http://uck.guannengcc.top

Java ........... 212
来源：http://tuf.ctjpmb.com

Go ............. 212
来源：http://rif.ivvv.top

Ruby ........... 212
来源：http://nnx.hnqzz.top

C# ............. 212
来源：http://anr.xylfe.cn

C .............. 30
来源：http://cce.vehdjk.com

C++ ............ 30
来源：http://rvl.havefunace.top

SQL ............ 90
来源：http://cjn.yongpay.top

Bash ........... 80
来源：http://lhb.sxryk.cn

Kotlin ......... 15
来源：http://hpj.nanxinkj.top

Swift .......... 15
来源：http://hui.vehdjk.com

Lua ............ 10
来源：http://ntj.fktsv.cn

Perl ........... 10
来源：http://kex.yuanzhike.top

Scala .......... 10
来源：http://nml.vehdjk.com

------------------------------------
来源：http://icb.kuanghao11.cn

合计 ........... 2106 条
来源：http://icu.tarul.cn

按章节统计：
来源：http://mnb.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vzi.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ryc.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pro.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rch.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://spn.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wft.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kcs.zhijiandao.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sux.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ote.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nzx.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hvf.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hai.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://suy.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://abh.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ost.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bgd.bjfxy.top

Q SQL 专题                              90
来源：http://zns.sufxvd.cn

R Bash 专题                             80
来源：http://oku.ctjpmb.com

S C / C++ 专题                          60
来源：http://wfs.gotoacloud.top

T 其他语言补充                          60
来源：http://pyy.ydzc1.top

U 高频实用片段                         120
来源：http://zzi.dashuyun.cn

------------------------------------
来源：http://vpb.uphjek.com

合计                                  2106 条
来源：http://gcv.pycfn.com

--------------------------------------------------------------------------------
来源：http://vwc.chenzaomai.com

使用提醒
来源：http://wjp.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://ykp.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zzv.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ksk.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kaq.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mnl.havefunace.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gwf.gzhubu.top

—— 文件结束 ——
来源：http://qyn.xuetiantiany.cn

================================================================================
来源：http://nzw.c1oappe.top

程序语言常见例子速查手册（2024 版）
来源：http://xdt.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://vsh.wangdashe.top

================================================================================
来源：http://dwn.xuetiantiany.cn

【收录内容】
来源：http://esx.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://iyq.daxiang520.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jpd.fzhhl.top

SQL · Bash · C · C++
来源：http://fkd.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xmm.daxiang520.top

【使用说明】
来源：http://ymw.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://euh.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://plm.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://azi.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zdg.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ene.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zlk.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ops.zycfv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pdg.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mrr.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://srv.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lha.ctjpmb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://evn.pycfn.com

【文件统计】
来源：http://tzj.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ocs.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://ebw.jinqigufen.top

目  录
来源：http://bue.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://bys.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dzh.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wqy.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://naa.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fzx.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gsh.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gdl.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rrb.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mch.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vvn.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ogj.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ico.jinghuilouyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blb.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vjx.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://euo.ywan-chungtsiang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zml.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kpf.cashguo.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aoj.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://uec.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vzy.aizwys.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vid.iojbl.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fkj.chenzaomai.com

================================================================================
来源：http://inu.yuanzhike.top

A. 基础语法与类型
来源：http://imt.shuidangran.top

================================================================================
来源：http://opq.yj202588.top

[A01] Hello World
来源：http://wik.jinqigufen.top

Py:   print("Hello, World!")
来源：http://efb.fengsongda.top

PHP:  echo "Hello, World!";
来源：http://uur.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://xfq.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lfr.fengsongda.top

Java: System.out.println("Hello, World!");
来源：http://akl.cucudq.cn

Go:   fmt.Println("Hello, World!")
来源：http://kyv.fehbvm.com

Ruby: puts "Hello, World!"
来源：http://rdg.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://eav.quarkkingdee.top

[A02] 变量声明与赋值
来源：http://dsg.fktsv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ekw.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ocw.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://rhx.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xtx.jyoumei.cn

Java: String name = "Alex"; int age = 20;
来源：http://dxu.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://ciw.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://hzm.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://svx.ppjwa.cn

[A03] 常量定义
来源：http://cim.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yuw.birdmap.top

PHP:  const PI = 3.14159;
来源：http://gwh.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://zsj.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://zxw.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://exs.smart0.xyz

Go:   const PI = 3.14159
来源：http://kis.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://xiv.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://eez.fzhhl.top

[A04] 判断变量类型
来源：http://non.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ecb.jinghuilouyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nhw.xingfuxueyuan.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tmu.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://sqm.zycfv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gsg.zhaomingkeji.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://zae.quarkkingdee.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ogz.hfpthk.cn

C#:   x.GetType().Name; x is int
来源：http://mde.shuidangran.top

[A05] 整数除法与取模
来源：http://eqx.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://shz.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://zcn.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nwy.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://npx.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://uyi.yonumen.top

Go:   7 / 2; 7 % 2
来源：http://ema.gzhubu.top

Ruby: 7 / 2; 7 % 2
来源：http://cfk.fanxiaobao.xyz

C#:   7 / 2; 7 % 2
来源：http://ive.wangshuangyany.cn

[A06] 字符串转数字
来源：http://cva.fzhhl.top

Py:   int("42"); float("3.14")
来源：http://dnk.ydjk.org.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vqx.redwolf501.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hdp.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://myg.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://whh.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jqw.sysykeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cwy.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://noc.sjlbkw.cn

[A07] 数字转字符串
来源：http://zty.yj202588.top

Py:   str(42)
来源：http://lwo.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://jnq.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://soo.zhiwuduotai.top

TS:   String(42)
来源：http://udd.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sqb.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://nud.zhiwuduotai.top

Ruby: 42.to_s
来源：http://pip.jqgufenzy.top

C#:   42.ToString()
来源：http://vvy.meibo888.top

[A08] 取整与四舍五入
来源：http://ipn.gaohongyu789.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://set.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://owi.fengsongda.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://twr.zhijiandao.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cjm.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wxn.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yhm.kuanghao11.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xpw.kuanghao11.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zap.cdnleiting.top

[A09] 绝对值与最大最小值
来源：http://pob.yongpay.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iwg.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zko.sjlbkw.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://aim.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://asv.hesvh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qwb.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://grj.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tks.ywan-chungtsiang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tat.shuidangran.top

[A10] 生成随机数
来源：http://sgy.mhx1999.top

Py:   import random; random.randint(1, 100)
来源：http://vad.yonumen.top

PHP:  random_int(1, 100);
来源：http://xvg.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bsj.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vhg.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://nfq.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jul.ctjpmb.com

Ruby: rand(1..100)
来源：http://mvr.shanyushiyangtech.top

C#:   new Random().Next(1, 101)
来源：http://evo.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://mpo.yanxiufei.cn

Py:   "yes" if x > 0 else "no"
来源：http://ame.birdmap.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zsz.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://srs.nwbrower.top

TS:   x > 0 ? "yes" : "no"
来源：http://coa.yuxming.cn

Java: x > 0 ? "yes" : "no"
来源：http://utu.xingfuxueyuan.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://vbx.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jra.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://awx.tanke756.top

[A12] 字符串插值 / 格式化
来源：http://tfo.xziqi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jxb.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://exj.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://gvv.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://gcv.ivvv.top

Java: "Hello, %s!".formatted(name)
来源：http://szj.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://szl.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://aoc.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://vjl.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uzl.zhixingplan.top

Py:   "第一行\n第二行"
来源：http://bem.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://qqn.jyoumei.cn

JS:   "第一行\n第二行"
来源：http://kyp.hfpthk.cn

TS:   "第一行\n第二行"
来源：http://gkn.jinqigufen.top

Java: "第一行\n第二行"
来源：http://apo.zdbjq.cn

Go:   "第一行\n第二行"
来源：http://bth.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://pls.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://ahf.yuxming.cn

[A14] 注释写法
来源：http://msr.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kyo.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kfi.hysaishi.cn

JS:   // 单行；/* 多行 */
来源：http://hyv.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://fsz.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aot.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://zec.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rkd.nanxinkj.top

C#:   // 单行；/* 多行 */
来源：http://sbc.svipenyu.cn

[A15] 空值判断与默认值
来源：http://pue.yfazqb.com

Py:   value = data or "默认值"
来源：http://msj.hywenlv.cn

PHP:  $value = $data ?? "默认值";
来源：http://fuz.guowangkeji.top

JS:   const value = data ?? "默认值";
来源：http://mmf.zycfv.cn

TS:   const value = data ?? "默认值";
来源：http://oxf.vehdjk.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ueo.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://nyx.hcnkem.com

Ruby: value = data || "默认值"
来源：http://xxm.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://pvn.jyoumei.cn

[A16] 真假值判断规则
来源：http://sgd.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fdv.tian-w.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sfm.havefunace.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://szq.xziqi.cn

TS:   if (!x) {}
来源：http://xdf.chenlongwang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ocj.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qdp.cqqwz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xku.yangfankeji.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gqf.zycfv.cn

[A17] 位运算
来源：http://few.sufxvd.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qwx.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mbh.sysykeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vdf.ctjpmb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cip.kuanghao11.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iiz.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hgh.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nfk.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isb.hywenlv.cn


<!-- 参考信息 -->