代发 wailian999

[U99] JS：事件监听
来源：http://ove.uphjek.com

el.addEventListener("click", e => {})
来源：http://ocu.chenzaomai.com

[U100] JS：DOM 查询
来源：http://mam.bjfxy.top

document.querySelector(".item")
来源：http://izi.haohaochexian.top

[U101] JS：classList 操作
来源：http://plh.zdqjudy.top

el.classList.toggle("active")
来源：http://exd.wangshuangyany.cn

[U102] JS：本地存储
来源：http://ops.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zjs.jinqigfzy.top

[U103] JS：定时器
来源：http://dqx.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dng.xuanzx.com

[U104] JS：防抖
来源：http://lky.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpg.hnxiangtu.top

[U105] JS：节流
来源：http://skv.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aqu.yj20258888.top

[U106] JS：日期格式化
来源：http://phb.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oxt.xuanzx.com

[U107] JS：数字千分位
来源：http://hci.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kgp.yj202588.top

[U108] JS：随机整数
来源：http://rrf.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fqc.svipenyu.cn

[U109] JS：数组分组
来源：http://tcb.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://kal.gotoacloud.top

[U110] JS：数组分块
来源：http://rim.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ivh.wangdashe.top

[U111] JS：对象转 Map
来源：http://xbf.birdmap.top

new Map(Object.entries(obj))
来源：http://gtp.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://mck.yj20258888.top

"7".padStart(3, "0")
来源：http://lun.nanxinkj.top

[U113] JS：正则替换全部
来源：http://gjz.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://qsa.zycfv.cn

[U114] JS：JSON 深比较
来源：http://xdl.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kxc.xinyue.icu

[U115] JS：生成 UUID
来源：http://tpu.yanxiufei.cn

crypto.randomUUID()
来源：http://hdt.daria6918.cn

[U116] JS：类型检查（JSDoc）
来源：http://kvh.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://gji.sjlbkw.cn

[U117] JS：单元测试
来源：http://awb.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://iqr.yonumen.top

[U118] JS：开发服务器
来源：http://hwa.bbcook.cn

npm i -D vite;  npx vite
来源：http://wkt.nanxinkj.top

[U119] JS：生产构建
来源：http://dvy.jinqigfzy.top

npx vite build
来源：http://rnx.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://uur.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://djv.ehwqpu.com

================================================================================
来源：http://vxn.chenzaomai.com

统计汇总
来源：http://kxd.jianghu66.top

================================================================================
来源：http://mbh.cqqwz.cn

按语言统计（条）：
来源：http://xzw.yj202588.top

Python ......... 252
来源：http://hfd.quarkkingdee.top

PHP ............ 252
来源：http://eim.316326.xyz

JavaScript ..... 252
来源：http://agk.yonumen.top

TypeScript ..... 212
来源：http://cpp.fengsongda.top

Java ........... 212
来源：http://scs.nanxinkj.top

Go ............. 212
来源：http://rot.tarul.cn

Ruby ........... 212
来源：http://jkc.gzhubu.top

C# ............. 212
来源：http://nxn.pycfn.com

C .............. 30
来源：http://zpn.bjfxy.top

C++ ............ 30
来源：http://eiz.daria6918.cn

SQL ............ 90
来源：http://bji.gzhubu.top

Bash ........... 80
来源：http://flj.jqgfzy.top

Kotlin ......... 15
来源：http://axd.tianlin.xyz

Swift .......... 15
来源：http://nqv.cucudq.cn

Lua ............ 10
来源：http://dxp.havefunace.top

Perl ........... 10
来源：http://lpo.cucudq.cn

Scala .......... 10
来源：http://hzu.tanke756.top

------------------------------------
来源：http://jsr.sweek.top

合计 ........... 2106 条
来源：http://bbq.zhongyouzk.top

按章节统计：
来源：http://ilc.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oil.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nup.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ptn.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iry.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hoy.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fxy.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gta.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xco.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lep.gotoacloud.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dxz.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ixm.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tpr.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ykq.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lpe.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vyg.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aao.nanxinkj.top

Q SQL 专题                              90
来源：http://wha.ppjwa.cn

R Bash 专题                             80
来源：http://yxs.0kj1m.cn

S C / C++ 专题                          60
来源：http://gnv.aibaodan.cn

T 其他语言补充                          60
来源：http://gzj.yongpay.top

U 高频实用片段                         120
来源：http://gml.sxryk.cn

------------------------------------
来源：http://nnc.feifeiyinyue.top

合计                                  2106 条
来源：http://swk.hesvh.cn

--------------------------------------------------------------------------------
来源：http://egg.shzxlz.cn

使用提醒
来源：http://zxe.uphjek.com

--------------------------------------------------------------------------------
来源：http://rjb.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cff.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xps.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fzw.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vme.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://guc.fengsongda.top

—— 文件结束 ——
来源：http://sxj.gogol.net.cn

================================================================================
来源：http://jnf.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://yln.sjlbkw.cn

Common Programming Examples Cheat Book
来源：http://otf.gotoacloud.top

================================================================================
来源：http://ica.vqdsnc.cn

【收录内容】
来源：http://ari.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://byq.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fch.jinqigfzy.top

SQL · Bash · C · C++
来源：http://zsz.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lza.zdbjq.cn

【使用说明】
来源：http://grq.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rjt.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bfu.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vru.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qsx.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://boq.jinqigfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ehf.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://myw.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gzv.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mil.zhaomingkeji.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jdo.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oyc.tanke756.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dkw.uphjek.com

【文件统计】
来源：http://rtq.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yne.c1oappe.top

--------------------------------------------------------------------------------
来源：http://vyy.haohaochexian.top

目  录
来源：http://hyf.xuanzx.com

--------------------------------------------------------------------------------
来源：http://imy.zycfv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ema.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mgu.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wqb.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fqd.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fco.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qtj.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://moo.yuanzhike.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yaa.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jlh.ehwqpu.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wwu.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gac.gaohongyu789.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ajv.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ysk.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ras.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eoi.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sol.shzxlz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://taa.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cck.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ncx.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxe.gzhubu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gzl.zhixingplan.top

================================================================================
来源：http://utl.gaohongyu789.top

A. 基础语法与类型
来源：http://gid.ywan-chungtsiang.top

================================================================================
来源：http://klj.chenjidiqi.icu

[A01] Hello World
来源：http://zgr.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://djf.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://zca.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://mpb.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mgz.jinqigfzy.top

Java: System.out.println("Hello, World!");
来源：http://fhh.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://uiu.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://kvf.redwolf501.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ydc.guannengcc.top

[A02] 变量声明与赋值
来源：http://sgf.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://veh.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hzw.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://cwi.yuanzhike.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://flo.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://dwc.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://qko.gzhubu.top

Ruby: name = "Alex"; age = 20
来源：http://mio.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://emt.xinyue.icu

[A03] 常量定义
来源：http://wdl.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xlu.aibaodan.cn

PHP:  const PI = 3.14159;
来源：http://tfp.yongpay.top

JS:   const PI = 3.14159;
来源：http://yns.shangyingyoupin.top

TS:   const PI: number = 3.14159;
来源：http://vof.yj20258.top

Java: static final double PI = 3.14159;
来源：http://rez.xinyue.icu

Go:   const PI = 3.14159
来源：http://efs.dianchejie.cn

Ruby: PI = 3.14159
来源：http://mki.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://nhk.vehdjk.com

[A04] 判断变量类型
来源：http://ncu.gzhubu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bah.shanyushiyangtech.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fal.xuanzx.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dws.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://xiq.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dcg.ydzc1.top

Go:   reflect.TypeOf(x).Name()
来源：http://hdg.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rbj.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://pas.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://sex.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://afd.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://bin.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gaj.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kzb.pycfn.com

Java: 7 / 2; 7 % 2
来源：http://daj.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://sky.hongshengwenyu.top

Ruby: 7 / 2; 7 % 2
来源：http://qhc.birdmap.top

C#:   7 / 2; 7 % 2
来源：http://udm.yanxiufei.cn

[A06] 字符串转数字
来源：http://dcv.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://mbw.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tvd.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fxz.havefunace.top

TS:   parseInt("42", 10); Number("42")
来源：http://vhn.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://haq.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vly.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://agy.hcnkem.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kry.snrcjt.cn

[A07] 数字转字符串
来源：http://nxt.xziqi.cn

Py:   str(42)
来源：http://ngc.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://zfn.cheryme.top

JS:   String(42); (42).toString()
来源：http://nvn.xziqi.cn

TS:   String(42)
来源：http://szu.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://kfk.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://ywu.dianchejie.cn

Ruby: 42.to_s
来源：http://ngc.cucudq.cn

C#:   42.ToString()
来源：http://njb.hongshengwenyu.top

[A08] 取整与四舍五入
来源：http://ifs.hnqzz.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sgc.bbcook.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wit.52xcode.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oxc.shangyingyoupin.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nzd.hfpthk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vbb.fengsongda.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xoh.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bjj.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cfy.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://fpf.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://swi.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hyi.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dac.chenzaomai.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aza.hywenlv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rfx.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tmo.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uvw.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rzx.epnwcf.com

[A10] 生成随机数
来源：http://mjz.xinyue.icu

Py:   import random; random.randint(1, 100)
来源：http://evp.dianchejie.cn

PHP:  random_int(1, 100);
来源：http://oxy.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cbg.fzhhl.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lax.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://aea.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ajf.hammf.cn

Ruby: rand(1..100)
来源：http://kqr.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://xzl.zhiwuduotai.top

[A11] 条件表达式（三元）
来源：http://cae.xylfe.cn

Py:   "yes" if x > 0 else "no"
来源：http://lbg.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://keq.zycfv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qqd.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://eid.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://dgb.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lcb.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bcz.havefunace.top

C#:   x > 0 ? "yes" : "no"
来源：http://ujz.jianghu66.top

[A12] 字符串插值 / 格式化
来源：http://bgi.haohaochexian.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kfg.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jdg.cqqwz.cn

JS:   `Hello, ${name}!`
来源：http://apw.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://lmt.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://gam.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uxr.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://fqp.gotoacloud.top

C#:   $"Hello, {name}!"
来源：http://efp.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fsw.hammf.cn

Py:   "第一行\n第二行"
来源：http://mkz.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://bib.xinyue.icu

JS:   "第一行\n第二行"
来源：http://cvc.svipenyu.cn

TS:   "第一行\n第二行"
来源：http://bfr.gogol.net.cn

Java: "第一行\n第二行"
来源：http://vpo.jiagoushi.top

Go:   "第一行\n第二行"
来源：http://vsu.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://qdr.316326.xyz

C#:   "第一行\n第二行"
来源：http://mxa.aizwys.cn

[A14] 注释写法
来源：http://jyp.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tnq.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ltw.aizwys.cn

JS:   // 单行；/* 多行 */
来源：http://fwf.zhongyouzk.top

TS:   // 单行；/* 多行 */
来源：http://ure.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yfb.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://dyn.daria6918.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cad.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://hol.xinyue.icu

[A15] 空值判断与默认值
来源：http://sdb.hcnkem.com

Py:   value = data or "默认值"
来源：http://ema.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://wjd.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://yxr.c1oappe.top

TS:   const value = data ?? "默认值";
来源：http://tfy.wangdashe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ysy.nanxuanxn.top

Go:   if data == "" { data = "默认值" }
来源：http://ufo.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://dom.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://juh.316326.xyz

[A16] 真假值判断规则
来源：http://zev.pengpengdd.cyou

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bhd.hesvh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ejs.shangyingyoupin.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nsq.yuanzhike.top

TS:   if (!x) {}
来源：http://anb.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vhf.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://acb.316326.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://uki.sufxvd.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pdc.chenjidiqi.icu

[A17] 位运算
来源：http://ylx.nwbrower.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zbt.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mzw.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmn.hcnkem.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vin.xinyue.icu


<!-- 参考信息 -->