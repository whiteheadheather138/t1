代发 wailian999

[U99] JS：事件监听
来源：http://zih.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://ddc.fehbvm.com

[U100] JS：DOM 查询
来源：http://gka.xuetiantiany.cn

document.querySelector(".item")
来源：http://npt.dianchejie.cn

[U101] JS：classList 操作
来源：http://xja.cheryme.top

el.classList.toggle("active")
来源：http://jje.fktsv.cn

[U102] JS：本地存储
来源：http://gmq.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mie.zhengqikj.top

[U103] JS：定时器
来源：http://vpz.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dzq.chenzaomai.com

[U104] JS：防抖
来源：http://jjd.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvz.cheryme.top

[U105] JS：节流
来源：http://wzg.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cbq.mhx1999.top

[U106] JS：日期格式化
来源：http://iab.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kfw.0kj1m.cn

[U107] JS：数字千分位
来源：http://ngl.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fer.hnqzz.top

[U108] JS：随机整数
来源：http://wmq.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://deh.dianchejie.cn

[U109] JS：数组分组
来源：http://dcq.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://rpj.sxryk.cn

[U110] JS：数组分块
来源：http://qgj.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wrw.zdqjudy.top

[U111] JS：对象转 Map
来源：http://loe.yonumen.top

new Map(Object.entries(obj))
来源：http://avj.zdqjudy.top

[U112] JS：字符串补位
来源：http://hik.zhoulong.xyz

"7".padStart(3, "0")
来源：http://zia.dashuyun.cn

[U113] JS：正则替换全部
来源：http://spw.chenzaomai.com

s.replaceAll("a", "b")
来源：http://bkf.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://zyh.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://jtb.bbcook.cn

[U115] JS：生成 UUID
来源：http://rtq.wangshuangyany.cn

crypto.randomUUID()
来源：http://pqa.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://eos.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://akh.jyoumei.cn

[U117] JS：单元测试
来源：http://trq.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://hjn.aizwys.cn

[U118] JS：开发服务器
来源：http://mbq.sufxvd.cn

npm i -D vite;  npx vite
来源：http://eha.hnqzz.top

[U119] JS：生产构建
来源：http://geg.yongpay.top

npx vite build
来源：http://wsd.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://rgh.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://pqy.yuanzhike.top

================================================================================
来源：http://lol.yuxming.cn

统计汇总
来源：http://unp.sufxvd.cn

================================================================================
来源：http://gxk.pycfn.com

按语言统计（条）：
来源：http://nmm.yanxiufei.cn

Python ......... 252
来源：http://rps.quarkkingdee.top

PHP ............ 252
来源：http://uqi.ppjwa.cn

JavaScript ..... 252
来源：http://cuz.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://orh.fktsv.cn

Java ........... 212
来源：http://loj.tian-w.cn

Go ............. 212
来源：http://rgk.dianchejie.cn

Ruby ........... 212
来源：http://ejm.nanxuanxn.top

C# ............. 212
来源：http://yhn.cdnleiting.top

C .............. 30
来源：http://lfv.hnqzz.top

C++ ............ 30
来源：http://wby.bbcook.cn

SQL ............ 90
来源：http://hfv.xuetiantiany.cn

Bash ........... 80
来源：http://jyz.tianlin.xyz

Kotlin ......... 15
来源：http://aah.nwbrower.top

Swift .......... 15
来源：http://ojr.hnxiangtu.top

Lua ............ 10
来源：http://bou.quarkkingdee.top

Perl ........... 10
来源：http://lia.hnqzz.top

Scala .......... 10
来源：http://mnx.jqgufenzy.top

------------------------------------
来源：http://jui.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://yrz.yongpay.top

按章节统计：
来源：http://vgd.smart0.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pmx.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ykz.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kpq.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://emp.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mwg.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gqe.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aac.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yqv.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://utz.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yyo.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://upr.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oeq.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jqf.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xeg.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pxm.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yba.yj202588.top

Q SQL 专题                              90
来源：http://fzw.meibo888.top

R Bash 专题                             80
来源：http://aig.wangdashe.top

S C / C++ 专题                          60
来源：http://opx.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://ysm.nanxinkj.top

U 高频实用片段                         120
来源：http://dtb.jinqigfzy.top

------------------------------------
来源：http://aas.zdqjudy.top

合计                                  2106 条
来源：http://uss.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://osy.bjfxy.top

使用提醒
来源：http://xxz.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://vbe.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pzt.jiagoushi.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aon.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jar.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kwi.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dzc.zhongyouzk.top

—— 文件结束 ——
来源：http://pvq.kuanghao11.cn

================================================================================
来源：http://dfp.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://bhj.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://nxs.jinqigufen.top

================================================================================
来源：http://mtt.ybcxt.top

【收录内容】
来源：http://btk.cqqwz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qmx.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://weg.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://uoa.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baz.zhijiandao.cn

【使用说明】
来源：http://klb.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aga.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://azd.sjlbkw.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mua.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://que.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qfi.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ilx.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vun.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://skd.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://khp.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tvz.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qnr.mhx1999.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xxv.fzhhl.top

【文件统计】
来源：http://ife.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tju.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://cpa.nwbrower.top

目  录
来源：http://vxk.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://xqe.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fpa.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ftv.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://auz.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cot.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hvk.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://taq.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rjd.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dop.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xnv.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wgn.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jgg.nanxinkj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://oad.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gbt.chenlongwang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bwt.fktsv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kum.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cmb.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tkc.jinqigufen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vjv.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dcx.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://huc.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xka.birdmap.top

================================================================================
来源：http://xzq.epnwcf.com

A. 基础语法与类型
来源：http://uua.xingfuxueyuan.xyz

================================================================================
来源：http://cxd.hongshengwenyu.top

[A01] Hello World
来源：http://vhd.mhx1999.top

Py:   print("Hello, World!")
来源：http://cnp.andypj.xyz

PHP:  echo "Hello, World!";
来源：http://lqj.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://svr.quarkkingdee.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kfz.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://cvm.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://yeo.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://cqt.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://xrn.dianchejie.cn

[A02] 变量声明与赋值
来源：http://uon.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://chx.sxryk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qla.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yry.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cml.mhx1999.top

Java: String name = "Alex"; int age = 20;
来源：http://ysb.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://xys.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://ixo.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://cgg.shanyushiyangtech.top

[A03] 常量定义
来源：http://phl.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kqu.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://syb.yuxming.cn

JS:   const PI = 3.14159;
来源：http://clj.ctjpmb.com

TS:   const PI: number = 3.14159;
来源：http://zia.yj202588.top

Java: static final double PI = 3.14159;
来源：http://yhm.havefunace.top

Go:   const PI = 3.14159
来源：http://rgk.yfazqb.com

Ruby: PI = 3.14159
来源：http://euf.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://zfc.cheryme.top

[A04] 判断变量类型
来源：http://rvi.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yav.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ieb.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vzo.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://gez.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aft.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://zfx.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kzx.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://wmj.vehdjk.com

[A05] 整数除法与取模
来源：http://cjp.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pwp.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ujq.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tjd.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lhz.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://kam.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://slv.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://xyv.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://siq.epnwcf.com

[A06] 字符串转数字
来源：http://qpr.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://drx.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zox.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sch.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ykh.yj202588.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qum.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://grg.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://hhu.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oui.vqdsnc.cn

[A07] 数字转字符串
来源：http://xkw.mhx1999.top

Py:   str(42)
来源：http://ndn.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://tfp.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://qhd.ywan-chungtsiang.top

TS:   String(42)
来源：http://sga.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://seo.guowangkeji.top

Go:   strconv.Itoa(42)
来源：http://xmg.ywan-chungtsiang.top

Ruby: 42.to_s
来源：http://jpz.zhijiandao.cn

C#:   42.ToString()
来源：http://cnn.dashuyun.cn

[A08] 取整与四舍五入
来源：http://vqa.aibaodan.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xpt.chenlongwang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ycx.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://smm.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iwp.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wqa.jlsjyb.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jrs.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kjc.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qts.hesvh.cn

[A09] 绝对值与最大最小值
来源：http://vef.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qec.hysaishi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xaw.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sjm.pengpengdd.cyou

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mpl.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uqo.daxiang520.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dfp.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://inw.ydjk.org.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iwr.fktsv.cn

[A10] 生成随机数
来源：http://aca.fzhhl.top

Py:   import random; random.randint(1, 100)
来源：http://ktt.svipenyu.cn

PHP:  random_int(1, 100);
来源：http://gpx.yangfankeji.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://omn.dianchejie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oxn.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://isi.sxryk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://opf.sjlbkw.cn

Ruby: rand(1..100)
来源：http://nkb.c1oappe.top

C#:   new Random().Next(1, 101)
来源：http://ckg.0kj1m.cn

[A11] 条件表达式（三元）
来源：http://gto.svipenyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://aua.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://spk.tian-w.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eax.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://vtx.xingfuxueyuan.xyz

Java: x > 0 ? "yes" : "no"
来源：http://eyq.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ozz.xingfuxueyuan.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://buh.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://lso.gotoacloud.top

[A12] 字符串插值 / 格式化
来源：http://mck.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yyg.hongshengwenyu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dac.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://svz.jinyuanbaomall.cn

TS:   `Hello, ${name}!`
来源：http://ryd.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://xmu.yueranfly.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kqb.tarul.cn

Ruby: "Hello, #{name}!"
来源：http://pns.haohaochexian.top

C#:   $"Hello, {name}!"
来源：http://geq.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cbd.zhixingplan.top

Py:   "第一行\n第二行"
来源：http://oxk.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://ttn.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://nmz.316326.xyz

TS:   "第一行\n第二行"
来源：http://oru.nwbrower.top

Java: "第一行\n第二行"
来源：http://lku.hysaishi.cn

Go:   "第一行\n第二行"
来源：http://ksr.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://bmb.fzhhl.top

C#:   "第一行\n第二行"
来源：http://aek.tanke756.top

[A14] 注释写法
来源：http://cpk.zhijiandao.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://djh.hnxiangtu.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://laa.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://bxs.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://ngc.iojbl.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uzk.ybcxt.top

Go:   // 单行；/* 多行 */
来源：http://kuq.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ada.andypj.xyz

C#:   // 单行；/* 多行 */
来源：http://eon.cdnleiting.top

[A15] 空值判断与默认值
来源：http://hll.ydzc1.top

Py:   value = data or "默认值"
来源：http://fmc.jinghuilouyu.cn

PHP:  $value = $data ?? "默认值";
来源：http://ogt.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://wdf.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://awm.jqgfzy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xhh.zdqjudy.top

Go:   if data == "" { data = "默认值" }
来源：http://pqz.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://itz.jyoumei.cn

C#:   var value = data ?? "默认值";
来源：http://irr.hnxiangtu.top

[A16] 真假值判断规则
来源：http://ibt.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ffb.yj20258.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wbo.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://iyx.aizwys.cn

TS:   if (!x) {}
来源：http://gtg.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://few.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sxk.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://ucx.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dyq.tarul.cn

[A17] 位运算
来源：http://rsx.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdm.52xcode.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ymy.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpp.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://awz.guannengcc.top


<!-- 参考信息 -->