代发 wailian999

[U105] JS：节流
来源：http://wjj.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://drx.svipenyu.cn

[U106] JS：日期格式化
来源：http://zaj.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lwt.yonumen.top

[U107] JS：数字千分位
来源：http://oin.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ymx.hongshengwenyu.top

[U108] JS：随机整数
来源：http://hde.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xcb.zdqjudy.top

[U109] JS：数组分组
来源：http://apq.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://rji.316326.xyz

[U110] JS：数组分块
来源：http://hqk.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lnx.redwolf501.top

[U111] JS：对象转 Map
来源：http://ovh.daxiang520.top

new Map(Object.entries(obj))
来源：http://aum.guannengcc.top

[U112] JS：字符串补位
来源：http://ivv.zycfv.cn

"7".padStart(3, "0")
来源：http://gvj.zhixingplan.top

[U113] JS：正则替换全部
来源：http://cih.nanxinkj.top

s.replaceAll("a", "b")
来源：http://hcr.fehbvm.com

[U114] JS：JSON 深比较
来源：http://spy.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ruf.jyoumei.cn

[U115] JS：生成 UUID
来源：http://ogi.svipenyu.cn

crypto.randomUUID()
来源：http://cvh.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://dew.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://ypr.chenlongwang.top

[U117] JS：单元测试
来源：http://ovh.ivvv.top

npm i -D vitest;  npx vitest
来源：http://fcn.guowangkeji.top

[U118] JS：开发服务器
来源：http://ayl.yuxming.cn

npm i -D vite;  npx vite
来源：http://dsj.guannengcc.top

[U119] JS：生产构建
来源：http://gig.zdbjq.cn

npx vite build
来源：http://psz.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://kbw.316326.xyz

import.meta.env.VITE_API_URL
来源：http://xhn.daria6918.cn

================================================================================
来源：http://ghy.c1oappe.top

统计汇总
来源：http://ceh.yonumen.top

================================================================================
来源：http://zeb.yangfankeji.com

按语言统计（条）：
来源：http://rbg.ybcxt.top

Python ......... 252
来源：http://fhz.ywan-chungtsiang.top

PHP ............ 252
来源：http://jbh.yj20258.top

JavaScript ..... 252
来源：http://qej.jyoumei.cn

TypeScript ..... 212
来源：http://iww.dashuyun.cn

Java ........... 212
来源：http://ahu.zhengqikj.top

Go ............. 212
来源：http://hwy.smart0.xyz

Ruby ........... 212
来源：http://ukx.bjfxy.top

C# ............. 212
来源：http://oxk.sysykeji.top

C .............. 30
来源：http://exa.sjlbkw.cn

C++ ............ 30
来源：http://fdf.yueranfly.top

SQL ............ 90
来源：http://tmp.gogol.net.cn

Bash ........... 80
来源：http://xkt.52xcode.cn

Kotlin ......... 15
来源：http://voi.iojbl.cn

Swift .......... 15
来源：http://kif.yfazqb.com

Lua ............ 10
来源：http://lhd.cqqwz.cn

Perl ........... 10
来源：http://ivl.bjfxy.top

Scala .......... 10
来源：http://rtk.yongpay.top

------------------------------------
来源：http://mhi.zdbjq.cn

合计 ........... 2106 条
来源：http://xhn.ppjwa.cn

按章节统计：
来源：http://jpo.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://skt.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aye.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hcm.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hkg.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ude.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ryh.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zvd.jinqigufen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wtl.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xwq.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bay.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://agm.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lbv.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pvs.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dlu.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dzq.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qlr.yangfankeji.com

Q SQL 专题                              90
来源：http://rae.nanxinkj.top

R Bash 专题                             80
来源：http://vcf.jqgfzy.top

S C / C++ 专题                          60
来源：http://mkz.pengpengdd.cyou

T 其他语言补充                          60
来源：http://bow.ydjk.org.cn

U 高频实用片段                         120
来源：http://zxu.mhx1999.top

------------------------------------
来源：http://vfb.hesvh.cn

合计                                  2106 条
来源：http://bxv.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://ssl.yuanzhike.top

使用提醒
来源：http://cfg.cheryme.top

--------------------------------------------------------------------------------
来源：http://uzd.pycfn.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://twi.sxryk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xtm.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yad.havefunace.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ijf.aizwys.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pvq.yueranfly.top

—— 文件结束 ——
来源：http://euw.vehdjk.com

================================================================================
来源：http://odd.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://xzf.yj20258888.top

Common Programming Examples Cheat Book
来源：http://qqt.c1oappe.top

================================================================================
来源：http://xfo.pengpengdd.cyou

【收录内容】
来源：http://jja.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vuc.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pqd.fengsongda.top

SQL · Bash · C · C++
来源：http://uhg.c1oappe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://buw.aizwys.cn

【使用说明】
来源：http://cdo.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tym.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ama.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mov.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://flq.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rxu.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fpg.bbcook.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zdy.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xoy.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fiz.shanyushiyangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vxs.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oqi.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lih.chenjidiqi.icu

【文件统计】
来源：http://ydo.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nzg.xylfe.cn

--------------------------------------------------------------------------------
来源：http://drb.yj20258.top

目  录
来源：http://ibr.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://bpm.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://byh.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://asj.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wae.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yby.shuidangran.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oho.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://etw.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jgm.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cda.gaohongyu789.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qii.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bmn.cheryme.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ras.jinqigfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://axn.yuxming.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zfa.gzhubu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zng.hfpthk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fne.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://srx.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jsp.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://jbq.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ypj.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vqs.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tyz.c1oappe.top

================================================================================
来源：http://mud.birdmap.top

A. 基础语法与类型
来源：http://zwe.jinyuanbaomall.cn

================================================================================
来源：http://zpn.9152youxi.cn

[A01] Hello World
来源：http://knz.guowangkeji.top

Py:   print("Hello, World!")
来源：http://aai.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://pfa.zdqjudy.top

JS:   console.log("Hello, World!");
来源：http://vfo.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zkw.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://cci.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://otc.svipenyu.cn

Ruby: puts "Hello, World!"
来源：http://aqk.shangyingyoupin.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xls.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://adl.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fli.zdbjq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nmk.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://jls.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jjq.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://umb.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://yyx.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://zfv.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://uaa.hywenlv.cn

[A03] 常量定义
来源：http://uod.svipenyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fqu.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://ljp.xylfe.cn

JS:   const PI = 3.14159;
来源：http://xpf.hywenlv.cn

TS:   const PI: number = 3.14159;
来源：http://pnr.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://mgl.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://jpl.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://vow.jqgfzy.top

C#:   const double PI = 3.14159;
来源：http://luv.hcnkem.com

[A04] 判断变量类型
来源：http://djf.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yuj.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dyy.ywan-chungtsiang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ybu.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://umk.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zsz.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://ncz.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ptv.yangfankeji.com

C#:   x.GetType().Name; x is int
来源：http://mpj.ybcxt.top

[A05] 整数除法与取模
来源：http://tat.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jmr.jqgfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://fln.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tlu.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sic.ppjwa.cn

Java: 7 / 2; 7 % 2
来源：http://ijv.gaohongyu789.top

Go:   7 / 2; 7 % 2
来源：http://czl.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://jst.hywenlv.cn

C#:   7 / 2; 7 % 2
来源：http://vrl.nanxuanxn.top

[A06] 字符串转数字
来源：http://aui.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://ouy.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eir.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rdo.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://ozu.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mab.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xvg.zhixingplan.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vrk.jinqigfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dds.zycfv.cn

[A07] 数字转字符串
来源：http://dii.yanxiufei.cn

Py:   str(42)
来源：http://vuo.sweek.top

PHP:  (string) 42; strval(42)
来源：http://zwm.gzhubu.top

JS:   String(42); (42).toString()
来源：http://grd.meibo888.top

TS:   String(42)
来源：http://lli.shzxlz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pjc.iojbl.cn

Go:   strconv.Itoa(42)
来源：http://pau.uphjek.com

Ruby: 42.to_s
来源：http://dtk.bjfxy.top

C#:   42.ToString()
来源：http://iry.gzhubu.top

[A08] 取整与四舍五入
来源：http://gfq.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://spv.smart0.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jse.sxryk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://szq.zdbjq.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ias.iojbl.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vfw.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eoa.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qeh.sxryk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mgc.ydzc1.top

[A09] 绝对值与最大最小值
来源：http://fpz.jiagoushi.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ndp.fanxiaobao.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yta.wangshuangyany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ybp.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://chc.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ktg.bbcook.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ris.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nzo.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qor.hcnkem.com

[A10] 生成随机数
来源：http://ypd.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://tzf.yvedp.cn

PHP:  random_int(1, 100);
来源：http://jra.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cob.feifeiyinyue.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wwz.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://wny.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qii.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://fqo.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://faw.yongpay.top

[A11] 条件表达式（三元）
来源：http://ynf.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://asg.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ruo.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://fhh.hnqzz.top

TS:   x > 0 ? "yes" : "no"
来源：http://knu.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://cgu.hnxiangtu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gwq.epnwcf.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ork.chenjidiqi.icu

C#:   x > 0 ? "yes" : "no"
来源：http://qtg.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://yuu.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hnm.jinyuanbaomall.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jnx.zhiwuduotai.top

JS:   `Hello, ${name}!`
来源：http://aeq.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://nkb.hnqzz.top

Java: "Hello, %s!".formatted(name)
来源：http://xah.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zfw.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://hpe.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://kyp.yuxming.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mff.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://uyz.snrcjt.cn

PHP:  "第一行\n第二行"
来源：http://gbl.zhongyouzk.top

JS:   "第一行\n第二行"
来源：http://iov.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://mkl.sufxvd.cn

Java: "第一行\n第二行"
来源：http://pjd.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://hja.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://wyl.cucudq.cn

C#:   "第一行\n第二行"
来源：http://kvw.ctjpmb.com

[A14] 注释写法
来源：http://eds.aizwys.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mrp.cucudq.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://syq.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://rkb.smart0.xyz

TS:   // 单行；/* 多行 */
来源：http://siy.fktsv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ngz.zhengqikj.top

Go:   // 单行；/* 多行 */
来源：http://zqo.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yvv.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://tha.hfpthk.cn

[A15] 空值判断与默认值
来源：http://vyl.daxiang520.top

Py:   value = data or "默认值"
来源：http://vur.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://hcm.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://ccb.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://kqj.ehwqpu.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yqb.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://xli.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://sfk.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://xwd.dashuyun.cn

[A16] 真假值判断规则
来源：http://deo.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ohp.shuidangran.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iwv.yangfankeji.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yej.zdqjudy.top

TS:   if (!x) {}
来源：http://zvh.cdnleiting.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://poz.jyoumei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fzt.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pdv.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ykm.xuanzx.com

[A17] 位运算
来源：http://jbd.smart0.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gom.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jxz.yfazqb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sjl.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xbh.zhongyouzk.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://btk.vqdsnc.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pec.chenzaomai.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rdk.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bpm.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://idl.zhaomingkeji.xyz

Py:   ord("A"); chr(65)
来源：http://zts.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://iky.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ygm.ywan-chungtsiang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ecs.yfazqb.com

Java: (int) 'A'; (char) 65
来源：http://lmt.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vxd.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://jlf.smart0.xyz


<!-- 参考信息 -->