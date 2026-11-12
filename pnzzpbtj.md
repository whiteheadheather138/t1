代发 wailian999

[U101] JS：classList 操作
来源：http://xwo.uphjek.com

el.classList.toggle("active")
来源：http://jpb.xziqi.cn

[U102] JS：本地存储
来源：http://oov.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://abb.havefunace.top

[U103] JS：定时器
来源：http://dya.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fen.hnxiangtu.top

[U104] JS：防抖
来源：http://vex.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbt.yueranfly.top

[U105] JS：节流
来源：http://gln.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://snm.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://plf.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rtl.ehwqpu.com

[U107] JS：数字千分位
来源：http://vad.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lwm.fktsv.cn

[U108] JS：随机整数
来源：http://zul.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xxa.aibaodan.cn

[U109] JS：数组分组
来源：http://zuq.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://nhf.vehdjk.com

[U110] JS：数组分块
来源：http://djn.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ivs.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://cam.aibaodan.cn

new Map(Object.entries(obj))
来源：http://mmd.pycfn.com

[U112] JS：字符串补位
来源：http://nzs.yuxming.cn

"7".padStart(3, "0")
来源：http://cwv.0kj1m.cn

[U113] JS：正则替换全部
来源：http://tps.aibaodan.cn

s.replaceAll("a", "b")
来源：http://fha.iojbl.cn

[U114] JS：JSON 深比较
来源：http://prz.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pgy.sxryk.cn

[U115] JS：生成 UUID
来源：http://rqr.kuanghao11.cn

crypto.randomUUID()
来源：http://skb.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://mcv.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://gyq.jqgfzy.top

[U117] JS：单元测试
来源：http://pxm.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://ppo.havefunace.top

[U118] JS：开发服务器
来源：http://tzs.yuanzhike.top

npm i -D vite;  npx vite
来源：http://epz.cqqwz.cn

[U119] JS：生产构建
来源：http://cwl.xuetiantiany.cn

npx vite build
来源：http://ctg.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://ljn.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://swd.jqgufenzy.top

================================================================================
来源：http://cle.cqqwz.cn

统计汇总
来源：http://buq.cheryme.top

================================================================================
来源：http://stb.zdbjq.cn

按语言统计（条）：
来源：http://byn.mhx1999.top

Python ......... 252
来源：http://nzd.smart0.xyz

PHP ............ 252
来源：http://aum.snrcjt.cn

JavaScript ..... 252
来源：http://isx.nanxinkj.top

TypeScript ..... 212
来源：http://esq.yueranfly.top

Java ........... 212
来源：http://bzr.xuanzx.com

Go ............. 212
来源：http://dis.haohaochexian.top

Ruby ........... 212
来源：http://gkh.smart0.xyz

C# ............. 212
来源：http://dvp.chenzaomai.com

C .............. 30
来源：http://kqk.iojbl.cn

C++ ............ 30
来源：http://dep.nwbrower.top

SQL ............ 90
来源：http://ylz.chenjidiqi.icu

Bash ........... 80
来源：http://xtk.sysykeji.top

Kotlin ......... 15
来源：http://fim.hnqzz.top

Swift .......... 15
来源：http://vma.hfpthk.cn

Lua ............ 10
来源：http://acg.yuxming.cn

Perl ........... 10
来源：http://las.vqdsnc.cn

Scala .......... 10
来源：http://zkz.fengsongda.top

------------------------------------
来源：http://neu.fengsongda.top

合计 ........... 2106 条
来源：http://uhe.aizwys.cn

按章节统计：
来源：http://yup.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gpf.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cse.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ofv.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qtx.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eqd.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qjh.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vog.yvedp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ygf.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kog.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rsd.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hhk.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mgx.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hmt.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ydh.c1oappe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qoh.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://anq.hnqzz.top

Q SQL 专题                              90
来源：http://yrl.jinqigufen.top

R Bash 专题                             80
来源：http://dnh.ybcxt.top

S C / C++ 专题                          60
来源：http://ghm.shzxlz.cn

T 其他语言补充                          60
来源：http://wdp.svipenyu.cn

U 高频实用片段                         120
来源：http://rdu.sufxvd.cn

------------------------------------
来源：http://zge.xuetiantiany.cn

合计                                  2106 条
来源：http://mdv.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://ttk.shanyushiyangtech.top

使用提醒
来源：http://luy.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://omo.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mel.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fsp.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pld.bjfxy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://env.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://att.cdnleiting.top

—— 文件结束 ——
来源：http://qzu.fehbvm.com

================================================================================
来源：http://gta.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://nuc.wangdashe.top

Common Programming Examples Cheat Book
来源：http://qig.hesvh.cn

================================================================================
来源：http://arx.jinyuanbaomall.cn

【收录内容】
来源：http://bwr.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://drk.jinqigufen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hrk.316326.xyz

SQL · Bash · C · C++
来源：http://zpe.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mfg.zhixingplan.top

【使用说明】
来源：http://xqz.yj20258888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://myt.jlsjyb.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qgy.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wbh.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aqw.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://oys.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ggk.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nvm.jiagoushi.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lmz.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cap.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jqk.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ika.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vzb.fktsv.cn

【文件统计】
来源：http://tdw.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kfq.cheryme.top

--------------------------------------------------------------------------------
来源：http://yra.zhongyouzk.top

目  录
来源：http://czk.wangdashe.top

--------------------------------------------------------------------------------
来源：http://bxk.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://quz.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cpz.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gcf.yanxiufei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vdj.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aao.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://auf.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jdh.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zdr.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tgq.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dwa.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://waj.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jdd.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pwh.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rts.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eof.daxiang520.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mkz.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kkl.wangshuangyany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uoi.ybcxt.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fpw.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jck.guowangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dli.jinyuanbaomall.cn

================================================================================
来源：http://vwy.jinghuilouyu.cn

A. 基础语法与类型
来源：http://tpn.c1oappe.top

================================================================================
来源：http://djj.meibo888.top

[A01] Hello World
来源：http://ull.dianchejie.cn

Py:   print("Hello, World!")
来源：http://zin.uphjek.com

PHP:  echo "Hello, World!";
来源：http://mki.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://gau.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qzr.gotoacloud.top

Java: System.out.println("Hello, World!");
来源：http://the.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://zih.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://qmw.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://hga.yueranfly.top

[A02] 变量声明与赋值
来源：http://tmx.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qtp.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zck.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nlu.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dlk.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://kls.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://piv.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://ivf.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lfv.uphjek.com

[A03] 常量定义
来源：http://nld.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qom.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://ndg.zycfv.cn

JS:   const PI = 3.14159;
来源：http://ldn.sufxvd.cn

TS:   const PI: number = 3.14159;
来源：http://flq.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://cmk.xylfe.cn

Go:   const PI = 3.14159
来源：http://nxc.0kj1m.cn

Ruby: PI = 3.14159
来源：http://ywh.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://jee.sysykeji.top

[A04] 判断变量类型
来源：http://yhz.ywan-chungtsiang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pam.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vll.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iuz.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://ayu.gaohongyu789.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hxu.chenjidiqi.icu

Go:   reflect.TypeOf(x).Name()
来源：http://yqc.yonumen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fhr.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://qim.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://bjx.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lcd.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ijn.yangfankeji.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vgi.iojbl.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zmn.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://kfv.xziqi.cn

Go:   7 / 2; 7 % 2
来源：http://mgg.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://tra.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://dsj.uphjek.com

[A06] 字符串转数字
来源：http://vcz.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://mlh.xziqi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dqy.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jln.yuanzhike.top

TS:   parseInt("42", 10); Number("42")
来源：http://gkc.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lzf.tarul.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iev.cucudq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fxm.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kfk.cdnleiting.top

[A07] 数字转字符串
来源：http://ben.hongshengwenyu.top

Py:   str(42)
来源：http://mqb.havefunace.top

PHP:  (string) 42; strval(42)
来源：http://hdx.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://zvn.shuidangran.top

TS:   String(42)
来源：http://qbc.tarul.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nzy.xziqi.cn

Go:   strconv.Itoa(42)
来源：http://lwb.guannengcc.top

Ruby: 42.to_s
来源：http://ons.sxryk.cn

C#:   42.ToString()
来源：http://qte.nanxinkj.top

[A08] 取整与四舍五入
来源：http://hdr.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ugk.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yzk.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gzd.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://icu.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dkm.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fvf.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zam.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zqm.hesvh.cn

[A09] 绝对值与最大最小值
来源：http://kil.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wmd.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://oas.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pjb.yj202588.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ggc.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zxw.vehdjk.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://siq.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gdx.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xpg.shzxlz.cn

[A10] 生成随机数
来源：http://atv.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://urh.wangshuangyany.cn

PHP:  random_int(1, 100);
来源：http://xud.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cjy.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rng.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://cus.nanxinkj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yel.fzhhl.top

Ruby: rand(1..100)
来源：http://ldz.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://lly.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://qsp.zhaomingkeji.xyz

Py:   "yes" if x > 0 else "no"
来源：http://pwc.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ltk.xingfuxueyuan.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://ubr.jqgufenzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://hrt.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://bvv.shanyushiyangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ddy.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dpx.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://ltm.guowangkeji.top

[A12] 字符串插值 / 格式化
来源：http://dsv.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://igj.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tyc.yonumen.top

JS:   `Hello, ${name}!`
来源：http://iji.daria6918.cn

TS:   `Hello, ${name}!`
来源：http://jto.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://mav.sysykeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ylm.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://urs.vqdsnc.cn

C#:   $"Hello, {name}!"
来源：http://ngh.aizwys.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lth.ehwqpu.com

Py:   "第一行\n第二行"
来源：http://aut.cdnleiting.top

PHP:  "第一行\n第二行"
来源：http://sql.yj20258888.top

JS:   "第一行\n第二行"
来源：http://jkb.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://vor.zhijiandao.cn

Java: "第一行\n第二行"
来源：http://psc.fengsongda.top

Go:   "第一行\n第二行"
来源：http://ghh.zycfv.cn

Ruby: "第一行\n第二行"
来源：http://cvx.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://gaq.hfpthk.cn

[A14] 注释写法
来源：http://ypc.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vve.zhijiandao.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tls.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://avl.zhijiandao.cn

TS:   // 单行；/* 多行 */
来源：http://usi.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hpz.chenjidiqi.icu

Go:   // 单行；/* 多行 */
来源：http://ynb.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://nfg.dashuyun.cn

C#:   // 单行；/* 多行 */
来源：http://fjg.mhx1999.top

[A15] 空值判断与默认值
来源：http://wsd.yonumen.top

Py:   value = data or "默认值"
来源：http://czf.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://czo.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://jse.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://uhf.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bir.yuanzhike.top

Go:   if data == "" { data = "默认值" }
来源：http://hqc.cheryme.top

Ruby: value = data || "默认值"
来源：http://mgh.cqqwz.cn

C#:   var value = data ?? "默认值";
来源：http://png.gaohongyu789.top

[A16] 真假值判断规则
来源：http://wis.tarul.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://csm.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fzu.cucudq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ifz.sxryk.cn

TS:   if (!x) {}
来源：http://mbe.yangfankeji.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zth.fengsongda.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sqw.tarul.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vnn.vehdjk.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dec.vehdjk.com

[A17] 位运算
来源：http://vek.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pnd.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bpf.gaohongyu789.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xez.xinyue.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sak.yfazqb.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qyv.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bxy.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmm.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://asi.c1oappe.top


<!-- 参考信息 -->