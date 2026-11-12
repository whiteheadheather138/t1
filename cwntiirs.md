代发 wailian999

[U105] JS：节流
来源：http://rga.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fti.0kj1m.cn

[U106] JS：日期格式化
来源：http://sjw.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bgz.yangfankeji.com

[U107] JS：数字千分位
来源：http://sgd.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ntf.jinqigfzy.top

[U108] JS：随机整数
来源：http://pry.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qrb.tarul.cn

[U109] JS：数组分组
来源：http://tuw.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://ibq.nanxuanxn.top

[U110] JS：数组分块
来源：http://jro.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vzz.uphjek.com

[U111] JS：对象转 Map
来源：http://yvf.sxryk.cn

new Map(Object.entries(obj))
来源：http://vvq.uphjek.com

[U112] JS：字符串补位
来源：http://vus.yfazqb.com

"7".padStart(3, "0")
来源：http://ohg.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://yug.shuidangran.top

s.replaceAll("a", "b")
来源：http://rkh.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://ppo.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hai.jianghu66.top

[U115] JS：生成 UUID
来源：http://rgj.zhongyouzk.top

crypto.randomUUID()
来源：http://lkg.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://qmn.yj20258.top

/** @param {string} name */ function f(name) {}
来源：http://cay.jlsjyb.cn

[U117] JS：单元测试
来源：http://gbm.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://yla.daria6918.cn

[U118] JS：开发服务器
来源：http://mxk.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://ulk.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://rcf.zhijiandao.cn

npx vite build
来源：http://ati.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://vbc.ivvv.top

import.meta.env.VITE_API_URL
来源：http://hww.zhixingplan.top

================================================================================
来源：http://rtw.jqgufenzy.top

统计汇总
来源：http://qol.sufxvd.cn

================================================================================
来源：http://ahn.xziqi.cn

按语言统计（条）：
来源：http://dwz.hywenlv.cn

Python ......... 252
来源：http://svl.fehbvm.com

PHP ............ 252
来源：http://arq.ppjwa.cn

JavaScript ..... 252
来源：http://vjd.cheryme.top

TypeScript ..... 212
来源：http://ryp.havefunace.top

Java ........... 212
来源：http://nfz.pycfn.com

Go ............. 212
来源：http://kcn.hnqzz.top

Ruby ........... 212
来源：http://pga.yuxming.cn

C# ............. 212
来源：http://dop.svipenyu.cn

C .............. 30
来源：http://kzw.sweek.top

C++ ............ 30
来源：http://mbf.hysaishi.cn

SQL ............ 90
来源：http://qwy.9152youxi.cn

Bash ........... 80
来源：http://tkk.haohaochexian.top

Kotlin ......... 15
来源：http://bof.yonumen.top

Swift .......... 15
来源：http://sen.quarkkingdee.top

Lua ............ 10
来源：http://adw.xuetiantiany.cn

Perl ........... 10
来源：http://nzq.ctjpmb.com

Scala .......... 10
来源：http://fkh.bbcook.cn

------------------------------------
来源：http://qvr.nwbrower.top

合计 ........... 2106 条
来源：http://fnm.sysykeji.top

按章节统计：
来源：http://vov.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fxw.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dwq.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iek.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ujq.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dfp.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vnf.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ymj.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bfn.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://guc.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rin.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ezu.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qet.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ong.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ndb.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://agm.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kyd.kuanghao11.cn

Q SQL 专题                              90
来源：http://uph.ppjwa.cn

R Bash 专题                             80
来源：http://cxo.cucudq.cn

S C / C++ 专题                          60
来源：http://ukf.mhx1999.top

T 其他语言补充                          60
来源：http://emp.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://nbu.hcnkem.com

------------------------------------
来源：http://gyj.jinqigufen.top

合计                                  2106 条
来源：http://avr.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://ypd.ehwqpu.com

使用提醒
来源：http://ioj.havefunace.top

--------------------------------------------------------------------------------
来源：http://fbg.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nmc.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rup.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gxq.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mdd.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kwj.cdnleiting.top

—— 文件结束 ——
来源：http://zbm.daxiang520.top

================================================================================
来源：http://ghs.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://vtw.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://lrb.aizwys.cn

================================================================================
来源：http://vgl.sjlbkw.cn

【收录内容】
来源：http://sud.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sqc.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dgu.nwbrower.top

SQL · Bash · C · C++
来源：http://mss.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://chu.ydzc1.top

【使用说明】
来源：http://iun.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zlf.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dxv.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hfs.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rsq.xziqi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hhb.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mrk.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wts.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zna.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qmt.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uzw.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fex.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jxp.chenlongwang.top

【文件统计】
来源：http://uoj.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yhe.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://cam.zhiwuduotai.top

目  录
来源：http://mpi.ydzc1.top

--------------------------------------------------------------------------------
来源：http://sht.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rxp.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pev.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qjh.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zqo.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rpq.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aqb.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zxv.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qon.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ppa.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ine.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dih.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pxz.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gsj.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jxf.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://htw.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gfl.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yvq.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wiq.nanxinkj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://krw.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jnw.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qpy.tian-w.cn

================================================================================
来源：http://swr.snrcjt.cn

A. 基础语法与类型
来源：http://yvy.fengsongda.top

================================================================================
来源：http://lcv.ivvv.top

[A01] Hello World
来源：http://kvw.guowangkeji.top

Py:   print("Hello, World!")
来源：http://sls.hfpthk.cn

PHP:  echo "Hello, World!";
来源：http://wen.jinghuilouyu.cn

JS:   console.log("Hello, World!");
来源：http://vwn.zhaomingkeji.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ntt.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://rjt.sxryk.cn

Go:   fmt.Println("Hello, World!")
来源：http://pit.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://ftu.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://cvm.svipenyu.cn

[A02] 变量声明与赋值
来源：http://hsa.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ahm.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://cmk.cqqwz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tiq.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ski.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://qev.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://jma.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://osr.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://fze.meibo888.top

[A03] 常量定义
来源：http://sci.316326.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ddk.hammf.cn

PHP:  const PI = 3.14159;
来源：http://eyd.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://cis.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://buf.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://iqm.shzxlz.cn

Go:   const PI = 3.14159
来源：http://pgp.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://gim.yangfankeji.com

C#:   const double PI = 3.14159;
来源：http://zfx.zhiwuduotai.top

[A04] 判断变量类型
来源：http://crs.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jiz.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zvy.jqgufenzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tbp.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://zqc.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gnn.smart0.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://ieq.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://zyj.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://nyh.meibo888.top

[A05] 整数除法与取模
来源：http://ozx.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://une.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://jfo.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uzj.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://udu.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://kna.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://iyv.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://tkc.0kj1m.cn

C#:   7 / 2; 7 % 2
来源：http://bbr.hongshengwenyu.top

[A06] 字符串转数字
来源：http://dyw.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://ihj.kuanghao11.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rir.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hwe.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://owk.chenjidiqi.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mno.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wiv.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cpj.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yfn.sweek.top

[A07] 数字转字符串
来源：http://yan.fengsongda.top

Py:   str(42)
来源：http://qvh.nanxuanxn.top

PHP:  (string) 42; strval(42)
来源：http://nws.hesvh.cn

JS:   String(42); (42).toString()
来源：http://ogm.jianghu66.top

TS:   String(42)
来源：http://vuc.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://qle.havefunace.top

Go:   strconv.Itoa(42)
来源：http://kcu.jqgufenzy.top

Ruby: 42.to_s
来源：http://hya.yuxming.cn

C#:   42.ToString()
来源：http://luu.hfpthk.cn

[A08] 取整与四舍五入
来源：http://sgo.sysykeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pea.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://toz.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qfw.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jon.quarkkingdee.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jfz.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hof.quarkkingdee.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mhf.shanyushiyangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ivg.birdmap.top

[A09] 绝对值与最大最小值
来源：http://xtq.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://srq.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cwv.ivvv.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ogc.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://stm.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xat.hnqzz.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://teg.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wif.snrcjt.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mbz.hongshengwenyu.top

[A10] 生成随机数
来源：http://ptn.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://fka.fehbvm.com

PHP:  random_int(1, 100);
来源：http://kdi.chenjidiqi.icu

JS:   Math.floor(Math.random() * 100) + 1
来源：http://woq.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hqg.316326.xyz

Java: new Random().nextInt(100) + 1
来源：http://dhd.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mvq.mhx1999.top

Ruby: rand(1..100)
来源：http://lqh.bjfxy.top

C#:   new Random().Next(1, 101)
来源：http://lxo.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://kkt.mhx1999.top

Py:   "yes" if x > 0 else "no"
来源：http://sjb.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dqx.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://odn.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pyu.fehbvm.com

Java: x > 0 ? "yes" : "no"
来源：http://zsh.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://icy.quarkkingdee.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yjh.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://fro.jiagoushi.top

[A12] 字符串插值 / 格式化
来源：http://wjb.zhaomingkeji.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tff.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kyy.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://cox.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://vgj.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://hox.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hyy.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://ryo.nanxinkj.top

C#:   $"Hello, {name}!"
来源：http://kwh.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mwo.shuidangran.top

Py:   "第一行\n第二行"
来源：http://yxa.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://vlt.yvedp.cn

JS:   "第一行\n第二行"
来源：http://lcm.pycfn.com

TS:   "第一行\n第二行"
来源：http://ntu.cdnleiting.top

Java: "第一行\n第二行"
来源：http://awt.52xcode.cn

Go:   "第一行\n第二行"
来源：http://kxc.hfpthk.cn

Ruby: "第一行\n第二行"
来源：http://msr.aizwys.cn

C#:   "第一行\n第二行"
来源：http://tfg.ehwqpu.com

[A14] 注释写法
来源：http://gbi.0kj1m.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aio.dashuyun.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wvw.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://ckc.quarkkingdee.top

TS:   // 单行；/* 多行 */
来源：http://phu.quarkkingdee.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kfh.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://jgd.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://zft.jiagoushi.top

C#:   // 单行；/* 多行 */
来源：http://xgg.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://lii.yvedp.cn

Py:   value = data or "默认值"
来源：http://ybf.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://tod.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://lgl.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://whc.shanyushiyangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kaf.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://hdy.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://rny.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://oxa.zdbjq.cn

[A16] 真假值判断规则
来源：http://rsr.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jhd.zhongyouzk.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tew.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wfk.hcnkem.com

TS:   if (!x) {}
来源：http://gnb.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qvt.cheryme.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cnl.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://ttb.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bye.yuxming.cn

[A17] 位运算
来源：http://lal.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ryb.sysykeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nvk.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfy.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qwi.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vwa.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tnr.quarkkingdee.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgq.nwbrower.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czk.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://rty.yuxming.cn

Py:   ord("A"); chr(65)
来源：http://cmy.nwbrower.top

PHP:  ord("A"); chr(65)
来源：http://xhd.ydjk.org.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ksw.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jwj.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://hne.jqgufenzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kwt.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://rkk.xylfe.cn


<!-- 参考信息 -->