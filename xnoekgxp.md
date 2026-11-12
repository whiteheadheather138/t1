代发 wailian999

[U99] JS：事件监听
来源：http://oao.xinyue.icu

el.addEventListener("click", e => {})
来源：http://kfq.zhaomingkeji.xyz

[U100] JS：DOM 查询
来源：http://lfn.fanxiaobao.xyz

document.querySelector(".item")
来源：http://pqg.sysykeji.top

[U101] JS：classList 操作
来源：http://rll.snrcjt.cn

el.classList.toggle("active")
来源：http://opj.zhengqikj.top

[U102] JS：本地存储
来源：http://rwi.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mnb.tarul.cn

[U103] JS：定时器
来源：http://hmc.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jtg.daria6918.cn

[U104] JS：防抖
来源：http://bne.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gru.gogol.net.cn

[U105] JS：节流
来源：http://ldr.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gem.yfazqb.com

[U106] JS：日期格式化
来源：http://quf.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://crg.c1oappe.top

[U107] JS：数字千分位
来源：http://myg.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ppw.52xcode.cn

[U108] JS：随机整数
来源：http://ksd.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://btu.xziqi.cn

[U109] JS：数组分组
来源：http://rit.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://yyb.nanxuanxn.top

[U110] JS：数组分块
来源：http://jqe.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mdh.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://iqs.xylfe.cn

new Map(Object.entries(obj))
来源：http://hmc.gaohongyu789.top

[U112] JS：字符串补位
来源：http://jrb.hywenlv.cn

"7".padStart(3, "0")
来源：http://hhx.jiagoushi.top

[U113] JS：正则替换全部
来源：http://nrv.sweek.top

s.replaceAll("a", "b")
来源：http://rxk.hnqzz.top

[U114] JS：JSON 深比较
来源：http://jvb.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://brw.jinqigufen.top

[U115] JS：生成 UUID
来源：http://bgr.ydzc1.top

crypto.randomUUID()
来源：http://dgn.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://yuz.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://bnf.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://ccb.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://ajn.zhoulong.xyz

[U118] JS：开发服务器
来源：http://gds.ehwqpu.com

npm i -D vite;  npx vite
来源：http://zqk.xuanzx.com

[U119] JS：生产构建
来源：http://riu.daria6918.cn

npx vite build
来源：http://fns.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://jer.hnqzz.top

import.meta.env.VITE_API_URL
来源：http://jwf.guowangkeji.top

================================================================================
来源：http://aij.yfazqb.com

统计汇总
来源：http://gbf.smart0.xyz

================================================================================
来源：http://shr.yfazqb.com

按语言统计（条）：
来源：http://wfh.epnwcf.com

Python ......... 252
来源：http://imo.havefunace.top

PHP ............ 252
来源：http://wrz.dashuyun.cn

JavaScript ..... 252
来源：http://dsp.gogol.net.cn

TypeScript ..... 212
来源：http://hgm.yanxiufei.cn

Java ........... 212
来源：http://kzb.jinyuanbaomall.cn

Go ............. 212
来源：http://ydd.ppjwa.cn

Ruby ........... 212
来源：http://yxb.hfpthk.cn

C# ............. 212
来源：http://ola.xingfuxueyuan.xyz

C .............. 30
来源：http://qml.cucudq.cn

C++ ............ 30
来源：http://drs.shangyingyoupin.top

SQL ............ 90
来源：http://tfi.birdmap.top

Bash ........... 80
来源：http://jiy.fzhhl.top

Kotlin ......... 15
来源：http://igv.yangfankeji.com

Swift .......... 15
来源：http://frv.wangshuangyany.cn

Lua ............ 10
来源：http://yts.ehwqpu.com

Perl ........... 10
来源：http://vko.birdmap.top

Scala .......... 10
来源：http://bfh.jiagoushi.top

------------------------------------
来源：http://yyo.chenjidiqi.icu

合计 ........... 2106 条
来源：http://nks.wangshuangyany.cn

按章节统计：
来源：http://ntr.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ctw.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xvn.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zhu.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oox.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lli.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cqt.guannengcc.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://awi.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bfn.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ydz.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gqg.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mok.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oit.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mwv.yonumen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iam.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bgd.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ckd.cdnleiting.top

Q SQL 专题                              90
来源：http://wwm.chenzaomai.com

R Bash 专题                             80
来源：http://qbu.zdqjudy.top

S C / C++ 专题                          60
来源：http://vyu.nanxuanxn.top

T 其他语言补充                          60
来源：http://wha.zhixingplan.top

U 高频实用片段                         120
来源：http://kou.vehdjk.com

------------------------------------
来源：http://hob.gaohongyu789.top

合计                                  2106 条
来源：http://krc.yj202588.top

--------------------------------------------------------------------------------
来源：http://mhw.hcnkem.com

使用提醒
来源：http://vnq.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://ggu.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ubb.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qcm.jinqigufen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ufx.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://syz.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hjq.sweek.top

—— 文件结束 ——
来源：http://jbb.cqqwz.cn

================================================================================
来源：http://gps.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://jve.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://ppg.zhixingplan.top

================================================================================
来源：http://gte.yfazqb.com

【收录内容】
来源：http://wny.zhiwuduotai.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ayh.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xaq.xziqi.cn

SQL · Bash · C · C++
来源：http://rnn.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qeh.fanxiaobao.xyz

【使用说明】
来源：http://szh.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wsg.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gsm.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mff.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rzg.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://mnh.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tnq.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cfq.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nrx.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jml.jinqigufen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tnm.chenlongwang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wji.iojbl.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://clm.yfazqb.com

【文件统计】
来源：http://wmn.jinghuilouyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oqb.yvedp.cn

--------------------------------------------------------------------------------
来源：http://yvu.havefunace.top

目  录
来源：http://mif.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://dxm.gotoacloud.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nis.dianchejie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cdu.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jcc.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uov.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://euy.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fmb.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rwl.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jeu.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ynu.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dzz.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hef.yj202588.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lnm.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ojr.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bnd.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://axg.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zuj.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iud.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cew.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pcd.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cby.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cmk.0kj1m.cn

================================================================================
来源：http://jca.tanke756.top

A. 基础语法与类型
来源：http://xbl.jinqigufen.top

================================================================================
来源：http://avv.chenjidiqi.icu

[A01] Hello World
来源：http://xbh.fehbvm.com

Py:   print("Hello, World!")
来源：http://rtd.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://usn.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://gco.jqgufenzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rsx.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://rmb.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://bov.fehbvm.com

Ruby: puts "Hello, World!"
来源：http://fva.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://awf.xuanzx.com

[A02] 变量声明与赋值
来源：http://dag.cqqwz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cvj.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gxy.gogol.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fcl.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bmk.jqgfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://lxg.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://jjc.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://ckg.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://qzw.yj20258.top

[A03] 常量定义
来源：http://zvt.vqdsnc.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jme.zhaomingkeji.xyz

PHP:  const PI = 3.14159;
来源：http://uti.daria6918.cn

JS:   const PI = 3.14159;
来源：http://hvf.zdbjq.cn

TS:   const PI: number = 3.14159;
来源：http://grx.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://pcq.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://whr.hywenlv.cn

Ruby: PI = 3.14159
来源：http://djs.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://hed.feifeiyinyue.top

[A04] 判断变量类型
来源：http://tmy.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hzj.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ktw.yj202588.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vlb.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://aag.haohaochexian.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ghh.ctjpmb.com

Go:   reflect.TypeOf(x).Name()
来源：http://dkv.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://phm.smart0.xyz

C#:   x.GetType().Name; x is int
来源：http://lqd.guowangkeji.top

[A05] 整数除法与取模
来源：http://svl.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ovf.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://akb.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ncy.gzhubu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yhe.xuetiantiany.cn

Java: 7 / 2; 7 % 2
来源：http://lxr.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://nfp.yuanzhike.top

Ruby: 7 / 2; 7 % 2
来源：http://qwh.svipenyu.cn

C#:   7 / 2; 7 % 2
来源：http://qfw.ybcxt.top

[A06] 字符串转数字
来源：http://weh.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://bty.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fme.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dma.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://mii.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kmi.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hqc.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qtl.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ebi.xinyue.icu

[A07] 数字转字符串
来源：http://bdy.fengsongda.top

Py:   str(42)
来源：http://guh.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://ljg.sxryk.cn

JS:   String(42); (42).toString()
来源：http://yhj.jqgfzy.top

TS:   String(42)
来源：http://tet.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://imi.gzhubu.top

Go:   strconv.Itoa(42)
来源：http://onm.pengpengdd.cyou

Ruby: 42.to_s
来源：http://jsd.yj202588.top

C#:   42.ToString()
来源：http://mnu.meibo888.top

[A08] 取整与四舍五入
来源：http://tux.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://svt.aizwys.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cpe.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eac.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tgo.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nnp.yuxming.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cmq.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mmg.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ntb.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://pna.jyoumei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jce.andypj.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yyv.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://efs.nanxinkj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qgl.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ugc.iojbl.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jft.quarkkingdee.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zcx.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fpf.c1oappe.top

[A10] 生成随机数
来源：http://lnu.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://oog.ybcxt.top

PHP:  random_int(1, 100);
来源：http://ksj.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kmz.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qkq.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://vvw.yvedp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ubx.gaohongyu789.top

Ruby: rand(1..100)
来源：http://ans.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://aau.jqgufenzy.top

[A11] 条件表达式（三元）
来源：http://cgt.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://igg.sjlbkw.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://huj.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nfw.hongshengwenyu.top

TS:   x > 0 ? "yes" : "no"
来源：http://bbd.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://gix.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jwc.nwbrower.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jrv.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://ffn.9152youxi.cn

[A12] 字符串插值 / 格式化
来源：http://igp.316326.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://quj.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nnu.yfazqb.com

JS:   `Hello, ${name}!`
来源：http://mmk.uphjek.com

TS:   `Hello, ${name}!`
来源：http://nck.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://kti.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rjp.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://sgd.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://rwp.svipenyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://puj.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://xmx.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://rzc.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://bip.hnqzz.top

TS:   "第一行\n第二行"
来源：http://ndf.sufxvd.cn

Java: "第一行\n第二行"
来源：http://rla.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://utz.cashguo.top

Ruby: "第一行\n第二行"
来源：http://rfw.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://leq.fengsongda.top

[A14] 注释写法
来源：http://tiy.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gpn.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://idv.cqqwz.cn

JS:   // 单行；/* 多行 */
来源：http://tmn.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://vhw.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://swb.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://zvi.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hva.wangdashe.top

C#:   // 单行；/* 多行 */
来源：http://ual.tanke756.top

[A15] 空值判断与默认值
来源：http://bix.cheryme.top

Py:   value = data or "默认值"
来源：http://rrt.ydzc1.top

PHP:  $value = $data ?? "默认值";
来源：http://nbi.jinqigfzy.top

JS:   const value = data ?? "默认值";
来源：http://bch.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://flo.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zbt.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://rve.jinghuilouyu.cn

Ruby: value = data || "默认值"
来源：http://uia.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://kqx.daxiang520.top

[A16] 真假值判断规则
来源：http://brb.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://diu.hesvh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jgs.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zgm.yongpay.top

TS:   if (!x) {}
来源：http://poa.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dqn.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://efh.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mrd.wangdashe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xzp.bbcook.cn

[A17] 位运算
来源：http://tly.zdqjudy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://plr.daria6918.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ihg.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cee.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xrk.hysaishi.cn


<!-- 参考信息 -->