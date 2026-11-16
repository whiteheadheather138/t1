代发 wailian999

[U95] JS：Promise 包装
来源：http://ckm.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://jiu.smart0.xyz

[U96] JS：async/await 与异常
来源：http://qpq.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zxn.meibo888.top

[U97] JS：并发请求
来源：http://bpk.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://vmw.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://nwn.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kkc.yangfankeji.com

[U99] JS：事件监听
来源：http://cip.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://dqf.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://cmy.smart0.xyz

document.querySelector(".item")
来源：http://ldq.jiagoushi.top

[U101] JS：classList 操作
来源：http://ymj.chenlongwang.top

el.classList.toggle("active")
来源：http://yte.hysaishi.cn

[U102] JS：本地存储
来源：http://vya.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ynz.birdmap.top

[U103] JS：定时器
来源：http://gux.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wlz.yfazqb.com

[U104] JS：防抖
来源：http://igi.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwb.shanyushiyangkeji.top

[U105] JS：节流
来源：http://gke.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hey.hesvh.cn

[U106] JS：日期格式化
来源：http://ckf.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://klc.jyoumei.cn

[U107] JS：数字千分位
来源：http://qqe.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rdg.shzxlz.cn

[U108] JS：随机整数
来源：http://fqx.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ybh.xylfe.cn

[U109] JS：数组分组
来源：http://mbk.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://oyn.tianlin.xyz

[U110] JS：数组分块
来源：http://emt.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aqr.ehwqpu.com

[U111] JS：对象转 Map
来源：http://jax.meibo888.top

new Map(Object.entries(obj))
来源：http://zag.yj20258888.top

[U112] JS：字符串补位
来源：http://pzw.fktsv.cn

"7".padStart(3, "0")
来源：http://byz.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://hgq.daria6918.cn

s.replaceAll("a", "b")
来源：http://bir.havefunace.top

[U114] JS：JSON 深比较
来源：http://rra.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qnp.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://jyl.xuanzx.com

crypto.randomUUID()
来源：http://kxj.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://vmu.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://fqu.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://rtv.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://ivp.ehwqpu.com

[U118] JS：开发服务器
来源：http://cjb.ivvv.top

npm i -D vite;  npx vite
来源：http://ayf.chenjidiqi.icu

[U119] JS：生产构建
来源：http://lip.mhx1999.top

npx vite build
来源：http://grb.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://kto.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://mjj.kuanghao11.cn

================================================================================
来源：http://glc.zdbjq.cn

统计汇总
来源：http://gtk.bbcook.cn

================================================================================
来源：http://gpq.sweek.top

按语言统计（条）：
来源：http://cxq.yueranfly.top

Python ......... 252
来源：http://dgs.shangyingyoupin.top

PHP ............ 252
来源：http://byp.yuanzhike.top

JavaScript ..... 252
来源：http://nej.daxiang520.top

TypeScript ..... 212
来源：http://xrm.jianghu66.top

Java ........... 212
来源：http://qty.xuetiantiany.cn

Go ............. 212
来源：http://lhr.hnqzz.top

Ruby ........... 212
来源：http://kfg.yfazqb.com

C# ............. 212
来源：http://ubb.yongpay.top

C .............. 30
来源：http://fje.yangfankeji.com

C++ ............ 30
来源：http://hmh.tian-w.cn

SQL ............ 90
来源：http://iyo.jinqigfzy.top

Bash ........... 80
来源：http://quu.yfazqb.com

Kotlin ......... 15
来源：http://kmi.fktsv.cn

Swift .......... 15
来源：http://nse.andypj.xyz

Lua ............ 10
来源：http://dqf.yuxming.cn

Perl ........... 10
来源：http://hhs.hcnkem.com

Scala .......... 10
来源：http://nuv.zhoulong.xyz

------------------------------------
来源：http://kfv.yongpay.top

合计 ........... 2106 条
来源：http://vpp.9152youxi.cn

按章节统计：
来源：http://ckr.svipenyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pxl.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nso.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yag.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vuy.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xtl.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zff.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://inr.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://acf.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://khc.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://woe.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cdh.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aid.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oem.zdqjudy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gbw.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ycl.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://now.fehbvm.com

Q SQL 专题                              90
来源：http://vem.chenlongwang.top

R Bash 专题                             80
来源：http://peq.epnwcf.com

S C / C++ 专题                          60
来源：http://iqd.xziqi.cn

T 其他语言补充                          60
来源：http://dmi.fehbvm.com

U 高频实用片段                         120
来源：http://ttb.ybcxt.top

------------------------------------
来源：http://qms.jqgfzy.top

合计                                  2106 条
来源：http://ajm.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://klu.hfpthk.cn

使用提醒
来源：http://lii.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://fgl.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cnf.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bvg.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ckv.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uhn.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mga.xuetiantiany.cn

—— 文件结束 ——
来源：http://fbn.jqgufenzy.top

================================================================================
来源：http://gfs.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://ail.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://lmm.shangyingyoupin.top

================================================================================
来源：http://vht.xinyue.icu

【收录内容】
来源：http://tpm.jinghuilouyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mny.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dxx.aibaodan.cn

SQL · Bash · C · C++
来源：http://qiu.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sda.yj202588.top

【使用说明】
来源：http://jyl.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ire.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://siq.xingfuxueyuan.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dbl.uphjek.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ibd.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dio.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://naw.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://esm.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nfd.yj202588.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sxt.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gxi.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://emf.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lzp.chenzaomai.com

【文件统计】
来源：http://nkm.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fwu.yonumen.top

--------------------------------------------------------------------------------
来源：http://udz.dashuyun.cn

目  录
来源：http://tox.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://tjz.guowangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uwz.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cmp.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iex.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zmo.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xtp.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rhq.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nek.pycfn.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rmw.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://egp.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uyf.chenjidiqi.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eig.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rcg.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dmi.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://thv.52xcode.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vib.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kvb.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cck.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yro.jqgfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lzm.daxiang520.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://txx.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ydc.tianlin.xyz

================================================================================
来源：http://jck.dashuyun.cn

A. 基础语法与类型
来源：http://uev.hongshengwenyu.top

================================================================================
来源：http://pof.xylfe.cn

[A01] Hello World
来源：http://jfv.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://mxq.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://xet.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://fvf.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rjx.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://ymd.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://xbx.ivvv.top

Ruby: puts "Hello, World!"
来源：http://lub.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://zwr.zdbjq.cn

[A02] 变量声明与赋值
来源：http://gup.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tci.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qfw.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gpg.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dsh.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://ytw.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://ymt.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://hbr.guannengcc.top

C#:   string name = "Alex"; int age = 20;
来源：http://mih.ywan-chungtsiang.top

[A03] 常量定义
来源：http://smw.daxiang520.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rsr.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://fse.feifeiyinyue.top

JS:   const PI = 3.14159;
来源：http://pfs.xingfuxueyuan.xyz

TS:   const PI: number = 3.14159;
来源：http://wcp.snrcjt.cn

Java: static final double PI = 3.14159;
来源：http://bdc.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://uli.jyoumei.cn

Ruby: PI = 3.14159
来源：http://ttg.gzhubu.top

C#:   const double PI = 3.14159;
来源：http://faq.316326.xyz

[A04] 判断变量类型
来源：http://gpw.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hfx.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lfl.sjlbkw.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lqm.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://oxj.nanxinkj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hiv.pengpengdd.cyou

Go:   reflect.TypeOf(x).Name()
来源：http://edx.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wtm.gzhubu.top

C#:   x.GetType().Name; x is int
来源：http://ogd.hammf.cn

[A05] 整数除法与取模
来源：http://qut.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fmf.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iem.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gts.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zbf.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://qea.c1oappe.top

Go:   7 / 2; 7 % 2
来源：http://uti.jianghu66.top

Ruby: 7 / 2; 7 % 2
来源：http://zyf.yuxming.cn

C#:   7 / 2; 7 % 2
来源：http://rop.daria6918.cn

[A06] 字符串转数字
来源：http://rqt.tarul.cn

Py:   int("42"); float("3.14")
来源：http://uhm.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pjs.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gra.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://esj.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pzp.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://njq.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://oil.hcnkem.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eps.meibo888.top

[A07] 数字转字符串
来源：http://mzn.bjfxy.top

Py:   str(42)
来源：http://rto.kuanghao11.cn

PHP:  (string) 42; strval(42)
来源：http://tcr.guannengcc.top

JS:   String(42); (42).toString()
来源：http://ool.gzhubu.top

TS:   String(42)
来源：http://rxx.wangdashe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dlj.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://qnq.hammf.cn

Ruby: 42.to_s
来源：http://aff.gogol.net.cn

C#:   42.ToString()
来源：http://pbb.epnwcf.com

[A08] 取整与四舍五入
来源：http://xax.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bpy.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lfz.aizwys.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eov.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://grk.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cot.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xsh.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://rfy.feifeiyinyue.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hqn.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://sjq.yangfankeji.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ahh.quarkkingdee.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rvm.ehwqpu.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ssr.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hsv.nanxuanxn.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ayj.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zwo.ppjwa.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://met.gaohongyu789.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jta.tianlin.xyz

[A10] 生成随机数
来源：http://wky.birdmap.top

Py:   import random; random.randint(1, 100)
来源：http://amo.tanke756.top

PHP:  random_int(1, 100);
来源：http://uns.316326.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://byo.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xgy.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://bby.hammf.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rwj.smart0.xyz

Ruby: rand(1..100)
来源：http://uze.ppjwa.cn

C#:   new Random().Next(1, 101)
来源：http://iuh.fengsongda.top

[A11] 条件表达式（三元）
来源：http://fya.daxiang520.top

Py:   "yes" if x > 0 else "no"
来源：http://ipl.chenjidiqi.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://gxx.hongshengwenyu.top

JS:   x > 0 ? "yes" : "no"
来源：http://kkj.andypj.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://vyr.bbcook.cn

Java: x > 0 ? "yes" : "no"
来源：http://okp.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tug.yonumen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mxx.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://twn.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://rmq.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ohs.tarul.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sjk.feifeiyinyue.top

JS:   `Hello, ${name}!`
来源：http://xxp.nanxuanxn.top

TS:   `Hello, ${name}!`
来源：http://bdr.hesvh.cn

Java: "Hello, %s!".formatted(name)
来源：http://uro.yanxiufei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://stl.yfazqb.com

Ruby: "Hello, #{name}!"
来源：http://rtr.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://kln.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hjv.yongpay.top

Py:   "第一行\n第二行"
来源：http://tjd.ehwqpu.com

PHP:  "第一行\n第二行"
来源：http://gzj.fengsongda.top

JS:   "第一行\n第二行"
来源：http://oiq.bjfxy.top

TS:   "第一行\n第二行"
来源：http://cyi.sjlbkw.cn

Java: "第一行\n第二行"
来源：http://rlf.smart0.xyz

Go:   "第一行\n第二行"
来源：http://vay.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://kla.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://jxq.zdbjq.cn

[A14] 注释写法
来源：http://cdi.birdmap.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://aya.shangyingyoupin.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yko.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://lrt.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://gif.xylfe.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iyz.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://shf.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://yny.yj202588.top

C#:   // 单行；/* 多行 */
来源：http://izp.havefunace.top

[A15] 空值判断与默认值
来源：http://yqv.jqgfzy.top

Py:   value = data or "默认值"
来源：http://ayz.redwolf501.top

PHP:  $value = $data ?? "默认值";
来源：http://tgk.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://yxm.ywan-chungtsiang.top

TS:   const value = data ?? "默认值";
来源：http://lan.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bsz.xuetiantiany.cn

Go:   if data == "" { data = "默认值" }
来源：http://jog.sweek.top

Ruby: value = data || "默认值"
来源：http://ufc.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://mbz.andypj.xyz

[A16] 真假值判断规则
来源：http://ybz.yueranfly.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rwf.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://phj.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lpj.ctjpmb.com

TS:   if (!x) {}
来源：http://pfm.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rny.yueranfly.top


<!-- 参考信息 -->