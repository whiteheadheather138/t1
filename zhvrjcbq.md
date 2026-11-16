代发 wailian999

[U101] JS：classList 操作
来源：http://ghk.meibo888.top

el.classList.toggle("active")
来源：http://wkw.bbcook.cn

[U102] JS：本地存储
来源：http://lha.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vbt.gzhubu.top

[U103] JS：定时器
来源：http://vdj.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://awf.yj202588.top

[U104] JS：防抖
来源：http://nnn.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sbq.zhixingplan.top

[U105] JS：节流
来源：http://mwk.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dfp.shzxlz.cn

[U106] JS：日期格式化
来源：http://nlo.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bhc.jyoumei.cn

[U107] JS：数字千分位
来源：http://nae.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nbb.zhongyouzk.top

[U108] JS：随机整数
来源：http://noh.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nrk.xuetiantiany.cn

[U109] JS：数组分组
来源：http://zpj.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://thy.wangshuangyany.cn

[U110] JS：数组分块
来源：http://hpc.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zso.birdmap.top

[U111] JS：对象转 Map
来源：http://kbu.daria6918.cn

new Map(Object.entries(obj))
来源：http://nts.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://wnr.zycfv.cn

"7".padStart(3, "0")
来源：http://yrr.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://oho.c1oappe.top

s.replaceAll("a", "b")
来源：http://rxk.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://ocp.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jlw.jyoumei.cn

[U115] JS：生成 UUID
来源：http://bgc.sweek.top

crypto.randomUUID()
来源：http://gaj.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://yhn.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://jea.hongshengwenyu.top

[U117] JS：单元测试
来源：http://rws.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://tks.pycfn.com

[U118] JS：开发服务器
来源：http://qfb.tianlin.xyz

npm i -D vite;  npx vite
来源：http://coj.zhijiandao.cn

[U119] JS：生产构建
来源：http://beb.guannengcc.top

npx vite build
来源：http://gjl.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://jjg.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://pqi.jyoumei.cn

================================================================================
来源：http://qlx.uphjek.com

统计汇总
来源：http://uoq.zdbjq.cn

================================================================================
来源：http://vih.yanxiufei.cn

按语言统计（条）：
来源：http://mck.shuidangran.top

Python ......... 252
来源：http://tyu.iojbl.cn

PHP ............ 252
来源：http://tcy.yj20258.top

JavaScript ..... 252
来源：http://xrk.mhx1999.top

TypeScript ..... 212
来源：http://chp.gzhubu.top

Java ........... 212
来源：http://nmx.dashuyun.cn

Go ............. 212
来源：http://rtk.xylfe.cn

Ruby ........... 212
来源：http://fuk.pycfn.com

C# ............. 212
来源：http://rzx.sweek.top

C .............. 30
来源：http://avk.zhiwuduotai.top

C++ ............ 30
来源：http://drt.fktsv.cn

SQL ............ 90
来源：http://egj.shanyushiyangkeji.top

Bash ........... 80
来源：http://ouw.ehwqpu.com

Kotlin ......... 15
来源：http://ave.ppjwa.cn

Swift .......... 15
来源：http://khn.sjlbkw.cn

Lua ............ 10
来源：http://oub.iojbl.cn

Perl ........... 10
来源：http://knz.yfazqb.com

Scala .......... 10
来源：http://oim.vehdjk.com

------------------------------------
来源：http://seh.smart0.xyz

合计 ........... 2106 条
来源：http://lbj.yuxming.cn

按章节统计：
来源：http://hpt.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fnn.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rgc.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tqv.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://llo.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ybc.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rdn.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ech.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qfw.fengsongda.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oor.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fsw.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xfw.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ctn.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rzc.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jcw.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://avc.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wrh.yuxming.cn

Q SQL 专题                              90
来源：http://kbm.xylfe.cn

R Bash 专题                             80
来源：http://nzv.zdbjq.cn

S C / C++ 专题                          60
来源：http://gjc.ctjpmb.com

T 其他语言补充                          60
来源：http://nge.vehdjk.com

U 高频实用片段                         120
来源：http://shq.pycfn.com

------------------------------------
来源：http://cfj.sufxvd.cn

合计                                  2106 条
来源：http://vyt.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://eow.nwbrower.top

使用提醒
来源：http://hur.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://qvr.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hwa.yuxming.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vmq.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bns.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vkl.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cwt.wangdashe.top

—— 文件结束 ——
来源：http://xfp.xuetiantiany.cn

================================================================================
来源：http://iph.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://zoh.52xcode.cn

Common Programming Examples Cheat Book
来源：http://syc.guowangkeji.top

================================================================================
来源：http://mmm.gzhubu.top

【收录内容】
来源：http://fpq.ehwqpu.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://mvm.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://awk.quarkkingdee.top

SQL · Bash · C · C++
来源：http://wog.sysykeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jig.nanxuanxn.top

【使用说明】
来源：http://bvg.kuanghao11.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wxz.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xyi.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oqb.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yne.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://avq.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://flk.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vxo.haohaochexian.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xba.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nho.yj20258.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rqo.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tqb.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ios.zycfv.cn

【文件统计】
来源：http://eua.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qyl.guannengcc.top

--------------------------------------------------------------------------------
来源：http://mra.yj20258.top

目  录
来源：http://gzj.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://wgj.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yid.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tub.hnxiangtu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xfd.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wah.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yyk.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xhd.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iqu.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lhn.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pvv.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gjh.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://trh.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cxr.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://isr.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kbq.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cwa.jqgfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qyz.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qyw.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sfi.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ziy.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://quv.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jel.cqqwz.cn

================================================================================
来源：http://hhr.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://mwr.aibaodan.cn

================================================================================
来源：http://edc.jqgufenzy.top

[A01] Hello World
来源：http://nxn.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://qlr.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://yqf.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://fuw.shanyushiyangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bvu.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://gqk.fehbvm.com

Go:   fmt.Println("Hello, World!")
来源：http://wzh.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://jzb.birdmap.top

C#:   Console.WriteLine("Hello, World!");
来源：http://unp.tian-w.cn

[A02] 变量声明与赋值
来源：http://oyo.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://job.guowangkeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://exf.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://dfq.yangfankeji.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ido.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://aqj.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://muf.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://wsx.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fwy.gotoacloud.top

[A03] 常量定义
来源：http://jur.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oym.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://onc.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://zvp.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://tuw.yfazqb.com

Java: static final double PI = 3.14159;
来源：http://udp.yuanzhike.top

Go:   const PI = 3.14159
来源：http://ziq.tarul.cn

Ruby: PI = 3.14159
来源：http://zje.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://hcg.jqgfzy.top

[A04] 判断变量类型
来源：http://kxw.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tib.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iet.sjlbkw.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jto.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://obk.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eop.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://wdd.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sdb.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://udl.redwolf501.top

[A05] 整数除法与取模
来源：http://ngt.0kj1m.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ill.ehwqpu.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://voi.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ckd.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://raw.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://qqt.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://olh.tarul.cn

Ruby: 7 / 2; 7 % 2
来源：http://smd.iojbl.cn

C#:   7 / 2; 7 % 2
来源：http://fzt.dashuyun.cn

[A06] 字符串转数字
来源：http://lzu.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://msj.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qdl.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gxl.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://zhb.aibaodan.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://euc.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wcb.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uql.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jpx.yanxiufei.cn

[A07] 数字转字符串
来源：http://zqe.nwbrower.top

Py:   str(42)
来源：http://hoj.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://hsi.fehbvm.com

JS:   String(42); (42).toString()
来源：http://zxf.feifeiyinyue.top

TS:   String(42)
来源：http://kzv.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://dni.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://wxm.gotoacloud.top

Ruby: 42.to_s
来源：http://uvh.mhx1999.top

C#:   42.ToString()
来源：http://frd.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://wxx.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wbo.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uou.zhiwuduotai.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zbx.smart0.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ayl.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lrp.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jax.gaohongyu789.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ist.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rsc.cucudq.cn

[A09] 绝对值与最大最小值
来源：http://dri.meibo888.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xvx.gotoacloud.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gmo.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xyc.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jpv.dianchejie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kug.sufxvd.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cmj.yuanzhike.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jcx.birdmap.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dth.havefunace.top

[A10] 生成随机数
来源：http://inw.52xcode.cn

Py:   import random; random.randint(1, 100)
来源：http://rcb.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://qcm.fktsv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xfo.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dak.wangdashe.top

Java: new Random().nextInt(100) + 1
来源：http://llx.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hyt.hnxiangtu.top

Ruby: rand(1..100)
来源：http://yyz.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://uyb.hnqzz.top

[A11] 条件表达式（三元）
来源：http://wro.zycfv.cn

Py:   "yes" if x > 0 else "no"
来源：http://pjj.zhongyouzk.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wiy.guannengcc.top

JS:   x > 0 ? "yes" : "no"
来源：http://yms.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://wjp.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://sny.pycfn.com

Go:   // 无三元运算符，需用 if 语句
来源：http://gxl.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pdn.mhx1999.top

C#:   x > 0 ? "yes" : "no"
来源：http://ond.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://kdo.hnqzz.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vvy.zhoulong.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://msg.shzxlz.cn

JS:   `Hello, ${name}!`
来源：http://yyp.zhixingplan.top

TS:   `Hello, ${name}!`
来源：http://zuq.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://hfo.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kry.nanxinkj.top

Ruby: "Hello, #{name}!"
来源：http://gca.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://jyf.jiagoushi.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dco.daria6918.cn

Py:   "第一行\n第二行"
来源：http://une.hfpthk.cn

PHP:  "第一行\n第二行"
来源：http://uhz.daxiang520.top

JS:   "第一行\n第二行"
来源：http://zoq.fzhhl.top

TS:   "第一行\n第二行"
来源：http://fwv.c1oappe.top

Java: "第一行\n第二行"
来源：http://jes.jinqigufen.top

Go:   "第一行\n第二行"
来源：http://ibv.jinyuanbaomall.cn

Ruby: "第一行\n第二行"
来源：http://acp.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://moz.yvedp.cn

[A14] 注释写法
来源：http://phj.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gpi.tianlin.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://ifz.wangshuangyany.cn

JS:   // 单行；/* 多行 */
来源：http://ylx.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://ied.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aav.wangdashe.top

Go:   // 单行；/* 多行 */
来源：http://myn.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cie.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://fox.nanxuanxn.top

[A15] 空值判断与默认值
来源：http://ryc.birdmap.top

Py:   value = data or "默认值"
来源：http://xjw.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://orn.epnwcf.com

JS:   const value = data ?? "默认值";
来源：http://qyn.chenzaomai.com

TS:   const value = data ?? "默认值";
来源：http://oue.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jpn.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://wka.hnqzz.top

Ruby: value = data || "默认值"
来源：http://dal.gogol.net.cn

C#:   var value = data ?? "默认值";
来源：http://jlb.yj20258.top

[A16] 真假值判断规则
来源：http://nal.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kbp.andypj.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://who.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qpc.jqgufenzy.top

TS:   if (!x) {}
来源：http://tha.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ute.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lnm.shuidangran.top

Ruby: unless x            # nil 与 false 为假
来源：http://xrc.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sax.vqdsnc.cn

[A17] 位运算
来源：http://cqr.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrw.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wmb.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gur.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rbc.tanke756.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcx.shanyushiyangtech.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kss.shanyushiyangtech.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iov.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wtm.meibo888.top


<!-- 参考信息 -->