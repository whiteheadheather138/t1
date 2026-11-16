代发 wailian999

[U103] JS：定时器
来源：http://ymq.zhoulong.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dyo.c1oappe.top

[U104] JS：防抖
来源：http://edw.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zev.meibo888.top

[U105] JS：节流
来源：http://wzk.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gey.shuidangran.top

[U106] JS：日期格式化
来源：http://mgy.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yip.zhongyouzk.top

[U107] JS：数字千分位
来源：http://tyl.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jyf.cdnleiting.top

[U108] JS：随机整数
来源：http://euq.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ufc.aibaodan.cn

[U109] JS：数组分组
来源：http://npv.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://nwi.gaohongyu789.top

[U110] JS：数组分块
来源：http://vyq.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lkg.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://srh.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://mwm.bbcook.cn

[U112] JS：字符串补位
来源：http://zpf.jyoumei.cn

"7".padStart(3, "0")
来源：http://cal.smart0.xyz

[U113] JS：正则替换全部
来源：http://qeo.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://wbt.xuanzx.com

[U114] JS：JSON 深比较
来源：http://nbw.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zyc.nwbrower.top

[U115] JS：生成 UUID
来源：http://yxz.ppjwa.cn

crypto.randomUUID()
来源：http://znr.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://cei.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://unj.zdbjq.cn

[U117] JS：单元测试
来源：http://owd.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://syb.sweek.top

[U118] JS：开发服务器
来源：http://meh.hfpthk.cn

npm i -D vite;  npx vite
来源：http://inc.jqgfzy.top

[U119] JS：生产构建
来源：http://ges.redwolf501.top

npx vite build
来源：http://xir.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://csb.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://zou.zhoulong.xyz

================================================================================
来源：http://rfj.zhengqikj.top

统计汇总
来源：http://kak.andypj.xyz

================================================================================
来源：http://kur.yj202588.top

按语言统计（条）：
来源：http://xyh.ydzc1.top

Python ......... 252
来源：http://ojr.yuanzhike.top

PHP ............ 252
来源：http://nul.svipenyu.cn

JavaScript ..... 252
来源：http://cwr.yvedp.cn

TypeScript ..... 212
来源：http://ybo.nanxuanxn.top

Java ........... 212
来源：http://sqb.yanxiufei.cn

Go ............. 212
来源：http://vbj.hcnkem.com

Ruby ........... 212
来源：http://fhp.52xcode.cn

C# ............. 212
来源：http://fjl.tarul.cn

C .............. 30
来源：http://odq.52xcode.cn

C++ ............ 30
来源：http://biq.fktsv.cn

SQL ............ 90
来源：http://vps.yj20258.top

Bash ........... 80
来源：http://xoq.sysykeji.top

Kotlin ......... 15
来源：http://lip.cdnleiting.top

Swift .......... 15
来源：http://mmb.smart0.xyz

Lua ............ 10
来源：http://yub.svipenyu.cn

Perl ........... 10
来源：http://fky.sysykeji.top

Scala .......... 10
来源：http://lii.c1oappe.top

------------------------------------
来源：http://aof.ydjk.org.cn

合计 ........... 2106 条
来源：http://xfw.ywan-chungtsiang.top

按章节统计：
来源：http://ung.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ccm.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bkb.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wfm.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dgo.shuidangran.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wwg.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xgv.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ynr.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bff.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uqu.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://clr.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xth.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gtk.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vze.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jel.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://myk.zhiwuduotai.top

Q SQL 专题                              90
来源：http://jeq.hnxiangtu.top

R Bash 专题                             80
来源：http://ghr.nanxinkj.top

S C / C++ 专题                          60
来源：http://nei.hcnkem.com

T 其他语言补充                          60
来源：http://cwl.fanxiaobao.xyz

U 高频实用片段                         120
来源：http://wzh.sjlbkw.cn

------------------------------------
来源：http://ffh.aizwys.cn

合计                                  2106 条
来源：http://phz.mhx1999.top

--------------------------------------------------------------------------------
来源：http://lnr.cashguo.top

使用提醒
来源：http://chk.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://hvn.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mdn.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tcw.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://njj.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ewc.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blm.ydzc1.top

—— 文件结束 ——
来源：http://aie.hnqzz.top

================================================================================
来源：http://gzo.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://adu.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://ltv.iojbl.cn

================================================================================
来源：http://hlj.chenzaomai.com

【收录内容】
来源：http://ree.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://man.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wda.aibaodan.cn

SQL · Bash · C · C++
来源：http://nap.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rie.316326.xyz

【使用说明】
来源：http://sni.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qij.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kgg.bbcook.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://twm.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gvd.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bnx.yvedp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mlx.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jyi.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dhs.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pdf.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zfn.xylfe.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fnc.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xoj.yongpay.top

【文件统计】
来源：http://eiu.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qva.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://gtp.sxryk.cn

目  录
来源：http://fwo.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://fpp.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xgu.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aro.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qvk.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jqw.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mjf.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tgm.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lii.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cql.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nhv.meibo888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bat.epnwcf.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mcc.yueranfly.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rnq.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vkx.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sdb.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lyf.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pbl.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bkj.zycfv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://szb.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cmt.uphjek.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://njm.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qmh.yuanzhike.top

================================================================================
来源：http://ssx.birdmap.top

A. 基础语法与类型
来源：http://uir.ctjpmb.com

================================================================================
来源：http://fin.ivvv.top

[A01] Hello World
来源：http://ecn.jinqigufen.top

Py:   print("Hello, World!")
来源：http://ehr.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://bja.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://knf.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tzw.zdbjq.cn

Java: System.out.println("Hello, World!");
来源：http://suu.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://qgo.epnwcf.com

Ruby: puts "Hello, World!"
来源：http://vqg.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://xbc.52xcode.cn

[A02] 变量声明与赋值
来源：http://wod.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wqh.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lfy.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://vyc.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ruh.aibaodan.cn

Java: String name = "Alex"; int age = 20;
来源：http://voi.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://zpx.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://qgz.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://qeb.316326.xyz

[A03] 常量定义
来源：http://lfy.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ecy.uphjek.com

PHP:  const PI = 3.14159;
来源：http://guz.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://yki.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://eiv.redwolf501.top

Java: static final double PI = 3.14159;
来源：http://ivv.cdnleiting.top

Go:   const PI = 3.14159
来源：http://okf.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://oeh.cashguo.top

C#:   const double PI = 3.14159;
来源：http://plk.vqdsnc.cn

[A04] 判断变量类型
来源：http://zns.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://yca.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vod.cdnleiting.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://egw.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://xdx.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xyc.pycfn.com

Go:   reflect.TypeOf(x).Name()
来源：http://djv.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hqy.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://dsg.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://ovg.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sxc.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://acg.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ahi.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kvw.yangfankeji.com

Java: 7 / 2; 7 % 2
来源：http://slx.dashuyun.cn

Go:   7 / 2; 7 % 2
来源：http://yfs.svipenyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://nqd.jinqigfzy.top

C#:   7 / 2; 7 % 2
来源：http://jxk.zhongyouzk.top

[A06] 字符串转数字
来源：http://zqc.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://gmp.yj202588.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lho.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mwh.jinghuilouyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://znr.ppjwa.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://awj.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jqd.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jdc.cdnleiting.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://obz.nanxuanxn.top

[A07] 数字转字符串
来源：http://foj.gzhubu.top

Py:   str(42)
来源：http://urh.chenlongwang.top

PHP:  (string) 42; strval(42)
来源：http://lqk.gzhubu.top

JS:   String(42); (42).toString()
来源：http://det.snrcjt.cn

TS:   String(42)
来源：http://alx.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dcs.gotoacloud.top

Go:   strconv.Itoa(42)
来源：http://fub.hnxiangtu.top

Ruby: 42.to_s
来源：http://bgp.daxiang520.top

C#:   42.ToString()
来源：http://nqw.ywan-chungtsiang.top

[A08] 取整与四舍五入
来源：http://ycr.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yvb.zdqjudy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bab.gotoacloud.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://icp.daria6918.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cat.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ban.dianchejie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://woo.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lce.zhaomingkeji.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fuc.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://art.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iol.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kek.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dxb.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wgk.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://inr.feifeiyinyue.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jyk.gogol.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lsk.fktsv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tdh.guowangkeji.top

[A10] 生成随机数
来源：http://cip.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://smx.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://oax.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dzd.hongshengwenyu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ltu.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://rpd.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://max.yongpay.top

Ruby: rand(1..100)
来源：http://bkx.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://zci.tianlin.xyz

[A11] 条件表达式（三元）
来源：http://idv.gaohongyu789.top

Py:   "yes" if x > 0 else "no"
来源：http://xur.jianghu66.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qfk.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://zqc.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://dap.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://ygm.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ged.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pzi.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://nfk.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://klm.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tns.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ydx.nanxuanxn.top

JS:   `Hello, ${name}!`
来源：http://aap.yanxiufei.cn

TS:   `Hello, ${name}!`
来源：http://vue.chenlongwang.top

Java: "Hello, %s!".formatted(name)
来源：http://bsy.nanxinkj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hax.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://vhe.sweek.top

C#:   $"Hello, {name}!"
来源：http://qwu.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zve.cashguo.top

Py:   "第一行\n第二行"
来源：http://pxx.sjlbkw.cn

PHP:  "第一行\n第二行"
来源：http://hio.gzhubu.top

JS:   "第一行\n第二行"
来源：http://zmg.tanke756.top

TS:   "第一行\n第二行"
来源：http://xkz.aibaodan.cn

Java: "第一行\n第二行"
来源：http://bhg.wangdashe.top

Go:   "第一行\n第二行"
来源：http://ufc.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://oth.iojbl.cn

C#:   "第一行\n第二行"
来源：http://wrd.zdbjq.cn

[A14] 注释写法
来源：http://nog.mhx1999.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gfb.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qpb.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://gym.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://azj.chenjidiqi.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dte.smart0.xyz

Go:   // 单行；/* 多行 */
来源：http://fhy.havefunace.top

Ruby: # 单行；=begin 多行 =end
来源：http://peg.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://ijt.cdnleiting.top

[A15] 空值判断与默认值
来源：http://boo.chenjidiqi.icu

Py:   value = data or "默认值"
来源：http://hza.xylfe.cn

PHP:  $value = $data ?? "默认值";
来源：http://psw.zhiwuduotai.top

JS:   const value = data ?? "默认值";
来源：http://ryw.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://uhi.jqgufenzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wss.jlsjyb.cn

Go:   if data == "" { data = "默认值" }
来源：http://ddi.jinghuilouyu.cn

Ruby: value = data || "默认值"
来源：http://bxw.cqqwz.cn

C#:   var value = data ?? "默认值";
来源：http://woh.hongshengwenyu.top

[A16] 真假值判断规则
来源：http://noy.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jyn.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fzt.zhiwuduotai.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uct.ppjwa.cn

TS:   if (!x) {}
来源：http://xrx.cucudq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xoz.316326.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zcg.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zmn.ybcxt.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rkb.sysykeji.top

[A17] 位运算
来源：http://ywn.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://suk.jyoumei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://van.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://apg.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xiw.nanxuanxn.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://msz.bbcook.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jdd.gzhubu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vft.cheryme.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvt.fehbvm.com

[A18] 字符与 ASCII 码互转
来源：http://tkj.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://cdk.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://uov.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ojc.ehwqpu.com


<!-- 参考信息 -->