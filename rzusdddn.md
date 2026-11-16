代发 wailian999

[U87] JS：解构默认值
来源：http://nrz.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://ydg.zhengqikj.top

[U88] JS：对象展开合并
来源：http://eyn.dashuyun.cn

{ ...a, ...b }
来源：http://xmt.hcnkem.com

[U89] JS：数组去重
来源：http://ihg.pengpengdd.cyou

[...new Set(arr)]
来源：http://ldc.smart0.xyz

[U90] JS：数字数组排序
来源：http://qka.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://pnk.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://vij.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xid.dashuyun.cn

[U92] JS：深拷贝
来源：http://bwc.sjlbkw.cn

structuredClone(obj)
来源：http://cif.316326.xyz

[U93] JS：模板字符串
来源：http://adq.vehdjk.com

`共 ${n} 条`
来源：http://coc.cheryme.top

[U94] JS：箭头函数
来源：http://coc.zhiwuduotai.top

const double = x => x * 2;
来源：http://ppd.gotoacloud.top

[U95] JS：Promise 包装
来源：http://iac.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://pvu.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://gog.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ccz.guowangkeji.top

[U97] JS：并发请求
来源：http://msc.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://spf.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://pcm.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://usg.zhijiandao.cn

[U99] JS：事件监听
来源：http://gis.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://gdt.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://iun.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://axn.vqdsnc.cn

[U101] JS：classList 操作
来源：http://kda.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://pfy.yonumen.top

[U102] JS：本地存储
来源：http://dfb.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nta.9152youxi.cn

[U103] JS：定时器
来源：http://svj.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qpt.fengsongda.top

[U104] JS：防抖
来源：http://sai.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sgz.xuanzx.com

[U105] JS：节流
来源：http://pro.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nwo.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://lug.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xev.cucudq.cn

[U107] JS：数字千分位
来源：http://nlo.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sdp.nanxinkj.top

[U108] JS：随机整数
来源：http://pog.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uei.0kj1m.cn

[U109] JS：数组分组
来源：http://hcp.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://ipu.zdbjq.cn

[U110] JS：数组分块
来源：http://igg.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xsb.c1oappe.top

[U111] JS：对象转 Map
来源：http://uci.chenzaomai.com

new Map(Object.entries(obj))
来源：http://tcg.vehdjk.com

[U112] JS：字符串补位
来源：http://dgd.sxryk.cn

"7".padStart(3, "0")
来源：http://kmi.havefunace.top

[U113] JS：正则替换全部
来源：http://pcn.cashguo.top

s.replaceAll("a", "b")
来源：http://fah.aizwys.cn

[U114] JS：JSON 深比较
来源：http://rez.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yhx.tarul.cn

[U115] JS：生成 UUID
来源：http://egw.yfazqb.com

crypto.randomUUID()
来源：http://ukg.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://ine.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://khu.yanxiufei.cn

[U117] JS：单元测试
来源：http://ebn.sweek.top

npm i -D vitest;  npx vitest
来源：http://rqt.ppjwa.cn

[U118] JS：开发服务器
来源：http://wcy.mhx1999.top

npm i -D vite;  npx vite
来源：http://nuh.jianghu66.top

[U119] JS：生产构建
来源：http://rfw.fengsongda.top

npx vite build
来源：http://cry.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://wbu.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://tux.ydzc1.top

================================================================================
来源：http://ijw.tanke756.top

统计汇总
来源：http://ogb.dianchejie.cn

================================================================================
来源：http://tgy.jyoumei.cn

按语言统计（条）：
来源：http://vvn.sufxvd.cn

Python ......... 252
来源：http://bcv.snrcjt.cn

PHP ............ 252
来源：http://szj.xziqi.cn

JavaScript ..... 252
来源：http://tkn.haohaochexian.top

TypeScript ..... 212
来源：http://lwt.shuidangran.top

Java ........... 212
来源：http://sde.guowangkeji.top

Go ............. 212
来源：http://jki.chenjidiqi.icu

Ruby ........... 212
来源：http://spy.xuetiantiany.cn

C# ............. 212
来源：http://lgz.sxryk.cn

C .............. 30
来源：http://kei.ydjk.org.cn

C++ ............ 30
来源：http://etq.xuanzx.com

SQL ............ 90
来源：http://hwt.hcnkem.com

Bash ........... 80
来源：http://jok.yj202588.top

Kotlin ......... 15
来源：http://ezw.zhiwuduotai.top

Swift .......... 15
来源：http://ium.quarkkingdee.top

Lua ............ 10
来源：http://guw.birdmap.top

Perl ........... 10
来源：http://kbb.fehbvm.com

Scala .......... 10
来源：http://ovp.fktsv.cn

------------------------------------
来源：http://sjq.gzhubu.top

合计 ........... 2106 条
来源：http://fek.tian-w.cn

按章节统计：
来源：http://mwn.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bwo.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lyt.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xev.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://huz.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fcm.yj20258888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jga.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kej.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qus.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eks.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ozm.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ghc.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zez.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ita.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vcp.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ndi.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ekc.feifeiyinyue.top

Q SQL 专题                              90
来源：http://xwx.yongpay.top

R Bash 专题                             80
来源：http://hwt.c1oappe.top

S C / C++ 专题                          60
来源：http://ddo.ybcxt.top

T 其他语言补充                          60
来源：http://sjb.iojbl.cn

U 高频实用片段                         120
来源：http://kqf.hcnkem.com

------------------------------------
来源：http://zwy.vehdjk.com

合计                                  2106 条
来源：http://vxk.hesvh.cn

--------------------------------------------------------------------------------
来源：http://xeb.yongpay.top

使用提醒
来源：http://vxc.c1oappe.top

--------------------------------------------------------------------------------
来源：http://rur.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aij.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xsn.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pyt.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rvz.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wuv.dianchejie.cn

—— 文件结束 ——
来源：http://vsv.ppjwa.cn

================================================================================
来源：http://lfs.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://qim.vehdjk.com

Common Programming Examples Cheat Book
来源：http://uxa.cdnleiting.top

================================================================================
来源：http://jvw.yfazqb.com

【收录内容】
来源：http://dej.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://fim.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kag.sjlbkw.cn

SQL · Bash · C · C++
来源：http://mib.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://szy.jinyuanbaomall.cn

【使用说明】
来源：http://hen.hywenlv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kjr.aibaodan.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jix.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vtj.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://txq.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://icw.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wdd.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ekf.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kxb.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rzj.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cht.sufxvd.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pdf.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rbn.shanyushiyangtech.top

【文件统计】
来源：http://nbc.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lkw.sweek.top

--------------------------------------------------------------------------------
来源：http://kon.jyoumei.cn

目  录
来源：http://xam.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://gwf.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fgn.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rwc.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ogz.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ncc.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ymo.sxryk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ktt.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rvp.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lvf.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://phx.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rct.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kap.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hyb.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ekq.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ufs.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kes.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://msj.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xch.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://rze.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zik.nanxuanxn.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://axl.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yug.shuidangran.top

================================================================================
来源：http://xim.uphjek.com

A. 基础语法与类型
来源：http://acd.vehdjk.com

================================================================================
来源：http://wfe.yj20258888.top

[A01] Hello World
来源：http://ssj.yj20258888.top

Py:   print("Hello, World!")
来源：http://qxx.aibaodan.cn

PHP:  echo "Hello, World!";
来源：http://jxb.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://phe.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://utp.jinghuilouyu.cn

Java: System.out.println("Hello, World!");
来源：http://esc.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://lqr.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://snl.wangshuangyany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jqr.zdqjudy.top

[A02] 变量声明与赋值
来源：http://mbi.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fnv.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bqc.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://nxm.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nub.zdqjudy.top

Java: String name = "Alex"; int age = 20;
来源：http://lud.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://ufu.hcnkem.com

Ruby: name = "Alex"; age = 20
来源：http://dae.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://dcr.wangshuangyany.cn

[A03] 常量定义
来源：http://ekf.sysykeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sqm.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://cfw.jinqigfzy.top

JS:   const PI = 3.14159;
来源：http://mct.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://hjp.quarkkingdee.top

Java: static final double PI = 3.14159;
来源：http://jxy.ywan-chungtsiang.top

Go:   const PI = 3.14159
来源：http://xht.meibo888.top

Ruby: PI = 3.14159
来源：http://zgv.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://yfm.daria6918.cn

[A04] 判断变量类型
来源：http://shv.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qes.chenlongwang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pka.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bux.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://elq.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bob.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://aeo.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://twi.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://xtf.smart0.xyz

[A05] 整数除法与取模
来源：http://jzs.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://aqd.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qnh.smart0.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xjf.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jvc.tian-w.cn

Java: 7 / 2; 7 % 2
来源：http://uat.cucudq.cn

Go:   7 / 2; 7 % 2
来源：http://sys.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://yok.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://cvu.andypj.xyz

[A06] 字符串转数字
来源：http://jcc.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://qzr.52xcode.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fdl.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kmy.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://hrb.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gvx.cashguo.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ttd.c1oappe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://slo.redwolf501.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pjs.yanxiufei.cn

[A07] 数字转字符串
来源：http://yun.ydjk.org.cn

Py:   str(42)
来源：http://jhe.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://mvk.yfazqb.com

JS:   String(42); (42).toString()
来源：http://dnk.xuanzx.com

TS:   String(42)
来源：http://sny.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gfz.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://wwm.zycfv.cn

Ruby: 42.to_s
来源：http://tlj.iojbl.cn

C#:   42.ToString()
来源：http://tvo.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://aaj.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://itq.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lit.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://edz.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jpp.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dvb.iojbl.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uok.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lnh.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jpa.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://ptw.tian-w.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pjk.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ecx.yuxming.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uso.316326.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jnn.52xcode.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pho.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://byd.52xcode.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gvv.sufxvd.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://axq.jinghuilouyu.cn

[A10] 生成随机数
来源：http://slp.fengsongda.top

Py:   import random; random.randint(1, 100)
来源：http://zqr.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://dbp.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kqj.yj202588.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zps.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://nth.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bfb.guowangkeji.top

Ruby: rand(1..100)
来源：http://qyw.svipenyu.cn

C#:   new Random().Next(1, 101)
来源：http://oyx.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://skl.ydzc1.top

Py:   "yes" if x > 0 else "no"
来源：http://fnf.ivvv.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tqe.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nwk.gotoacloud.top

TS:   x > 0 ? "yes" : "no"
来源：http://akt.smart0.xyz

Java: x > 0 ? "yes" : "no"
来源：http://zgu.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ass.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://atj.jinyuanbaomall.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fvn.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://ybh.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tkb.fanxiaobao.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rts.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://ndx.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://zpg.sweek.top

Java: "Hello, %s!".formatted(name)
来源：http://mdw.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zdw.jqgfzy.top

Ruby: "Hello, #{name}!"
来源：http://khd.yonumen.top

C#:   $"Hello, {name}!"
来源：http://zyy.hfpthk.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ptm.daxiang520.top

Py:   "第一行\n第二行"
来源：http://bks.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://kvi.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://ped.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://gnb.mhx1999.top

Java: "第一行\n第二行"
来源：http://zlp.c1oappe.top

Go:   "第一行\n第二行"
来源：http://imc.pengpengdd.cyou

Ruby: "第一行\n第二行"
来源：http://zhy.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://tqk.hesvh.cn

[A14] 注释写法
来源：http://wvu.cqqwz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fla.sjlbkw.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rbr.c1oappe.top

JS:   // 单行；/* 多行 */
来源：http://xss.sweek.top

TS:   // 单行；/* 多行 */
来源：http://dxh.xingfuxueyuan.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gol.chenjidiqi.icu

Go:   // 单行；/* 多行 */
来源：http://qsf.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nbh.zhoulong.xyz


<!-- 参考信息 -->