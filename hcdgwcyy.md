代发 wailian999

[U97] JS：并发请求
来源：http://ipv.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gbu.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://jji.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://woh.shzxlz.cn

[U99] JS：事件监听
来源：http://sfk.vehdjk.com

el.addEventListener("click", e => {})
来源：http://iwf.redwolf501.top

[U100] JS：DOM 查询
来源：http://uyd.shangyingyoupin.top

document.querySelector(".item")
来源：http://ktt.xylfe.cn

[U101] JS：classList 操作
来源：http://fqy.iojbl.cn

el.classList.toggle("active")
来源：http://pso.zhijiandao.cn

[U102] JS：本地存储
来源：http://lwo.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fdz.fengsongda.top

[U103] JS：定时器
来源：http://nex.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dsf.fehbvm.com

[U104] JS：防抖
来源：http://shp.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vri.zhoulong.xyz

[U105] JS：节流
来源：http://xld.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yfn.hywenlv.cn

[U106] JS：日期格式化
来源：http://gft.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qgz.jqgfzy.top

[U107] JS：数字千分位
来源：http://jqb.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zio.hongshengwenyu.top

[U108] JS：随机整数
来源：http://rvx.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xkg.ybcxt.top

[U109] JS：数组分组
来源：http://une.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://pia.jqgfzy.top

[U110] JS：数组分块
来源：http://wxc.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rdp.yj20258888.top

[U111] JS：对象转 Map
来源：http://xws.sxryk.cn

new Map(Object.entries(obj))
来源：http://cwo.hesvh.cn

[U112] JS：字符串补位
来源：http://jtv.ehwqpu.com

"7".padStart(3, "0")
来源：http://oje.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://ikj.tianlin.xyz

s.replaceAll("a", "b")
来源：http://cpf.sysykeji.top

[U114] JS：JSON 深比较
来源：http://zji.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://vkn.uphjek.com

[U115] JS：生成 UUID
来源：http://zzq.wangshuangyany.cn

crypto.randomUUID()
来源：http://mtp.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://rkr.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://uur.gzhubu.top

[U117] JS：单元测试
来源：http://zop.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://zcx.hfpthk.cn

[U118] JS：开发服务器
来源：http://zaj.xziqi.cn

npm i -D vite;  npx vite
来源：http://lyj.cashguo.top

[U119] JS：生产构建
来源：http://kfq.cdnleiting.top

npx vite build
来源：http://lvj.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://kpu.ivvv.top

import.meta.env.VITE_API_URL
来源：http://ruj.jinghuilouyu.cn

================================================================================
来源：http://dxn.ywan-chungtsiang.top

统计汇总
来源：http://phq.jyoumei.cn

================================================================================
来源：http://yhr.gogol.net.cn

按语言统计（条）：
来源：http://yyx.sweek.top

Python ......... 252
来源：http://ldx.shanyushiyangtech.top

PHP ............ 252
来源：http://mmc.tanke756.top

JavaScript ..... 252
来源：http://wzs.xylfe.cn

TypeScript ..... 212
来源：http://lss.yvedp.cn

Java ........... 212
来源：http://gdp.zdqjudy.top

Go ............. 212
来源：http://uam.yanxiufei.cn

Ruby ........... 212
来源：http://vik.ehwqpu.com

C# ............. 212
来源：http://izs.sweek.top

C .............. 30
来源：http://akq.hongshengwenyu.top

C++ ............ 30
来源：http://yir.yj20258888.top

SQL ............ 90
来源：http://qmy.nanxinkj.top

Bash ........... 80
来源：http://tqq.shuidangran.top

Kotlin ......... 15
来源：http://vpf.zhaomingkeji.xyz

Swift .......... 15
来源：http://rle.yuxming.cn

Lua ............ 10
来源：http://zup.sxryk.cn

Perl ........... 10
来源：http://rpb.hnqzz.top

Scala .......... 10
来源：http://iio.hnqzz.top

------------------------------------
来源：http://hiv.hnxiangtu.top

合计 ........... 2106 条
来源：http://npu.yfazqb.com

按章节统计：
来源：http://xfn.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://izu.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tcq.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ikv.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wox.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jyu.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lti.fengsongda.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fnw.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://obp.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bua.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wsn.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jhf.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://khh.ybcxt.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mrn.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tvp.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qvc.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bki.redwolf501.top

Q SQL 专题                              90
来源：http://xzc.vqdsnc.cn

R Bash 专题                             80
来源：http://ipl.zdqjudy.top

S C / C++ 专题                          60
来源：http://rmr.fehbvm.com

T 其他语言补充                          60
来源：http://vle.xziqi.cn

U 高频实用片段                         120
来源：http://byf.jinqigfzy.top

------------------------------------
来源：http://bvc.jiagoushi.top

合计                                  2106 条
来源：http://sso.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://yxd.9152youxi.cn

使用提醒
来源：http://ivl.c1oappe.top

--------------------------------------------------------------------------------
来源：http://hkg.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ijr.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zuu.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xwj.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pyb.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bqa.hongshengwenyu.top

—— 文件结束 ——
来源：http://vsr.yongpay.top

================================================================================
来源：http://lmy.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://mxi.xylfe.cn

Common Programming Examples Cheat Book
来源：http://con.meibo888.top

================================================================================
来源：http://hav.xylfe.cn

【收录内容】
来源：http://vsk.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ovq.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ygc.shuidangran.top

SQL · Bash · C · C++
来源：http://ooh.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lcp.nanxinkj.top

【使用说明】
来源：http://lul.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vwz.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jae.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://owz.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qcn.yonumen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ipi.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tlq.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ndy.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ayx.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zkx.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yvs.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bce.jinghuilouyu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ofy.hammf.cn

【文件统计】
来源：http://exf.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qys.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://pth.aibaodan.cn

目  录
来源：http://ync.yongpay.top

--------------------------------------------------------------------------------
来源：http://gxa.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nbu.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://loq.meibo888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jrf.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cev.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uvy.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uct.chenlongwang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gyp.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://erp.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kyo.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ykl.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vqx.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hjn.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sic.meibo888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://efi.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bqm.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iap.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bjj.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xhv.9152youxi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qam.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ehc.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sds.pycfn.com

================================================================================
来源：http://bbe.ydjk.org.cn

A. 基础语法与类型
来源：http://btw.shangyingyoupin.top

================================================================================
来源：http://jus.fehbvm.com

[A01] Hello World
来源：http://kok.hfpthk.cn

Py:   print("Hello, World!")
来源：http://xrc.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://bde.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://pkb.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://beu.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://tkv.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://tud.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://raa.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://kjl.bjfxy.top

[A02] 变量声明与赋值
来源：http://gzv.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oro.pycfn.com

PHP:  $name = "Alex"; $age = 20;
来源：http://cyf.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bex.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sec.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://mjc.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://zku.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://vnj.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://qgl.yongpay.top

[A03] 常量定义
来源：http://amy.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pec.316326.xyz

PHP:  const PI = 3.14159;
来源：http://piv.hesvh.cn

JS:   const PI = 3.14159;
来源：http://ziw.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://lsy.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://rht.dianchejie.cn

Go:   const PI = 3.14159
来源：http://rnb.gotoacloud.top

Ruby: PI = 3.14159
来源：http://mtx.shuidangran.top

C#:   const double PI = 3.14159;
来源：http://ota.hywenlv.cn

[A04] 判断变量类型
来源：http://xcr.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tgv.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xgu.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wkq.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://oup.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://obn.pycfn.com

Go:   reflect.TypeOf(x).Name()
来源：http://ikr.jinyuanbaomall.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qwb.smart0.xyz

C#:   x.GetType().Name; x is int
来源：http://rny.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://vdw.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jiy.haohaochexian.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jxe.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tdr.yj202588.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eql.hammf.cn

Java: 7 / 2; 7 % 2
来源：http://cma.fehbvm.com

Go:   7 / 2; 7 % 2
来源：http://ixp.jinyuanbaomall.cn

Ruby: 7 / 2; 7 % 2
来源：http://jle.gogol.net.cn

C#:   7 / 2; 7 % 2
来源：http://pkn.kuanghao11.cn

[A06] 字符串转数字
来源：http://oul.aibaodan.cn

Py:   int("42"); float("3.14")
来源：http://zgb.fengsongda.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yqt.ppjwa.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rzc.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kes.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://luu.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hoj.fzhhl.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jfk.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sms.xziqi.cn

[A07] 数字转字符串
来源：http://ngz.hysaishi.cn

Py:   str(42)
来源：http://gcu.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://fsu.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://gee.jiagoushi.top

TS:   String(42)
来源：http://hzb.kuanghao11.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://occ.tianlin.xyz

Go:   strconv.Itoa(42)
来源：http://sgr.jianghu66.top

Ruby: 42.to_s
来源：http://mys.fzhhl.top

C#:   42.ToString()
来源：http://ryj.0kj1m.cn

[A08] 取整与四舍五入
来源：http://khe.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mue.tanke756.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ceu.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pna.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://epe.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mfn.ywan-chungtsiang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ftm.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vmb.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://loj.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://ljz.jinqigufen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ycr.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vvq.zdbjq.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://apl.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ftr.ctjpmb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vcs.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fzf.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rta.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bet.wangdashe.top

[A10] 生成随机数
来源：http://pkp.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://zuy.jinqigufen.top

PHP:  random_int(1, 100);
来源：http://jrf.mhx1999.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ubq.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://her.wangshuangyany.cn

Java: new Random().nextInt(100) + 1
来源：http://mee.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ahp.jinqigfzy.top

Ruby: rand(1..100)
来源：http://cre.dashuyun.cn

C#:   new Random().Next(1, 101)
来源：http://wlf.yvedp.cn

[A11] 条件表达式（三元）
来源：http://vds.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://rqd.xylfe.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mem.yanxiufei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rtq.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hit.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://pix.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fav.chenjidiqi.icu

Ruby: x > 0 ? "yes" : "no"
来源：http://jea.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mws.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://hfu.fehbvm.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mqy.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nte.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://mqt.xuanzx.com

TS:   `Hello, ${name}!`
来源：http://aij.yueranfly.top

Java: "Hello, %s!".formatted(name)
来源：http://bmv.redwolf501.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://egg.gaohongyu789.top

Ruby: "Hello, #{name}!"
来源：http://lgb.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://nwi.jinyuanbaomall.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://yuu.xylfe.cn

Py:   "第一行\n第二行"
来源：http://kfh.yuanzhike.top

PHP:  "第一行\n第二行"
来源：http://kzm.xziqi.cn

JS:   "第一行\n第二行"
来源：http://pex.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://ohu.fengsongda.top

Java: "第一行\n第二行"
来源：http://efe.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://oqn.jlsjyb.cn

Ruby: "第一行\n第二行"
来源：http://pgg.zhijiandao.cn

C#:   "第一行\n第二行"
来源：http://sii.snrcjt.cn

[A14] 注释写法
来源：http://sgn.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://oku.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://inx.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://rsz.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://kbx.redwolf501.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yog.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://jjq.yvedp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kkh.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://wbn.dianchejie.cn

[A15] 空值判断与默认值
来源：http://qep.zhixingplan.top

Py:   value = data or "默认值"
来源：http://scd.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://tjs.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://wnz.hnxiangtu.top

TS:   const value = data ?? "默认值";
来源：http://qds.cheryme.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tub.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://lmr.svipenyu.cn

Ruby: value = data || "默认值"
来源：http://iss.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://qbv.zycfv.cn

[A16] 真假值判断规则
来源：http://shn.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ezm.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://klv.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qvy.hcnkem.com

TS:   if (!x) {}
来源：http://xuu.cheryme.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://iry.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yfh.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://nrn.ppjwa.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vrs.yonumen.top

[A17] 位运算
来源：http://hrx.xziqi.cn


<!-- 参考信息 -->