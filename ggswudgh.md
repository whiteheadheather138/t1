代发 wailian999

[U101] JS：classList 操作
来源：http://ura.jiagoushi.top

el.classList.toggle("active")
来源：http://xgp.xinyue.icu

[U102] JS：本地存储
来源：http://voe.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wym.zhixingplan.top

[U103] JS：定时器
来源：http://afz.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://twe.redwolf501.top

[U104] JS：防抖
来源：http://ylr.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfs.zdbjq.cn

[U105] JS：节流
来源：http://rst.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kis.316326.xyz

[U106] JS：日期格式化
来源：http://zlp.cheryme.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sxc.zhongyouzk.top

[U107] JS：数字千分位
来源：http://fpi.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fbd.quarkkingdee.top

[U108] JS：随机整数
来源：http://obi.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pkw.vqdsnc.cn

[U109] JS：数组分组
来源：http://oed.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://mld.zhixingplan.top

[U110] JS：数组分块
来源：http://aoq.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zqg.shuidangran.top

[U111] JS：对象转 Map
来源：http://rkz.jinqigufen.top

new Map(Object.entries(obj))
来源：http://bde.uphjek.com

[U112] JS：字符串补位
来源：http://fcx.guowangkeji.top

"7".padStart(3, "0")
来源：http://dpn.daria6918.cn

[U113] JS：正则替换全部
来源：http://ozm.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://iqn.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://sbr.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zsn.dianchejie.cn

[U115] JS：生成 UUID
来源：http://etl.zdqjudy.top

crypto.randomUUID()
来源：http://kmg.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://tbr.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://ovm.c1oappe.top

[U117] JS：单元测试
来源：http://fiq.pycfn.com

npm i -D vitest;  npx vitest
来源：http://wig.fehbvm.com

[U118] JS：开发服务器
来源：http://rqu.tianlin.xyz

npm i -D vite;  npx vite
来源：http://iyz.yvedp.cn

[U119] JS：生产构建
来源：http://rej.pycfn.com

npx vite build
来源：http://uhu.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://lin.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://xsr.c1oappe.top

================================================================================
来源：http://wkf.yj20258.top

统计汇总
来源：http://acl.hcnkem.com

================================================================================
来源：http://mwj.wangshuangyany.cn

按语言统计（条）：
来源：http://ikt.ywan-chungtsiang.top

Python ......... 252
来源：http://bqq.yuanzhike.top

PHP ............ 252
来源：http://urn.0kj1m.cn

JavaScript ..... 252
来源：http://pis.9152youxi.cn

TypeScript ..... 212
来源：http://dxo.xinyue.icu

Java ........... 212
来源：http://zal.wangshuangyany.cn

Go ............. 212
来源：http://mwv.gogol.net.cn

Ruby ........... 212
来源：http://ukf.jyoumei.cn

C# ............. 212
来源：http://uqn.jiagoushi.top

C .............. 30
来源：http://tof.uphjek.com

C++ ............ 30
来源：http://akd.xziqi.cn

SQL ............ 90
来源：http://lld.pengpengdd.cyou

Bash ........... 80
来源：http://ozk.yj20258888.top

Kotlin ......... 15
来源：http://ylh.ybcxt.top

Swift .......... 15
来源：http://qeq.c1oappe.top

Lua ............ 10
来源：http://wac.316326.xyz

Perl ........... 10
来源：http://iko.ybcxt.top

Scala .......... 10
来源：http://ain.xinyue.icu

------------------------------------
来源：http://kxt.chenzaomai.com

合计 ........... 2106 条
来源：http://mcq.dianchejie.cn

按章节统计：
来源：http://npj.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qos.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jjg.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://omb.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rmo.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iua.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qyd.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qbs.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ssa.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ggs.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://geq.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gel.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lmx.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cxw.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wlc.yangfankeji.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jnf.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xey.zhijiandao.cn

Q SQL 专题                              90
来源：http://qxq.xuanzx.com

R Bash 专题                             80
来源：http://qzr.fktsv.cn

S C / C++ 专题                          60
来源：http://pvl.sufxvd.cn

T 其他语言补充                          60
来源：http://qol.c1oappe.top

U 高频实用片段                         120
来源：http://fkb.chenjidiqi.icu

------------------------------------
来源：http://uil.yueranfly.top

合计                                  2106 条
来源：http://yix.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://nnh.snrcjt.cn

使用提醒
来源：http://erd.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://ixz.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gjf.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qee.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rfh.ywan-chungtsiang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gtu.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eur.sweek.top

—— 文件结束 ——
来源：http://miy.gotoacloud.top

================================================================================
来源：http://sis.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://ewy.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://gbl.tian-w.cn

================================================================================
来源：http://zkm.hongshengwenyu.top

【收录内容】
来源：http://hyt.xinyue.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://sjt.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wxl.yvedp.cn

SQL · Bash · C · C++
来源：http://sfk.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://npl.dianchejie.cn

【使用说明】
来源：http://dxj.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mlu.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tib.aibaodan.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yfk.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bhi.jinghuilouyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cdd.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hen.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wwe.yueranfly.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hol.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://okp.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://llf.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tbz.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yoa.pycfn.com

【文件统计】
来源：http://wkq.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kbh.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://fts.vqdsnc.cn

目  录
来源：http://rry.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://pgt.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xln.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lno.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://prh.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yfy.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jzq.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nwx.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hse.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://prr.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qpl.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rcn.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yyu.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hfl.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ict.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bmh.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://znv.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wiw.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hfm.fanxiaobao.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://tti.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qzr.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ptt.tianlin.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vme.sweek.top

================================================================================
来源：http://mjk.cucudq.cn

A. 基础语法与类型
来源：http://sqr.wangshuangyany.cn

================================================================================
来源：http://pyo.cdnleiting.top

[A01] Hello World
来源：http://vyk.shuidangran.top

Py:   print("Hello, World!")
来源：http://oyv.yonumen.top

PHP:  echo "Hello, World!";
来源：http://xug.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://eio.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ipf.yuanzhike.top

Java: System.out.println("Hello, World!");
来源：http://ovf.daxiang520.top

Go:   fmt.Println("Hello, World!")
来源：http://gzq.havefunace.top

Ruby: puts "Hello, World!"
来源：http://bpk.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jad.gzhubu.top

[A02] 变量声明与赋值
来源：http://rzf.jinqigfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xgs.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uhz.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://yra.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://non.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://xgc.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://haw.wangshuangyany.cn

Ruby: name = "Alex"; age = 20
来源：http://tgt.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://byt.tanke756.top

[A03] 常量定义
来源：http://ewg.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wrp.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://xjy.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://wpo.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://vvi.kuanghao11.cn

Java: static final double PI = 3.14159;
来源：http://cwq.wangdashe.top

Go:   const PI = 3.14159
来源：http://qqg.vehdjk.com

Ruby: PI = 3.14159
来源：http://xkh.xuetiantiany.cn

C#:   const double PI = 3.14159;
来源：http://tae.ctjpmb.com

[A04] 判断变量类型
来源：http://rtj.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yxk.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pgr.hcnkem.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aiy.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://xve.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://msg.daria6918.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fhj.52xcode.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kqu.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://idr.yueranfly.top

[A05] 整数除法与取模
来源：http://gxb.zhengqikj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lbj.yuxming.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lva.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xgq.wangshuangyany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ymx.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://gws.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://skh.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://bmx.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://zbq.xingfuxueyuan.xyz

[A06] 字符串转数字
来源：http://xii.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://mte.tanke756.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ary.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hyp.xuetiantiany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xse.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xrw.zhijiandao.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hsh.hysaishi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rbj.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://onh.zhijiandao.cn

[A07] 数字转字符串
来源：http://yib.dashuyun.cn

Py:   str(42)
来源：http://rfs.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://wiu.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://pln.fzhhl.top

TS:   String(42)
来源：http://nta.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cyo.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://xio.sxryk.cn

Ruby: 42.to_s
来源：http://prc.sysykeji.top

C#:   42.ToString()
来源：http://bwh.gzhubu.top

[A08] 取整与四舍五入
来源：http://xge.hammf.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zne.svipenyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://czt.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qgk.guowangkeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sgs.ydzc1.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pgs.feifeiyinyue.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rob.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rdr.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lze.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://wce.zdbjq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jbo.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wzv.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fzs.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wgv.kuanghao11.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bpc.gzhubu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zlg.ywan-chungtsiang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sci.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zom.ydzc1.top

[A10] 生成随机数
来源：http://uac.zhoulong.xyz

Py:   import random; random.randint(1, 100)
来源：http://xxo.yuxming.cn

PHP:  random_int(1, 100);
来源：http://bbc.xingfuxueyuan.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ipi.xingfuxueyuan.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://suv.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://ixh.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mhq.shuidangran.top

Ruby: rand(1..100)
来源：http://rdy.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://jzs.jinghuilouyu.cn

[A11] 条件表达式（三元）
来源：http://xqh.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://qku.tianlin.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://nzo.zhengqikj.top

JS:   x > 0 ? "yes" : "no"
来源：http://rfd.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://wpg.hnxiangtu.top

Java: x > 0 ? "yes" : "no"
来源：http://epb.hnqzz.top

Go:   // 无三元运算符，需用 if 语句
来源：http://atd.yuanzhike.top

Ruby: x > 0 ? "yes" : "no"
来源：http://abk.hesvh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rgx.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://shi.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mso.nwbrower.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lnt.epnwcf.com

JS:   `Hello, ${name}!`
来源：http://ydq.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://lsk.yueranfly.top

Java: "Hello, %s!".formatted(name)
来源：http://glr.nanxinkj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hjm.daria6918.cn

Ruby: "Hello, #{name}!"
来源：http://epi.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://jro.zhixingplan.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uwk.aizwys.cn

Py:   "第一行\n第二行"
来源：http://cgn.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://jti.aizwys.cn

JS:   "第一行\n第二行"
来源：http://ddr.cheryme.top

TS:   "第一行\n第二行"
来源：http://hbt.andypj.xyz

Java: "第一行\n第二行"
来源：http://ixw.meibo888.top

Go:   "第一行\n第二行"
来源：http://uic.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://ctw.sweek.top

C#:   "第一行\n第二行"
来源：http://zme.hnxiangtu.top

[A14] 注释写法
来源：http://euj.yuanzhike.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fwc.tian-w.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://axk.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://ogs.ehwqpu.com

TS:   // 单行；/* 多行 */
来源：http://nqx.jinghuilouyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bst.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://cgm.hnxiangtu.top

Ruby: # 单行；=begin 多行 =end
来源：http://pqx.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://ege.cdnleiting.top

[A15] 空值判断与默认值
来源：http://kke.jlsjyb.cn

Py:   value = data or "默认值"
来源：http://fyn.guannengcc.top

PHP:  $value = $data ?? "默认值";
来源：http://xxt.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://irk.xziqi.cn

TS:   const value = data ?? "默认值";
来源：http://oyl.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kjs.sysykeji.top

Go:   if data == "" { data = "默认值" }
来源：http://gjc.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://xuy.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://kjo.yonumen.top

[A16] 真假值判断规则
来源：http://ocd.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qbo.andypj.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ptw.birdmap.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ztx.jinqigufen.top

TS:   if (!x) {}
来源：http://vrh.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cao.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kdx.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oii.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://shm.haohaochexian.top

[A17] 位运算
来源：http://wgc.jinghuilouyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://syd.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://spz.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nyu.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fwi.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cek.ydjk.org.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uor.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vod.ppjwa.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hbs.shuidangran.top


<!-- 参考信息 -->