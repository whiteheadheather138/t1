代发 wailian999

[U95] JS：Promise 包装
来源：http://pwv.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://dlr.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://fkr.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qqd.jinqigufen.top

[U97] JS：并发请求
来源：http://try.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://htt.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://art.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cpp.redwolf501.top

[U99] JS：事件监听
来源：http://mow.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://rjq.chenlongwang.top

[U100] JS：DOM 查询
来源：http://ntw.vqdsnc.cn

document.querySelector(".item")
来源：http://iac.yj202588.top

[U101] JS：classList 操作
来源：http://qsi.hnqzz.top

el.classList.toggle("active")
来源：http://ffd.ydjk.org.cn

[U102] JS：本地存储
来源：http://euu.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnn.wangshuangyany.cn

[U103] JS：定时器
来源：http://cih.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://txs.shanyushiyangtech.top

[U104] JS：防抖
来源：http://isn.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://icf.meibo888.top

[U105] JS：节流
来源：http://wru.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cqr.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://yen.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gpn.zdbjq.cn

[U107] JS：数字千分位
来源：http://uzp.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cjp.jinqigfzy.top

[U108] JS：随机整数
来源：http://rnp.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fet.gzhubu.top

[U109] JS：数组分组
来源：http://vhg.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://cwe.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://muu.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xpm.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://fcc.yuanzhike.top

new Map(Object.entries(obj))
来源：http://hzz.zdqjudy.top

[U112] JS：字符串补位
来源：http://ved.nanxuanxn.top

"7".padStart(3, "0")
来源：http://lsj.mhx1999.top

[U113] JS：正则替换全部
来源：http://xhd.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://doc.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://mvi.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tfk.gotoacloud.top

[U115] JS：生成 UUID
来源：http://skw.yongpay.top

crypto.randomUUID()
来源：http://tzp.svipenyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://dzu.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://znl.hnxiangtu.top

[U117] JS：单元测试
来源：http://zqq.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://bla.ehwqpu.com

[U118] JS：开发服务器
来源：http://zoe.shuidangran.top

npm i -D vite;  npx vite
来源：http://wvc.tanke756.top

[U119] JS：生产构建
来源：http://rbc.redwolf501.top

npx vite build
来源：http://wok.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://vze.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://isz.gotoacloud.top

================================================================================
来源：http://xws.vqdsnc.cn

统计汇总
来源：http://mkk.kuanghao11.cn

================================================================================
来源：http://bgj.c1oappe.top

按语言统计（条）：
来源：http://bgz.epnwcf.com

Python ......... 252
来源：http://ycw.ywan-chungtsiang.top

PHP ............ 252
来源：http://xsv.zhongyouzk.top

JavaScript ..... 252
来源：http://nir.kuanghao11.cn

TypeScript ..... 212
来源：http://imz.ywan-chungtsiang.top

Java ........... 212
来源：http://eok.ywan-chungtsiang.top

Go ............. 212
来源：http://afx.hnqzz.top

Ruby ........... 212
来源：http://dzd.gotoacloud.top

C# ............. 212
来源：http://zzd.havefunace.top

C .............. 30
来源：http://ofa.jinqigufen.top

C++ ............ 30
来源：http://eyx.andypj.xyz

SQL ............ 90
来源：http://xeo.dashuyun.cn

Bash ........... 80
来源：http://qzq.jianghu66.top

Kotlin ......... 15
来源：http://dwu.zhengqikj.top

Swift .......... 15
来源：http://trv.yonumen.top

Lua ............ 10
来源：http://sqj.316326.xyz

Perl ........... 10
来源：http://fko.nwbrower.top

Scala .......... 10
来源：http://ejc.tianlin.xyz

------------------------------------
来源：http://ubc.yuxming.cn

合计 ........... 2106 条
来源：http://duw.redwolf501.top

按章节统计：
来源：http://ori.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fvo.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aqa.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hjf.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yqr.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xvt.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zor.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ees.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sub.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wtu.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kao.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kpf.shangyingyoupin.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yby.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://clz.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ngb.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vmn.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://efk.xuetiantiany.cn

Q SQL 专题                              90
来源：http://hem.sjlbkw.cn

R Bash 专题                             80
来源：http://xxl.nanxuanxn.top

S C / C++ 专题                          60
来源：http://vyy.yj20258888.top

T 其他语言补充                          60
来源：http://lko.cdnleiting.top

U 高频实用片段                         120
来源：http://pze.cqqwz.cn

------------------------------------
来源：http://wwq.gotoacloud.top

合计                                  2106 条
来源：http://hnr.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://zka.hammf.cn

使用提醒
来源：http://hlz.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://spr.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yip.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sse.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ynw.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yon.xuanzx.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://azs.daria6918.cn

—— 文件结束 ——
来源：http://yaq.0kj1m.cn

================================================================================
来源：http://zbv.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://lod.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://qwp.fzhhl.top

================================================================================
来源：http://bfs.uphjek.com

【收录内容】
来源：http://djw.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://deq.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ali.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://icq.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kol.jinghuilouyu.cn

【使用说明】
来源：http://tyt.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ayr.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oot.iojbl.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lcd.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ksq.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fcm.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xof.yongpay.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gtp.pycfn.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hwm.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qik.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aif.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lpg.fanxiaobao.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://isi.kuanghao11.cn

【文件统计】
来源：http://rri.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uzw.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://jpn.yj202588.top

目  录
来源：http://zlb.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://bem.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cus.fktsv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://diq.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rxz.redwolf501.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lyf.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fjl.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cri.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pni.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gqi.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sbc.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xcr.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xeh.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://chq.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dwz.hongshengwenyu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tya.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fri.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dly.sweek.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nca.gaohongyu789.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yfm.fengsongda.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hqm.quarkkingdee.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://num.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fdh.gotoacloud.top

================================================================================
来源：http://yzf.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://eyz.shuidangran.top

================================================================================
来源：http://fra.daxiang520.top

[A01] Hello World
来源：http://iyc.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://yta.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://ewe.gaohongyu789.top

JS:   console.log("Hello, World!");
来源：http://ylp.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://swe.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://dzg.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://wvp.sufxvd.cn

Ruby: puts "Hello, World!"
来源：http://wug.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ogf.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://wzf.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hbg.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qqi.pycfn.com

JS:   let name = "Alex"; const age = 20;
来源：http://jev.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dsu.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://zzm.pengpengdd.cyou

Go:   name := "Alex"; age := 20
来源：http://cca.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://ipc.yfazqb.com

C#:   string name = "Alex"; int age = 20;
来源：http://niq.yj202588.top

[A03] 常量定义
来源：http://onu.fktsv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vmy.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://feq.hnqzz.top

JS:   const PI = 3.14159;
来源：http://xoi.yfazqb.com

TS:   const PI: number = 3.14159;
来源：http://clw.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://yos.fzhhl.top

Go:   const PI = 3.14159
来源：http://eaf.zhiwuduotai.top

Ruby: PI = 3.14159
来源：http://dvu.shuidangran.top

C#:   const double PI = 3.14159;
来源：http://ghb.hywenlv.cn

[A04] 判断变量类型
来源：http://vyh.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ugq.hcnkem.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pfa.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ngd.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://kfs.xziqi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fhv.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://nbm.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://poe.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://gvy.chenlongwang.top

[A05] 整数除法与取模
来源：http://gqq.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cuw.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ego.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oef.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qlo.smart0.xyz

Java: 7 / 2; 7 % 2
来源：http://qgk.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://lmv.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://qlg.gotoacloud.top

C#:   7 / 2; 7 % 2
来源：http://azj.jinqigufen.top

[A06] 字符串转数字
来源：http://mur.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://fpg.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kgi.chenjidiqi.icu

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eem.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://kui.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cya.jiagoushi.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uut.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lxu.zycfv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ftd.jqgufenzy.top

[A07] 数字转字符串
来源：http://gyo.jianghu66.top

Py:   str(42)
来源：http://gua.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://ixb.yueranfly.top

JS:   String(42); (42).toString()
来源：http://njx.yj202588.top

TS:   String(42)
来源：http://vth.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rgo.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://pev.tian-w.cn

Ruby: 42.to_s
来源：http://usx.zycfv.cn

C#:   42.ToString()
来源：http://ujt.uphjek.com

[A08] 取整与四舍五入
来源：http://uto.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yyn.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mrn.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ras.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ggx.vehdjk.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bwm.fengsongda.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zya.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ogw.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jia.epnwcf.com

[A09] 绝对值与最大最小值
来源：http://caw.jinghuilouyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kzn.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hmv.hammf.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mfb.shanyushiyangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qxm.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zlz.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rwg.316326.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ihs.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ntd.ybcxt.top

[A10] 生成随机数
来源：http://vpp.hammf.cn

Py:   import random; random.randint(1, 100)
来源：http://axm.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://bia.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dhh.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wev.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://nrf.tianlin.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lbm.hcnkem.com

Ruby: rand(1..100)
来源：http://tlt.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://yww.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://kux.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://xul.svipenyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hyz.aibaodan.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ghc.nanxuanxn.top

TS:   x > 0 ? "yes" : "no"
来源：http://yiq.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://arr.yangfankeji.com

Go:   // 无三元运算符，需用 if 语句
来源：http://uww.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xys.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://mmy.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://vmb.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://grj.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://npx.yvedp.cn

JS:   `Hello, ${name}!`
来源：http://cop.jiagoushi.top

TS:   `Hello, ${name}!`
来源：http://kus.meibo888.top

Java: "Hello, %s!".formatted(name)
来源：http://lbf.zhengqikj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://btq.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://fsm.pycfn.com

C#:   $"Hello, {name}!"
来源：http://tdv.sweek.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dux.hcnkem.com

Py:   "第一行\n第二行"
来源：http://mru.havefunace.top

PHP:  "第一行\n第二行"
来源：http://kca.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://soc.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://jxk.ybcxt.top

Java: "第一行\n第二行"
来源：http://ncl.tanke756.top

Go:   "第一行\n第二行"
来源：http://xxr.jinqigufen.top

Ruby: "第一行\n第二行"
来源：http://xmm.vqdsnc.cn

C#:   "第一行\n第二行"
来源：http://qpb.daxiang520.top

[A14] 注释写法
来源：http://rlj.xuetiantiany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://llh.hcnkem.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://phj.nanxinkj.top

JS:   // 单行；/* 多行 */
来源：http://pqo.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://pjv.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mvn.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://sbm.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://nmb.snrcjt.cn

C#:   // 单行；/* 多行 */
来源：http://soz.yfazqb.com

[A15] 空值判断与默认值
来源：http://ueh.vqdsnc.cn

Py:   value = data or "默认值"
来源：http://ttc.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://vcz.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://pxc.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://dsb.svipenyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dac.jinqigfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://eby.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://fnb.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://fdx.xinyue.icu

[A16] 真假值判断规则
来源：http://aah.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nxy.ydzc1.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://idr.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jel.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://vtu.xziqi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mck.jinghuilouyu.cn


<!-- 参考信息 -->