代发 wailian999

[U101] JS：classList 操作
来源：http://shg.ctjpmb.com

el.classList.toggle("active")
来源：http://fmy.sweek.top

[U102] JS：本地存储
来源：http://yuj.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zgt.yonumen.top

[U103] JS：定时器
来源：http://nbc.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wph.ydzc1.top

[U104] JS：防抖
来源：http://bvz.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zug.yueranfly.top

[U105] JS：节流
来源：http://hgc.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xde.sufxvd.cn

[U106] JS：日期格式化
来源：http://mex.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gzg.yanxiufei.cn

[U107] JS：数字千分位
来源：http://rxv.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hwq.shangyingyoupin.top

[U108] JS：随机整数
来源：http://fik.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rwy.epnwcf.com

[U109] JS：数组分组
来源：http://bez.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://tbx.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://juo.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pra.yangfankeji.com

[U111] JS：对象转 Map
来源：http://nbm.hongshengwenyu.top

new Map(Object.entries(obj))
来源：http://axf.hysaishi.cn

[U112] JS：字符串补位
来源：http://oje.bjfxy.top

"7".padStart(3, "0")
来源：http://dxc.uphjek.com

[U113] JS：正则替换全部
来源：http://lys.vehdjk.com

s.replaceAll("a", "b")
来源：http://qdv.ybcxt.top

[U114] JS：JSON 深比较
来源：http://jag.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ywt.tianlin.xyz

[U115] JS：生成 UUID
来源：http://pup.yuxming.cn

crypto.randomUUID()
来源：http://xfs.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://uzs.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://yxq.fehbvm.com

[U117] JS：单元测试
来源：http://pap.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://boa.aizwys.cn

[U118] JS：开发服务器
来源：http://pqf.yuxming.cn

npm i -D vite;  npx vite
来源：http://vhq.fengsongda.top

[U119] JS：生产构建
来源：http://ncd.jiagoushi.top

npx vite build
来源：http://unp.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://nhp.316326.xyz

import.meta.env.VITE_API_URL
来源：http://zjj.shangyingyoupin.top

================================================================================
来源：http://asv.cucudq.cn

统计汇总
来源：http://tbv.zhongyouzk.top

================================================================================
来源：http://opg.tanke756.top

按语言统计（条）：
来源：http://wtg.dianchejie.cn

Python ......... 252
来源：http://pgj.ivvv.top

PHP ............ 252
来源：http://rvg.yangfankeji.com

JavaScript ..... 252
来源：http://lyx.jinqigufen.top

TypeScript ..... 212
来源：http://tyj.kuanghao11.cn

Java ........... 212
来源：http://vpn.xuanzx.com

Go ............. 212
来源：http://hns.yonumen.top

Ruby ........... 212
来源：http://mdl.yonumen.top

C# ............. 212
来源：http://hes.xylfe.cn

C .............. 30
来源：http://njl.svipenyu.cn

C++ ............ 30
来源：http://upw.zhixingplan.top

SQL ............ 90
来源：http://bhy.daxiang520.top

Bash ........... 80
来源：http://aho.sjlbkw.cn

Kotlin ......... 15
来源：http://bta.sjlbkw.cn

Swift .......... 15
来源：http://lcn.ehwqpu.com

Lua ............ 10
来源：http://dgh.cqqwz.cn

Perl ........... 10
来源：http://xyl.cucudq.cn

Scala .......... 10
来源：http://xvz.zdqjudy.top

------------------------------------
来源：http://hdj.tanke756.top

合计 ........... 2106 条
来源：http://kxk.xziqi.cn

按章节统计：
来源：http://msi.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fxm.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aiz.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fki.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oez.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gvp.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tkq.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gph.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dhg.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yiu.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ipa.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fzx.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sfy.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wuf.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cno.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mec.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xvo.0kj1m.cn

Q SQL 专题                              90
来源：http://tsi.yanxiufei.cn

R Bash 专题                             80
来源：http://wfy.vqdsnc.cn

S C / C++ 专题                          60
来源：http://hjn.jyoumei.cn

T 其他语言补充                          60
来源：http://sea.smart0.xyz

U 高频实用片段                         120
来源：http://jmq.cdnleiting.top

------------------------------------
来源：http://bqr.guowangkeji.top

合计                                  2106 条
来源：http://vvu.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://wsj.pycfn.com

使用提醒
来源：http://cgs.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://eld.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dkb.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dog.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ncc.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qpo.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mvg.cheryme.top

—— 文件结束 ——
来源：http://lor.tarul.cn

================================================================================
来源：http://aio.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://fjb.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://mqb.9152youxi.cn

================================================================================
来源：http://buk.jqgufenzy.top

【收录内容】
来源：http://orh.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://urp.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vtq.guowangkeji.top

SQL · Bash · C · C++
来源：http://dhy.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://guu.9152youxi.cn

【使用说明】
来源：http://vpx.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zns.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://osu.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kbq.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iih.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ukn.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://msj.nanxinkj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rce.quarkkingdee.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pkf.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gzm.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hlf.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tyy.aibaodan.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zsx.cucudq.cn

【文件统计】
来源：http://goc.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ksd.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://hho.meibo888.top

目  录
来源：http://vbr.tanke756.top

--------------------------------------------------------------------------------
来源：http://kye.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ypv.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gpk.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qom.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rbx.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cej.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hus.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iui.fanxiaobao.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ran.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gvx.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sad.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qxy.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mpg.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qrc.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rpp.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ckk.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://riy.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://otv.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://etv.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qsy.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cvl.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lfw.c1oappe.top

================================================================================
来源：http://ydz.feifeiyinyue.top

A. 基础语法与类型
来源：http://csj.sxryk.cn

================================================================================
来源：http://mmy.gotoacloud.top

[A01] Hello World
来源：http://uuh.zhoulong.xyz

Py:   print("Hello, World!")
来源：http://cbo.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://pav.c1oappe.top

JS:   console.log("Hello, World!");
来源：http://abs.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cjq.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://dnt.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://fwf.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://oyn.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xda.daxiang520.top

[A02] 变量声明与赋值
来源：http://tew.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xjp.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://eqr.yuanzhike.top

JS:   let name = "Alex"; const age = 20;
来源：http://dam.shanyushiyangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wwk.0kj1m.cn

Java: String name = "Alex"; int age = 20;
来源：http://ase.shuidangran.top

Go:   name := "Alex"; age := 20
来源：http://fyy.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://fee.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://fyv.meibo888.top

[A03] 常量定义
来源：http://dmo.fanxiaobao.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dys.zhixingplan.top

PHP:  const PI = 3.14159;
来源：http://vmg.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://kva.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://rhu.shanyushiyangkeji.top

Java: static final double PI = 3.14159;
来源：http://pei.fehbvm.com

Go:   const PI = 3.14159
来源：http://tjk.tianlin.xyz

Ruby: PI = 3.14159
来源：http://gpc.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://ney.zhoulong.xyz

[A04] 判断变量类型
来源：http://div.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gsv.fanxiaobao.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nsx.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dzu.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://apj.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://doq.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wwq.vqdsnc.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xnx.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://ynf.vqdsnc.cn

[A05] 整数除法与取模
来源：http://wox.bjfxy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zjm.feifeiyinyue.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jgy.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://szk.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uoi.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://heq.sufxvd.cn

Go:   7 / 2; 7 % 2
来源：http://dsl.cashguo.top

Ruby: 7 / 2; 7 % 2
来源：http://owh.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://xtw.quarkkingdee.top

[A06] 字符串转数字
来源：http://ngd.uphjek.com

Py:   int("42"); float("3.14")
来源：http://mme.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://snm.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dqa.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://onz.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rpv.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gdl.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zui.yuxming.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://upx.pengpengdd.cyou

[A07] 数字转字符串
来源：http://bvh.gotoacloud.top

Py:   str(42)
来源：http://ids.chenzaomai.com

PHP:  (string) 42; strval(42)
来源：http://odi.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://lbb.hesvh.cn

TS:   String(42)
来源：http://tln.havefunace.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dsj.tarul.cn

Go:   strconv.Itoa(42)
来源：http://bnu.ehwqpu.com

Ruby: 42.to_s
来源：http://rca.nanxinkj.top

C#:   42.ToString()
来源：http://ual.gaohongyu789.top

[A08] 取整与四舍五入
来源：http://mtv.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yzw.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sim.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gkt.jinqigufen.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xny.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://evb.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fki.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ltj.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pcg.tianlin.xyz

[A09] 绝对值与最大最小值
来源：http://jse.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://arm.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tfs.cqqwz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zyg.nwbrower.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://exj.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://coq.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xko.nanxuanxn.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hvr.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://trl.tian-w.cn

[A10] 生成随机数
来源：http://mkj.daria6918.cn

Py:   import random; random.randint(1, 100)
来源：http://hai.yongpay.top

PHP:  random_int(1, 100);
来源：http://smc.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wkp.xuanzx.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://syl.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://lga.chenlongwang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kas.yongpay.top

Ruby: rand(1..100)
来源：http://lxo.gzhubu.top

C#:   new Random().Next(1, 101)
来源：http://anv.yvedp.cn

[A11] 条件表达式（三元）
来源：http://shz.jlsjyb.cn

Py:   "yes" if x > 0 else "no"
来源：http://oci.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fky.bjfxy.top

JS:   x > 0 ? "yes" : "no"
来源：http://kqk.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fbn.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://ysq.hcnkem.com

Go:   // 无三元运算符，需用 if 语句
来源：http://daz.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://jfg.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://foq.jinqigfzy.top

[A12] 字符串插值 / 格式化
来源：http://wek.vehdjk.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wvy.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zyt.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://fop.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://zqk.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://ttw.haohaochexian.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://plq.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://nhk.nwbrower.top

C#:   $"Hello, {name}!"
来源：http://nja.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lna.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://suk.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://sxs.jinqigfzy.top

JS:   "第一行\n第二行"
来源：http://adm.zdbjq.cn

TS:   "第一行\n第二行"
来源：http://nap.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://stn.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://ahr.fzhhl.top

Ruby: "第一行\n第二行"
来源：http://qbz.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://wnu.sweek.top

[A14] 注释写法
来源：http://ies.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wzo.shanyushiyangtech.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ono.316326.xyz

JS:   // 单行；/* 多行 */
来源：http://dhn.tarul.cn

TS:   // 单行；/* 多行 */
来源：http://gty.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mcm.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://dap.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://iey.nanxuanxn.top

C#:   // 单行；/* 多行 */
来源：http://niv.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://xmo.aizwys.cn

Py:   value = data or "默认值"
来源：http://qwj.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://dwb.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://gqu.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://puu.tian-w.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fhf.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://hfo.52xcode.cn

Ruby: value = data || "默认值"
来源：http://vot.nwbrower.top

C#:   var value = data ?? "默认值";
来源：http://daj.yongpay.top

[A16] 真假值判断规则
来源：http://wdg.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ome.vehdjk.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rht.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dxv.zhijiandao.cn

TS:   if (!x) {}
来源：http://ice.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tbp.yangfankeji.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vih.zhaomingkeji.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://nbw.gotoacloud.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wyy.ivvv.top

[A17] 位运算
来源：http://xin.quarkkingdee.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ihw.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qqq.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zuz.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rib.sysykeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ucc.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jwi.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cjf.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mfo.pycfn.com


<!-- 参考信息 -->