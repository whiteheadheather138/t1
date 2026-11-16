代发 wailian999

[U95] JS：Promise 包装
来源：http://oho.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://off.xinyue.icu

[U96] JS：async/await 与异常
来源：http://lsd.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://olx.haohaochexian.top

[U97] JS：并发请求
来源：http://ozq.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fbq.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://tln.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gjv.fengsongda.top

[U99] JS：事件监听
来源：http://xps.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://dxl.bjfxy.top

[U100] JS：DOM 查询
来源：http://sik.ppjwa.cn

document.querySelector(".item")
来源：http://gzb.zhijiandao.cn

[U101] JS：classList 操作
来源：http://bfj.yuanzhike.top

el.classList.toggle("active")
来源：http://umh.xinyue.icu

[U102] JS：本地存储
来源：http://ouw.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://nid.guannengcc.top

[U103] JS：定时器
来源：http://ejg.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fsr.zhiwuduotai.top

[U104] JS：防抖
来源：http://xrh.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qly.xziqi.cn

[U105] JS：节流
来源：http://hfm.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yet.yj20258888.top

[U106] JS：日期格式化
来源：http://ztb.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tyw.nanxuanxn.top

[U107] JS：数字千分位
来源：http://mdy.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nmz.ppjwa.cn

[U108] JS：随机整数
来源：http://kzl.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qgi.jlsjyb.cn

[U109] JS：数组分组
来源：http://exu.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://lqj.tianlin.xyz

[U110] JS：数组分块
来源：http://qnk.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zpy.9152youxi.cn

[U111] JS：对象转 Map
来源：http://nup.fzhhl.top

new Map(Object.entries(obj))
来源：http://cgd.fzhhl.top

[U112] JS：字符串补位
来源：http://noi.xuanzx.com

"7".padStart(3, "0")
来源：http://zkz.hcnkem.com

[U113] JS：正则替换全部
来源：http://clc.sysykeji.top

s.replaceAll("a", "b")
来源：http://tyv.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://ovm.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mnl.tanke756.top

[U115] JS：生成 UUID
来源：http://yqr.ydjk.org.cn

crypto.randomUUID()
来源：http://yrq.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://lgi.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://uqr.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://jmt.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://mfp.jyoumei.cn

[U118] JS：开发服务器
来源：http://tnv.tianlin.xyz

npm i -D vite;  npx vite
来源：http://ioo.svipenyu.cn

[U119] JS：生产构建
来源：http://koq.iojbl.cn

npx vite build
来源：http://prk.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://qqc.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://rbr.feifeiyinyue.top

================================================================================
来源：http://lwz.jlsjyb.cn

统计汇总
来源：http://bqb.zhiwuduotai.top

================================================================================
来源：http://rlw.zycfv.cn

按语言统计（条）：
来源：http://xpt.quarkkingdee.top

Python ......... 252
来源：http://vbh.jinqigfzy.top

PHP ............ 252
来源：http://vxi.nanxinkj.top

JavaScript ..... 252
来源：http://zxd.yuanzhike.top

TypeScript ..... 212
来源：http://xlc.jinghuilouyu.cn

Java ........... 212
来源：http://qug.sxryk.cn

Go ............. 212
来源：http://goq.hammf.cn

Ruby ........... 212
来源：http://oob.xuetiantiany.cn

C# ............. 212
来源：http://azs.chenlongwang.top

C .............. 30
来源：http://ron.epnwcf.com

C++ ............ 30
来源：http://zei.sjlbkw.cn

SQL ............ 90
来源：http://vai.cqqwz.cn

Bash ........... 80
来源：http://kry.dianchejie.cn

Kotlin ......... 15
来源：http://csn.havefunace.top

Swift .......... 15
来源：http://dok.shanyushiyangtech.top

Lua ............ 10
来源：http://gjf.gogol.net.cn

Perl ........... 10
来源：http://zgw.tarul.cn

Scala .......... 10
来源：http://vdi.meibo888.top

------------------------------------
来源：http://htz.zhiwuduotai.top

合计 ........... 2106 条
来源：http://lzq.mhx1999.top

按章节统计：
来源：http://ude.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nrh.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wod.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xkw.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vxk.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rzg.hysaishi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aiu.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://twq.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://enp.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tjz.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dkj.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pgu.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://moh.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zrk.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pes.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hjb.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zjv.havefunace.top

Q SQL 专题                              90
来源：http://dqi.hfpthk.cn

R Bash 专题                             80
来源：http://lzy.kuanghao11.cn

S C / C++ 专题                          60
来源：http://xxt.yfazqb.com

T 其他语言补充                          60
来源：http://xgy.ehwqpu.com

U 高频实用片段                         120
来源：http://ctt.9152youxi.cn

------------------------------------
来源：http://owi.guowangkeji.top

合计                                  2106 条
来源：http://ryj.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://cth.yongpay.top

使用提醒
来源：http://qul.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://foc.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dtu.yuxming.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://seh.316326.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tqn.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wse.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bwx.zhongyouzk.top

—— 文件结束 ——
来源：http://kpk.bbcook.cn

================================================================================
来源：http://rfw.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://imv.gzhubu.top

Common Programming Examples Cheat Book
来源：http://hna.sufxvd.cn

================================================================================
来源：http://pjp.fanxiaobao.xyz

【收录内容】
来源：http://kmp.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lpz.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lah.fengsongda.top

SQL · Bash · C · C++
来源：http://zaw.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nfu.yuxming.cn

【使用说明】
来源：http://ebi.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mnm.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qjg.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xxo.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nmt.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fre.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sjl.jinqigfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jsh.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tfx.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://daj.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yjo.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ewh.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pcx.jiagoushi.top

【文件统计】
来源：http://rnb.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ucr.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://pfq.zdbjq.cn

目  录
来源：http://zly.fzhhl.top

--------------------------------------------------------------------------------
来源：http://box.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lde.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nba.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://squ.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ddz.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ddn.yangfankeji.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gtp.hnxiangtu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qrr.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mde.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bqt.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ynw.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://owj.yfazqb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bsg.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yei.nanxinkj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nyt.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gzk.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zip.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zqa.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://skh.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uye.andypj.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rhp.tanke756.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vfh.vehdjk.com

================================================================================
来源：http://vna.aibaodan.cn

A. 基础语法与类型
来源：http://rxo.ppjwa.cn

================================================================================
来源：http://hsl.gaohongyu789.top

[A01] Hello World
来源：http://lbq.c1oappe.top

Py:   print("Hello, World!")
来源：http://uoh.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://exm.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://ftw.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cul.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://rwz.feifeiyinyue.top

Go:   fmt.Println("Hello, World!")
来源：http://yvg.ydzc1.top

Ruby: puts "Hello, World!"
来源：http://tcb.havefunace.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kuw.zhengqikj.top

[A02] 变量声明与赋值
来源：http://wmi.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ktx.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://drj.quarkkingdee.top

JS:   let name = "Alex"; const age = 20;
来源：http://vue.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pxn.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://hoi.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://oxt.hnqzz.top

Ruby: name = "Alex"; age = 20
来源：http://bkx.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://dmx.hnqzz.top

[A03] 常量定义
来源：http://jxz.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nzr.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://qnj.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://njc.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://far.hnqzz.top

Java: static final double PI = 3.14159;
来源：http://ykk.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://qwg.hnqzz.top

Ruby: PI = 3.14159
来源：http://dil.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://rzm.yuanzhike.top

[A04] 判断变量类型
来源：http://wqn.zhijiandao.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ptv.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kgx.tanke756.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iks.jqgfzy.top

TS:   typeof x; x instanceof Date
来源：http://czs.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tkf.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rto.snrcjt.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gdl.shzxlz.cn

C#:   x.GetType().Name; x is int
来源：http://ctv.andypj.xyz

[A05] 整数除法与取模
来源：http://wmj.yongpay.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ywi.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dhw.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iaj.uphjek.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dhq.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://bhg.ivvv.top

Go:   7 / 2; 7 % 2
来源：http://yzf.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://bbw.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://zrm.jiagoushi.top

[A06] 字符串转数字
来源：http://ibj.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://dmh.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kwg.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ooh.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://nwd.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xuv.sweek.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dey.quarkkingdee.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zjw.mhx1999.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ibb.sweek.top

[A07] 数字转字符串
来源：http://cqr.52xcode.cn

Py:   str(42)
来源：http://ysl.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://lqn.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://imp.zhaomingkeji.xyz

TS:   String(42)
来源：http://ptf.nanxuanxn.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lsy.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://wdb.zdbjq.cn

Ruby: 42.to_s
来源：http://pjw.yuxming.cn

C#:   42.ToString()
来源：http://kfm.jiagoushi.top

[A08] 取整与四舍五入
来源：http://osj.cqqwz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rfs.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ceq.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wtn.jinqigfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xpq.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nci.xuetiantiany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vae.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dug.xinyue.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xon.kuanghao11.cn

[A09] 绝对值与最大最小值
来源：http://yab.yvedp.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xrl.xziqi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://inz.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dth.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mtp.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vec.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kfp.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ijt.tianlin.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ehf.yuanzhike.top

[A10] 生成随机数
来源：http://vbv.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://kbi.meibo888.top

PHP:  random_int(1, 100);
来源：http://jwh.cashguo.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dha.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tuc.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://obb.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xwt.quarkkingdee.top

Ruby: rand(1..100)
来源：http://fef.dianchejie.cn

C#:   new Random().Next(1, 101)
来源：http://pkr.hnqzz.top

[A11] 条件表达式（三元）
来源：http://jnz.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://usv.tarul.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bmo.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jds.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://jos.xuanzx.com

Java: x > 0 ? "yes" : "no"
来源：http://eqx.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wlv.yj20258.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wpt.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://zms.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://rrv.chenzaomai.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hdr.kuanghao11.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mkn.cashguo.top

JS:   `Hello, ${name}!`
来源：http://qfp.ivvv.top

TS:   `Hello, ${name}!`
来源：http://ztm.jqgfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://fwd.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fwu.feifeiyinyue.top

Ruby: "Hello, #{name}!"
来源：http://zyy.yj202588.top

C#:   $"Hello, {name}!"
来源：http://peg.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://unx.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://nng.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://sec.guannengcc.top

JS:   "第一行\n第二行"
来源：http://vfa.dashuyun.cn

TS:   "第一行\n第二行"
来源：http://gpq.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://bep.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://zcf.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://zef.yj20258888.top

C#:   "第一行\n第二行"
来源：http://qqw.jyoumei.cn

[A14] 注释写法
来源：http://qzg.hnqzz.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yxk.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://med.hfpthk.cn

JS:   // 单行；/* 多行 */
来源：http://djf.shzxlz.cn

TS:   // 单行；/* 多行 */
来源：http://vkf.dianchejie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://whc.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://ogi.andypj.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://kom.zhixingplan.top

C#:   // 单行；/* 多行 */
来源：http://ufx.aizwys.cn

[A15] 空值判断与默认值
来源：http://eal.sufxvd.cn

Py:   value = data or "默认值"
来源：http://hsc.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://olg.bbcook.cn

JS:   const value = data ?? "默认值";
来源：http://fps.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://xvf.xuetiantiany.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qjb.xuetiantiany.cn

Go:   if data == "" { data = "默认值" }
来源：http://rcr.yj20258888.top

Ruby: value = data || "默认值"
来源：http://nyr.wangshuangyany.cn

C#:   var value = data ?? "默认值";
来源：http://xxj.yuxming.cn

[A16] 真假值判断规则
来源：http://los.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qct.0kj1m.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yvt.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xsu.feifeiyinyue.top

TS:   if (!x) {}
来源：http://voj.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uhb.tianlin.xyz


<!-- 参考信息 -->