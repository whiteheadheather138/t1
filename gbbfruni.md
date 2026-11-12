代发 wailian999

[U99] JS：事件监听
来源：http://ofd.316326.xyz

el.addEventListener("click", e => {})
来源：http://ryd.pycfn.com

[U100] JS：DOM 查询
来源：http://zkm.cdnleiting.top

document.querySelector(".item")
来源：http://hjk.nanxinkj.top

[U101] JS：classList 操作
来源：http://bkb.tianlin.xyz

el.classList.toggle("active")
来源：http://qlx.yuanzhike.top

[U102] JS：本地存储
来源：http://goa.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cxd.chenlongwang.top

[U103] JS：定时器
来源：http://doj.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zaq.ydzc1.top

[U104] JS：防抖
来源：http://pse.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://myx.redwolf501.top

[U105] JS：节流
来源：http://zxn.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tqq.yvedp.cn

[U106] JS：日期格式化
来源：http://uwh.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://orm.andypj.xyz

[U107] JS：数字千分位
来源：http://hos.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qdu.vqdsnc.cn

[U108] JS：随机整数
来源：http://kvm.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://klt.havefunace.top

[U109] JS：数组分组
来源：http://rqa.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://uex.chenzaomai.com

[U110] JS：数组分块
来源：http://iue.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yus.gzhubu.top

[U111] JS：对象转 Map
来源：http://xmh.yuanzhike.top

new Map(Object.entries(obj))
来源：http://ukn.sysykeji.top

[U112] JS：字符串补位
来源：http://acm.svipenyu.cn

"7".padStart(3, "0")
来源：http://xoj.fengsongda.top

[U113] JS：正则替换全部
来源：http://iyi.xinyue.icu

s.replaceAll("a", "b")
来源：http://zpd.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://mxb.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uns.316326.xyz

[U115] JS：生成 UUID
来源：http://fmn.jianghu66.top

crypto.randomUUID()
来源：http://hph.sweek.top

[U116] JS：类型检查（JSDoc）
来源：http://duw.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://ewh.yonumen.top

[U117] JS：单元测试
来源：http://wpp.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://cvb.sysykeji.top

[U118] JS：开发服务器
来源：http://mgm.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://tls.jlsjyb.cn

[U119] JS：生产构建
来源：http://iyo.ivvv.top

npx vite build
来源：http://jot.0kj1m.cn

[U120] JS：读取环境变量（Vite）
来源：http://tjf.cashguo.top

import.meta.env.VITE_API_URL
来源：http://vkr.0kj1m.cn

================================================================================
来源：http://jux.pycfn.com

统计汇总
来源：http://ezy.ybcxt.top

================================================================================
来源：http://wpo.zhengqikj.top

按语言统计（条）：
来源：http://kmu.jinyuanbaomall.cn

Python ......... 252
来源：http://jwi.jiagoushi.top

PHP ............ 252
来源：http://oav.xylfe.cn

JavaScript ..... 252
来源：http://ahl.ybcxt.top

TypeScript ..... 212
来源：http://jxw.jiagoushi.top

Java ........... 212
来源：http://ina.hesvh.cn

Go ............. 212
来源：http://jue.zdqjudy.top

Ruby ........... 212
来源：http://tgn.wangshuangyany.cn

C# ............. 212
来源：http://qsv.9152youxi.cn

C .............. 30
来源：http://zyd.shuidangran.top

C++ ............ 30
来源：http://pnp.ydzc1.top

SQL ............ 90
来源：http://meq.c1oappe.top

Bash ........... 80
来源：http://gji.fengsongda.top

Kotlin ......... 15
来源：http://zjw.yfazqb.com

Swift .......... 15
来源：http://jni.sufxvd.cn

Lua ............ 10
来源：http://acm.zycfv.cn

Perl ........... 10
来源：http://jqw.gogol.net.cn

Scala .......... 10
来源：http://sit.jlsjyb.cn

------------------------------------
来源：http://vnl.chenzaomai.com

合计 ........... 2106 条
来源：http://tig.cqqwz.cn

按章节统计：
来源：http://sfh.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uyu.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cjw.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nwm.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wzb.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vdf.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xzb.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lvv.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kmd.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dfu.dianchejie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://weu.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://flg.hywenlv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vhf.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://njd.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wov.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vkn.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://csv.guannengcc.top

Q SQL 专题                              90
来源：http://ecg.0kj1m.cn

R Bash 专题                             80
来源：http://fnl.meibo888.top

S C / C++ 专题                          60
来源：http://zjc.yonumen.top

T 其他语言补充                          60
来源：http://oen.iojbl.cn

U 高频实用片段                         120
来源：http://ccv.mhx1999.top

------------------------------------
来源：http://xgl.jinghuilouyu.cn

合计                                  2106 条
来源：http://apn.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://dhl.quarkkingdee.top

使用提醒
来源：http://mao.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://xqk.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hxy.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wab.hcnkem.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fkt.shanyushiyangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wrj.hcnkem.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nxa.52xcode.cn

—— 文件结束 ——
来源：http://rcd.redwolf501.top

================================================================================
来源：http://onh.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://brb.sysykeji.top

Common Programming Examples Cheat Book
来源：http://ehb.vqdsnc.cn

================================================================================
来源：http://nmy.jinqigufen.top

【收录内容】
来源：http://ciq.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jbx.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jxf.gaohongyu789.top

SQL · Bash · C · C++
来源：http://gnw.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mtb.yj20258.top

【使用说明】
来源：http://njg.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mgi.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hfp.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://abn.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://irx.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ohy.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bdw.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://frc.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bdh.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://avi.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gmd.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zua.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vuc.yongpay.top

【文件统计】
来源：http://hlz.shangyingyoupin.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://erx.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://rgd.shzxlz.cn

目  录
来源：http://gem.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://end.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rfy.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://huh.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sxi.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jbi.52xcode.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cny.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jnl.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vqj.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://png.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kzv.sjlbkw.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jzl.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cgq.9152youxi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bdn.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ttr.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ylp.sjlbkw.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mge.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://crj.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wzy.zhaomingkeji.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://eqy.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://btu.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sff.ydzc1.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://biw.jinyuanbaomall.cn

================================================================================
来源：http://mwq.gzhubu.top

A. 基础语法与类型
来源：http://atm.pengpengdd.cyou

================================================================================
来源：http://lzk.tanke756.top

[A01] Hello World
来源：http://kxz.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://zlj.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://ckg.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://qzz.bjfxy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://spk.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://ixh.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://hdl.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://rbh.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zow.kuanghao11.cn

[A02] 变量声明与赋值
来源：http://lyw.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://waj.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mes.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://dem.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mgb.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://jjw.sweek.top

Go:   name := "Alex"; age := 20
来源：http://vwp.hfpthk.cn

Ruby: name = "Alex"; age = 20
来源：http://rcj.sweek.top

C#:   string name = "Alex"; int age = 20;
来源：http://snk.wangdashe.top

[A03] 常量定义
来源：http://tln.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mjf.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://lue.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://mcq.sweek.top

TS:   const PI: number = 3.14159;
来源：http://fiu.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://xqr.yonumen.top

Go:   const PI = 3.14159
来源：http://xxw.yfazqb.com

Ruby: PI = 3.14159
来源：http://hob.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://oex.tian-w.cn

[A04] 判断变量类型
来源：http://pos.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://umr.jinyuanbaomall.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://erc.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nfd.yj20258888.top

TS:   typeof x; x instanceof Date
来源：http://adk.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zby.zhaomingkeji.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://ncv.hysaishi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xbi.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://gle.cashguo.top

[A05] 整数除法与取模
来源：http://xlb.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fvo.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://man.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.yonumen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bvz.aibaodan.cn

Java: 7 / 2; 7 % 2
来源：http://rxz.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://khp.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://gxx.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://scn.kuanghao11.cn

[A06] 字符串转数字
来源：http://ngl.zhixingplan.top

Py:   int("42"); float("3.14")
来源：http://pby.snrcjt.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://idt.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nkb.zhiwuduotai.top

TS:   parseInt("42", 10); Number("42")
来源：http://zwb.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tta.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vwh.jqgfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kza.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tmf.chenzaomai.com

[A07] 数字转字符串
来源：http://hnx.yuxming.cn

Py:   str(42)
来源：http://oyr.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://pvy.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://sjo.pengpengdd.cyou

TS:   String(42)
来源：http://jal.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vfp.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://yej.pycfn.com

Ruby: 42.to_s
来源：http://ggv.yongpay.top

C#:   42.ToString()
来源：http://cnm.xylfe.cn

[A08] 取整与四舍五入
来源：http://ivi.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hyb.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mun.pycfn.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uya.chenlongwang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ysl.yj202588.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qhs.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bwy.0kj1m.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://frv.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gye.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://gwp.yfazqb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tan.0kj1m.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nvm.gaohongyu789.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xdq.zhoulong.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dus.fktsv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://emw.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cfh.zycfv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://klm.yonumen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hvk.yanxiufei.cn

[A10] 生成随机数
来源：http://yyy.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://xsi.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://cfg.uphjek.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pow.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dmk.chenzaomai.com

Java: new Random().nextInt(100) + 1
来源：http://vkn.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vwb.xylfe.cn

Ruby: rand(1..100)
来源：http://ukm.mhx1999.top

C#:   new Random().Next(1, 101)
来源：http://uwv.cashguo.top

[A11] 条件表达式（三元）
来源：http://kal.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://djm.ivvv.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bre.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://mfj.wangshuangyany.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vxn.mhx1999.top

Java: x > 0 ? "yes" : "no"
来源：http://zpz.zdbjq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mxs.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qmn.xinyue.icu

C#:   x > 0 ? "yes" : "no"
来源：http://bqx.ppjwa.cn

[A12] 字符串插值 / 格式化
来源：http://mwc.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nja.jiagoushi.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xeh.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://prn.ctjpmb.com

TS:   `Hello, ${name}!`
来源：http://nmf.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://sgs.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://utg.0kj1m.cn

Ruby: "Hello, #{name}!"
来源：http://zea.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://xyc.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://plz.yj202588.top

Py:   "第一行\n第二行"
来源：http://ebp.yuanzhike.top

PHP:  "第一行\n第二行"
来源：http://uoh.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://mnb.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://cqq.snrcjt.cn

Java: "第一行\n第二行"
来源：http://suj.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://kcy.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://fpl.tarul.cn

C#:   "第一行\n第二行"
来源：http://qiy.jinqigfzy.top

[A14] 注释写法
来源：http://vcq.jiagoushi.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lxm.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://zej.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://ksy.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://koz.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://elg.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://dts.hnqzz.top

Ruby: # 单行；=begin 多行 =end
来源：http://vee.gotoacloud.top

C#:   // 单行；/* 多行 */
来源：http://ugx.hesvh.cn

[A15] 空值判断与默认值
来源：http://knw.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://rhy.ydjk.org.cn

PHP:  $value = $data ?? "默认值";
来源：http://far.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://kat.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://vek.yuanzhike.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mir.52xcode.cn

Go:   if data == "" { data = "默认值" }
来源：http://ote.redwolf501.top

Ruby: value = data || "默认值"
来源：http://jva.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://gjk.meibo888.top

[A16] 真假值判断规则
来源：http://tvd.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kaz.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://see.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ojp.guowangkeji.top

TS:   if (!x) {}
来源：http://etx.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://drz.gogol.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eqc.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://yop.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ttx.jianghu66.top

[A17] 位运算
来源：http://wso.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uox.jqgfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uah.jinyuanbaomall.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lkz.smart0.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ppm.havefunace.top


<!-- 参考信息 -->