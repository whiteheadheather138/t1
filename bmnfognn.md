代发 wailian999

[U99] JS：事件监听
来源：http://rys.vehdjk.com

el.addEventListener("click", e => {})
来源：http://fvc.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://ver.tarul.cn

document.querySelector(".item")
来源：http://eii.ppjwa.cn

[U101] JS：classList 操作
来源：http://xok.zdbjq.cn

el.classList.toggle("active")
来源：http://nya.jyoumei.cn

[U102] JS：本地存储
来源：http://ojn.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://kpz.feifeiyinyue.top

[U103] JS：定时器
来源：http://cqo.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://snb.zhijiandao.cn

[U104] JS：防抖
来源：http://zpl.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxh.jiagoushi.top

[U105] JS：节流
来源：http://pqq.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ios.snrcjt.cn

[U106] JS：日期格式化
来源：http://ghy.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hjn.chenzaomai.com

[U107] JS：数字千分位
来源：http://qrs.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qza.hfpthk.cn

[U108] JS：随机整数
来源：http://onv.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ufm.fzhhl.top

[U109] JS：数组分组
来源：http://avo.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://xyh.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://xfp.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pys.shzxlz.cn

[U111] JS：对象转 Map
来源：http://tpo.daria6918.cn

new Map(Object.entries(obj))
来源：http://ohf.0kj1m.cn

[U112] JS：字符串补位
来源：http://qed.fzhhl.top

"7".padStart(3, "0")
来源：http://ewr.yj20258.top

[U113] JS：正则替换全部
来源：http://rkf.svipenyu.cn

s.replaceAll("a", "b")
来源：http://rjs.bbcook.cn

[U114] JS：JSON 深比较
来源：http://pqi.xylfe.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://luu.hnqzz.top

[U115] JS：生成 UUID
来源：http://hzt.ybcxt.top

crypto.randomUUID()
来源：http://ddn.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://fqt.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://knd.hywenlv.cn

[U117] JS：单元测试
来源：http://ehv.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://neh.hysaishi.cn

[U118] JS：开发服务器
来源：http://qpx.tanke756.top

npm i -D vite;  npx vite
来源：http://nfr.yanxiufei.cn

[U119] JS：生产构建
来源：http://ltf.hnxiangtu.top

npx vite build
来源：http://adk.kuanghao11.cn

[U120] JS：读取环境变量（Vite）
来源：http://iux.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://ctl.sxryk.cn

================================================================================
来源：http://elz.nanxuanxn.top

统计汇总
来源：http://wqj.mhx1999.top

================================================================================
来源：http://frd.yuanzhike.top

按语言统计（条）：
来源：http://slq.andypj.xyz

Python ......... 252
来源：http://pvi.cdnleiting.top

PHP ............ 252
来源：http://brc.cheryme.top

JavaScript ..... 252
来源：http://ksa.yongpay.top

TypeScript ..... 212
来源：http://msx.hnqzz.top

Java ........... 212
来源：http://aod.ppjwa.cn

Go ............. 212
来源：http://cue.ehwqpu.com

Ruby ........... 212
来源：http://adz.feifeiyinyue.top

C# ............. 212
来源：http://dwo.ctjpmb.com

C .............. 30
来源：http://dnm.yj20258.top

C++ ............ 30
来源：http://yml.aibaodan.cn

SQL ............ 90
来源：http://ykz.sysykeji.top

Bash ........... 80
来源：http://gcj.pycfn.com

Kotlin ......... 15
来源：http://jjp.pycfn.com

Swift .......... 15
来源：http://vod.smart0.xyz

Lua ............ 10
来源：http://yue.tianlin.xyz

Perl ........... 10
来源：http://uwd.jinghuilouyu.cn

Scala .......... 10
来源：http://tkx.jqgfzy.top

------------------------------------
来源：http://nvd.hcnkem.com

合计 ........... 2106 条
来源：http://ddu.shanyushiyangkeji.top

按章节统计：
来源：http://uwu.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mvd.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xcw.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eud.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://irv.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jif.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eac.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://geu.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://abl.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wwr.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ebk.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wex.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jgx.cashguo.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qxu.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hgu.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fnm.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vth.yvedp.cn

Q SQL 专题                              90
来源：http://pxx.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://yzm.ppjwa.cn

S C / C++ 专题                          60
来源：http://xeo.tianlin.xyz

T 其他语言补充                          60
来源：http://fnq.jlsjyb.cn

U 高频实用片段                         120
来源：http://oez.bbcook.cn

------------------------------------
来源：http://tfj.9152youxi.cn

合计                                  2106 条
来源：http://gnt.fehbvm.com

--------------------------------------------------------------------------------
来源：http://tif.hysaishi.cn

使用提醒
来源：http://apx.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://qfk.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hhh.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cyq.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wex.chenlongwang.top

在旧版本上使用前请先确认语法支持情况。
来源：http://syl.yj20258888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://izo.yuxming.cn

—— 文件结束 ——
来源：http://pud.yvedp.cn

================================================================================
来源：http://vuz.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://xtp.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://jzi.gogol.net.cn

================================================================================
来源：http://ank.feifeiyinyue.top

【收录内容】
来源：http://xon.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yre.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oac.c1oappe.top

SQL · Bash · C · C++
来源：http://mgg.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://htm.ppjwa.cn

【使用说明】
来源：http://ioc.tanke756.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xrj.pengpengdd.cyou

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://way.havefunace.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lhz.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lrf.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://dqv.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lga.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://czf.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ngc.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iuz.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ngd.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ina.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://byy.hammf.cn

【文件统计】
来源：http://kyk.cheryme.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tfm.uphjek.com

--------------------------------------------------------------------------------
来源：http://nbo.zhoulong.xyz

目  录
来源：http://fcz.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://uib.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oau.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jcr.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oei.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rug.hesvh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bwx.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sos.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ydw.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://frb.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jtp.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lmy.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mcp.jinqigfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hkz.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bvb.ybcxt.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yei.chenjidiqi.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aps.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ojo.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://amf.ydjk.org.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rhw.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zid.tanke756.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dmh.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yzh.nanxinkj.top

================================================================================
来源：http://ghh.hfpthk.cn

A. 基础语法与类型
来源：http://wyb.ppjwa.cn

================================================================================
来源：http://uhl.jqgufenzy.top

[A01] Hello World
来源：http://smh.daxiang520.top

Py:   print("Hello, World!")
来源：http://kbk.hammf.cn

PHP:  echo "Hello, World!";
来源：http://sto.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://uzb.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://abj.zycfv.cn

Java: System.out.println("Hello, World!");
来源：http://jda.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://bjv.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://omy.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kic.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://wkf.shuidangran.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cfk.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mvw.316326.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://zuy.jqgfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://aht.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://btz.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://owl.wangshuangyany.cn

Ruby: name = "Alex"; age = 20
来源：http://hsv.pengpengdd.cyou

C#:   string name = "Alex"; int age = 20;
来源：http://aag.yvedp.cn

[A03] 常量定义
来源：http://sji.cdnleiting.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qfo.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://xil.cashguo.top

JS:   const PI = 3.14159;
来源：http://pxm.shanyushiyangtech.top

TS:   const PI: number = 3.14159;
来源：http://wxq.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://ahj.shanyushiyangtech.top

Go:   const PI = 3.14159
来源：http://ajy.316326.xyz

Ruby: PI = 3.14159
来源：http://cup.fzhhl.top

C#:   const double PI = 3.14159;
来源：http://ggw.fktsv.cn

[A04] 判断变量类型
来源：http://zmh.xziqi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qdr.sysykeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ewt.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qxt.mhx1999.top

TS:   typeof x; x instanceof Date
来源：http://slq.ivvv.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wni.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oix.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cox.xingfuxueyuan.xyz

C#:   x.GetType().Name; x is int
来源：http://zkv.zhengqikj.top

[A05] 整数除法与取模
来源：http://ibz.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yzv.meibo888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jft.aibaodan.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xnp.zhengqikj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pzk.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://hlt.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://ubf.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://lqj.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://fnr.aibaodan.cn

[A06] 字符串转数字
来源：http://ueo.aizwys.cn

Py:   int("42"); float("3.14")
来源：http://ynx.chenjidiqi.icu

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://utp.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wyb.meibo888.top

TS:   parseInt("42", 10); Number("42")
来源：http://tpm.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://thv.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nio.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://zdj.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jzh.sufxvd.cn

[A07] 数字转字符串
来源：http://thl.jlsjyb.cn

Py:   str(42)
来源：http://buk.hfpthk.cn

PHP:  (string) 42; strval(42)
来源：http://sru.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://ivj.chenzaomai.com

TS:   String(42)
来源：http://pur.gaohongyu789.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lxb.bjfxy.top

Go:   strconv.Itoa(42)
来源：http://izc.uphjek.com

Ruby: 42.to_s
来源：http://dvd.sysykeji.top

C#:   42.ToString()
来源：http://wwq.hysaishi.cn

[A08] 取整与四舍五入
来源：http://pnj.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uwc.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rrr.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nnw.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nhy.dianchejie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gww.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tin.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://brp.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ajo.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://azw.yangfankeji.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ngs.birdmap.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zyt.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dsv.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sqx.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xfm.jianghu66.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zgo.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hrh.xziqi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vul.zhijiandao.cn

[A10] 生成随机数
来源：http://hxb.zhixingplan.top

Py:   import random; random.randint(1, 100)
来源：http://uho.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://jky.yvedp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wyj.uphjek.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://clv.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://zrr.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qbg.jqgfzy.top

Ruby: rand(1..100)
来源：http://dyw.gzhubu.top

C#:   new Random().Next(1, 101)
来源：http://cni.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://dsp.tian-w.cn

Py:   "yes" if x > 0 else "no"
来源：http://gum.52xcode.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dcz.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://buq.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cnv.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://ssr.chenjidiqi.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://khe.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wlj.havefunace.top

C#:   x > 0 ? "yes" : "no"
来源：http://dzi.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://tve.jinyuanbaomall.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sfv.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iqo.birdmap.top

JS:   `Hello, ${name}!`
来源：http://jja.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://pll.shuidangran.top

Java: "Hello, %s!".formatted(name)
来源：http://res.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bnp.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://uwi.tanke756.top

C#:   $"Hello, {name}!"
来源：http://qyb.hesvh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sne.52xcode.cn

Py:   "第一行\n第二行"
来源：http://yzn.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://qvo.hesvh.cn

JS:   "第一行\n第二行"
来源：http://abp.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://lsv.haohaochexian.top

Java: "第一行\n第二行"
来源：http://xrq.hesvh.cn

Go:   "第一行\n第二行"
来源：http://lzs.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://owp.feifeiyinyue.top

C#:   "第一行\n第二行"
来源：http://mdo.jinghuilouyu.cn

[A14] 注释写法
来源：http://euw.daxiang520.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://fqs.chenjidiqi.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://qgi.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://rqd.redwolf501.top

TS:   // 单行；/* 多行 */
来源：http://pzu.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ipy.hammf.cn

Go:   // 单行；/* 多行 */
来源：http://ycr.c1oappe.top

Ruby: # 单行；=begin 多行 =end
来源：http://nod.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://whz.tarul.cn

[A15] 空值判断与默认值
来源：http://ayn.feifeiyinyue.top

Py:   value = data or "默认值"
来源：http://nep.chenjidiqi.icu

PHP:  $value = $data ?? "默认值";
来源：http://voa.uphjek.com

JS:   const value = data ?? "默认值";
来源：http://kct.sysykeji.top

TS:   const value = data ?? "默认值";
来源：http://iax.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wmd.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://suq.nwbrower.top

Ruby: value = data || "默认值"
来源：http://pmm.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://wtp.chenzaomai.com

[A16] 真假值判断规则
来源：http://inl.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hkb.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gfr.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hri.ybcxt.top

TS:   if (!x) {}
来源：http://rsa.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yfd.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://trv.316326.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ayv.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sjc.smart0.xyz

[A17] 位运算
来源：http://oqi.iojbl.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmn.iojbl.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nzw.aizwys.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iag.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ihp.tanke756.top


<!-- 参考信息 -->