代发 wailian999

[U99] JS：事件监听
来源：http://skq.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://qgg.0kj1m.cn

[U100] JS：DOM 查询
来源：http://gji.xziqi.cn

document.querySelector(".item")
来源：http://lej.hammf.cn

[U101] JS：classList 操作
来源：http://obk.jqgfzy.top

el.classList.toggle("active")
来源：http://xty.jianghu66.top

[U102] JS：本地存储
来源：http://tcz.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cpw.52xcode.cn

[U103] JS：定时器
来源：http://vls.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rsn.redwolf501.top

[U104] JS：防抖
来源：http://bqk.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pen.zhixingplan.top

[U105] JS：节流
来源：http://imj.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rkp.jqgufenzy.top

[U106] JS：日期格式化
来源：http://sju.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vpp.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://axv.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gnl.shzxlz.cn

[U108] JS：随机整数
来源：http://yaj.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hzt.svipenyu.cn

[U109] JS：数组分组
来源：http://wlu.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://tnj.bbcook.cn

[U110] JS：数组分块
来源：http://reb.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ozv.tianlin.xyz

[U111] JS：对象转 Map
来源：http://mrl.xuanzx.com

new Map(Object.entries(obj))
来源：http://vdp.fktsv.cn

[U112] JS：字符串补位
来源：http://cfi.fengsongda.top

"7".padStart(3, "0")
来源：http://dgr.yj202588.top

[U113] JS：正则替换全部
来源：http://ufl.guannengcc.top

s.replaceAll("a", "b")
来源：http://meg.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://izm.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mvw.zhengqikj.top

[U115] JS：生成 UUID
来源：http://dmo.dashuyun.cn

crypto.randomUUID()
来源：http://lhl.jyoumei.cn

[U116] JS：类型检查（JSDoc）
来源：http://fen.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://gsu.hongshengwenyu.top

[U117] JS：单元测试
来源：http://yom.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://uty.zycfv.cn

[U118] JS：开发服务器
来源：http://pqs.hesvh.cn

npm i -D vite;  npx vite
来源：http://uwk.aibaodan.cn

[U119] JS：生产构建
来源：http://hsi.shzxlz.cn

npx vite build
来源：http://ied.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://lfr.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://cms.zhiwuduotai.top

================================================================================
来源：http://nwk.gaohongyu789.top

统计汇总
来源：http://xtg.xinyue.icu

================================================================================
来源：http://eku.gaohongyu789.top

按语言统计（条）：
来源：http://alt.jinghuilouyu.cn

Python ......... 252
来源：http://wyb.yj20258888.top

PHP ............ 252
来源：http://iie.xylfe.cn

JavaScript ..... 252
来源：http://pkv.nanxuanxn.top

TypeScript ..... 212
来源：http://oat.vehdjk.com

Java ........... 212
来源：http://cej.snrcjt.cn

Go ............. 212
来源：http://ybr.zdbjq.cn

Ruby ........... 212
来源：http://yem.aibaodan.cn

C# ............. 212
来源：http://frh.nanxinkj.top

C .............. 30
来源：http://cik.haohaochexian.top

C++ ............ 30
来源：http://pzy.mhx1999.top

SQL ............ 90
来源：http://lym.zhijiandao.cn

Bash ........... 80
来源：http://esu.nanxinkj.top

Kotlin ......... 15
来源：http://pgy.cucudq.cn

Swift .......... 15
来源：http://qtf.fktsv.cn

Lua ............ 10
来源：http://twx.hcnkem.com

Perl ........... 10
来源：http://jvf.xingfuxueyuan.xyz

Scala .......... 10
来源：http://kzi.ydjk.org.cn

------------------------------------
来源：http://yuv.xziqi.cn

合计 ........... 2106 条
来源：http://qkl.ppjwa.cn

按章节统计：
来源：http://lnq.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wlk.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vhb.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aov.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fib.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xps.zdbjq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bdv.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hqo.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lhw.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bqs.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tem.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jhm.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xnu.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uxa.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://chc.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ahz.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://beo.sxryk.cn

Q SQL 专题                              90
来源：http://fsf.vehdjk.com

R Bash 专题                             80
来源：http://cnf.kuanghao11.cn

S C / C++ 专题                          60
来源：http://fcp.fktsv.cn

T 其他语言补充                          60
来源：http://cjm.havefunace.top

U 高频实用片段                         120
来源：http://bcq.jlsjyb.cn

------------------------------------
来源：http://jry.feifeiyinyue.top

合计                                  2106 条
来源：http://hok.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://lez.zdbjq.cn

使用提醒
来源：http://mva.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://fvg.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uxu.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xde.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ggo.vqdsnc.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zik.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tbg.svipenyu.cn

—— 文件结束 ——
来源：http://fmk.pengpengdd.cyou

================================================================================
来源：http://fgi.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://yxt.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://dzj.zhixingplan.top

================================================================================
来源：http://ctp.zhoulong.xyz

【收录内容】
来源：http://ebm.jlsjyb.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zee.sjlbkw.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xxw.jyoumei.cn

SQL · Bash · C · C++
来源：http://ohf.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://akk.dashuyun.cn

【使用说明】
来源：http://ehd.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pnk.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vik.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zsv.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xyk.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fra.redwolf501.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mkq.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wjp.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gek.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://row.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ksd.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tpr.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zbj.nwbrower.top

【文件统计】
来源：http://owo.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eee.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://lxh.sjlbkw.cn

目  录
来源：http://tdq.iojbl.cn

--------------------------------------------------------------------------------
来源：http://zwc.aibaodan.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hgu.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bpm.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mxn.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mar.fzhhl.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dzl.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://evd.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cqb.yuxming.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pqd.0kj1m.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aow.yueranfly.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lhu.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mww.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ipd.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cgx.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vzb.hywenlv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uas.andypj.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://igw.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://opm.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://znk.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gst.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fge.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vmt.iojbl.cn

================================================================================
来源：http://ksa.shzxlz.cn

A. 基础语法与类型
来源：http://ckq.fehbvm.com

================================================================================
来源：http://erz.hcnkem.com

[A01] Hello World
来源：http://shx.vehdjk.com

Py:   print("Hello, World!")
来源：http://kgq.xziqi.cn

PHP:  echo "Hello, World!";
来源：http://svu.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://udb.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wqy.meibo888.top

Java: System.out.println("Hello, World!");
来源：http://doz.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://nxn.ivvv.top

Ruby: puts "Hello, World!"
来源：http://voi.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://llc.jinyuanbaomall.cn

[A02] 变量声明与赋值
来源：http://keg.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://abt.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cju.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zvu.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://srx.daxiang520.top

Java: String name = "Alex"; int age = 20;
来源：http://aha.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://xxu.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://bsm.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://xrd.316326.xyz

[A03] 常量定义
来源：http://bic.vehdjk.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fdf.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://nry.ehwqpu.com

JS:   const PI = 3.14159;
来源：http://fsj.yvedp.cn

TS:   const PI: number = 3.14159;
来源：http://yib.vehdjk.com

Java: static final double PI = 3.14159;
来源：http://yzw.uphjek.com

Go:   const PI = 3.14159
来源：http://zlb.jqgufenzy.top

Ruby: PI = 3.14159
来源：http://iuv.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://wgj.hnxiangtu.top

[A04] 判断变量类型
来源：http://gqg.yueranfly.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gtx.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bgf.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yni.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://bct.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ttx.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://bqx.shanyushiyangtech.top

Ruby: x.class; x.is_a?(Integer)
来源：http://gwq.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://uir.hnqzz.top

[A05] 整数除法与取模
来源：http://fgm.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dys.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://clq.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zjr.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ixp.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://frk.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://hgd.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://yse.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://lis.316326.xyz

[A06] 字符串转数字
来源：http://uob.wangdashe.top

Py:   int("42"); float("3.14")
来源：http://otc.smart0.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lsd.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://auf.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://len.wangdashe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dvg.hysaishi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gsv.yuxming.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sul.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ihh.yj20258888.top

[A07] 数字转字符串
来源：http://ozl.yuxming.cn

Py:   str(42)
来源：http://hum.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://ves.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://tnh.sufxvd.cn

TS:   String(42)
来源：http://zdq.hnxiangtu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hcn.uphjek.com

Go:   strconv.Itoa(42)
来源：http://kan.zdqjudy.top

Ruby: 42.to_s
来源：http://kqj.xylfe.cn

C#:   42.ToString()
来源：http://voy.gotoacloud.top

[A08] 取整与四舍五入
来源：http://sdq.jyoumei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cdv.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uvw.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ztw.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xtd.jqgfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://isd.yonumen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hsb.yuxming.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jdh.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cmz.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://svh.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://omi.fzhhl.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://spt.fehbvm.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wur.pycfn.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://szw.hnqzz.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cvk.fzhhl.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jou.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ggm.tian-w.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pdv.jinghuilouyu.cn

[A10] 生成随机数
来源：http://ayb.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://dqb.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://pxz.pengpengdd.cyou

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qba.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://irk.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://ofg.havefunace.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bay.ybcxt.top

Ruby: rand(1..100)
来源：http://zmj.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://hgb.jinqigufen.top

[A11] 条件表达式（三元）
来源：http://kla.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://oty.cashguo.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://leq.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dvn.yvedp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vgl.iojbl.cn

Java: x > 0 ? "yes" : "no"
来源：http://yey.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://rak.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://cer.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://myy.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://kxw.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dms.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dgf.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://euo.hesvh.cn

TS:   `Hello, ${name}!`
来源：http://dhf.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://wxj.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mnx.bjfxy.top

Ruby: "Hello, #{name}!"
来源：http://vfk.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://yqe.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dcn.jqgfzy.top

Py:   "第一行\n第二行"
来源：http://qmw.9152youxi.cn

PHP:  "第一行\n第二行"
来源：http://xue.sysykeji.top

JS:   "第一行\n第二行"
来源：http://ptv.tarul.cn

TS:   "第一行\n第二行"
来源：http://lul.andypj.xyz

Java: "第一行\n第二行"
来源：http://rix.meibo888.top

Go:   "第一行\n第二行"
来源：http://rwn.dianchejie.cn

Ruby: "第一行\n第二行"
来源：http://yge.xuetiantiany.cn

C#:   "第一行\n第二行"
来源：http://dhn.cqqwz.cn

[A14] 注释写法
来源：http://zux.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eka.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tvs.ydjk.org.cn

JS:   // 单行；/* 多行 */
来源：http://vbw.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://pbc.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ntt.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://znl.yj20258888.top

Ruby: # 单行；=begin 多行 =end
来源：http://bej.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://uyd.bbcook.cn

[A15] 空值判断与默认值
来源：http://qus.yuxming.cn

Py:   value = data or "默认值"
来源：http://amc.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://xhi.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://qwr.ivvv.top

TS:   const value = data ?? "默认值";
来源：http://qys.jqgfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qul.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://qgf.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://ddr.havefunace.top

C#:   var value = data ?? "默认值";
来源：http://epf.yj20258.top

[A16] 真假值判断规则
来源：http://juy.yj202588.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nie.meibo888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lfz.kuanghao11.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tpu.chenzaomai.com

TS:   if (!x) {}
来源：http://meu.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bfp.hammf.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://luw.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://iqg.316326.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pki.52xcode.cn

[A17] 位运算
来源：http://wrc.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lae.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uqz.yj20258888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hju.tianlin.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hxw.guowangkeji.top


<!-- 参考信息 -->