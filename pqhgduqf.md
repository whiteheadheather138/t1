代发 wailian999

[U99] JS：事件监听
来源：http://jys.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://mgm.zycfv.cn

[U100] JS：DOM 查询
来源：http://wkz.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://jhz.cdnleiting.top

[U101] JS：classList 操作
来源：http://chp.andypj.xyz

el.classList.toggle("active")
来源：http://zgh.hammf.cn

[U102] JS：本地存储
来源：http://tpb.jinyuanbaomall.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gah.daria6918.cn

[U103] JS：定时器
来源：http://otv.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sfu.xylfe.cn

[U104] JS：防抖
来源：http://oyw.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfb.shanyushiyangkeji.top

[U105] JS：节流
来源：http://rum.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jlm.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://zzh.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cyb.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://cuo.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jrr.cheryme.top

[U108] JS：随机整数
来源：http://uyi.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pzg.hammf.cn

[U109] JS：数组分组
来源：http://orl.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://qoe.bbcook.cn

[U110] JS：数组分块
来源：http://zdt.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wev.c1oappe.top

[U111] JS：对象转 Map
来源：http://qsv.xziqi.cn

new Map(Object.entries(obj))
来源：http://ntt.shzxlz.cn

[U112] JS：字符串补位
来源：http://qfx.birdmap.top

"7".padStart(3, "0")
来源：http://kzk.hywenlv.cn

[U113] JS：正则替换全部
来源：http://nxs.gaohongyu789.top

s.replaceAll("a", "b")
来源：http://nwp.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://gcb.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tih.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://qnr.snrcjt.cn

crypto.randomUUID()
来源：http://yhg.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://ufy.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://jkj.shzxlz.cn

[U117] JS：单元测试
来源：http://uoz.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://ivp.chenlongwang.top

[U118] JS：开发服务器
来源：http://vsi.aizwys.cn

npm i -D vite;  npx vite
来源：http://vhq.vehdjk.com

[U119] JS：生产构建
来源：http://evo.zhaomingkeji.xyz

npx vite build
来源：http://xgy.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://tmw.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://kzl.fehbvm.com

================================================================================
来源：http://qia.uphjek.com

统计汇总
来源：http://ztw.ctjpmb.com

================================================================================
来源：http://fve.fengsongda.top

按语言统计（条）：
来源：http://fpl.yvedp.cn

Python ......... 252
来源：http://mtb.jinqigufen.top

PHP ............ 252
来源：http://nsr.jyoumei.cn

JavaScript ..... 252
来源：http://flw.hnxiangtu.top

TypeScript ..... 212
来源：http://axv.ctjpmb.com

Java ........... 212
来源：http://zpw.ydjk.org.cn

Go ............. 212
来源：http://jor.fehbvm.com

Ruby ........... 212
来源：http://gjn.gogol.net.cn

C# ............. 212
来源：http://eap.chenjidiqi.icu

C .............. 30
来源：http://qxm.ybcxt.top

C++ ............ 30
来源：http://sgf.zhengqikj.top

SQL ............ 90
来源：http://nyc.wangshuangyany.cn

Bash ........... 80
来源：http://iik.feifeiyinyue.top

Kotlin ......... 15
来源：http://fnx.gzhubu.top

Swift .......... 15
来源：http://nlu.ppjwa.cn

Lua ............ 10
来源：http://flb.xuanzx.com

Perl ........... 10
来源：http://bxq.fanxiaobao.xyz

Scala .......... 10
来源：http://fuh.zhengqikj.top

------------------------------------
来源：http://xon.tarul.cn

合计 ........... 2106 条
来源：http://mbq.ywan-chungtsiang.top

按章节统计：
来源：http://bph.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hjo.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rop.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mob.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rdr.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iyj.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lcl.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sbm.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ayh.ydzc1.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jmi.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ims.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rjx.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cnt.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nmc.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ahp.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tzl.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cle.yueranfly.top

Q SQL 专题                              90
来源：http://van.epnwcf.com

R Bash 专题                             80
来源：http://edg.jiagoushi.top

S C / C++ 专题                          60
来源：http://bbj.sxryk.cn

T 其他语言补充                          60
来源：http://dom.sweek.top

U 高频实用片段                         120
来源：http://ogu.meibo888.top

------------------------------------
来源：http://ijj.iojbl.cn

合计                                  2106 条
来源：http://win.cashguo.top

--------------------------------------------------------------------------------
来源：http://esu.zhoulong.xyz

使用提醒
来源：http://zze.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://hgx.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qyu.xinyue.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wox.hammf.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xnp.tanke756.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mha.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rrw.daxiang520.top

—— 文件结束 ——
来源：http://njc.jianghu66.top

================================================================================
来源：http://frp.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://gnp.andypj.xyz

Common Programming Examples Cheat Book
来源：http://xwf.yonumen.top

================================================================================
来源：http://xgq.yj202588.top

【收录内容】
来源：http://qok.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qan.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xzy.hesvh.cn

SQL · Bash · C · C++
来源：http://hrj.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nqb.ehwqpu.com

【使用说明】
来源：http://eqj.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mzv.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nqm.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ihs.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vjh.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hde.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eyw.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uuz.havefunace.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qgw.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yqk.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nse.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dnw.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tfn.yuxming.cn

【文件统计】
来源：http://pzv.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tcv.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://vti.zycfv.cn

目  录
来源：http://xfq.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://oij.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kza.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zfa.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://efs.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sji.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eoa.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hih.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vhm.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://crn.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lov.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://umd.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ejd.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tqg.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qdg.sxryk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wih.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vkj.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rud.zhijiandao.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qbc.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kwt.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yro.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kqq.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hzm.yuanzhike.top

================================================================================
来源：http://ozk.yfazqb.com

A. 基础语法与类型
来源：http://mzs.hysaishi.cn

================================================================================
来源：http://lau.hnxiangtu.top

[A01] Hello World
来源：http://mvh.zhengqikj.top

Py:   print("Hello, World!")
来源：http://bxj.dianchejie.cn

PHP:  echo "Hello, World!";
来源：http://gfr.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://uts.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dpl.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://gvx.ivvv.top

Go:   fmt.Println("Hello, World!")
来源：http://jls.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://mkd.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://pwy.ctjpmb.com

[A02] 变量声明与赋值
来源：http://iuo.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rau.jinqigufen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lsi.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://dbo.zdbjq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bbe.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://wst.tanke756.top

Go:   name := "Alex"; age := 20
来源：http://kkl.52xcode.cn

Ruby: name = "Alex"; age = 20
来源：http://dzn.xingfuxueyuan.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ufx.yj20258.top

[A03] 常量定义
来源：http://tvm.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://twf.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://htv.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://ses.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://ukg.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://ewv.cqqwz.cn

Go:   const PI = 3.14159
来源：http://ehw.shanyushiyangkeji.top

Ruby: PI = 3.14159
来源：http://gqu.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://xgi.ivvv.top

[A04] 判断变量类型
来源：http://bul.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kbt.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://brb.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jni.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://wqt.xuetiantiany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://odz.jqgfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://eed.sufxvd.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://url.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://qhm.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://mhr.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kzm.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dxe.jinghuilouyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mtn.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://elc.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://grf.hesvh.cn

Go:   7 / 2; 7 % 2
来源：http://mbq.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://fjn.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://pyo.redwolf501.top

[A06] 字符串转数字
来源：http://ayg.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://qxm.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pwk.haohaochexian.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vdv.ctjpmb.com

TS:   parseInt("42", 10); Number("42")
来源：http://zay.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ivb.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ems.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://amq.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mww.snrcjt.cn

[A07] 数字转字符串
来源：http://dyr.jinghuilouyu.cn

Py:   str(42)
来源：http://sdl.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://asw.fzhhl.top

JS:   String(42); (42).toString()
来源：http://nxx.shanyushiyangtech.top

TS:   String(42)
来源：http://iyq.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://sjr.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://rqv.jianghu66.top

Ruby: 42.to_s
来源：http://uga.yangfankeji.com

C#:   42.ToString()
来源：http://wry.gotoacloud.top

[A08] 取整与四舍五入
来源：http://gzf.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qjh.jinqigfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bbq.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nyw.c1oappe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wzk.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rts.yfazqb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qiw.xuetiantiany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eth.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zde.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://ohj.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://egq.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qeo.0kj1m.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pbk.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yln.sjlbkw.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fvf.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xuv.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://znr.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hcq.nanxinkj.top

[A10] 生成随机数
来源：http://kzy.epnwcf.com

Py:   import random; random.randint(1, 100)
来源：http://aby.sweek.top

PHP:  random_int(1, 100);
来源：http://kda.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kjx.guannengcc.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gff.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://thl.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://utr.zhijiandao.cn

Ruby: rand(1..100)
来源：http://ngm.cashguo.top

C#:   new Random().Next(1, 101)
来源：http://qbo.pengpengdd.cyou

[A11] 条件表达式（三元）
来源：http://ndf.kuanghao11.cn

Py:   "yes" if x > 0 else "no"
来源：http://dbi.daxiang520.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qwk.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dqp.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lul.epnwcf.com

Java: x > 0 ? "yes" : "no"
来源：http://pzw.jiagoushi.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ufi.zhoulong.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://nwu.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://nxz.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://xvz.cheryme.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://twb.fengsongda.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://akb.wangshuangyany.cn

JS:   `Hello, ${name}!`
来源：http://iws.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://zgb.svipenyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://idv.ivvv.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lyf.yanxiufei.cn

Ruby: "Hello, #{name}!"
来源：http://kgj.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://jal.zhijiandao.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cce.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://hnc.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://kre.yuxming.cn

JS:   "第一行\n第二行"
来源：http://kix.tanke756.top

TS:   "第一行\n第二行"
来源：http://hiq.jinqigfzy.top

Java: "第一行\n第二行"
来源：http://fls.sweek.top

Go:   "第一行\n第二行"
来源：http://tfa.zhengqikj.top

Ruby: "第一行\n第二行"
来源：http://pzy.yuxming.cn

C#:   "第一行\n第二行"
来源：http://boi.gzhubu.top

[A14] 注释写法
来源：http://zgg.tarul.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xba.vqdsnc.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fjm.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://mdj.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://nuo.0kj1m.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://koy.wangshuangyany.cn

Go:   // 单行；/* 多行 */
来源：http://znr.vqdsnc.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cmv.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://ehi.shzxlz.cn

[A15] 空值判断与默认值
来源：http://tbw.cashguo.top

Py:   value = data or "默认值"
来源：http://kbk.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://vmb.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://hgj.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://pgt.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://quu.yj20258.top

Go:   if data == "" { data = "默认值" }
来源：http://fwj.9152youxi.cn

Ruby: value = data || "默认值"
来源：http://fxx.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://ltn.chenzaomai.com

[A16] 真假值判断规则
来源：http://bkr.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gqa.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://irm.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lmo.nwbrower.top

TS:   if (!x) {}
来源：http://cvt.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wek.yonumen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gve.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://dit.zycfv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hkj.tian-w.cn

[A17] 位运算
来源：http://gdr.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmp.shzxlz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hwk.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ryr.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kno.zhiwuduotai.top


<!-- 参考信息 -->