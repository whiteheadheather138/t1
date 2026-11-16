代发 wailian999

[U105] JS：节流
来源：http://iwq.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gok.shzxlz.cn

[U106] JS：日期格式化
来源：http://auk.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jrt.52xcode.cn

[U107] JS：数字千分位
来源：http://syf.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rhl.nwbrower.top

[U108] JS：随机整数
来源：http://vfe.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nys.gotoacloud.top

[U109] JS：数组分组
来源：http://bej.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://syu.yfazqb.com

[U110] JS：数组分块
来源：http://atw.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://csw.fzhhl.top

[U111] JS：对象转 Map
来源：http://mth.316326.xyz

new Map(Object.entries(obj))
来源：http://peo.shuidangran.top

[U112] JS：字符串补位
来源：http://hco.vqdsnc.cn

"7".padStart(3, "0")
来源：http://ppz.cdnleiting.top

[U113] JS：正则替换全部
来源：http://pyl.fktsv.cn

s.replaceAll("a", "b")
来源：http://iws.jianghu66.top

[U114] JS：JSON 深比较
来源：http://cxl.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://igs.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://nsh.pycfn.com

crypto.randomUUID()
来源：http://qph.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://qfu.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://prf.xylfe.cn

[U117] JS：单元测试
来源：http://fjv.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://ivn.zhoulong.xyz

[U118] JS：开发服务器
来源：http://tci.tian-w.cn

npm i -D vite;  npx vite
来源：http://bpk.gzhubu.top

[U119] JS：生产构建
来源：http://khy.ehwqpu.com

npx vite build
来源：http://oru.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://xqm.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://ddp.yuxming.cn

================================================================================
来源：http://rbl.zhoulong.xyz

统计汇总
来源：http://ksd.yj20258888.top

================================================================================
来源：http://dor.gotoacloud.top

按语言统计（条）：
来源：http://mpi.shzxlz.cn

Python ......... 252
来源：http://pjl.hongshengwenyu.top

PHP ............ 252
来源：http://cth.yj202588.top

JavaScript ..... 252
来源：http://zcf.nanxuanxn.top

TypeScript ..... 212
来源：http://rqe.zycfv.cn

Java ........... 212
来源：http://xxg.daxiang520.top

Go ............. 212
来源：http://rtt.hywenlv.cn

Ruby ........... 212
来源：http://gvi.dianchejie.cn

C# ............. 212
来源：http://yxo.jiagoushi.top

C .............. 30
来源：http://zxm.nanxuanxn.top

C++ ............ 30
来源：http://qrx.sjlbkw.cn

SQL ............ 90
来源：http://sxj.aizwys.cn

Bash ........... 80
来源：http://zmu.uphjek.com

Kotlin ......... 15
来源：http://qap.daria6918.cn

Swift .......... 15
来源：http://zwm.gotoacloud.top

Lua ............ 10
来源：http://nzc.chenjidiqi.icu

Perl ........... 10
来源：http://pxw.zhijiandao.cn

Scala .......... 10
来源：http://ose.fehbvm.com

------------------------------------
来源：http://zfx.cashguo.top

合计 ........... 2106 条
来源：http://bny.wangshuangyany.cn

按章节统计：
来源：http://ygw.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bsd.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yoi.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uej.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hxx.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bjg.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pkv.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qwg.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nkc.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qlv.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://amb.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qnz.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yoi.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://itu.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xef.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lxs.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jxm.jinqigufen.top

Q SQL 专题                              90
来源：http://css.cqqwz.cn

R Bash 专题                             80
来源：http://agj.daria6918.cn

S C / C++ 专题                          60
来源：http://twx.hnqzz.top

T 其他语言补充                          60
来源：http://twx.fzhhl.top

U 高频实用片段                         120
来源：http://qlk.fehbvm.com

------------------------------------
来源：http://rik.shangyingyoupin.top

合计                                  2106 条
来源：http://une.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://cmz.zhoulong.xyz

使用提醒
来源：http://zyo.mhx1999.top

--------------------------------------------------------------------------------
来源：http://dbj.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://urj.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fxe.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nge.svipenyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://onx.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rtb.hnxiangtu.top

—— 文件结束 ——
来源：http://ujr.xylfe.cn

================================================================================
来源：http://yxp.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://yby.aizwys.cn

Common Programming Examples Cheat Book
来源：http://spa.fanxiaobao.xyz

================================================================================
来源：http://hds.tianlin.xyz

【收录内容】
来源：http://fpg.jlsjyb.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vct.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mdc.haohaochexian.top

SQL · Bash · C · C++
来源：http://jwg.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mzp.uphjek.com

【使用说明】
来源：http://xjv.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://auv.aizwys.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jsm.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jxo.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ndt.ydjk.org.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kxx.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://goe.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://umv.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://doe.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://njm.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ras.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://luc.wangshuangyany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hly.sxryk.cn

【文件统计】
来源：http://nod.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ggw.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://kaf.jlsjyb.cn

目  录
来源：http://odq.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://abw.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jnz.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://agt.hysaishi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://axj.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ypl.52xcode.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://klh.chenjidiqi.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://soe.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pag.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bii.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uyt.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mss.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://spq.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nry.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxv.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aeo.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tdk.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eyk.yj20258888.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://thc.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yum.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://juk.zhixingplan.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cam.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://twp.vehdjk.com

================================================================================
来源：http://ugj.ybcxt.top

A. 基础语法与类型
来源：http://gbr.9152youxi.cn

================================================================================
来源：http://mhj.smart0.xyz

[A01] Hello World
来源：http://dtn.bbcook.cn

Py:   print("Hello, World!")
来源：http://sci.fktsv.cn

PHP:  echo "Hello, World!";
来源：http://nyg.yj20258888.top

JS:   console.log("Hello, World!");
来源：http://bwd.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gsy.yj20258.top

Java: System.out.println("Hello, World!");
来源：http://hfh.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://uam.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://pen.pycfn.com

C#:   Console.WriteLine("Hello, World!");
来源：http://mwx.yonumen.top

[A02] 变量声明与赋值
来源：http://hlk.dianchejie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://edq.jinqigfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://sjy.zhixingplan.top

JS:   let name = "Alex"; const age = 20;
来源：http://ntq.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tsh.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://dum.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://lji.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://cvw.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://gse.chenjidiqi.icu

[A03] 常量定义
来源：http://sku.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://swn.cheryme.top

PHP:  const PI = 3.14159;
来源：http://dmk.yj20258.top

JS:   const PI = 3.14159;
来源：http://gep.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://uyr.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://erd.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://yjx.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://lla.xylfe.cn

C#:   const double PI = 3.14159;
来源：http://fee.daxiang520.top

[A04] 判断变量类型
来源：http://hdd.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bws.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xxr.nanxinkj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lio.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://nwb.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vny.quarkkingdee.top

Go:   reflect.TypeOf(x).Name()
来源：http://tmr.dianchejie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tsv.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://iqa.shzxlz.cn

[A05] 整数除法与取模
来源：http://omc.fehbvm.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://soh.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dac.chenjidiqi.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hpc.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xsg.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://lri.jqgufenzy.top

Go:   7 / 2; 7 % 2
来源：http://ltw.ctjpmb.com

Ruby: 7 / 2; 7 % 2
来源：http://udf.cdnleiting.top

C#:   7 / 2; 7 % 2
来源：http://yvk.hammf.cn

[A06] 字符串转数字
来源：http://gcj.hywenlv.cn

Py:   int("42"); float("3.14")
来源：http://kdy.jinqigfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sxs.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jww.bbcook.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jcm.kuanghao11.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ohr.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kkg.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vsy.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ebb.yvedp.cn

[A07] 数字转字符串
来源：http://otx.snrcjt.cn

Py:   str(42)
来源：http://hbi.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://fua.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://zhs.chenzaomai.com

TS:   String(42)
来源：http://fvt.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sky.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://rrc.hammf.cn

Ruby: 42.to_s
来源：http://ujg.shuidangran.top

C#:   42.ToString()
来源：http://dda.jinyuanbaomall.cn

[A08] 取整与四舍五入
来源：http://mjb.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zzv.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fyi.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cwk.wangshuangyany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dyq.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rlk.jqgufenzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://szr.fehbvm.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ylj.gaohongyu789.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dhf.ydjk.org.cn

[A09] 绝对值与最大最小值
来源：http://rhb.nanxinkj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qmy.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tpf.birdmap.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://txs.yvedp.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ufv.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tpj.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ztb.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ubz.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jqn.feifeiyinyue.top

[A10] 生成随机数
来源：http://zbp.tianlin.xyz

Py:   import random; random.randint(1, 100)
来源：http://dqt.sysykeji.top

PHP:  random_int(1, 100);
来源：http://rqk.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zfe.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gsc.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://gev.birdmap.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://juf.svipenyu.cn

Ruby: rand(1..100)
来源：http://rrh.yvedp.cn

C#:   new Random().Next(1, 101)
来源：http://ziv.ivvv.top

[A11] 条件表达式（三元）
来源：http://dqa.ywan-chungtsiang.top

Py:   "yes" if x > 0 else "no"
来源：http://bnm.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://zdl.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://hxn.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://ymr.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://rjp.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hln.c1oappe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://dou.bbcook.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mmw.zdbjq.cn

[A12] 字符串插值 / 格式化
来源：http://bos.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xbr.jqgfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://abl.pycfn.com

JS:   `Hello, ${name}!`
来源：http://dgj.zdqjudy.top

TS:   `Hello, ${name}!`
来源：http://uie.jinghuilouyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://zwl.jqgfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kgb.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://atx.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://ejt.guowangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ofr.sweek.top

Py:   "第一行\n第二行"
来源：http://zfe.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://prn.daria6918.cn

JS:   "第一行\n第二行"
来源：http://sen.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://giz.meibo888.top

Java: "第一行\n第二行"
来源：http://pid.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://dwt.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://dop.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://ofw.jqgufenzy.top

[A14] 注释写法
来源：http://bmb.mhx1999.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vej.nanxuanxn.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jsa.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://ikc.meibo888.top

TS:   // 单行；/* 多行 */
来源：http://wfu.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mob.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://ghx.bbcook.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ukz.sufxvd.cn

C#:   // 单行；/* 多行 */
来源：http://aog.zhixingplan.top

[A15] 空值判断与默认值
来源：http://nmo.cdnleiting.top

Py:   value = data or "默认值"
来源：http://pvh.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://mag.vqdsnc.cn

JS:   const value = data ?? "默认值";
来源：http://cqm.ywan-chungtsiang.top

TS:   const value = data ?? "默认值";
来源：http://wuh.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blh.havefunace.top

Go:   if data == "" { data = "默认值" }
来源：http://jno.nanxinkj.top

Ruby: value = data || "默认值"
来源：http://tck.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://qbq.tianlin.xyz

[A16] 真假值判断规则
来源：http://vnx.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qix.chenlongwang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tkx.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xmu.zhixingplan.top

TS:   if (!x) {}
来源：http://csu.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jex.yuxming.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fcx.zhaomingkeji.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://qty.cucudq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kfq.hywenlv.cn

[A17] 位运算
来源：http://pqs.ydzc1.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prh.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cpt.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyb.wangshuangyany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tiy.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hlx.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mej.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oni.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qjl.pycfn.com

[A18] 字符与 ASCII 码互转
来源：http://xnh.hysaishi.cn

Py:   ord("A"); chr(65)
来源：http://ubb.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://muj.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eri.daxiang520.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kui.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://yzb.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pfa.ivvv.top

Ruby: "A".ord; 65.chr
来源：http://npl.316326.xyz


<!-- 参考信息 -->