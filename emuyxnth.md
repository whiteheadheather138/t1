代发 wailian999

[U101] JS：classList 操作
来源：http://rer.sweek.top

el.classList.toggle("active")
来源：http://txv.yj20258.top

[U102] JS：本地存储
来源：http://xag.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ulj.aizwys.cn

[U103] JS：定时器
来源：http://rsa.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gwv.daria6918.cn

[U104] JS：防抖
来源：http://akv.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpr.yangfankeji.com

[U105] JS：节流
来源：http://vof.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kit.xuanzx.com

[U106] JS：日期格式化
来源：http://xyd.aibaodan.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wby.gaohongyu789.top

[U107] JS：数字千分位
来源：http://smo.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nri.9152youxi.cn

[U108] JS：随机整数
来源：http://ujt.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wty.tanke756.top

[U109] JS：数组分组
来源：http://noo.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://xik.hysaishi.cn

[U110] JS：数组分块
来源：http://rdw.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://exa.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://hxa.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://yes.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://tqr.nanxuanxn.top

"7".padStart(3, "0")
来源：http://out.hesvh.cn

[U113] JS：正则替换全部
来源：http://ysu.tianlin.xyz

s.replaceAll("a", "b")
来源：http://gfs.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://pvx.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zqa.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://thx.zhoulong.xyz

crypto.randomUUID()
来源：http://pil.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://tdj.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://nut.hfpthk.cn

[U117] JS：单元测试
来源：http://vnk.0kj1m.cn

npm i -D vitest;  npx vitest
来源：http://pad.pycfn.com

[U118] JS：开发服务器
来源：http://nao.zycfv.cn

npm i -D vite;  npx vite
来源：http://ruo.hesvh.cn

[U119] JS：生产构建
来源：http://rox.kuanghao11.cn

npx vite build
来源：http://bng.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://muj.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://mqm.jqgfzy.top

================================================================================
来源：http://cjj.ppjwa.cn

统计汇总
来源：http://eok.ctjpmb.com

================================================================================
来源：http://dfm.fengsongda.top

按语言统计（条）：
来源：http://wmm.ctjpmb.com

Python ......... 252
来源：http://mrh.zhengqikj.top

PHP ............ 252
来源：http://fyz.ppjwa.cn

JavaScript ..... 252
来源：http://bia.aizwys.cn

TypeScript ..... 212
来源：http://ehl.cashguo.top

Java ........... 212
来源：http://fme.smart0.xyz

Go ............. 212
来源：http://gfs.yfazqb.com

Ruby ........... 212
来源：http://hva.vehdjk.com

C# ............. 212
来源：http://otp.cashguo.top

C .............. 30
来源：http://ymd.zhijiandao.cn

C++ ............ 30
来源：http://jju.redwolf501.top

SQL ............ 90
来源：http://bjl.ywan-chungtsiang.top

Bash ........... 80
来源：http://fmo.yj202588.top

Kotlin ......... 15
来源：http://tiw.hywenlv.cn

Swift .......... 15
来源：http://yyt.0kj1m.cn

Lua ............ 10
来源：http://yeh.fanxiaobao.xyz

Perl ........... 10
来源：http://lmb.quarkkingdee.top

Scala .......... 10
来源：http://okk.vehdjk.com

------------------------------------
来源：http://lxr.nwbrower.top

合计 ........... 2106 条
来源：http://erl.ehwqpu.com

按章节统计：
来源：http://csg.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://srb.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pux.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kgm.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://adr.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hcn.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lxd.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jfm.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oka.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vik.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zox.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kks.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gin.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dtt.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uxk.c1oappe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gwe.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hss.feifeiyinyue.top

Q SQL 专题                              90
来源：http://jkn.yangfankeji.com

R Bash 专题                             80
来源：http://edz.guowangkeji.top

S C / C++ 专题                          60
来源：http://soc.jlsjyb.cn

T 其他语言补充                          60
来源：http://koa.yongpay.top

U 高频实用片段                         120
来源：http://krv.yvedp.cn

------------------------------------
来源：http://kkt.yuxming.cn

合计                                  2106 条
来源：http://hsg.uphjek.com

--------------------------------------------------------------------------------
来源：http://qnn.mhx1999.top

使用提醒
来源：http://rhh.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ffp.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qqo.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fmd.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mid.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xwn.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dph.daria6918.cn

—— 文件结束 ——
来源：http://eid.nanxuanxn.top

================================================================================
来源：http://sua.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://rwt.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://wwo.hysaishi.cn

================================================================================
来源：http://cfy.jinqigufen.top

【收录内容】
来源：http://gyz.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gfu.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vmz.iojbl.cn

SQL · Bash · C · C++
来源：http://sxf.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vrh.sjlbkw.cn

【使用说明】
来源：http://stq.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://abh.redwolf501.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fpw.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://krs.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bea.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eyp.mhx1999.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cds.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mlr.xziqi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://leb.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://euh.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rha.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uth.sxryk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gsf.bjfxy.top

【文件统计】
来源：http://cce.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://goj.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://lpj.svipenyu.cn

目  录
来源：http://aho.ybcxt.top

--------------------------------------------------------------------------------
来源：http://bhx.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ojh.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://htw.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ssz.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zcm.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kvh.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sgr.yanxiufei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uey.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://frc.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bnn.hesvh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jrd.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wmr.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ryy.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://snp.andypj.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fcd.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oer.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qiw.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uaz.hfpthk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://utq.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tfd.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://etg.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wvm.yuxming.cn

================================================================================
来源：http://vor.daxiang520.top

A. 基础语法与类型
来源：http://cgk.bjfxy.top

================================================================================
来源：http://fst.nanxinkj.top

[A01] Hello World
来源：http://kpy.svipenyu.cn

Py:   print("Hello, World!")
来源：http://cax.pycfn.com

PHP:  echo "Hello, World!";
来源：http://zye.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://pjw.bjfxy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://icg.jinqigufen.top

Java: System.out.println("Hello, World!");
来源：http://lcz.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://ego.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://rrx.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://liw.fehbvm.com

[A02] 变量声明与赋值
来源：http://oqu.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://arz.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://bsh.tanke756.top

JS:   let name = "Alex"; const age = 20;
来源：http://ecl.guowangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://brt.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://bzi.ctjpmb.com

Go:   name := "Alex"; age := 20
来源：http://oxq.cucudq.cn

Ruby: name = "Alex"; age = 20
来源：http://ulb.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://egz.bjfxy.top

[A03] 常量定义
来源：http://ucv.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yrl.tianlin.xyz

PHP:  const PI = 3.14159;
来源：http://akt.yueranfly.top

JS:   const PI = 3.14159;
来源：http://zin.ywan-chungtsiang.top

TS:   const PI: number = 3.14159;
来源：http://gns.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://zzt.guannengcc.top

Go:   const PI = 3.14159
来源：http://dau.bjfxy.top

Ruby: PI = 3.14159
来源：http://bsl.guannengcc.top

C#:   const double PI = 3.14159;
来源：http://tyw.sysykeji.top

[A04] 判断变量类型
来源：http://hrj.sweek.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vok.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://otz.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://osg.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://uiw.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://stp.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mwp.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://bfj.hfpthk.cn

C#:   x.GetType().Name; x is int
来源：http://pcc.xuanzx.com

[A05] 整数除法与取模
来源：http://lbs.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pty.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uno.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eyt.aizwys.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mdz.ivvv.top

Java: 7 / 2; 7 % 2
来源：http://kar.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://glg.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://tre.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://lxc.zhixingplan.top

[A06] 字符串转数字
来源：http://hri.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://xvd.jinqigfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qwh.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wip.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://kqn.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kjh.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://seq.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://haz.havefunace.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uaz.yonumen.top

[A07] 数字转字符串
来源：http://mma.jyoumei.cn

Py:   str(42)
来源：http://vpg.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://bei.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://lzb.ppjwa.cn

TS:   String(42)
来源：http://iyg.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://akc.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://sjw.sjlbkw.cn

Ruby: 42.to_s
来源：http://jhs.smart0.xyz

C#:   42.ToString()
来源：http://dww.sysykeji.top

[A08] 取整与四舍五入
来源：http://rgy.wangdashe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vvu.tarul.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mqu.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://msd.bbcook.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kxu.xinyue.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rcu.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jtl.ydzc1.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xya.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ytl.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://nta.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cjf.zhoulong.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://emp.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fae.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sin.shanyushiyangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kld.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qnz.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://glx.fktsv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gfn.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://wxk.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://tjl.fengsongda.top

PHP:  random_int(1, 100);
来源：http://ftr.zhijiandao.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ccz.0kj1m.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://plf.jinghuilouyu.cn

Java: new Random().nextInt(100) + 1
来源：http://gxr.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://idx.andypj.xyz

Ruby: rand(1..100)
来源：http://osr.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://azz.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://xtw.ywan-chungtsiang.top

Py:   "yes" if x > 0 else "no"
来源：http://oxu.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://zvr.jinyuanbaomall.cn

JS:   x > 0 ? "yes" : "no"
来源：http://prf.zhaomingkeji.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://sbn.haohaochexian.top

Java: x > 0 ? "yes" : "no"
来源：http://jjv.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://onp.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vgx.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://okb.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://jsl.yj20258888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://exc.birdmap.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hal.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://xdj.jlsjyb.cn

TS:   `Hello, ${name}!`
来源：http://ohs.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://kow.jinqigfzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tjb.havefunace.top

Ruby: "Hello, #{name}!"
来源：http://pdn.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://gfb.quarkkingdee.top

[A13] 多行字符串（练习 \n 转义）
来源：http://mjd.yueranfly.top

Py:   "第一行\n第二行"
来源：http://dpj.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://dlj.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://yus.vehdjk.com

TS:   "第一行\n第二行"
来源：http://dwy.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://xfx.birdmap.top

Go:   "第一行\n第二行"
来源：http://luk.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://bsw.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://zlo.wangshuangyany.cn

[A14] 注释写法
来源：http://uft.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gbe.aizwys.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ase.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://lwl.shuidangran.top

TS:   // 单行；/* 多行 */
来源：http://fnf.xingfuxueyuan.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dxm.tanke756.top

Go:   // 单行；/* 多行 */
来源：http://sef.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fzo.yuanzhike.top

C#:   // 单行；/* 多行 */
来源：http://dtk.redwolf501.top

[A15] 空值判断与默认值
来源：http://amv.zdqjudy.top

Py:   value = data or "默认值"
来源：http://smt.cashguo.top

PHP:  $value = $data ?? "默认值";
来源：http://mtt.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://ijn.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://ous.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wya.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://ofj.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://jkz.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://gvp.tanke756.top

[A16] 真假值判断规则
来源：http://bmo.ivvv.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vvy.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://flu.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ktt.yfazqb.com

TS:   if (!x) {}
来源：http://ikl.aizwys.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wfh.sysykeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nmw.sxryk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yzc.redwolf501.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ekm.zhiwuduotai.top

[A17] 位运算
来源：http://jrw.hfpthk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wck.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://evx.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kup.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ixv.tarul.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xnj.iojbl.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yur.dianchejie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xuq.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tbd.hnxiangtu.top


<!-- 参考信息 -->