代发 wailian999

[U103] JS：定时器
来源：http://djy.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qpc.sufxvd.cn

[U104] JS：防抖
来源：http://vju.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxi.haohaochexian.top

[U105] JS：节流
来源：http://agm.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://urj.bjfxy.top

[U106] JS：日期格式化
来源：http://tlt.zhixingplan.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ksb.sweek.top

[U107] JS：数字千分位
来源：http://rmz.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hck.sufxvd.cn

[U108] JS：随机整数
来源：http://ufm.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vmz.pengpengdd.cyou

[U109] JS：数组分组
来源：http://tyd.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://pup.smart0.xyz

[U110] JS：数组分块
来源：http://dgw.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iip.fktsv.cn

[U111] JS：对象转 Map
来源：http://hsx.tarul.cn

new Map(Object.entries(obj))
来源：http://ebz.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://xio.yj20258.top

"7".padStart(3, "0")
来源：http://tdo.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://sgu.jyoumei.cn

s.replaceAll("a", "b")
来源：http://rob.cucudq.cn

[U114] JS：JSON 深比较
来源：http://toi.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qjw.yueranfly.top

[U115] JS：生成 UUID
来源：http://nka.cashguo.top

crypto.randomUUID()
来源：http://jus.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://pfa.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://pmg.wangdashe.top

[U117] JS：单元测试
来源：http://fxx.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://aio.nwbrower.top

[U118] JS：开发服务器
来源：http://msl.ehwqpu.com

npm i -D vite;  npx vite
来源：http://qiv.jinqigfzy.top

[U119] JS：生产构建
来源：http://zqe.tian-w.cn

npx vite build
来源：http://zar.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://ztt.cashguo.top

import.meta.env.VITE_API_URL
来源：http://qpk.daria6918.cn

================================================================================
来源：http://rxz.wangdashe.top

统计汇总
来源：http://gcr.gogol.net.cn

================================================================================
来源：http://wer.wangdashe.top

按语言统计（条）：
来源：http://ijd.fktsv.cn

Python ......... 252
来源：http://sgm.fengsongda.top

PHP ............ 252
来源：http://opp.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://jra.jyoumei.cn

TypeScript ..... 212
来源：http://dmb.smart0.xyz

Java ........... 212
来源：http://aai.ydzc1.top

Go ............. 212
来源：http://wnv.cheryme.top

Ruby ........... 212
来源：http://app.cucudq.cn

C# ............. 212
来源：http://zxx.chenjidiqi.icu

C .............. 30
来源：http://jsp.nwbrower.top

C++ ............ 30
来源：http://xpp.0kj1m.cn

SQL ............ 90
来源：http://kea.jyoumei.cn

Bash ........... 80
来源：http://jvl.shangyingyoupin.top

Kotlin ......... 15
来源：http://afb.yuxming.cn

Swift .......... 15
来源：http://gne.sufxvd.cn

Lua ............ 10
来源：http://zqk.fzhhl.top

Perl ........... 10
来源：http://vrn.xinyue.icu

Scala .......... 10
来源：http://qff.daxiang520.top

------------------------------------
来源：http://eiz.cheryme.top

合计 ........... 2106 条
来源：http://val.316326.xyz

按章节统计：
来源：http://pbv.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dix.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zxh.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nxf.cdnleiting.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://orw.xylfe.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lgk.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ajj.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://meo.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ctv.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rkq.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://txd.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wfv.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zrt.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://azs.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vrv.ehwqpu.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zhs.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gtu.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://ivh.tianlin.xyz

R Bash 专题                             80
来源：http://oyp.ybcxt.top

S C / C++ 专题                          60
来源：http://sdc.smart0.xyz

T 其他语言补充                          60
来源：http://kpm.0kj1m.cn

U 高频实用片段                         120
来源：http://zew.0kj1m.cn

------------------------------------
来源：http://jwg.yangfankeji.com

合计                                  2106 条
来源：http://ugh.mhx1999.top

--------------------------------------------------------------------------------
来源：http://yyb.kuanghao11.cn

使用提醒
来源：http://yic.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://rxo.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fxx.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xho.xuetiantiany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tvp.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://fnh.sysykeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jwn.52xcode.cn

—— 文件结束 ——
来源：http://wtl.yj20258888.top

================================================================================
来源：http://sje.bjfxy.top

程序语言常见例子速查手册（2024 版）
来源：http://clp.yfazqb.com

Common Programming Examples Cheat Book
来源：http://erf.hnxiangtu.top

================================================================================
来源：http://srb.nanxuanxn.top

【收录内容】
来源：http://wks.sufxvd.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wua.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tvv.jianghu66.top

SQL · Bash · C · C++
来源：http://ioi.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uzd.ywan-chungtsiang.top

【使用说明】
来源：http://reo.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ghq.redwolf501.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cus.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://amn.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yrg.xingfuxueyuan.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ecz.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hsi.ydzc1.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dms.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://npf.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uqq.yuanzhike.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gsl.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://imr.wangdashe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rga.jqgfzy.top

【文件统计】
来源：http://evy.cheryme.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lzg.cheryme.top

--------------------------------------------------------------------------------
来源：http://guu.xylfe.cn

目  录
来源：http://kgb.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://uwc.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yhg.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://grm.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dbq.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hxs.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://afj.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mul.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hgj.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oqu.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xgk.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zhi.meibo888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eya.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mmn.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://huj.chenzaomai.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rjk.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ksg.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kqh.epnwcf.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://riv.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cke.gaohongyu789.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wer.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dnb.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zdw.ybcxt.top

================================================================================
来源：http://ccp.nwbrower.top

A. 基础语法与类型
来源：http://unw.zdqjudy.top

================================================================================
来源：http://fxm.bjfxy.top

[A01] Hello World
来源：http://iog.yj20258888.top

Py:   print("Hello, World!")
来源：http://djh.pycfn.com

PHP:  echo "Hello, World!";
来源：http://rle.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://wik.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cfn.hesvh.cn

Java: System.out.println("Hello, World!");
来源：http://kkw.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://ivn.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://rav.havefunace.top

C#:   Console.WriteLine("Hello, World!");
来源：http://waj.yj202588.top

[A02] 变量声明与赋值
来源：http://qts.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ghe.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mjc.yueranfly.top

JS:   let name = "Alex"; const age = 20;
来源：http://fvf.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://poc.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://qin.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://vfq.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://ojf.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://kwi.0kj1m.cn

[A03] 常量定义
来源：http://udy.havefunace.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ncw.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://fat.xylfe.cn

JS:   const PI = 3.14159;
来源：http://szg.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://qwf.xuetiantiany.cn

Java: static final double PI = 3.14159;
来源：http://ldw.fengsongda.top

Go:   const PI = 3.14159
来源：http://zhj.yj20258888.top

Ruby: PI = 3.14159
来源：http://ned.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://ebm.guannengcc.top

[A04] 判断变量类型
来源：http://gyo.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://sph.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kwq.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://btk.zhixingplan.top

TS:   typeof x; x instanceof Date
来源：http://rva.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://phi.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://tur.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ipl.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://ewv.bjfxy.top

[A05] 整数除法与取模
来源：http://zne.yangfankeji.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fhj.ivvv.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rts.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://czm.zhaomingkeji.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://che.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://ymd.quarkkingdee.top

Go:   7 / 2; 7 % 2
来源：http://uja.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://dbo.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://piw.zdbjq.cn

[A06] 字符串转数字
来源：http://jxw.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://syn.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qho.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ljq.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://nfy.yj20258.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xnw.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dks.xingfuxueyuan.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://kbl.fanxiaobao.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ltw.zhixingplan.top

[A07] 数字转字符串
来源：http://tnc.yonumen.top

Py:   str(42)
来源：http://aqm.jinyuanbaomall.cn

PHP:  (string) 42; strval(42)
来源：http://yzv.pycfn.com

JS:   String(42); (42).toString()
来源：http://awd.yangfankeji.com

TS:   String(42)
来源：http://xap.0kj1m.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ymc.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://oxt.tian-w.cn

Ruby: 42.to_s
来源：http://eby.jianghu66.top

C#:   42.ToString()
来源：http://mmd.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://bqt.gogol.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ktc.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ckc.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://msf.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oho.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pxv.chenlongwang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mgn.epnwcf.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://dhv.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iro.sjlbkw.cn

[A09] 绝对值与最大最小值
来源：http://dxd.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fpo.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ehb.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qmt.316326.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://igt.fzhhl.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://now.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xjf.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vcq.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hvb.sjlbkw.cn

[A10] 生成随机数
来源：http://pfw.yangfankeji.com

Py:   import random; random.randint(1, 100)
来源：http://qce.fengsongda.top

PHP:  random_int(1, 100);
来源：http://upc.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bkl.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uir.yuxming.cn

Java: new Random().nextInt(100) + 1
来源：http://uqj.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ihz.hnxiangtu.top

Ruby: rand(1..100)
来源：http://gyz.yj20258.top

C#:   new Random().Next(1, 101)
来源：http://sgn.aizwys.cn

[A11] 条件表达式（三元）
来源：http://zhp.havefunace.top

Py:   "yes" if x > 0 else "no"
来源：http://aur.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tno.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://dqz.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://zhz.sysykeji.top

Java: x > 0 ? "yes" : "no"
来源：http://dfz.yj202588.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qyo.0kj1m.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zon.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rhq.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://njl.yvedp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://stv.yueranfly.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://npt.nanxuanxn.top

JS:   `Hello, ${name}!`
来源：http://pku.wangdashe.top

TS:   `Hello, ${name}!`
来源：http://nyy.316326.xyz

Java: "Hello, %s!".formatted(name)
来源：http://dpr.shanyushiyangkeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vpo.mhx1999.top

Ruby: "Hello, #{name}!"
来源：http://brf.pycfn.com

C#:   $"Hello, {name}!"
来源：http://gda.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://feu.52xcode.cn

Py:   "第一行\n第二行"
来源：http://uui.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://sty.havefunace.top

JS:   "第一行\n第二行"
来源：http://beg.epnwcf.com

TS:   "第一行\n第二行"
来源：http://agh.yj202588.top

Java: "第一行\n第二行"
来源：http://foj.tarul.cn

Go:   "第一行\n第二行"
来源：http://qdy.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://goj.zycfv.cn

C#:   "第一行\n第二行"
来源：http://hyn.kuanghao11.cn

[A14] 注释写法
来源：http://ebl.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qpg.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jsu.jyoumei.cn

JS:   // 单行；/* 多行 */
来源：http://ljo.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://wan.svipenyu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://awx.jinqigufen.top

Go:   // 单行；/* 多行 */
来源：http://jlx.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://yfm.vehdjk.com

C#:   // 单行；/* 多行 */
来源：http://ysy.cheryme.top

[A15] 空值判断与默认值
来源：http://jjv.yuxming.cn

Py:   value = data or "默认值"
来源：http://isq.ydjk.org.cn

PHP:  $value = $data ?? "默认值";
来源：http://qjm.kuanghao11.cn

JS:   const value = data ?? "默认值";
来源：http://wgs.hysaishi.cn

TS:   const value = data ?? "默认值";
来源：http://kxi.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://flb.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://olq.wangdashe.top

Ruby: value = data || "默认值"
来源：http://ubx.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://jih.pengpengdd.cyou

[A16] 真假值判断规则
来源：http://bri.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xib.guannengcc.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rhm.yanxiufei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://urq.hnqzz.top

TS:   if (!x) {}
来源：http://uzd.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ywy.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jte.hnqzz.top

Ruby: unless x            # nil 与 false 为假
来源：http://lye.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qon.daria6918.cn

[A17] 位运算
来源：http://wqo.ywan-chungtsiang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ugu.hfpthk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ekt.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fok.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iju.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gzb.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://awu.hammf.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://odr.xuetiantiany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhx.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://cdr.yonumen.top

Py:   ord("A"); chr(65)
来源：http://zvm.sysykeji.top

PHP:  ord("A"); chr(65)
来源：http://dgw.nanxinkj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uva.shanyushiyangkeji.top


<!-- 参考信息 -->