代发 wailian999

[U99] JS：事件监听
来源：http://oyf.xuanzx.com

el.addEventListener("click", e => {})
来源：http://fed.cdnleiting.top

[U100] JS：DOM 查询
来源：http://lib.ppjwa.cn

document.querySelector(".item")
来源：http://qcf.hysaishi.cn

[U101] JS：classList 操作
来源：http://hxf.0kj1m.cn

el.classList.toggle("active")
来源：http://ipc.9152youxi.cn

[U102] JS：本地存储
来源：http://esx.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hpm.cucudq.cn

[U103] JS：定时器
来源：http://bpg.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://htf.sxryk.cn

[U104] JS：防抖
来源：http://bxs.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsy.52xcode.cn

[U105] JS：节流
来源：http://fnh.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mxe.jyoumei.cn

[U106] JS：日期格式化
来源：http://ibr.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oii.quarkkingdee.top

[U107] JS：数字千分位
来源：http://etq.fzhhl.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfl.316326.xyz

[U108] JS：随机整数
来源：http://lay.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dfr.smart0.xyz

[U109] JS：数组分组
来源：http://ify.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://zgl.yonumen.top

[U110] JS：数组分块
来源：http://uqc.kuanghao11.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jsd.shuidangran.top

[U111] JS：对象转 Map
来源：http://kui.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://mpf.tian-w.cn

[U112] JS：字符串补位
来源：http://knp.kuanghao11.cn

"7".padStart(3, "0")
来源：http://zhd.fengsongda.top

[U113] JS：正则替换全部
来源：http://tki.chenzaomai.com

s.replaceAll("a", "b")
来源：http://nrf.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://qym.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qdl.sweek.top

[U115] JS：生成 UUID
来源：http://xfq.quarkkingdee.top

crypto.randomUUID()
来源：http://dnl.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://nxd.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://tgf.sysykeji.top

[U117] JS：单元测试
来源：http://byg.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://elk.ivvv.top

[U118] JS：开发服务器
来源：http://uac.haohaochexian.top

npm i -D vite;  npx vite
来源：http://ofu.ybcxt.top

[U119] JS：生产构建
来源：http://nfs.zhoulong.xyz

npx vite build
来源：http://enh.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://bne.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://zpg.hcnkem.com

================================================================================
来源：http://qoe.jinqigufen.top

统计汇总
来源：http://nav.dashuyun.cn

================================================================================
来源：http://iit.jyoumei.cn

按语言统计（条）：
来源：http://yyt.jinqigfzy.top

Python ......... 252
来源：http://iem.shuidangran.top

PHP ............ 252
来源：http://npp.52xcode.cn

JavaScript ..... 252
来源：http://dvt.hfpthk.cn

TypeScript ..... 212
来源：http://epk.zhoulong.xyz

Java ........... 212
来源：http://djz.zdqjudy.top

Go ............. 212
来源：http://vks.fengsongda.top

Ruby ........... 212
来源：http://xup.jiagoushi.top

C# ............. 212
来源：http://ich.andypj.xyz

C .............. 30
来源：http://gdv.hammf.cn

C++ ............ 30
来源：http://qcs.hongshengwenyu.top

SQL ............ 90
来源：http://xzm.cqqwz.cn

Bash ........... 80
来源：http://ivx.bjfxy.top

Kotlin ......... 15
来源：http://pum.jianghu66.top

Swift .......... 15
来源：http://ayk.hnxiangtu.top

Lua ............ 10
来源：http://vep.kuanghao11.cn

Perl ........... 10
来源：http://ffm.tianlin.xyz

Scala .......... 10
来源：http://rie.yonumen.top

------------------------------------
来源：http://wbz.yj20258888.top

合计 ........... 2106 条
来源：http://few.gogol.net.cn

按章节统计：
来源：http://nki.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dsl.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hpn.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://clk.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mlh.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pag.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dsp.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lqr.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gcu.sysykeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vfi.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://htf.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ynt.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://les.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://igu.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://szt.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mdz.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eps.zhoulong.xyz

Q SQL 专题                              90
来源：http://kjj.wangshuangyany.cn

R Bash 专题                             80
来源：http://cyi.jqgfzy.top

S C / C++ 专题                          60
来源：http://qpt.wangshuangyany.cn

T 其他语言补充                          60
来源：http://idx.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://bnt.gaohongyu789.top

------------------------------------
来源：http://cqg.tianlin.xyz

合计                                  2106 条
来源：http://gxv.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ofp.yvedp.cn

使用提醒
来源：http://mwy.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://gae.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eau.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jbh.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://trc.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tdd.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dqh.fktsv.cn

—— 文件结束 ——
来源：http://ylj.cdnleiting.top

================================================================================
来源：http://via.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://jky.yj20258.top

Common Programming Examples Cheat Book
来源：http://qxz.vehdjk.com

================================================================================
来源：http://ukc.yvedp.cn

【收录内容】
来源：http://reb.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tos.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tzc.yonumen.top

SQL · Bash · C · C++
来源：http://kpc.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ppk.jqgfzy.top

【使用说明】
来源：http://rgj.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://huz.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hye.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ypo.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cxt.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://coi.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tuy.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://klx.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uvp.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ixf.hysaishi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dam.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tyr.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fuj.zdbjq.cn

【文件统计】
来源：http://wdd.zhaomingkeji.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ksa.birdmap.top

--------------------------------------------------------------------------------
来源：http://isx.vehdjk.com

目  录
来源：http://jaj.hammf.cn

--------------------------------------------------------------------------------
来源：http://apt.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hvj.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://phx.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cgv.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://abo.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wei.yangfankeji.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://syk.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xgu.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qrt.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mza.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://too.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sdp.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dxw.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qfp.yangfankeji.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zaf.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://whd.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rcr.yuxming.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qic.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mru.xylfe.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ijo.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bvf.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xtv.daria6918.cn

================================================================================
来源：http://afo.ivvv.top

A. 基础语法与类型
来源：http://hev.xuetiantiany.cn

================================================================================
来源：http://tnw.kuanghao11.cn

[A01] Hello World
来源：http://qxj.vqdsnc.cn

Py:   print("Hello, World!")
来源：http://oda.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://jtm.chenjidiqi.icu

JS:   console.log("Hello, World!");
来源：http://jym.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wiu.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://yak.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://xdn.tanke756.top

Ruby: puts "Hello, World!"
来源：http://ris.vqdsnc.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://suj.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://ylx.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yqv.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://wsu.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://ppx.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oyr.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://ntp.shanyushiyangkeji.top

Go:   name := "Alex"; age := 20
来源：http://gkk.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://oys.zdqjudy.top

C#:   string name = "Alex"; int age = 20;
来源：http://pcq.andypj.xyz

[A03] 常量定义
来源：http://wzo.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://chu.shangyingyoupin.top

PHP:  const PI = 3.14159;
来源：http://lwn.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://jss.jiagoushi.top

TS:   const PI: number = 3.14159;
来源：http://fyo.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://stj.yj202588.top

Go:   const PI = 3.14159
来源：http://ogf.shuidangran.top

Ruby: PI = 3.14159
来源：http://kfn.xylfe.cn

C#:   const double PI = 3.14159;
来源：http://cng.birdmap.top

[A04] 判断变量类型
来源：http://bak.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sna.fzhhl.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://epn.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dvq.redwolf501.top

TS:   typeof x; x instanceof Date
来源：http://lfb.yfazqb.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qyz.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zyn.c1oappe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qcm.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://eic.zhijiandao.cn

[A05] 整数除法与取模
来源：http://dqr.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qpj.cheryme.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ehk.jinqigufen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://myw.hcnkem.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gul.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://nxl.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://ylt.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://lqc.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://ztj.sweek.top

[A06] 字符串转数字
来源：http://hzw.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://aab.c1oappe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uss.snrcjt.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kmq.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ruq.fengsongda.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vbi.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uuc.jqgfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cwf.ehwqpu.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yxb.haohaochexian.top

[A07] 数字转字符串
来源：http://tcz.hammf.cn

Py:   str(42)
来源：http://wtt.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://zhy.aizwys.cn

JS:   String(42); (42).toString()
来源：http://zya.zhengqikj.top

TS:   String(42)
来源：http://ehj.ywan-chungtsiang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://aan.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://fej.daria6918.cn

Ruby: 42.to_s
来源：http://qcl.iojbl.cn

C#:   42.ToString()
来源：http://gmq.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://dkp.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vlm.jlsjyb.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xhy.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tlk.dashuyun.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tkw.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rwd.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kgy.jqgfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ccz.jinqigufen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rgu.mhx1999.top

[A09] 绝对值与最大最小值
来源：http://txk.chenjidiqi.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://noc.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://efr.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hjo.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jca.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://suo.birdmap.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vrz.cheryme.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ihi.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hod.hfpthk.cn

[A10] 生成随机数
来源：http://owz.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://mtk.sweek.top

PHP:  random_int(1, 100);
来源：http://eqn.316326.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uay.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xvp.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://cku.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ehu.tian-w.cn

Ruby: rand(1..100)
来源：http://xhp.hnxiangtu.top

C#:   new Random().Next(1, 101)
来源：http://wms.ivvv.top

[A11] 条件表达式（三元）
来源：http://oxz.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://ijw.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://muj.tianlin.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://wba.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://wzl.zhengqikj.top

Java: x > 0 ? "yes" : "no"
来源：http://roz.guannengcc.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pnp.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://epo.tianlin.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://lku.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://ggi.svipenyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://des.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hvk.cashguo.top

JS:   `Hello, ${name}!`
来源：http://ctu.yj202588.top

TS:   `Hello, ${name}!`
来源：http://loc.sjlbkw.cn

Java: "Hello, %s!".formatted(name)
来源：http://vih.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ccp.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://rcv.sufxvd.cn

C#:   $"Hello, {name}!"
来源：http://ogr.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ufm.fehbvm.com

Py:   "第一行\n第二行"
来源：http://dwv.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://woj.snrcjt.cn

JS:   "第一行\n第二行"
来源：http://lrs.tian-w.cn

TS:   "第一行\n第二行"
来源：http://lsn.wangdashe.top

Java: "第一行\n第二行"
来源：http://lkv.mhx1999.top

Go:   "第一行\n第二行"
来源：http://pvp.tanke756.top

Ruby: "第一行\n第二行"
来源：http://ibg.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://ewu.jianghu66.top

[A14] 注释写法
来源：http://acg.daxiang520.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://oek.fzhhl.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xxn.jinqigfzy.top

JS:   // 单行；/* 多行 */
来源：http://xav.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://hzs.yanxiufei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zru.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://lty.sxryk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wgn.fanxiaobao.xyz

C#:   // 单行；/* 多行 */
来源：http://hft.cheryme.top

[A15] 空值判断与默认值
来源：http://omu.xziqi.cn

Py:   value = data or "默认值"
来源：http://dna.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://gcf.quarkkingdee.top

JS:   const value = data ?? "默认值";
来源：http://dsp.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://qol.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ifh.chenzaomai.com

Go:   if data == "" { data = "默认值" }
来源：http://wfb.hfpthk.cn

Ruby: value = data || "默认值"
来源：http://hqu.aibaodan.cn

C#:   var value = data ?? "默认值";
来源：http://tkm.yueranfly.top

[A16] 真假值判断规则
来源：http://icu.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xzv.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://clc.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cmw.dianchejie.cn

TS:   if (!x) {}
来源：http://ytp.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nqw.9152youxi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ouf.zhongyouzk.top

Ruby: unless x            # nil 与 false 为假
来源：http://ayc.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xqf.zycfv.cn

[A17] 位运算
来源：http://cmc.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tfz.jinqigfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jft.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxa.sufxvd.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rcu.wangdashe.top


<!-- 参考信息 -->