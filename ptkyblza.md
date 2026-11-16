代发 wailian999

[U105] JS：节流
来源：http://kun.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hem.ivvv.top

[U106] JS：日期格式化
来源：http://fit.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bpa.sjlbkw.cn

[U107] JS：数字千分位
来源：http://omg.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kop.yuanzhike.top

[U108] JS：随机整数
来源：http://bbk.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lbi.yongpay.top

[U109] JS：数组分组
来源：http://ddh.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://swy.c1oappe.top

[U110] JS：数组分块
来源：http://lwz.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tvb.yj20258888.top

[U111] JS：对象转 Map
来源：http://pdt.cdnleiting.top

new Map(Object.entries(obj))
来源：http://fzj.xuanzx.com

[U112] JS：字符串补位
来源：http://kai.tarul.cn

"7".padStart(3, "0")
来源：http://snb.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://uwz.aibaodan.cn

s.replaceAll("a", "b")
来源：http://qnl.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://sqx.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cwn.daxiang520.top

[U115] JS：生成 UUID
来源：http://pyg.zhiwuduotai.top

crypto.randomUUID()
来源：http://ekp.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://ejs.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://gyq.fehbvm.com

[U117] JS：单元测试
来源：http://vzp.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://dxx.guowangkeji.top

[U118] JS：开发服务器
来源：http://zvk.ehwqpu.com

npm i -D vite;  npx vite
来源：http://cyp.smart0.xyz

[U119] JS：生产构建
来源：http://gyy.zhaomingkeji.xyz

npx vite build
来源：http://czg.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://iqs.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://qze.zhengqikj.top

================================================================================
来源：http://duc.jlsjyb.cn

统计汇总
来源：http://iku.svipenyu.cn

================================================================================
来源：http://zju.zdqjudy.top

按语言统计（条）：
来源：http://fse.bjfxy.top

Python ......... 252
来源：http://rom.yonumen.top

PHP ............ 252
来源：http://dcj.jqgfzy.top

JavaScript ..... 252
来源：http://zdt.xuetiantiany.cn

TypeScript ..... 212
来源：http://tgc.chenjidiqi.icu

Java ........... 212
来源：http://dcm.andypj.xyz

Go ............. 212
来源：http://zdm.yuxming.cn

Ruby ........... 212
来源：http://ggx.yuanzhike.top

C# ............. 212
来源：http://zwu.chenlongwang.top

C .............. 30
来源：http://hht.fehbvm.com

C++ ............ 30
来源：http://nqw.yj20258888.top

SQL ............ 90
来源：http://ogs.ydzc1.top

Bash ........... 80
来源：http://wta.yanxiufei.cn

Kotlin ......... 15
来源：http://gkn.hysaishi.cn

Swift .......... 15
来源：http://gxi.jqgfzy.top

Lua ............ 10
来源：http://guw.yj20258888.top

Perl ........... 10
来源：http://skb.wangdashe.top

Scala .......... 10
来源：http://cdl.jiagoushi.top

------------------------------------
来源：http://dyn.zhiwuduotai.top

合计 ........... 2106 条
来源：http://yyd.yuxming.cn

按章节统计：
来源：http://ezj.gogol.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mnb.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wjk.ivvv.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tuj.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gkf.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sea.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://opg.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ing.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lkr.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://adn.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bkv.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mwx.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://onj.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://psp.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cbq.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ydo.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vvj.aizwys.cn

Q SQL 专题                              90
来源：http://psk.xinyue.icu

R Bash 专题                             80
来源：http://ujt.yj20258.top

S C / C++ 专题                          60
来源：http://kdh.316326.xyz

T 其他语言补充                          60
来源：http://oii.yfazqb.com

U 高频实用片段                         120
来源：http://kxi.sweek.top

------------------------------------
来源：http://pja.shanyushiyangkeji.top

合计                                  2106 条
来源：http://cbh.yj20258888.top

--------------------------------------------------------------------------------
来源：http://bhv.dashuyun.cn

使用提醒
来源：http://gmi.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://mbj.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jte.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fxl.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://utm.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zkk.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mjt.0kj1m.cn

—— 文件结束 ——
来源：http://qnp.hesvh.cn

================================================================================
来源：http://zuq.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://zbm.sweek.top

Common Programming Examples Cheat Book
来源：http://cbe.iojbl.cn

================================================================================
来源：http://xqd.sxryk.cn

【收录内容】
来源：http://rsb.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mqn.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://puo.snrcjt.cn

SQL · Bash · C · C++
来源：http://tkf.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dal.jqgfzy.top

【使用说明】
来源：http://bea.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qev.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://anq.daxiang520.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wvg.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ygt.cdnleiting.top

Bash:  Shell         C:     C             C++:   C++
来源：http://avy.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zts.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bam.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ymr.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kea.ivvv.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ffe.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ojf.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qmi.0kj1m.cn

【文件统计】
来源：http://ysu.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fub.havefunace.top

--------------------------------------------------------------------------------
来源：http://yas.dianchejie.cn

目  录
来源：http://wtm.shuidangran.top

--------------------------------------------------------------------------------
来源：http://phq.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fdp.ppjwa.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://krx.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jis.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mtq.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gqi.ydzc1.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wnx.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://weo.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qfg.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rvq.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zwl.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sti.cdnleiting.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zbo.xuanzx.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oam.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zir.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bhs.jianghu66.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dfj.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://exb.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ifv.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nyy.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wnd.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wfk.zhixingplan.top

================================================================================
来源：http://vvj.mhx1999.top

A. 基础语法与类型
来源：http://fyg.wangshuangyany.cn

================================================================================
来源：http://aqy.ppjwa.cn

[A01] Hello World
来源：http://ssp.bjfxy.top

Py:   print("Hello, World!")
来源：http://bow.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://hsl.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://rbw.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://faz.guannengcc.top

Java: System.out.println("Hello, World!");
来源：http://yxa.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://kqf.yj202588.top

Ruby: puts "Hello, World!"
来源：http://xod.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://nrl.vehdjk.com

[A02] 变量声明与赋值
来源：http://akw.jianghu66.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vct.hesvh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xuh.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://sfk.hammf.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://crb.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://yqs.xziqi.cn

Go:   name := "Alex"; age := 20
来源：http://wiq.zhoulong.xyz

Ruby: name = "Alex"; age = 20
来源：http://yfp.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://pvb.yuxming.cn

[A03] 常量定义
来源：http://vkc.jinqigufen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zjt.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://ojg.bbcook.cn

JS:   const PI = 3.14159;
来源：http://szt.cheryme.top

TS:   const PI: number = 3.14159;
来源：http://wud.hywenlv.cn

Java: static final double PI = 3.14159;
来源：http://sbh.xziqi.cn

Go:   const PI = 3.14159
来源：http://ofq.vqdsnc.cn

Ruby: PI = 3.14159
来源：http://lzx.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://olf.hfpthk.cn

[A04] 判断变量类型
来源：http://frd.hnqzz.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lhm.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ltx.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eez.bbcook.cn

TS:   typeof x; x instanceof Date
来源：http://xyw.jinqigfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://adc.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://efg.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bbp.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://czd.cqqwz.cn

[A05] 整数除法与取模
来源：http://tdg.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qsh.aizwys.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gyq.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ulj.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://emu.zycfv.cn

Java: 7 / 2; 7 % 2
来源：http://qgz.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://yqp.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://xsp.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://kyg.jianghu66.top

[A06] 字符串转数字
来源：http://gzk.pycfn.com

Py:   int("42"); float("3.14")
来源：http://xhd.gaohongyu789.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pad.shanyushiyangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://axd.fehbvm.com

TS:   parseInt("42", 10); Number("42")
来源：http://jcu.xingfuxueyuan.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wul.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kip.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://plh.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bhg.aibaodan.cn

[A07] 数字转字符串
来源：http://jkp.fktsv.cn

Py:   str(42)
来源：http://sgo.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://nse.tarul.cn

JS:   String(42); (42).toString()
来源：http://txm.fanxiaobao.xyz

TS:   String(42)
来源：http://rou.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mot.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://okt.svipenyu.cn

Ruby: 42.to_s
来源：http://arq.c1oappe.top

C#:   42.ToString()
来源：http://cmi.yj202588.top

[A08] 取整与四舍五入
来源：http://fzg.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pii.zdqjudy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nxz.fengsongda.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://prz.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lue.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ftc.bbcook.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mjw.fanxiaobao.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://ifh.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bmp.xziqi.cn

[A09] 绝对值与最大最小值
来源：http://cha.gotoacloud.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dch.pengpengdd.cyou

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://apw.jianghu66.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tyt.xinyue.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yde.wangdashe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://aqi.c1oappe.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uyu.bjfxy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://otl.gaohongyu789.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jmz.zhoulong.xyz

[A10] 生成随机数
来源：http://kzl.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://lgu.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://kpn.pycfn.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wyq.chenjidiqi.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ueo.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://iqs.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://grf.bbcook.cn

Ruby: rand(1..100)
来源：http://iax.hammf.cn

C#:   new Random().Next(1, 101)
来源：http://ltl.yuanzhike.top

[A11] 条件表达式（三元）
来源：http://eqt.yfazqb.com

Py:   "yes" if x > 0 else "no"
来源：http://ihr.dashuyun.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ded.jinqigufen.top

JS:   x > 0 ? "yes" : "no"
来源：http://frs.daxiang520.top

TS:   x > 0 ? "yes" : "no"
来源：http://ahm.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://odc.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ufh.fktsv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pvi.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://lzn.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://izy.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://owm.nanxuanxn.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kjp.fengsongda.top

JS:   `Hello, ${name}!`
来源：http://xsf.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://qkm.shanyushiyangtech.top

Java: "Hello, %s!".formatted(name)
来源：http://wgp.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mbr.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://oku.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://via.cheryme.top

[A13] 多行字符串（练习 \n 转义）
来源：http://azt.mhx1999.top

Py:   "第一行\n第二行"
来源：http://rfg.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://six.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://uib.fengsongda.top

TS:   "第一行\n第二行"
来源：http://qzv.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://mvk.xingfuxueyuan.xyz

Go:   "第一行\n第二行"
来源：http://upi.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://uwm.pycfn.com

C#:   "第一行\n第二行"
来源：http://xtp.smart0.xyz

[A14] 注释写法
来源：http://fnp.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ewy.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://bxw.gogol.net.cn

JS:   // 单行；/* 多行 */
来源：http://qfa.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://min.redwolf501.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rcn.andypj.xyz

Go:   // 单行；/* 多行 */
来源：http://drx.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wkx.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://ldv.zdbjq.cn

[A15] 空值判断与默认值
来源：http://oot.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://nxk.fanxiaobao.xyz

PHP:  $value = $data ?? "默认值";
来源：http://sxe.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://jnb.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://xpz.yongpay.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hgb.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://ghu.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://lvn.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://rzd.xuanzx.com

[A16] 真假值判断规则
来源：http://gtv.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://aax.quarkkingdee.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mye.gzhubu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ztr.fzhhl.top

TS:   if (!x) {}
来源：http://xtg.hnqzz.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kku.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kle.zhiwuduotai.top

Ruby: unless x            # nil 与 false 为假
来源：http://rgh.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uye.hongshengwenyu.top

[A17] 位运算
来源：http://liu.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxm.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ydp.epnwcf.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://swt.vqdsnc.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wur.redwolf501.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://boj.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pew.jqgfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxm.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ris.kuanghao11.cn

[A18] 字符与 ASCII 码互转
来源：http://mrg.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://fdg.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://sdt.gotoacloud.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://spx.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dux.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://odw.xingfuxueyuan.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ddi.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://hhv.guowangkeji.top


<!-- 参考信息 -->