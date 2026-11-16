代发 wailian999

[U99] JS：事件监听
来源：http://nry.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://llz.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://klr.snrcjt.cn

document.querySelector(".item")
来源：http://nik.sysykeji.top

[U101] JS：classList 操作
来源：http://wvr.pycfn.com

el.classList.toggle("active")
来源：http://urq.9152youxi.cn

[U102] JS：本地存储
来源：http://vjz.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bnc.ydjk.org.cn

[U103] JS：定时器
来源：http://qkq.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xnm.yanxiufei.cn

[U104] JS：防抖
来源：http://lkj.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ded.316326.xyz

[U105] JS：节流
来源：http://xpr.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bgv.zdbjq.cn

[U106] JS：日期格式化
来源：http://oyk.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qbw.cdnleiting.top

[U107] JS：数字千分位
来源：http://kjq.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://olg.quarkkingdee.top

[U108] JS：随机整数
来源：http://quk.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tyd.hnqzz.top

[U109] JS：数组分组
来源：http://ezv.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://rqw.9152youxi.cn

[U110] JS：数组分块
来源：http://irw.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cqk.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://thg.ydzc1.top

new Map(Object.entries(obj))
来源：http://kvk.guannengcc.top

[U112] JS：字符串补位
来源：http://zkz.zdqjudy.top

"7".padStart(3, "0")
来源：http://euv.yuxming.cn

[U113] JS：正则替换全部
来源：http://yns.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://lec.yvedp.cn

[U114] JS：JSON 深比较
来源：http://spq.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vyb.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://eps.uphjek.com

crypto.randomUUID()
来源：http://vxa.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://nzg.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://hoh.xziqi.cn

[U117] JS：单元测试
来源：http://jjz.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://orh.hywenlv.cn

[U118] JS：开发服务器
来源：http://iuy.sysykeji.top

npm i -D vite;  npx vite
来源：http://bpf.sweek.top

[U119] JS：生产构建
来源：http://gsu.hnqzz.top

npx vite build
来源：http://udo.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://uuj.yj202588.top

import.meta.env.VITE_API_URL
来源：http://stq.bbcook.cn

================================================================================
来源：http://hzi.svipenyu.cn

统计汇总
来源：http://sje.yonumen.top

================================================================================
来源：http://fbj.smart0.xyz

按语言统计（条）：
来源：http://zie.jinqigfzy.top

Python ......... 252
来源：http://xut.iojbl.cn

PHP ............ 252
来源：http://jtq.zhengqikj.top

JavaScript ..... 252
来源：http://rgw.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://sry.bbcook.cn

Java ........... 212
来源：http://kyg.bbcook.cn

Go ............. 212
来源：http://ycz.vehdjk.com

Ruby ........... 212
来源：http://jvv.yvedp.cn

C# ............. 212
来源：http://nzl.dashuyun.cn

C .............. 30
来源：http://xtc.gotoacloud.top

C++ ............ 30
来源：http://ejs.hammf.cn

SQL ............ 90
来源：http://mpw.fktsv.cn

Bash ........... 80
来源：http://egw.xuetiantiany.cn

Kotlin ......... 15
来源：http://wny.xuanzx.com

Swift .......... 15
来源：http://ujx.yonumen.top

Lua ............ 10
来源：http://djr.dianchejie.cn

Perl ........... 10
来源：http://hbn.hywenlv.cn

Scala .......... 10
来源：http://cpy.hesvh.cn

------------------------------------
来源：http://azq.yj202588.top

合计 ........... 2106 条
来源：http://kjs.zdbjq.cn

按章节统计：
来源：http://agc.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nzk.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uqn.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://boi.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bru.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yzz.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kch.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ppl.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kto.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wbt.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cog.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yij.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tmq.sysykeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uqh.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hca.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gjm.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dln.jqgufenzy.top

Q SQL 专题                              90
来源：http://irw.aibaodan.cn

R Bash 专题                             80
来源：http://jje.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://nle.yuanzhike.top

T 其他语言补充                          60
来源：http://dpn.aizwys.cn

U 高频实用片段                         120
来源：http://ons.316326.xyz

------------------------------------
来源：http://xgw.zhiwuduotai.top

合计                                  2106 条
来源：http://php.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://gkp.ydjk.org.cn

使用提醒
来源：http://ple.shuidangran.top

--------------------------------------------------------------------------------
来源：http://fqt.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nao.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://omp.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fon.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://btk.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rpa.zhengqikj.top

—— 文件结束 ——
来源：http://nev.daxiang520.top

================================================================================
来源：http://xtm.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://tjf.52xcode.cn

Common Programming Examples Cheat Book
来源：http://oku.smart0.xyz

================================================================================
来源：http://mao.hywenlv.cn

【收录内容】
来源：http://sbh.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://msr.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pbz.zycfv.cn

SQL · Bash · C · C++
来源：http://kvv.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wvy.bjfxy.top

【使用说明】
来源：http://cah.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aeq.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gzd.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zmd.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://epj.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kqv.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vsf.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blx.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nxd.yj20258888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qnj.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ijn.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lcj.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dxl.aibaodan.cn

【文件统计】
来源：http://ozk.andypj.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jyu.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://bmo.birdmap.top

目  录
来源：http://psn.xylfe.cn

--------------------------------------------------------------------------------
来源：http://ywg.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://idn.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uaj.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qqo.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rtb.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jks.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://usi.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cot.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kjx.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nlz.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rkh.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ckm.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cbf.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://apr.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://caa.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lpf.zhiwuduotai.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pax.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qjg.nanxinkj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zqs.jinqigufen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qhy.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ibg.guowangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yqu.ctjpmb.com

================================================================================
来源：http://ayx.cqqwz.cn

A. 基础语法与类型
来源：http://akc.dianchejie.cn

================================================================================
来源：http://kif.andypj.xyz

[A01] Hello World
来源：http://taj.chenzaomai.com

Py:   print("Hello, World!")
来源：http://dmb.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://gch.ctjpmb.com

JS:   console.log("Hello, World!");
来源：http://zly.ppjwa.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://deg.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://lxh.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://zvo.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://cdy.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fge.52xcode.cn

[A02] 变量声明与赋值
来源：http://spb.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ozc.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ftq.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://qfi.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ofa.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://yre.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://njz.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://mdv.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://wqu.cucudq.cn

[A03] 常量定义
来源：http://xzu.ydzc1.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cpo.hongshengwenyu.top

PHP:  const PI = 3.14159;
来源：http://jhy.haohaochexian.top

JS:   const PI = 3.14159;
来源：http://pfd.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://mgu.jinghuilouyu.cn

Java: static final double PI = 3.14159;
来源：http://xtn.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://ses.iojbl.cn

Ruby: PI = 3.14159
来源：http://fbn.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://pyi.yuxming.cn

[A04] 判断变量类型
来源：http://axk.ivvv.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tnl.zhiwuduotai.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://njf.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nui.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://ifx.kuanghao11.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fcc.chenjidiqi.icu

Go:   reflect.TypeOf(x).Name()
来源：http://xvw.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yux.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://kdi.bbcook.cn

[A05] 整数除法与取模
来源：http://egx.fzhhl.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wnn.zhengqikj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://kvc.jianghu66.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jvc.shzxlz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wuo.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://lvz.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://exr.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://rmb.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://vlc.jlsjyb.cn

[A06] 字符串转数字
来源：http://ooe.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://kig.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ixb.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iqc.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://voq.iojbl.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pbc.ctjpmb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yme.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vql.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bxb.yueranfly.top

[A07] 数字转字符串
来源：http://ksd.nanxinkj.top

Py:   str(42)
来源：http://lni.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://naz.ybcxt.top

JS:   String(42); (42).toString()
来源：http://gwe.jianghu66.top

TS:   String(42)
来源：http://bed.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zai.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://buj.cheryme.top

Ruby: 42.to_s
来源：http://quv.smart0.xyz

C#:   42.ToString()
来源：http://slc.gogol.net.cn

[A08] 取整与四舍五入
来源：http://hro.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ror.yonumen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oeu.ehwqpu.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qun.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wcd.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wzo.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lid.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jxi.aibaodan.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://aps.bjfxy.top

[A09] 绝对值与最大最小值
来源：http://ebi.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://boo.xuanzx.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qpi.hcnkem.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://quk.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gav.bbcook.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lxy.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nes.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hsn.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kfd.yangfankeji.com

[A10] 生成随机数
来源：http://yeu.zycfv.cn

Py:   import random; random.randint(1, 100)
来源：http://isx.jinqigfzy.top

PHP:  random_int(1, 100);
来源：http://oym.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jdn.yueranfly.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ifi.shuidangran.top

Java: new Random().nextInt(100) + 1
来源：http://hve.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tct.zycfv.cn

Ruby: rand(1..100)
来源：http://bbj.yuanzhike.top

C#:   new Random().Next(1, 101)
来源：http://fzf.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://kif.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://yvv.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zgj.9152youxi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eqy.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://muv.jyoumei.cn

Java: x > 0 ? "yes" : "no"
来源：http://kzw.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vmr.zycfv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zqi.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://tlu.9152youxi.cn

[A12] 字符串插值 / 格式化
来源：http://usq.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://njx.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eei.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://sxi.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://gcg.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://lpe.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://scp.dianchejie.cn

Ruby: "Hello, #{name}!"
来源：http://ake.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://ddq.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gwf.nanxuanxn.top

Py:   "第一行\n第二行"
来源：http://hbw.shanyushiyangtech.top

PHP:  "第一行\n第二行"
来源：http://olk.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://wby.wangshuangyany.cn

TS:   "第一行\n第二行"
来源：http://jrv.nanxuanxn.top

Java: "第一行\n第二行"
来源：http://uyr.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://jfe.yj20258.top

Ruby: "第一行\n第二行"
来源：http://ayt.pycfn.com

C#:   "第一行\n第二行"
来源：http://zou.birdmap.top

[A14] 注释写法
来源：http://qvn.smart0.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://znl.cqqwz.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mmp.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://axu.smart0.xyz

TS:   // 单行；/* 多行 */
来源：http://ymf.xylfe.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ytf.cheryme.top

Go:   // 单行；/* 多行 */
来源：http://rdp.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tzn.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://gid.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://vjn.cqqwz.cn

Py:   value = data or "默认值"
来源：http://ust.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://fza.uphjek.com

JS:   const value = data ?? "默认值";
来源：http://ewt.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://rhe.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zzz.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://fab.yongpay.top

Ruby: value = data || "默认值"
来源：http://crm.hcnkem.com

C#:   var value = data ?? "默认值";
来源：http://khr.jyoumei.cn

[A16] 真假值判断规则
来源：http://xky.xinyue.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bmt.vqdsnc.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cvz.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pgv.vehdjk.com

TS:   if (!x) {}
来源：http://ckg.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hyw.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gvg.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://nwy.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bts.yj20258.top

[A17] 位运算
来源：http://pml.yj20258888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmo.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jdw.cashguo.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://itz.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wrb.0kj1m.cn


<!-- 参考信息 -->