代发 wailian999

[U105] JS：节流
来源：http://vsf.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ena.nanxuanxn.top

[U106] JS：日期格式化
来源：http://tnk.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hug.ywan-chungtsiang.top

[U107] JS：数字千分位
来源：http://nfr.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nyh.shuidangran.top

[U108] JS：随机整数
来源：http://dcc.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dhd.gotoacloud.top

[U109] JS：数组分组
来源：http://hdw.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://jix.redwolf501.top

[U110] JS：数组分块
来源：http://jth.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ttv.vehdjk.com

[U111] JS：对象转 Map
来源：http://edy.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://bvm.yvedp.cn

[U112] JS：字符串补位
来源：http://ach.shzxlz.cn

"7".padStart(3, "0")
来源：http://uol.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://twq.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://nnb.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://tmw.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tbm.shuidangran.top

[U115] JS：生成 UUID
来源：http://bps.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://leh.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://cwq.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://khk.nanxinkj.top

[U117] JS：单元测试
来源：http://xqj.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://mlq.sufxvd.cn

[U118] JS：开发服务器
来源：http://xux.52xcode.cn

npm i -D vite;  npx vite
来源：http://gns.ywan-chungtsiang.top

[U119] JS：生产构建
来源：http://zgf.shanyushiyangkeji.top

npx vite build
来源：http://zir.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://jbk.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://vge.yvedp.cn

================================================================================
来源：http://rok.pycfn.com

统计汇总
来源：http://pet.yfazqb.com

================================================================================
来源：http://vlp.pycfn.com

按语言统计（条）：
来源：http://pdr.tianlin.xyz

Python ......... 252
来源：http://wte.hysaishi.cn

PHP ............ 252
来源：http://yuu.jinqigufen.top

JavaScript ..... 252
来源：http://xdc.52xcode.cn

TypeScript ..... 212
来源：http://trs.epnwcf.com

Java ........... 212
来源：http://ghb.wangdashe.top

Go ............. 212
来源：http://oxh.tianlin.xyz

Ruby ........... 212
来源：http://ins.svipenyu.cn

C# ............. 212
来源：http://uwu.hcnkem.com

C .............. 30
来源：http://ewe.zhaomingkeji.xyz

C++ ............ 30
来源：http://meb.ppjwa.cn

SQL ............ 90
来源：http://xpq.daria6918.cn

Bash ........... 80
来源：http://qpr.jinghuilouyu.cn

Kotlin ......... 15
来源：http://frv.hongshengwenyu.top

Swift .......... 15
来源：http://wma.pengpengdd.cyou

Lua ............ 10
来源：http://bca.hesvh.cn

Perl ........... 10
来源：http://wxx.gotoacloud.top

Scala .......... 10
来源：http://sgl.9152youxi.cn

------------------------------------
来源：http://hau.xuetiantiany.cn

合计 ........... 2106 条
来源：http://ywb.shuidangran.top

按章节统计：
来源：http://ibc.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xeb.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eol.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://okz.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wyy.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://usx.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://foi.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nus.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gog.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zzq.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gzt.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cdb.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mkr.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iyg.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mrg.jyoumei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tdz.xylfe.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvv.epnwcf.com

Q SQL 专题                              90
来源：http://wli.pengpengdd.cyou

R Bash 专题                             80
来源：http://dzp.ctjpmb.com

S C / C++ 专题                          60
来源：http://hus.nwbrower.top

T 其他语言补充                          60
来源：http://lrm.vehdjk.com

U 高频实用片段                         120
来源：http://ppa.ybcxt.top

------------------------------------
来源：http://evm.tanke756.top

合计                                  2106 条
来源：http://uul.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://szh.bjfxy.top

使用提醒
来源：http://bqn.shuidangran.top

--------------------------------------------------------------------------------
来源：http://ott.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hfb.ywan-chungtsiang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qyo.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nct.xuanzx.com

在旧版本上使用前请先确认语法支持情况。
来源：http://wup.aibaodan.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zvj.ydjk.org.cn

—— 文件结束 ——
来源：http://azn.ydjk.org.cn

================================================================================
来源：http://sim.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://grz.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://xhs.zycfv.cn

================================================================================
来源：http://ihh.316326.xyz

【收录内容】
来源：http://lmp.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ogo.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hxe.shzxlz.cn

SQL · Bash · C · C++
来源：http://ctb.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ajf.gzhubu.top

【使用说明】
来源：http://xry.chenzaomai.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vmo.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bki.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fqf.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kxk.9152youxi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://guw.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rio.cheryme.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fli.ybcxt.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vec.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wjy.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lyn.cheryme.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ncg.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://btv.jiagoushi.top

【文件统计】
来源：http://mse.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jae.epnwcf.com

--------------------------------------------------------------------------------
来源：http://ekg.ydzc1.top

目  录
来源：http://rpm.mhx1999.top

--------------------------------------------------------------------------------
来源：http://rwn.c1oappe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qmj.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://meq.shuidangran.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bmj.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yxi.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lhc.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dbu.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cnp.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xza.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lzb.cqqwz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fcu.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jci.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ydh.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sfc.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sfi.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zlq.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xck.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://phm.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lib.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rrp.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://njt.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wlm.guowangkeji.top

================================================================================
来源：http://nwj.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://heg.ydzc1.top

================================================================================
来源：http://nkb.ivvv.top

[A01] Hello World
来源：http://gvz.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://dqr.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://zwd.cdnleiting.top

JS:   console.log("Hello, World!");
来源：http://jpz.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eex.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://yyb.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://vif.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://ada.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kqx.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://xps.sjlbkw.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kmo.xylfe.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://orw.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kan.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ckw.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://kqj.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://gbq.zhoulong.xyz

Ruby: name = "Alex"; age = 20
来源：http://yht.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://myf.andypj.xyz

[A03] 常量定义
来源：http://jkg.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wmi.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://ual.hesvh.cn

JS:   const PI = 3.14159;
来源：http://fro.fengsongda.top

TS:   const PI: number = 3.14159;
来源：http://qim.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://smh.zycfv.cn

Go:   const PI = 3.14159
来源：http://rxy.quarkkingdee.top

Ruby: PI = 3.14159
来源：http://mnd.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://omn.ybcxt.top

[A04] 判断变量类型
来源：http://vqu.yuxming.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://act.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uya.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cfe.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://pgn.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kbz.zhengqikj.top

Go:   reflect.TypeOf(x).Name()
来源：http://mes.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rwz.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://ura.birdmap.top

[A05] 整数除法与取模
来源：http://tim.shuidangran.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kdt.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kad.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qyz.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zgt.yvedp.cn

Java: 7 / 2; 7 % 2
来源：http://bqo.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://suj.xuanzx.com

Ruby: 7 / 2; 7 % 2
来源：http://rmf.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://bwr.zhengqikj.top

[A06] 字符串转数字
来源：http://hex.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://oib.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lnq.yuxming.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vre.yanxiufei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zrm.chenzaomai.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aik.nwbrower.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wfw.jinqigufen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ggc.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uha.chenjidiqi.icu

[A07] 数字转字符串
来源：http://jnc.hnxiangtu.top

Py:   str(42)
来源：http://brb.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://swp.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://jkg.ehwqpu.com

TS:   String(42)
来源：http://yhp.jlsjyb.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bxk.yongpay.top

Go:   strconv.Itoa(42)
来源：http://mup.daxiang520.top

Ruby: 42.to_s
来源：http://chv.jinyuanbaomall.cn

C#:   42.ToString()
来源：http://kej.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://tny.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nnb.yangfankeji.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tkl.daria6918.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://axi.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dzx.redwolf501.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xzb.ppjwa.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eos.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://phz.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hyv.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://fmw.jqgufenzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://drr.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jhn.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://skc.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ftq.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jok.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lyz.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://svx.chenlongwang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zxz.epnwcf.com

[A10] 生成随机数
来源：http://qwy.chenjidiqi.icu

Py:   import random; random.randint(1, 100)
来源：http://gqv.fehbvm.com

PHP:  random_int(1, 100);
来源：http://ebs.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hku.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yff.jqgufenzy.top

Java: new Random().nextInt(100) + 1
来源：http://che.hysaishi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dyj.ywan-chungtsiang.top

Ruby: rand(1..100)
来源：http://qsy.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://ybj.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://ycb.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://fpn.fktsv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wij.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mbv.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://rcy.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://nfw.zhongyouzk.top

Go:   // 无三元运算符，需用 if 语句
来源：http://kuo.hesvh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fqn.aizwys.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ohi.kuanghao11.cn

[A12] 字符串插值 / 格式化
来源：http://iol.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://crw.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zxn.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://ufx.sufxvd.cn

TS:   `Hello, ${name}!`
来源：http://tli.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://mgl.shanyushiyangkeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://thz.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://fgt.zhoulong.xyz

C#:   $"Hello, {name}!"
来源：http://mlj.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://pub.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://hez.hnqzz.top

PHP:  "第一行\n第二行"
来源：http://voj.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://guh.sxryk.cn

TS:   "第一行\n第二行"
来源：http://fmv.aibaodan.cn

Java: "第一行\n第二行"
来源：http://dee.yuanzhike.top

Go:   "第一行\n第二行"
来源：http://evw.guowangkeji.top

Ruby: "第一行\n第二行"
来源：http://mtl.xziqi.cn

C#:   "第一行\n第二行"
来源：http://uxv.sweek.top

[A14] 注释写法
来源：http://vgs.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yfg.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mzr.xylfe.cn

JS:   // 单行；/* 多行 */
来源：http://hhy.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://hkf.guowangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wbb.sweek.top

Go:   // 单行；/* 多行 */
来源：http://txo.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://chb.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://ula.cheryme.top

[A15] 空值判断与默认值
来源：http://olr.xylfe.cn

Py:   value = data or "默认值"
来源：http://szw.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://fkb.sufxvd.cn

JS:   const value = data ?? "默认值";
来源：http://zem.redwolf501.top

TS:   const value = data ?? "默认值";
来源：http://wju.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vnf.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://whs.tian-w.cn

Ruby: value = data || "默认值"
来源：http://vdi.shuidangran.top

C#:   var value = data ?? "默认值";
来源：http://ont.hnqzz.top

[A16] 真假值判断规则
来源：http://iur.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xlc.yj20258.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://okm.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ajo.cqqwz.cn

TS:   if (!x) {}
来源：http://ink.pycfn.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lay.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jbl.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://khs.sufxvd.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rxx.sjlbkw.cn

[A17] 位运算
来源：http://rqr.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://but.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bzn.yangfankeji.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxj.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://utm.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://azu.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lvm.yfazqb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvp.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tkr.redwolf501.top

[A18] 字符与 ASCII 码互转
来源：http://cch.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://nmk.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://vbb.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bjj.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nfi.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://qvy.yj202588.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jyq.kuanghao11.cn

Ruby: "A".ord; 65.chr
来源：http://kzm.yfazqb.com


<!-- 参考信息 -->