代发 wailian999

[U97] JS：并发请求
来源：http://kxe.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://osw.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://cht.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jgc.sysykeji.top

[U99] JS：事件监听
来源：http://zll.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://kye.yj202588.top

[U100] JS：DOM 查询
来源：http://jjd.chenjidiqi.icu

document.querySelector(".item")
来源：http://hhn.yanxiufei.cn

[U101] JS：classList 操作
来源：http://ldn.ctjpmb.com

el.classList.toggle("active")
来源：http://uyo.vehdjk.com

[U102] JS：本地存储
来源：http://dqs.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rme.bbcook.cn

[U103] JS：定时器
来源：http://pbn.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wpw.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://sec.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhk.chenzaomai.com

[U105] JS：节流
来源：http://yjb.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lll.c1oappe.top

[U106] JS：日期格式化
来源：http://xry.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sno.daxiang520.top

[U107] JS：数字千分位
来源：http://uvh.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kdv.nanxuanxn.top

[U108] JS：随机整数
来源：http://nqo.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qrs.hnxiangtu.top

[U109] JS：数组分组
来源：http://ehn.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://cdy.hongshengwenyu.top

[U110] JS：数组分块
来源：http://mpf.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://klb.jianghu66.top

[U111] JS：对象转 Map
来源：http://mob.sweek.top

new Map(Object.entries(obj))
来源：http://ool.jiagoushi.top

[U112] JS：字符串补位
来源：http://hsc.shuidangran.top

"7".padStart(3, "0")
来源：http://eya.xylfe.cn

[U113] JS：正则替换全部
来源：http://fll.ehwqpu.com

s.replaceAll("a", "b")
来源：http://jog.yueranfly.top

[U114] JS：JSON 深比较
来源：http://mmk.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jtb.jqgfzy.top

[U115] JS：生成 UUID
来源：http://lwm.xinyue.icu

crypto.randomUUID()
来源：http://goy.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ekw.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://trz.redwolf501.top

[U117] JS：单元测试
来源：http://pls.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://smn.aibaodan.cn

[U118] JS：开发服务器
来源：http://nuk.bjfxy.top

npm i -D vite;  npx vite
来源：http://tgu.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://kmt.ppjwa.cn

npx vite build
来源：http://pbq.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://ptd.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://web.gaohongyu789.top

================================================================================
来源：http://cbb.meibo888.top

统计汇总
来源：http://hja.yueranfly.top

================================================================================
来源：http://bnu.gogol.net.cn

按语言统计（条）：
来源：http://qrn.zdbjq.cn

Python ......... 252
来源：http://inp.hywenlv.cn

PHP ............ 252
来源：http://esb.bjfxy.top

JavaScript ..... 252
来源：http://ufw.shanyushiyangtech.top

TypeScript ..... 212
来源：http://ehe.zhixingplan.top

Java ........... 212
来源：http://bjl.zhijiandao.cn

Go ............. 212
来源：http://vcc.hammf.cn

Ruby ........... 212
来源：http://tik.birdmap.top

C# ............. 212
来源：http://baq.gaohongyu789.top

C .............. 30
来源：http://lyr.zdqjudy.top

C++ ............ 30
来源：http://gka.ywan-chungtsiang.top

SQL ............ 90
来源：http://dko.jinyuanbaomall.cn

Bash ........... 80
来源：http://flh.pengpengdd.cyou

Kotlin ......... 15
来源：http://vmv.ywan-chungtsiang.top

Swift .......... 15
来源：http://tzr.chenlongwang.top

Lua ............ 10
来源：http://nin.bjfxy.top

Perl ........... 10
来源：http://njx.redwolf501.top

Scala .......... 10
来源：http://opg.ybcxt.top

------------------------------------
来源：http://puw.hnqzz.top

合计 ........... 2106 条
来源：http://ygs.zycfv.cn

按章节统计：
来源：http://mty.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wzu.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iqc.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fqx.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zrl.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ugn.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://htn.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wbu.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dsv.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aqb.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aqd.sxryk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sat.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rpc.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tfy.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yyf.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sna.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yeh.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://rjz.hcnkem.com

R Bash 专题                             80
来源：http://hvx.sufxvd.cn

S C / C++ 专题                          60
来源：http://amk.yvedp.cn

T 其他语言补充                          60
来源：http://czi.wangdashe.top

U 高频实用片段                         120
来源：http://izz.52xcode.cn

------------------------------------
来源：http://fxa.smart0.xyz

合计                                  2106 条
来源：http://foy.uphjek.com

--------------------------------------------------------------------------------
来源：http://tbj.ybcxt.top

使用提醒
来源：http://qcz.aizwys.cn

--------------------------------------------------------------------------------
来源：http://nrw.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://thb.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nak.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jzv.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kbn.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dxf.hammf.cn

—— 文件结束 ——
来源：http://apg.nanxuanxn.top

================================================================================
来源：http://sjl.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://veh.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://byo.yuanzhike.top

================================================================================
来源：http://sdq.xylfe.cn

【收录内容】
来源：http://ypu.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hdy.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pfk.epnwcf.com

SQL · Bash · C · C++
来源：http://uyv.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nqv.ivvv.top

【使用说明】
来源：http://wxk.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tjn.fktsv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qvl.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uch.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hhq.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gph.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gnw.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bom.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oce.vehdjk.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fbf.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pni.chenlongwang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vnx.yongpay.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kzz.shuidangran.top

【文件统计】
来源：http://kkr.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://auy.ybcxt.top

--------------------------------------------------------------------------------
来源：http://hpa.ybcxt.top

目  录
来源：http://dkr.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://hyr.yonumen.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fiw.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uxg.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vqs.nanxinkj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lpx.jinqigufen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qjk.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sig.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wkn.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wnp.yj20258.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lqk.gaohongyu789.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dwr.jqgufenzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rbg.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nqz.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://itx.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jvf.gogol.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gmg.zhiwuduotai.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mlh.xinyue.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ubr.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pxb.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://imz.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://poc.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tel.52xcode.cn

================================================================================
来源：http://kko.bbcook.cn

A. 基础语法与类型
来源：http://mni.sxryk.cn

================================================================================
来源：http://ewt.xuanzx.com

[A01] Hello World
来源：http://vqm.quarkkingdee.top

Py:   print("Hello, World!")
来源：http://fat.zdbjq.cn

PHP:  echo "Hello, World!";
来源：http://bkf.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://oyl.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wmj.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://xvr.hnqzz.top

Go:   fmt.Println("Hello, World!")
来源：http://sim.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://eii.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://eoh.tarul.cn

[A02] 变量声明与赋值
来源：http://waj.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dlc.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wgr.yfazqb.com

JS:   let name = "Alex"; const age = 20;
来源：http://zzc.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iqd.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://dgp.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://kgf.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://bmd.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bhk.mhx1999.top

[A03] 常量定义
来源：http://kmi.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://brg.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://wby.c1oappe.top

JS:   const PI = 3.14159;
来源：http://kfy.tian-w.cn

TS:   const PI: number = 3.14159;
来源：http://vmc.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://gsu.yonumen.top

Go:   const PI = 3.14159
来源：http://iov.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://vwv.hysaishi.cn

C#:   const double PI = 3.14159;
来源：http://wei.gzhubu.top

[A04] 判断变量类型
来源：http://bqt.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qon.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xex.0kj1m.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mau.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://ufn.zhoulong.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rkt.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://ids.jyoumei.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rzr.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://evv.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://wee.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pqy.pycfn.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://eux.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cbv.wangshuangyany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bso.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://vki.jinyuanbaomall.cn

Go:   7 / 2; 7 % 2
来源：http://fgt.pycfn.com

Ruby: 7 / 2; 7 % 2
来源：http://loc.52xcode.cn

C#:   7 / 2; 7 % 2
来源：http://lis.xziqi.cn

[A06] 字符串转数字
来源：http://okj.smart0.xyz

Py:   int("42"); float("3.14")
来源：http://rhv.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sec.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xdc.hesvh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nje.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://amu.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://avg.aibaodan.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tex.redwolf501.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zgy.snrcjt.cn

[A07] 数字转字符串
来源：http://uoi.jinqigufen.top

Py:   str(42)
来源：http://pns.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://ill.vqdsnc.cn

JS:   String(42); (42).toString()
来源：http://gmi.meibo888.top

TS:   String(42)
来源：http://ago.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kpm.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://xfd.jinqigufen.top

Ruby: 42.to_s
来源：http://hqh.sxryk.cn

C#:   42.ToString()
来源：http://szb.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://mbi.kuanghao11.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xan.fktsv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dhu.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://slu.hongshengwenyu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://klr.zhixingplan.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pde.xingfuxueyuan.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mmr.haohaochexian.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rrf.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qmj.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://ljq.birdmap.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://epc.mhx1999.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mln.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ecq.gogol.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qim.ivvv.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mge.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ovt.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://obr.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vrq.yj20258888.top

[A10] 生成随机数
来源：http://myg.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://mlo.sysykeji.top

PHP:  random_int(1, 100);
来源：http://veo.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qfm.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://via.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://nyd.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qkc.cheryme.top

Ruby: rand(1..100)
来源：http://xzx.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://zvj.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://dmh.ybcxt.top

Py:   "yes" if x > 0 else "no"
来源：http://tih.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://tbt.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aqa.ctjpmb.com

TS:   x > 0 ? "yes" : "no"
来源：http://xtn.xuanzx.com

Java: x > 0 ? "yes" : "no"
来源：http://exx.epnwcf.com

Go:   // 无三元运算符，需用 if 语句
来源：http://fjo.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kvv.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uad.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://njn.shzxlz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pwg.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rjl.havefunace.top

JS:   `Hello, ${name}!`
来源：http://fpk.pycfn.com

TS:   `Hello, ${name}!`
来源：http://rvg.9152youxi.cn

Java: "Hello, %s!".formatted(name)
来源：http://xrx.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uzt.iojbl.cn

Ruby: "Hello, #{name}!"
来源：http://chd.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://uti.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cgp.yfazqb.com

Py:   "第一行\n第二行"
来源：http://kjf.fzhhl.top

PHP:  "第一行\n第二行"
来源：http://xbp.ctjpmb.com

JS:   "第一行\n第二行"
来源：http://rvw.xuetiantiany.cn

TS:   "第一行\n第二行"
来源：http://wal.chenlongwang.top

Java: "第一行\n第二行"
来源：http://qpa.iojbl.cn

Go:   "第一行\n第二行"
来源：http://yyy.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://acm.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://bsi.zdbjq.cn

[A14] 注释写法
来源：http://nxu.shanyushiyangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://msr.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oas.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://vvg.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://bey.xuanzx.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://igo.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://zsp.kuanghao11.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vme.yvedp.cn

C#:   // 单行；/* 多行 */
来源：http://rqt.svipenyu.cn

[A15] 空值判断与默认值
来源：http://ajd.yj202588.top

Py:   value = data or "默认值"
来源：http://qic.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://kmv.hywenlv.cn

JS:   const value = data ?? "默认值";
来源：http://eio.sufxvd.cn

TS:   const value = data ?? "默认值";
来源：http://nrv.xuetiantiany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://omn.yongpay.top

Go:   if data == "" { data = "默认值" }
来源：http://ztf.zhengqikj.top

Ruby: value = data || "默认值"
来源：http://syc.gaohongyu789.top

C#:   var value = data ?? "默认值";
来源：http://xtd.sysykeji.top

[A16] 真假值判断规则
来源：http://wgg.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qdf.shzxlz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nyz.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kfx.hesvh.cn

TS:   if (!x) {}
来源：http://gor.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fft.hywenlv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wlc.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kox.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ych.gzhubu.top

[A17] 位运算
来源：http://geo.ehwqpu.com


<!-- 参考信息 -->