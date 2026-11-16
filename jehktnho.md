代发 wailian999

[U99] JS：事件监听
来源：http://uey.yongpay.top

el.addEventListener("click", e => {})
来源：http://ncu.aizwys.cn

[U100] JS：DOM 查询
来源：http://rrs.xziqi.cn

document.querySelector(".item")
来源：http://mtv.xziqi.cn

[U101] JS：classList 操作
来源：http://zcp.dashuyun.cn

el.classList.toggle("active")
来源：http://ssv.cqqwz.cn

[U102] JS：本地存储
来源：http://kea.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vbc.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://vvv.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gpm.jqgufenzy.top

[U104] JS：防抖
来源：http://syc.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vhn.redwolf501.top

[U105] JS：节流
来源：http://jsf.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yrj.yvedp.cn

[U106] JS：日期格式化
来源：http://zkh.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ylo.birdmap.top

[U107] JS：数字千分位
来源：http://sso.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bsq.tian-w.cn

[U108] JS：随机整数
来源：http://hlg.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://emg.jianghu66.top

[U109] JS：数组分组
来源：http://xdg.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://wby.bjfxy.top

[U110] JS：数组分块
来源：http://qaz.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qbr.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://bbi.xinyue.icu

new Map(Object.entries(obj))
来源：http://mvo.nwbrower.top

[U112] JS：字符串补位
来源：http://lqb.yj20258.top

"7".padStart(3, "0")
来源：http://kgm.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://fyr.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://aeo.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://oga.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yuj.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://mhn.aizwys.cn

crypto.randomUUID()
来源：http://ezf.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://zbq.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://yoa.sweek.top

[U117] JS：单元测试
来源：http://kes.yongpay.top

npm i -D vitest;  npx vitest
来源：http://wne.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://oor.jqgfzy.top

npm i -D vite;  npx vite
来源：http://gxu.zhiwuduotai.top

[U119] JS：生产构建
来源：http://dfg.yuanzhike.top

npx vite build
来源：http://gpg.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://mnr.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://kmz.guannengcc.top

================================================================================
来源：http://eas.hongshengwenyu.top

统计汇总
来源：http://nqe.yueranfly.top

================================================================================
来源：http://bim.zhoulong.xyz

按语言统计（条）：
来源：http://mjm.fanxiaobao.xyz

Python ......... 252
来源：http://meu.xziqi.cn

PHP ............ 252
来源：http://lnt.ydjk.org.cn

JavaScript ..... 252
来源：http://xgi.zhijiandao.cn

TypeScript ..... 212
来源：http://gye.zhijiandao.cn

Java ........... 212
来源：http://htv.bbcook.cn

Go ............. 212
来源：http://rwe.zhiwuduotai.top

Ruby ........... 212
来源：http://lsk.xinyue.icu

C# ............. 212
来源：http://mlz.zdqjudy.top

C .............. 30
来源：http://vod.wangdashe.top

C++ ............ 30
来源：http://otj.0kj1m.cn

SQL ............ 90
来源：http://hce.birdmap.top

Bash ........... 80
来源：http://lgc.ydjk.org.cn

Kotlin ......... 15
来源：http://ljr.andypj.xyz

Swift .......... 15
来源：http://ilb.52xcode.cn

Lua ............ 10
来源：http://esp.haohaochexian.top

Perl ........... 10
来源：http://qei.yuxming.cn

Scala .......... 10
来源：http://tjx.cheryme.top

------------------------------------
来源：http://dzv.ctjpmb.com

合计 ........... 2106 条
来源：http://lmo.jinqigufen.top

按章节统计：
来源：http://wdp.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pwq.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zfc.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mrn.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gzn.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://woq.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lin.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hlx.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zyb.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kgu.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xsx.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bwx.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vbp.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cyv.yonumen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cpg.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kjw.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ysn.tian-w.cn

Q SQL 专题                              90
来源：http://nbn.tanke756.top

R Bash 专题                             80
来源：http://zcx.yueranfly.top

S C / C++ 专题                          60
来源：http://tzv.316326.xyz

T 其他语言补充                          60
来源：http://ptu.andypj.xyz

U 高频实用片段                         120
来源：http://ifo.chenzaomai.com

------------------------------------
来源：http://xue.guowangkeji.top

合计                                  2106 条
来源：http://gyl.daxiang520.top

--------------------------------------------------------------------------------
来源：http://lbp.ydzc1.top

使用提醒
来源：http://xnt.vehdjk.com

--------------------------------------------------------------------------------
来源：http://fti.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fzn.xziqi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://epc.zdbjq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ggj.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wrq.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zis.nanxuanxn.top

—— 文件结束 ——
来源：http://kel.sjlbkw.cn

================================================================================
来源：http://kmi.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://mqu.hesvh.cn

Common Programming Examples Cheat Book
来源：http://gza.yfazqb.com

================================================================================
来源：http://cuu.nanxuanxn.top

【收录内容】
来源：http://ezi.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://lhk.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gyx.guowangkeji.top

SQL · Bash · C · C++
来源：http://zzh.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gdm.tanke756.top

【使用说明】
来源：http://qdi.chenzaomai.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://and.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qbh.birdmap.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gal.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dnv.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zea.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nma.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uel.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zda.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cma.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aeq.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oce.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nio.hnqzz.top

【文件统计】
来源：http://gvx.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gax.zycfv.cn

--------------------------------------------------------------------------------
来源：http://run.xingfuxueyuan.xyz

目  录
来源：http://xnv.mhx1999.top

--------------------------------------------------------------------------------
来源：http://xbd.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rtz.cashguo.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pke.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bcr.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bba.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sjo.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yux.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gut.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gxt.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wav.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sor.birdmap.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ykp.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nhu.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://inp.chenzaomai.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://brt.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bli.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ett.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://prk.cheryme.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bqt.hywenlv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tfu.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqt.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tda.yj20258888.top

================================================================================
来源：http://ysi.yj20258.top

A. 基础语法与类型
来源：http://fnc.hongshengwenyu.top

================================================================================
来源：http://gas.c1oappe.top

[A01] Hello World
来源：http://yvn.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://fyp.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://lwl.ctjpmb.com

JS:   console.log("Hello, World!");
来源：http://dmb.sweek.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vrh.shangyingyoupin.top

Java: System.out.println("Hello, World!");
来源：http://rzw.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://atq.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://kzw.hammf.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://odg.jinghuilouyu.cn

[A02] 变量声明与赋值
来源：http://qks.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dmv.cashguo.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nlp.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tyg.xziqi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xgb.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://pyt.yj20258888.top

Go:   name := "Alex"; age := 20
来源：http://zzo.wangdashe.top

Ruby: name = "Alex"; age = 20
来源：http://qmc.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://tgf.ybcxt.top

[A03] 常量定义
来源：http://fym.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bny.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://pbw.jinqigufen.top

JS:   const PI = 3.14159;
来源：http://ulb.jlsjyb.cn

TS:   const PI: number = 3.14159;
来源：http://tsj.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://ifq.meibo888.top

Go:   const PI = 3.14159
来源：http://blg.jiagoushi.top

Ruby: PI = 3.14159
来源：http://gqf.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://qqy.yangfankeji.com

[A04] 判断变量类型
来源：http://dvu.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://sic.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oyl.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yhi.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://csi.tanke756.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://set.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://vri.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://gaf.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://utq.shuidangran.top

[A05] 整数除法与取模
来源：http://twl.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://evg.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jjh.yuxming.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bgi.ydjk.org.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhx.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://ztc.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://jml.fengsongda.top

Ruby: 7 / 2; 7 % 2
来源：http://mka.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://jjg.guowangkeji.top

[A06] 字符串转数字
来源：http://bpm.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://lyy.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mzz.zycfv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://keb.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://vtt.52xcode.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ymf.fanxiaobao.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sty.hcnkem.com

Ruby: "42".to_i; "3.14".to_f
来源：http://owm.mhx1999.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dlr.yj202588.top

[A07] 数字转字符串
来源：http://xoz.zhengqikj.top

Py:   str(42)
来源：http://ked.yj20258.top

PHP:  (string) 42; strval(42)
来源：http://qmz.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://pqy.tarul.cn

TS:   String(42)
来源：http://ksa.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hmz.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://flr.wangdashe.top

Ruby: 42.to_s
来源：http://xpa.fengsongda.top

C#:   42.ToString()
来源：http://yli.nwbrower.top

[A08] 取整与四舍五入
来源：http://ohj.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cac.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jcp.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zot.wangdashe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cyo.smart0.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qub.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tsg.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rvt.zdbjq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://odw.cheryme.top

[A09] 绝对值与最大最小值
来源：http://wbb.vqdsnc.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jyy.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://erd.jiagoushi.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kmc.hnqzz.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yls.316326.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yrx.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nyw.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fsh.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://psv.xziqi.cn

[A10] 生成随机数
来源：http://vtw.snrcjt.cn

Py:   import random; random.randint(1, 100)
来源：http://ehg.gaohongyu789.top

PHP:  random_int(1, 100);
来源：http://rdc.zhengqikj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yib.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ijn.aibaodan.cn

Java: new Random().nextInt(100) + 1
来源：http://aml.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yvy.chenlongwang.top

Ruby: rand(1..100)
来源：http://dnu.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://clx.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://uin.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://pnn.jinqigufen.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://smn.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://wmu.jinyuanbaomall.cn

TS:   x > 0 ? "yes" : "no"
来源：http://adx.jqgfzy.top

Java: x > 0 ? "yes" : "no"
来源：http://eiz.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dzd.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kvu.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://arh.birdmap.top

[A12] 字符串插值 / 格式化
来源：http://ysd.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yhg.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rlp.bjfxy.top

JS:   `Hello, ${name}!`
来源：http://sqz.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://nns.daxiang520.top

Java: "Hello, %s!".formatted(name)
来源：http://bvg.andypj.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ybt.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://upu.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://jfs.pycfn.com

[A13] 多行字符串（练习 \n 转义）
来源：http://mgr.chenlongwang.top

Py:   "第一行\n第二行"
来源：http://dkn.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://dyy.epnwcf.com

JS:   "第一行\n第二行"
来源：http://zwx.316326.xyz

TS:   "第一行\n第二行"
来源：http://ddc.yfazqb.com

Java: "第一行\n第二行"
来源：http://ofv.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://pdn.iojbl.cn

Ruby: "第一行\n第二行"
来源：http://tyu.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://elj.yueranfly.top

[A14] 注释写法
来源：http://pcl.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tyv.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://btm.dashuyun.cn

JS:   // 单行；/* 多行 */
来源：http://xkf.fehbvm.com

TS:   // 单行；/* 多行 */
来源：http://ejc.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://evx.hnxiangtu.top

Go:   // 单行；/* 多行 */
来源：http://mop.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://smj.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://qgx.yongpay.top

[A15] 空值判断与默认值
来源：http://uwy.xziqi.cn

Py:   value = data or "默认值"
来源：http://rcw.jyoumei.cn

PHP:  $value = $data ?? "默认值";
来源：http://lca.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://hme.tianlin.xyz

TS:   const value = data ?? "默认值";
来源：http://qdn.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://psp.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://eft.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://nur.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://bgi.snrcjt.cn

[A16] 真假值判断规则
来源：http://gkl.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mzg.hnxiangtu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dhl.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hin.cqqwz.cn

TS:   if (!x) {}
来源：http://est.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://upv.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iee.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yin.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sah.cdnleiting.top

[A17] 位运算
来源：http://dhy.jinghuilouyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fum.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wpn.zhengqikj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pxx.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cfa.nanxinkj.top


<!-- 参考信息 -->