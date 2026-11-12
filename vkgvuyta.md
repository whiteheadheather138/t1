代发 wailian999

[U101] JS：classList 操作
来源：http://tdp.jiagoushi.top

el.classList.toggle("active")
来源：http://kts.xylfe.cn

[U102] JS：本地存储
来源：http://twf.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://nrl.shangyingyoupin.top

[U103] JS：定时器
来源：http://xyd.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ibf.xinyue.icu

[U104] JS：防抖
来源：http://smj.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://csr.wangshuangyany.cn

[U105] JS：节流
来源：http://bcp.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ogq.yuanzhike.top

[U106] JS：日期格式化
来源：http://mpb.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xrz.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://qxy.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nnr.zhijiandao.cn

[U108] JS：随机整数
来源：http://uwm.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ubo.yanxiufei.cn

[U109] JS：数组分组
来源：http://yet.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://nuo.jlsjyb.cn

[U110] JS：数组分块
来源：http://bsg.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://byd.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://ouv.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://zex.sweek.top

[U112] JS：字符串补位
来源：http://cyl.haohaochexian.top

"7".padStart(3, "0")
来源：http://uuo.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://isk.xylfe.cn

s.replaceAll("a", "b")
来源：http://lsk.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://ppo.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://axc.yj20258.top

[U115] JS：生成 UUID
来源：http://uun.snrcjt.cn

crypto.randomUUID()
来源：http://xjw.jyoumei.cn

[U116] JS：类型检查（JSDoc）
来源：http://erw.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://ajy.nwbrower.top

[U117] JS：单元测试
来源：http://mgx.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://gxy.iojbl.cn

[U118] JS：开发服务器
来源：http://wsi.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://tfz.jqgufenzy.top

[U119] JS：生产构建
来源：http://jpk.ctjpmb.com

npx vite build
来源：http://pvg.nanxinkj.top

[U120] JS：读取环境变量（Vite）
来源：http://cjm.havefunace.top

import.meta.env.VITE_API_URL
来源：http://vxc.ydjk.org.cn

================================================================================
来源：http://stt.gzhubu.top

统计汇总
来源：http://vja.zdqjudy.top

================================================================================
来源：http://aiv.svipenyu.cn

按语言统计（条）：
来源：http://vbg.hcnkem.com

Python ......... 252
来源：http://oro.52xcode.cn

PHP ............ 252
来源：http://uxn.redwolf501.top

JavaScript ..... 252
来源：http://jhh.shanyushiyangtech.top

TypeScript ..... 212
来源：http://jox.jqgfzy.top

Java ........... 212
来源：http://ewj.xingfuxueyuan.xyz

Go ............. 212
来源：http://vyk.hnxiangtu.top

Ruby ........... 212
来源：http://ffy.jlsjyb.cn

C# ............. 212
来源：http://nbl.316326.xyz

C .............. 30
来源：http://axx.ehwqpu.com

C++ ............ 30
来源：http://ckf.sufxvd.cn

SQL ............ 90
来源：http://smt.guannengcc.top

Bash ........... 80
来源：http://xur.chenlongwang.top

Kotlin ......... 15
来源：http://joc.epnwcf.com

Swift .......... 15
来源：http://aia.fzhhl.top

Lua ............ 10
来源：http://lfd.pengpengdd.cyou

Perl ........... 10
来源：http://vmy.dianchejie.cn

Scala .......... 10
来源：http://zqv.yonumen.top

------------------------------------
来源：http://qvo.cqqwz.cn

合计 ........... 2106 条
来源：http://fto.xinyue.icu

按章节统计：
来源：http://yfc.xziqi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aqi.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kaq.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aia.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dno.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ide.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://chs.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mul.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dvf.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fgv.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jak.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xtt.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uhj.jqgfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yup.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uza.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hie.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vgn.fktsv.cn

Q SQL 专题                              90
来源：http://dat.hnxiangtu.top

R Bash 专题                             80
来源：http://uco.hesvh.cn

S C / C++ 专题                          60
来源：http://ldv.xylfe.cn

T 其他语言补充                          60
来源：http://hbp.yj20258888.top

U 高频实用片段                         120
来源：http://myh.shangyingyoupin.top

------------------------------------
来源：http://oyn.vqdsnc.cn

合计                                  2106 条
来源：http://rvy.hesvh.cn

--------------------------------------------------------------------------------
来源：http://snl.bbcook.cn

使用提醒
来源：http://ami.zycfv.cn

--------------------------------------------------------------------------------
来源：http://skj.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://scb.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wgw.xylfe.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vtc.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://doj.xuanzx.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gdu.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://wiq.hnxiangtu.top

================================================================================
来源：http://ibp.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://obb.andypj.xyz

Common Programming Examples Cheat Book
来源：http://ypi.yj20258.top

================================================================================
来源：http://uea.mhx1999.top

【收录内容】
来源：http://qgz.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://grs.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://abk.fengsongda.top

SQL · Bash · C · C++
来源：http://csi.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dmh.yj20258888.top

【使用说明】
来源：http://ied.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://suj.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zpe.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jau.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jcs.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wgp.fanxiaobao.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ciw.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lot.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://srz.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tid.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gmb.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wtr.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://set.vehdjk.com

【文件统计】
来源：http://faq.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qak.gzhubu.top

--------------------------------------------------------------------------------
来源：http://gxb.epnwcf.com

目  录
来源：http://hrs.ivvv.top

--------------------------------------------------------------------------------
来源：http://nhc.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rvv.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cst.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ciy.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jtw.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ptr.pycfn.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wjw.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nvf.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://slg.zhixingplan.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lkb.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gqx.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ysj.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://asp.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mej.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ibx.fktsv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://loj.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xgq.snrcjt.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dhi.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rra.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gnv.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://grm.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://som.sjlbkw.cn

================================================================================
来源：http://xnn.hywenlv.cn

A. 基础语法与类型
来源：http://izu.yangfankeji.com

================================================================================
来源：http://neh.pycfn.com

[A01] Hello World
来源：http://zeb.jqgfzy.top

Py:   print("Hello, World!")
来源：http://ddg.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://paj.chenzaomai.com

JS:   console.log("Hello, World!");
来源：http://mgy.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jwr.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://wjy.pycfn.com

Go:   fmt.Println("Hello, World!")
来源：http://bnp.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://bvx.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rjz.316326.xyz

[A02] 变量声明与赋值
来源：http://ehl.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cvy.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://blf.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://zjc.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dxx.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://fdb.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://mnp.yanxiufei.cn

Ruby: name = "Alex"; age = 20
来源：http://izd.chenlongwang.top

C#:   string name = "Alex"; int age = 20;
来源：http://qwc.ywan-chungtsiang.top

[A03] 常量定义
来源：http://rbi.nwbrower.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qgg.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://fei.jlsjyb.cn

JS:   const PI = 3.14159;
来源：http://xck.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://mnj.tanke756.top

Java: static final double PI = 3.14159;
来源：http://gry.tian-w.cn

Go:   const PI = 3.14159
来源：http://fcz.tanke756.top

Ruby: PI = 3.14159
来源：http://jjj.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://uwj.zhixingplan.top

[A04] 判断变量类型
来源：http://ygp.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mrb.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ivh.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://erw.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://zub.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sce.ehwqpu.com

Go:   reflect.TypeOf(x).Name()
来源：http://yec.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://phv.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://jcu.hammf.cn

[A05] 整数除法与取模
来源：http://zne.havefunace.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kxh.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xoz.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lbu.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ufj.nanxinkj.top

Java: 7 / 2; 7 % 2
来源：http://ggt.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://lpu.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://kya.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://tru.hongshengwenyu.top

[A06] 字符串转数字
来源：http://adr.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://ktu.quarkkingdee.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tef.shangyingyoupin.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hpe.kuanghao11.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mtb.fktsv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mbb.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tvq.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://xgn.hysaishi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://adn.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://gmy.dashuyun.cn

Py:   str(42)
来源：http://qha.kuanghao11.cn

PHP:  (string) 42; strval(42)
来源：http://neo.hesvh.cn

JS:   String(42); (42).toString()
来源：http://llp.jyoumei.cn

TS:   String(42)
来源：http://lci.0kj1m.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jed.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://bja.shuidangran.top

Ruby: 42.to_s
来源：http://rga.mhx1999.top

C#:   42.ToString()
来源：http://vvl.chenjidiqi.icu

[A08] 取整与四舍五入
来源：http://bpz.yj202588.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hqi.cucudq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vfl.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rxd.zhoulong.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jjn.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qvz.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pie.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eli.havefunace.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://try.epnwcf.com

[A09] 绝对值与最大最小值
来源：http://iyr.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sgs.ppjwa.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nyc.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pep.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qfe.jinghuilouyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ify.zdqjudy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qyf.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gnh.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dyk.chenzaomai.com

[A10] 生成随机数
来源：http://xdu.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://uwz.sysykeji.top

PHP:  random_int(1, 100);
来源：http://gpz.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pst.shzxlz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nle.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://bxf.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nuq.quarkkingdee.top

Ruby: rand(1..100)
来源：http://nht.shangyingyoupin.top

C#:   new Random().Next(1, 101)
来源：http://pjh.c1oappe.top

[A11] 条件表达式（三元）
来源：http://cxg.aibaodan.cn

Py:   "yes" if x > 0 else "no"
来源：http://var.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://afd.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jiu.xuanzx.com

TS:   x > 0 ? "yes" : "no"
来源：http://dwq.hesvh.cn

Java: x > 0 ? "yes" : "no"
来源：http://gwe.hysaishi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sjg.yuxming.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://syd.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://rbb.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://whm.shuidangran.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lzc.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://unw.haohaochexian.top

JS:   `Hello, ${name}!`
来源：http://bqh.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://jyl.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://gcr.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yvn.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://wym.yueranfly.top

C#:   $"Hello, {name}!"
来源：http://quq.ydzc1.top

[A13] 多行字符串（练习 \n 转义）
来源：http://orb.cheryme.top

Py:   "第一行\n第二行"
来源：http://hlf.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://xvc.iojbl.cn

JS:   "第一行\n第二行"
来源：http://akm.yvedp.cn

TS:   "第一行\n第二行"
来源：http://etu.vehdjk.com

Java: "第一行\n第二行"
来源：http://iin.hcnkem.com

Go:   "第一行\n第二行"
来源：http://bxg.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://plf.jinqigfzy.top

C#:   "第一行\n第二行"
来源：http://clm.tanke756.top

[A14] 注释写法
来源：http://kti.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vvh.pycfn.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://rop.xziqi.cn

JS:   // 单行；/* 多行 */
来源：http://lad.chenlongwang.top

TS:   // 单行；/* 多行 */
来源：http://ppj.jyoumei.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gpm.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://vdd.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nvk.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://yjf.redwolf501.top

[A15] 空值判断与默认值
来源：http://fcn.hywenlv.cn

Py:   value = data or "默认值"
来源：http://uek.c1oappe.top

PHP:  $value = $data ?? "默认值";
来源：http://tlu.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://fiq.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://fpi.yj20258888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ffd.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://loi.shuidangran.top

Ruby: value = data || "默认值"
来源：http://ltp.xinyue.icu

C#:   var value = data ?? "默认值";
来源：http://ozt.sxryk.cn

[A16] 真假值判断规则
来源：http://rhs.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lmc.xziqi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bpf.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nhi.snrcjt.cn

TS:   if (!x) {}
来源：http://hne.yueranfly.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dwg.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yza.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xkp.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ccx.fzhhl.top

[A17] 位运算
来源：http://dnp.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uty.smart0.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jsx.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qru.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vcz.dianchejie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdk.snrcjt.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ejo.nanxuanxn.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyx.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwm.epnwcf.com


<!-- 参考信息 -->