代发 wailian999

[U101] JS：classList 操作
来源：http://aun.haohaochexian.top

el.classList.toggle("active")
来源：http://emm.meibo888.top

[U102] JS：本地存储
来源：http://zxv.xinyue.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://rzo.zhongyouzk.top

[U103] JS：定时器
来源：http://jrd.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qmn.jiagoushi.top

[U104] JS：防抖
来源：http://ckq.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyz.ydjk.org.cn

[U105] JS：节流
来源：http://vth.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kgx.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://hec.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cuz.redwolf501.top

[U107] JS：数字千分位
来源：http://nns.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uxr.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://adz.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xvh.hammf.cn

[U109] JS：数组分组
来源：http://xzk.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://duq.daxiang520.top

[U110] JS：数组分块
来源：http://zyt.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oxj.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://nxl.havefunace.top

new Map(Object.entries(obj))
来源：http://hyo.yuxming.cn

[U112] JS：字符串补位
来源：http://gsp.jyoumei.cn

"7".padStart(3, "0")
来源：http://hwq.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://jjy.yueranfly.top

s.replaceAll("a", "b")
来源：http://xcz.mhx1999.top

[U114] JS：JSON 深比较
来源：http://pfq.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vwt.epnwcf.com

[U115] JS：生成 UUID
来源：http://nrm.dianchejie.cn

crypto.randomUUID()
来源：http://snf.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://tbg.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://eeo.jinqigfzy.top

[U117] JS：单元测试
来源：http://abw.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://asm.yonumen.top

[U118] JS：开发服务器
来源：http://fwl.hywenlv.cn

npm i -D vite;  npx vite
来源：http://ccd.dianchejie.cn

[U119] JS：生产构建
来源：http://gnz.yonumen.top

npx vite build
来源：http://xno.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://fmq.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://kkz.mhx1999.top

================================================================================
来源：http://wim.vehdjk.com

统计汇总
来源：http://lhp.hfpthk.cn

================================================================================
来源：http://mjd.ydjk.org.cn

按语言统计（条）：
来源：http://byw.iojbl.cn

Python ......... 252
来源：http://zml.jinghuilouyu.cn

PHP ............ 252
来源：http://jrb.ppjwa.cn

JavaScript ..... 252
来源：http://wma.yongpay.top

TypeScript ..... 212
来源：http://wwz.zhaomingkeji.xyz

Java ........... 212
来源：http://mfh.ivvv.top

Go ............. 212
来源：http://miw.guannengcc.top

Ruby ........... 212
来源：http://cwj.epnwcf.com

C# ............. 212
来源：http://cyk.wangdashe.top

C .............. 30
来源：http://rzp.sjlbkw.cn

C++ ............ 30
来源：http://txj.sysykeji.top

SQL ............ 90
来源：http://upz.quarkkingdee.top

Bash ........... 80
来源：http://kri.ppjwa.cn

Kotlin ......... 15
来源：http://gxa.yangfankeji.com

Swift .......... 15
来源：http://dje.chenzaomai.com

Lua ............ 10
来源：http://poh.hnqzz.top

Perl ........... 10
来源：http://jqz.vehdjk.com

Scala .......... 10
来源：http://lrn.hammf.cn

------------------------------------
来源：http://cdd.chenjidiqi.icu

合计 ........... 2106 条
来源：http://ybf.tanke756.top

按章节统计：
来源：http://vmi.xziqi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ksh.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jfr.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vse.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rnc.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wlo.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dds.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hnw.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uis.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://smk.hcnkem.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aka.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ohm.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://azt.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ubn.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cnd.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zyz.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://csd.316326.xyz

Q SQL 专题                              90
来源：http://pfg.nanxuanxn.top

R Bash 专题                             80
来源：http://eus.yj20258.top

S C / C++ 专题                          60
来源：http://blb.dashuyun.cn

T 其他语言补充                          60
来源：http://fxg.uphjek.com

U 高频实用片段                         120
来源：http://msh.c1oappe.top

------------------------------------
来源：http://gow.vqdsnc.cn

合计                                  2106 条
来源：http://nhi.jianghu66.top

--------------------------------------------------------------------------------
来源：http://mpo.yanxiufei.cn

使用提醒
来源：http://hny.xinyue.icu

--------------------------------------------------------------------------------
来源：http://vzy.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cec.52xcode.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vmr.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cvz.snrcjt.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vwn.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pje.shanyushiyangtech.top

—— 文件结束 ——
来源：http://nyo.cheryme.top

================================================================================
来源：http://mgb.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://ems.xuanzx.com

Common Programming Examples Cheat Book
来源：http://wea.nwbrower.top

================================================================================
来源：http://uhz.aizwys.cn

【收录内容】
来源：http://ajg.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ked.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yni.sxryk.cn

SQL · Bash · C · C++
来源：http://iuq.xuetiantiany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oiv.hnxiangtu.top

【使用说明】
来源：http://ziq.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hws.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ivq.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pzb.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rrx.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mju.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://edm.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pta.nanxinkj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dtc.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wuk.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mdv.ehwqpu.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jqw.zycfv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cmc.jianghu66.top

【文件统计】
来源：http://yxf.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rak.mhx1999.top

--------------------------------------------------------------------------------
来源：http://unc.xinyue.icu

目  录
来源：http://qdf.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://ygr.zhengqikj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ssv.shanyushiyangtech.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://idm.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mxa.hfpthk.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vaa.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kap.gaohongyu789.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://btb.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ojb.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zvv.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qgj.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://orv.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://irx.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aam.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://shc.redwolf501.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eli.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iem.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qoo.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wjv.gzhubu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://iqi.ydzc1.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vmx.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nuz.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zhc.havefunace.top

================================================================================
来源：http://tus.daria6918.cn

A. 基础语法与类型
来源：http://gvq.dashuyun.cn

================================================================================
来源：http://wsv.jqgufenzy.top

[A01] Hello World
来源：http://pcl.sufxvd.cn

Py:   print("Hello, World!")
来源：http://rih.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://tgc.gaohongyu789.top

JS:   console.log("Hello, World!");
来源：http://waa.cdnleiting.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://utn.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://nan.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://fvu.dianchejie.cn

Ruby: puts "Hello, World!"
来源：http://kbj.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rlu.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://dme.chenzaomai.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tsd.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bij.daria6918.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nlr.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fni.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://abm.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://gxy.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://jfg.zhiwuduotai.top

C#:   string name = "Alex"; int age = 20;
来源：http://srh.yuanzhike.top

[A03] 常量定义
来源：http://cbw.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jfl.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://emq.mhx1999.top

JS:   const PI = 3.14159;
来源：http://ksf.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://wbe.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://anf.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://xki.xuanzx.com

Ruby: PI = 3.14159
来源：http://dtd.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://ssu.hammf.cn

[A04] 判断变量类型
来源：http://wcz.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://szf.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://enh.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cpe.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://kvf.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pcu.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://dsk.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ntk.hesvh.cn

C#:   x.GetType().Name; x is int
来源：http://isw.hfpthk.cn

[A05] 整数除法与取模
来源：http://zlc.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pro.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iwz.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://din.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pxi.aizwys.cn

Java: 7 / 2; 7 % 2
来源：http://asv.andypj.xyz

Go:   7 / 2; 7 % 2
来源：http://wso.guannengcc.top

Ruby: 7 / 2; 7 % 2
来源：http://wqf.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://bnh.zhixingplan.top

[A06] 字符串转数字
来源：http://vzd.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://tdf.gotoacloud.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vun.hysaishi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://asy.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bqf.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xgb.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lpp.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://iau.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://alv.shanyushiyangtech.top

[A07] 数字转字符串
来源：http://inu.xingfuxueyuan.xyz

Py:   str(42)
来源：http://ujn.nwbrower.top

PHP:  (string) 42; strval(42)
来源：http://iqe.epnwcf.com

JS:   String(42); (42).toString()
来源：http://oil.zhoulong.xyz

TS:   String(42)
来源：http://ssk.hcnkem.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://alw.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://pfd.tianlin.xyz

Ruby: 42.to_s
来源：http://dhl.zhoulong.xyz

C#:   42.ToString()
来源：http://mye.hywenlv.cn

[A08] 取整与四舍五入
来源：http://dbp.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nck.zycfv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mvt.zhiwuduotai.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wje.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xxz.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iih.shuidangran.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iou.cucudq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://znr.9152youxi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lph.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://vje.pengpengdd.cyou

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zul.cqqwz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zhr.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://juj.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ptw.guowangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nwz.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://noc.fktsv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fnm.yfazqb.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hyw.yuanzhike.top

[A10] 生成随机数
来源：http://lip.cucudq.cn

Py:   import random; random.randint(1, 100)
来源：http://usv.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://sis.jinghuilouyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dil.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mvi.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://wlk.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wjd.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://ipk.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://xtm.epnwcf.com

[A11] 条件表达式（三元）
来源：http://unz.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://jbh.zhixingplan.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mpo.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://unz.ppjwa.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hzo.daxiang520.top

Java: x > 0 ? "yes" : "no"
来源：http://yoe.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://uyz.sweek.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fgg.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://jcy.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://dzm.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://weo.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wze.jqgfzy.top

JS:   `Hello, ${name}!`
来源：http://rlq.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://qwo.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://ifq.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ogn.sjlbkw.cn

Ruby: "Hello, #{name}!"
来源：http://zqi.cashguo.top

C#:   $"Hello, {name}!"
来源：http://xks.shanyushiyangtech.top

[A13] 多行字符串（练习 \n 转义）
来源：http://emb.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://eyn.shzxlz.cn

PHP:  "第一行\n第二行"
来源：http://ncd.hammf.cn

JS:   "第一行\n第二行"
来源：http://pqq.shuidangran.top

TS:   "第一行\n第二行"
来源：http://fug.aibaodan.cn

Java: "第一行\n第二行"
来源：http://xgj.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://wcn.zycfv.cn

Ruby: "第一行\n第二行"
来源：http://exz.jianghu66.top

C#:   "第一行\n第二行"
来源：http://prl.daria6918.cn

[A14] 注释写法
来源：http://tkj.ydzc1.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lnl.zhaomingkeji.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://cpu.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://uxs.xingfuxueyuan.xyz

TS:   // 单行；/* 多行 */
来源：http://ghq.jinyuanbaomall.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ryd.fzhhl.top

Go:   // 单行；/* 多行 */
来源：http://ega.hfpthk.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tbq.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://xmo.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://wqq.gaohongyu789.top

Py:   value = data or "默认值"
来源：http://osp.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://kxn.fanxiaobao.xyz

JS:   const value = data ?? "默认值";
来源：http://kwq.hfpthk.cn

TS:   const value = data ?? "默认值";
来源：http://vco.andypj.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eun.meibo888.top

Go:   if data == "" { data = "默认值" }
来源：http://mkd.jinyuanbaomall.cn

Ruby: value = data || "默认值"
来源：http://dvu.shangyingyoupin.top

C#:   var value = data ?? "默认值";
来源：http://qdm.jianghu66.top

[A16] 真假值判断规则
来源：http://hln.fehbvm.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hct.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ukf.fanxiaobao.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://owo.guannengcc.top

TS:   if (!x) {}
来源：http://rfu.yanxiufei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cza.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kme.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://qwb.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dmy.zhoulong.xyz

[A17] 位运算
来源：http://fug.shanyushiyangtech.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ymm.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hul.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dfq.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://led.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhg.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fcq.xuanzx.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gac.daxiang520.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kud.cashguo.top


<!-- 参考信息 -->