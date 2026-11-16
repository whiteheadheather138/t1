代发 wailian999

[U105] JS：节流
来源：http://xld.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gzg.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://zpp.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wgy.yvedp.cn

[U107] JS：数字千分位
来源：http://lkm.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qsm.jyoumei.cn

[U108] JS：随机整数
来源：http://qvr.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dkl.dashuyun.cn

[U109] JS：数组分组
来源：http://cuk.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://mhr.sjlbkw.cn

[U110] JS：数组分块
来源：http://vvb.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oom.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://iuf.zdqjudy.top

new Map(Object.entries(obj))
来源：http://kru.yfazqb.com

[U112] JS：字符串补位
来源：http://upm.sjlbkw.cn

"7".padStart(3, "0")
来源：http://pgk.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://inv.fengsongda.top

s.replaceAll("a", "b")
来源：http://mcb.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://sdz.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pon.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://zoj.xuetiantiany.cn

crypto.randomUUID()
来源：http://wkz.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://vfa.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://pqh.fktsv.cn

[U117] JS：单元测试
来源：http://goh.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://oaj.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://jqz.0kj1m.cn

npm i -D vite;  npx vite
来源：http://shg.feifeiyinyue.top

[U119] JS：生产构建
来源：http://pek.zhixingplan.top

npx vite build
来源：http://zxc.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://bol.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://pcm.chenzaomai.com

================================================================================
来源：http://nlw.hesvh.cn

统计汇总
来源：http://rbl.c1oappe.top

================================================================================
来源：http://xjs.vqdsnc.cn

按语言统计（条）：
来源：http://znv.gotoacloud.top

Python ......... 252
来源：http://qyk.hesvh.cn

PHP ............ 252
来源：http://uxh.zhixingplan.top

JavaScript ..... 252
来源：http://xaa.vehdjk.com

TypeScript ..... 212
来源：http://pzl.jinghuilouyu.cn

Java ........... 212
来源：http://lqs.fanxiaobao.xyz

Go ............. 212
来源：http://rhg.tarul.cn

Ruby ........... 212
来源：http://etx.dianchejie.cn

C# ............. 212
来源：http://iak.jqgfzy.top

C .............. 30
来源：http://grt.yongpay.top

C++ ............ 30
来源：http://yfj.chenlongwang.top

SQL ............ 90
来源：http://ofu.snrcjt.cn

Bash ........... 80
来源：http://rkz.havefunace.top

Kotlin ......... 15
来源：http://rgh.yonumen.top

Swift .......... 15
来源：http://tvj.shanyushiyangtech.top

Lua ............ 10
来源：http://zig.yj20258.top

Perl ........... 10
来源：http://gma.sysykeji.top

Scala .......... 10
来源：http://smg.feifeiyinyue.top

------------------------------------
来源：http://ict.cqqwz.cn

合计 ........... 2106 条
来源：http://lpg.cqqwz.cn

按章节统计：
来源：http://xcy.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nkv.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://umx.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nbd.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vcd.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tot.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kgs.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uxa.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zkv.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ylu.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yst.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://scn.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rqp.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yof.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mji.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ycu.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wrw.gogol.net.cn

Q SQL 专题                              90
来源：http://pgm.hysaishi.cn

R Bash 专题                             80
来源：http://doo.havefunace.top

S C / C++ 专题                          60
来源：http://bya.hnqzz.top

T 其他语言补充                          60
来源：http://igd.fanxiaobao.xyz

U 高频实用片段                         120
来源：http://mds.aibaodan.cn

------------------------------------
来源：http://yyu.nanxuanxn.top

合计                                  2106 条
来源：http://eib.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://njt.chenzaomai.com

使用提醒
来源：http://kxg.guannengcc.top

--------------------------------------------------------------------------------
来源：http://kzi.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iiz.iojbl.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hdi.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://snn.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cvo.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xza.cdnleiting.top

—— 文件结束 ——
来源：http://hdq.yj20258888.top

================================================================================
来源：http://kps.cdnleiting.top

程序语言常见例子速查手册（2024 版）
来源：http://ojc.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://brx.sweek.top

================================================================================
来源：http://pqa.sweek.top

【收录内容】
来源：http://npq.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://arr.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tvm.nanxinkj.top

SQL · Bash · C · C++
来源：http://lpx.andypj.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ofe.tian-w.cn

【使用说明】
来源：http://ewc.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ueg.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wqw.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vyh.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bay.wangdashe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hjg.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fff.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zoe.tian-w.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mag.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rjw.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nar.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tcr.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bga.yj20258.top

【文件统计】
来源：http://bue.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://exz.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://rnk.fzhhl.top

目  录
来源：http://cea.nwbrower.top

--------------------------------------------------------------------------------
来源：http://hza.zhiwuduotai.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://csi.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tmg.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xbc.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lsm.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bqt.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://okw.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lnv.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nlx.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wlm.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qnb.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fwv.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jli.jlsjyb.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cmk.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://imx.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eyj.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rgo.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://srh.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ndp.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qsy.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://apk.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wld.shangyingyoupin.top

================================================================================
来源：http://zpc.yongpay.top

A. 基础语法与类型
来源：http://uet.zhixingplan.top

================================================================================
来源：http://klp.wangdashe.top

[A01] Hello World
来源：http://knc.shuidangran.top

Py:   print("Hello, World!")
来源：http://ldv.zhengqikj.top

PHP:  echo "Hello, World!";
来源：http://lpw.yonumen.top

JS:   console.log("Hello, World!");
来源：http://nca.chenzaomai.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lhy.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://gij.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://vlo.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://ddv.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://bps.yfazqb.com

[A02] 变量声明与赋值
来源：http://khn.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ahm.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ahn.316326.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://inp.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gjv.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://fju.zhaomingkeji.xyz

Go:   name := "Alex"; age := 20
来源：http://has.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://jwz.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://isx.redwolf501.top

[A03] 常量定义
来源：http://jhu.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wui.tanke756.top

PHP:  const PI = 3.14159;
来源：http://fix.shuidangran.top

JS:   const PI = 3.14159;
来源：http://ngj.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://qjj.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://cdf.cheryme.top

Go:   const PI = 3.14159
来源：http://kxu.cashguo.top

Ruby: PI = 3.14159
来源：http://vtu.shanyushiyangkeji.top

C#:   const double PI = 3.14159;
来源：http://jcc.tian-w.cn

[A04] 判断变量类型
来源：http://sfy.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xql.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tps.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ugd.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://nnn.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hde.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://pza.yj20258888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kcj.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://gid.jianghu66.top

[A05] 整数除法与取模
来源：http://cxg.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vws.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fhe.jqgfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vhs.fktsv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ttx.fktsv.cn

Java: 7 / 2; 7 % 2
来源：http://zrt.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://wqb.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://wea.chenzaomai.com

C#:   7 / 2; 7 % 2
来源：http://lnx.52xcode.cn

[A06] 字符串转数字
来源：http://dus.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://twv.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://adi.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jlw.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://lzm.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ggq.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zhn.guowangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wha.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rju.havefunace.top

[A07] 数字转字符串
来源：http://vqb.zhixingplan.top

Py:   str(42)
来源：http://rrq.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://xip.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://mzu.bjfxy.top

TS:   String(42)
来源：http://bhw.xylfe.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gyr.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://syf.zhiwuduotai.top

Ruby: 42.to_s
来源：http://wes.bbcook.cn

C#:   42.ToString()
来源：http://ovn.yonumen.top

[A08] 取整与四舍五入
来源：http://erk.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qcm.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nqh.vehdjk.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mnc.xuanzx.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://obx.birdmap.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ygz.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://phk.hfpthk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gro.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gvp.uphjek.com

[A09] 绝对值与最大最小值
来源：http://osq.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dii.jqgfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://veo.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vjb.jinqigufen.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://quo.gzhubu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qrd.jinghuilouyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://avb.yongpay.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mvf.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ikg.bjfxy.top

[A10] 生成随机数
来源：http://hku.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://xum.zhaomingkeji.xyz

PHP:  random_int(1, 100);
来源：http://vxg.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pki.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qii.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://cjr.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ccl.bjfxy.top

Ruby: rand(1..100)
来源：http://lqr.sweek.top

C#:   new Random().Next(1, 101)
来源：http://xhl.ehwqpu.com

[A11] 条件表达式（三元）
来源：http://teu.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://zao.pycfn.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://cnb.jqgufenzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://wek.ybcxt.top

TS:   x > 0 ? "yes" : "no"
来源：http://hug.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://xgw.zhoulong.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://bjr.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://fmx.dashuyun.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wts.fzhhl.top

[A12] 字符串插值 / 格式化
来源：http://kkl.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nvi.yuxming.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hew.sufxvd.cn

JS:   `Hello, ${name}!`
来源：http://aqt.xylfe.cn

TS:   `Hello, ${name}!`
来源：http://lyw.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://tec.chenjidiqi.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nni.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://mvd.zdqjudy.top

C#:   $"Hello, {name}!"
来源：http://zxh.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iio.gogol.net.cn

Py:   "第一行\n第二行"
来源：http://ppe.sweek.top

PHP:  "第一行\n第二行"
来源：http://adl.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://dsa.fanxiaobao.xyz

TS:   "第一行\n第二行"
来源：http://ipx.zhoulong.xyz

Java: "第一行\n第二行"
来源：http://ymw.aizwys.cn

Go:   "第一行\n第二行"
来源：http://czk.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://edn.mhx1999.top

C#:   "第一行\n第二行"
来源：http://rvh.jinqigufen.top

[A14] 注释写法
来源：http://pge.yfazqb.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://wak.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pma.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://ghw.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://dnn.cashguo.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ike.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://faf.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vcj.tianlin.xyz

C#:   // 单行；/* 多行 */
来源：http://jws.cheryme.top

[A15] 空值判断与默认值
来源：http://vsk.ehwqpu.com

Py:   value = data or "默认值"
来源：http://hsz.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://bdz.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://bcv.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://mjz.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kue.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://sut.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://jdw.vqdsnc.cn

C#:   var value = data ?? "默认值";
来源：http://fue.cheryme.top

[A16] 真假值判断规则
来源：http://ntw.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dce.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dzy.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://crm.meibo888.top

TS:   if (!x) {}
来源：http://djg.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hoa.zhiwuduotai.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://elr.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://biz.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jmy.yuanzhike.top

[A17] 位运算
来源：http://zkr.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fcu.mhx1999.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://arq.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxy.fzhhl.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vfm.jianghu66.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hef.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://icf.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hkj.xylfe.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aba.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://dei.daxiang520.top

Py:   ord("A"); chr(65)
来源：http://tca.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://oge.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xcu.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ety.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://abl.shanyushiyangtech.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ivv.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://luo.pycfn.com


<!-- 参考信息 -->