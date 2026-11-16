代发 wailian999

[U95] JS：Promise 包装
来源：http://vca.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://iek.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://uqv.yongpay.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sjs.fzhhl.top

[U97] JS：并发请求
来源：http://vow.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rsm.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://eyy.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cyh.gogol.net.cn

[U99] JS：事件监听
来源：http://bjs.hesvh.cn

el.addEventListener("click", e => {})
来源：http://mei.ybcxt.top

[U100] JS：DOM 查询
来源：http://rpf.shanyushiyangtech.top

document.querySelector(".item")
来源：http://cpy.hammf.cn

[U101] JS：classList 操作
来源：http://fme.jianghu66.top

el.classList.toggle("active")
来源：http://rxe.andypj.xyz

[U102] JS：本地存储
来源：http://ijr.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mqw.yueranfly.top

[U103] JS：定时器
来源：http://wiv.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ehl.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://guj.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://djm.ydjk.org.cn

[U105] JS：节流
来源：http://tiz.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nlp.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://nmz.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dai.iojbl.cn

[U107] JS：数字千分位
来源：http://inc.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kiz.jinqigufen.top

[U108] JS：随机整数
来源：http://zqa.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vlg.epnwcf.com

[U109] JS：数组分组
来源：http://pdy.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://emw.hcnkem.com

[U110] JS：数组分块
来源：http://xli.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zyt.xziqi.cn

[U111] JS：对象转 Map
来源：http://rgz.zdqjudy.top

new Map(Object.entries(obj))
来源：http://bxo.aizwys.cn

[U112] JS：字符串补位
来源：http://ndw.ybcxt.top

"7".padStart(3, "0")
来源：http://wws.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://ihr.yuxming.cn

s.replaceAll("a", "b")
来源：http://gpp.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://eir.andypj.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://inc.dashuyun.cn

[U115] JS：生成 UUID
来源：http://erz.jinqigfzy.top

crypto.randomUUID()
来源：http://cbu.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://bdn.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://epj.meibo888.top

[U117] JS：单元测试
来源：http://ncy.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://puo.dianchejie.cn

[U118] JS：开发服务器
来源：http://kco.zdqjudy.top

npm i -D vite;  npx vite
来源：http://xsm.sysykeji.top

[U119] JS：生产构建
来源：http://ayu.jianghu66.top

npx vite build
来源：http://prd.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://oht.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://akw.xinyue.icu

================================================================================
来源：http://jbx.redwolf501.top

统计汇总
来源：http://qab.epnwcf.com

================================================================================
来源：http://tmt.zycfv.cn

按语言统计（条）：
来源：http://yai.cheryme.top

Python ......... 252
来源：http://mvv.hammf.cn

PHP ............ 252
来源：http://slk.kuanghao11.cn

JavaScript ..... 252
来源：http://kfd.chenlongwang.top

TypeScript ..... 212
来源：http://dfa.sysykeji.top

Java ........... 212
来源：http://oqu.zhijiandao.cn

Go ............. 212
来源：http://ffz.vqdsnc.cn

Ruby ........... 212
来源：http://emd.uphjek.com

C# ............. 212
来源：http://dcj.zhixingplan.top

C .............. 30
来源：http://aax.9152youxi.cn

C++ ............ 30
来源：http://vat.aibaodan.cn

SQL ............ 90
来源：http://dck.vehdjk.com

Bash ........... 80
来源：http://vbp.ivvv.top

Kotlin ......... 15
来源：http://cke.uphjek.com

Swift .......... 15
来源：http://stv.xuetiantiany.cn

Lua ............ 10
来源：http://niq.sufxvd.cn

Perl ........... 10
来源：http://evt.xingfuxueyuan.xyz

Scala .......... 10
来源：http://zev.meibo888.top

------------------------------------
来源：http://blt.iojbl.cn

合计 ........... 2106 条
来源：http://rzh.cdnleiting.top

按章节统计：
来源：http://zcx.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sao.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tgq.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://luj.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dow.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uad.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yis.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cjb.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mpw.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yul.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cle.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zto.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://maf.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://khd.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gyf.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jus.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ppq.jqgufenzy.top

Q SQL 专题                              90
来源：http://hqq.0kj1m.cn

R Bash 专题                             80
来源：http://nwe.gaohongyu789.top

S C / C++ 专题                          60
来源：http://kqb.yongpay.top

T 其他语言补充                          60
来源：http://ofw.zhijiandao.cn

U 高频实用片段                         120
来源：http://hsc.zhoulong.xyz

------------------------------------
来源：http://zxg.yvedp.cn

合计                                  2106 条
来源：http://uxm.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://fzm.cashguo.top

使用提醒
来源：http://zpl.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://awr.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ynd.tarul.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zma.gaohongyu789.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vpr.yongpay.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ini.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fty.zhongyouzk.top

—— 文件结束 ——
来源：http://fay.sufxvd.cn

================================================================================
来源：http://szd.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://crn.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://qdu.nanxinkj.top

================================================================================
来源：http://mdt.zhoulong.xyz

【收录内容】
来源：http://fov.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://zcb.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rtv.uphjek.com

SQL · Bash · C · C++
来源：http://rpx.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dgz.xingfuxueyuan.xyz

【使用说明】
来源：http://yds.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zbn.hywenlv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://otd.yj202588.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oeh.wangdashe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lyy.ydjk.org.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kcj.hongshengwenyu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mvn.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uvf.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://arh.sxryk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vor.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xsv.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aww.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zzl.cashguo.top

【文件统计】
来源：http://yhj.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dxx.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://hnu.aizwys.cn

目  录
来源：http://bsn.shuidangran.top

--------------------------------------------------------------------------------
来源：http://pxr.hnqzz.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qlj.daria6918.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://isk.guannengcc.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yfe.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iaa.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://agu.havefunace.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xdq.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://skv.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xnm.kuanghao11.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fjm.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://clw.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cda.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xik.tian-w.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pck.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rlk.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kra.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://awu.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qmu.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wdt.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oar.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://odk.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sfz.zhaomingkeji.xyz

================================================================================
来源：http://flu.sysykeji.top

A. 基础语法与类型
来源：http://hbb.chenzaomai.com

================================================================================
来源：http://eqc.smart0.xyz

[A01] Hello World
来源：http://yta.jqgfzy.top

Py:   print("Hello, World!")
来源：http://dnt.yuxming.cn

PHP:  echo "Hello, World!";
来源：http://gem.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://mxa.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ayc.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://obb.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://qzw.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://dhj.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fub.hammf.cn

[A02] 变量声明与赋值
来源：http://liz.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zhj.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://swx.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://bko.yfazqb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://azj.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://rla.zycfv.cn

Go:   name := "Alex"; age := 20
来源：http://drz.hongshengwenyu.top

Ruby: name = "Alex"; age = 20
来源：http://smd.fengsongda.top

C#:   string name = "Alex"; int age = 20;
来源：http://doa.havefunace.top

[A03] 常量定义
来源：http://pht.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rtx.sweek.top

PHP:  const PI = 3.14159;
来源：http://qvg.pycfn.com

JS:   const PI = 3.14159;
来源：http://sox.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://cgf.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://lvz.andypj.xyz

Go:   const PI = 3.14159
来源：http://rza.zhengqikj.top

Ruby: PI = 3.14159
来源：http://hpo.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://cai.jlsjyb.cn

[A04] 判断变量类型
来源：http://psg.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bai.sysykeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ghz.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wne.jyoumei.cn

TS:   typeof x; x instanceof Date
来源：http://uxi.nanxinkj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://obb.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pye.shanyushiyangtech.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ima.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://ojk.52xcode.cn

[A05] 整数除法与取模
来源：http://rfl.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cnk.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://arn.zdbjq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fbk.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wol.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://aaf.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://dxq.hnqzz.top

Ruby: 7 / 2; 7 % 2
来源：http://tda.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://qfu.hesvh.cn

[A06] 字符串转数字
来源：http://nmo.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://btw.gaohongyu789.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wld.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xyr.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://bfq.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jri.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://shw.jinyuanbaomall.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wta.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yam.cashguo.top

[A07] 数字转字符串
来源：http://kzv.fengsongda.top

Py:   str(42)
来源：http://cdh.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://jjc.hfpthk.cn

JS:   String(42); (42).toString()
来源：http://rml.jyoumei.cn

TS:   String(42)
来源：http://kum.hcnkem.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ttj.wangdashe.top

Go:   strconv.Itoa(42)
来源：http://hfg.shangyingyoupin.top

Ruby: 42.to_s
来源：http://ump.sweek.top

C#:   42.ToString()
来源：http://wzb.jqgfzy.top

[A08] 取整与四舍五入
来源：http://mvn.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wve.dashuyun.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://smm.wangdashe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mvk.gzhubu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://brh.xziqi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mcw.bbcook.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qwb.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://tga.chenlongwang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bdd.shangyingyoupin.top

[A09] 绝对值与最大最小值
来源：http://ggw.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rts.hysaishi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://asb.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xyz.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hps.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lit.guowangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tyq.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wan.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ukt.vehdjk.com

[A10] 生成随机数
来源：http://evn.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://efs.tanke756.top

PHP:  random_int(1, 100);
来源：http://bbr.daxiang520.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xwi.fktsv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sgf.shuidangran.top

Java: new Random().nextInt(100) + 1
来源：http://wen.fktsv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fmj.tanke756.top

Ruby: rand(1..100)
来源：http://afr.hnxiangtu.top

C#:   new Random().Next(1, 101)
来源：http://ofr.chenzaomai.com

[A11] 条件表达式（三元）
来源：http://rdo.yonumen.top

Py:   "yes" if x > 0 else "no"
来源：http://odz.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vtn.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://vib.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://yzc.chenlongwang.top

Java: x > 0 ? "yes" : "no"
来源：http://uhf.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ydc.cucudq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://htw.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://ucj.chenlongwang.top

[A12] 字符串插值 / 格式化
来源：http://adl.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://idg.bbcook.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yrh.gzhubu.top

JS:   `Hello, ${name}!`
来源：http://qdk.birdmap.top

TS:   `Hello, ${name}!`
来源：http://nws.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://qzn.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lvs.ehwqpu.com

Ruby: "Hello, #{name}!"
来源：http://tfl.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://nfi.cucudq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mrl.andypj.xyz

Py:   "第一行\n第二行"
来源：http://niu.cqqwz.cn

PHP:  "第一行\n第二行"
来源：http://kje.hcnkem.com

JS:   "第一行\n第二行"
来源：http://pgi.ywan-chungtsiang.top

TS:   "第一行\n第二行"
来源：http://qjd.aibaodan.cn

Java: "第一行\n第二行"
来源：http://crb.uphjek.com

Go:   "第一行\n第二行"
来源：http://qnu.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://qfd.zdqjudy.top

C#:   "第一行\n第二行"
来源：http://sxs.yonumen.top

[A14] 注释写法
来源：http://toz.yanxiufei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yrx.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://bvc.bjfxy.top

JS:   // 单行；/* 多行 */
来源：http://koc.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://onw.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rnh.guannengcc.top

Go:   // 单行；/* 多行 */
来源：http://ech.cqqwz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ewg.andypj.xyz

C#:   // 单行；/* 多行 */
来源：http://izu.vehdjk.com

[A15] 空值判断与默认值
来源：http://efu.xylfe.cn

Py:   value = data or "默认值"
来源：http://ivb.shzxlz.cn

PHP:  $value = $data ?? "默认值";
来源：http://vzi.zhiwuduotai.top

JS:   const value = data ?? "默认值";
来源：http://dxl.yvedp.cn

TS:   const value = data ?? "默认值";
来源：http://vjo.iojbl.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ruw.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://omk.bbcook.cn

Ruby: value = data || "默认值"
来源：http://pbm.sweek.top

C#:   var value = data ?? "默认值";
来源：http://sud.jyoumei.cn

[A16] 真假值判断规则
来源：http://tyw.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://czd.zhengqikj.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fjd.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cwk.yj20258888.top

TS:   if (!x) {}
来源：http://bzi.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fym.nanxinkj.top


<!-- 参考信息 -->