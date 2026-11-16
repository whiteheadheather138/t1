代发 wailian999

[U93] JS：模板字符串
来源：http://ggc.cucudq.cn

`共 ${n} 条`
来源：http://afm.hnxiangtu.top

[U94] JS：箭头函数
来源：http://moa.jlsjyb.cn

const double = x => x * 2;
来源：http://nlx.jinqigufen.top

[U95] JS：Promise 包装
来源：http://bfq.yongpay.top

new Promise((resolve, reject) => {})
来源：http://zjp.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://xmt.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cic.c1oappe.top

[U97] JS：并发请求
来源：http://pgv.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ghp.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://bxa.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eeb.shzxlz.cn

[U99] JS：事件监听
来源：http://jgf.mhx1999.top

el.addEventListener("click", e => {})
来源：http://jxg.dashuyun.cn

[U100] JS：DOM 查询
来源：http://sxa.wangdashe.top

document.querySelector(".item")
来源：http://boa.zhoulong.xyz

[U101] JS：classList 操作
来源：http://nuf.pycfn.com

el.classList.toggle("active")
来源：http://guc.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://uyt.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vsi.pycfn.com

[U103] JS：定时器
来源：http://yws.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zef.tanke756.top

[U104] JS：防抖
来源：http://qvc.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wyi.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://ihx.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xtg.zdbjq.cn

[U106] JS：日期格式化
来源：http://plh.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dgt.nanxuanxn.top

[U107] JS：数字千分位
来源：http://cce.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aor.ydzc1.top

[U108] JS：随机整数
来源：http://djm.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tvu.chenjidiqi.icu

[U109] JS：数组分组
来源：http://twr.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://czs.snrcjt.cn

[U110] JS：数组分块
来源：http://htz.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ydy.iojbl.cn

[U111] JS：对象转 Map
来源：http://gpa.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://grp.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://qvm.fengsongda.top

"7".padStart(3, "0")
来源：http://eqz.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://qov.cdnleiting.top

s.replaceAll("a", "b")
来源：http://hol.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://iwz.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://haq.zhengqikj.top

[U115] JS：生成 UUID
来源：http://enj.fanxiaobao.xyz

crypto.randomUUID()
来源：http://hte.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://bjc.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://tmr.yj20258888.top

[U117] JS：单元测试
来源：http://sca.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://voq.yj202588.top

[U118] JS：开发服务器
来源：http://wzx.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://jez.uphjek.com

[U119] JS：生产构建
来源：http://upa.guannengcc.top

npx vite build
来源：http://zfk.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://uch.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://axs.shzxlz.cn

================================================================================
来源：http://zqz.yangfankeji.com

统计汇总
来源：http://sqr.nanxinkj.top

================================================================================
来源：http://mts.jinqigufen.top

按语言统计（条）：
来源：http://hjj.hesvh.cn

Python ......... 252
来源：http://qcp.vqdsnc.cn

PHP ............ 252
来源：http://vfo.daxiang520.top

JavaScript ..... 252
来源：http://fmd.hesvh.cn

TypeScript ..... 212
来源：http://wjl.cqqwz.cn

Java ........... 212
来源：http://tbz.nanxuanxn.top

Go ............. 212
来源：http://wam.yj202588.top

Ruby ........... 212
来源：http://acf.xylfe.cn

C# ............. 212
来源：http://sfe.cashguo.top

C .............. 30
来源：http://kgz.yongpay.top

C++ ............ 30
来源：http://iei.yj202588.top

SQL ............ 90
来源：http://sye.hesvh.cn

Bash ........... 80
来源：http://fdy.cashguo.top

Kotlin ......... 15
来源：http://kxa.yonumen.top

Swift .......... 15
来源：http://ndd.ehwqpu.com

Lua ............ 10
来源：http://mtq.wangdashe.top

Perl ........... 10
来源：http://qth.daxiang520.top

Scala .......... 10
来源：http://uky.fengsongda.top

------------------------------------
来源：http://xzj.zdqjudy.top

合计 ........... 2106 条
来源：http://ndi.smart0.xyz

按章节统计：
来源：http://efo.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fwg.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yke.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ucl.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hgi.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iks.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kjb.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ddp.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wen.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nsx.nwbrower.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sif.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ois.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://est.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://szx.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://imk.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lml.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hvt.cdnleiting.top

Q SQL 专题                              90
来源：http://rjt.yongpay.top

R Bash 专题                             80
来源：http://jhe.kuanghao11.cn

S C / C++ 专题                          60
来源：http://yqt.sweek.top

T 其他语言补充                          60
来源：http://vct.316326.xyz

U 高频实用片段                         120
来源：http://lrj.guannengcc.top

------------------------------------
来源：http://ugf.wangshuangyany.cn

合计                                  2106 条
来源：http://thi.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://xcs.shuidangran.top

使用提醒
来源：http://iqz.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://ebf.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uqu.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iln.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://efv.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vzc.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zoo.zycfv.cn

—— 文件结束 ——
来源：http://wwv.hongshengwenyu.top

================================================================================
来源：http://rmo.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://cjq.jinghuilouyu.cn

Common Programming Examples Cheat Book
来源：http://csv.yvedp.cn

================================================================================
来源：http://iod.jinqigufen.top

【收录内容】
来源：http://acd.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ool.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ars.hywenlv.cn

SQL · Bash · C · C++
来源：http://xql.nwbrower.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://klz.birdmap.top

【使用说明】
来源：http://zaf.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qnx.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ncg.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aee.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zzt.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ofl.fengsongda.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nhn.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rhh.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://glb.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uau.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yfl.zdqjudy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ctj.yj20258888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://anf.nanxuanxn.top

【文件统计】
来源：http://zmb.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ohv.cucudq.cn

--------------------------------------------------------------------------------
来源：http://htm.yangfankeji.com

目  录
来源：http://iol.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://kwt.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vkx.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://esc.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ysg.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://toj.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yqo.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aul.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://woj.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gqt.cheryme.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eww.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yfp.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ght.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qna.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gtf.shanyushiyangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hjt.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tpq.fzhhl.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jbh.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://chx.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://orv.meibo888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cte.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://csx.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ovz.sxryk.cn

================================================================================
来源：http://cth.ctjpmb.com

A. 基础语法与类型
来源：http://kbt.zhengqikj.top

================================================================================
来源：http://ptp.xingfuxueyuan.xyz

[A01] Hello World
来源：http://kvb.aibaodan.cn

Py:   print("Hello, World!")
来源：http://epy.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://mds.316326.xyz

JS:   console.log("Hello, World!");
来源：http://ycu.zhixingplan.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qzw.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://ecx.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://lnx.pycfn.com

Ruby: puts "Hello, World!"
来源：http://ygn.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wcc.sxryk.cn

[A02] 变量声明与赋值
来源：http://wwm.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nay.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://waj.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://exh.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sfv.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://fon.tian-w.cn

Go:   name := "Alex"; age := 20
来源：http://nef.jyoumei.cn

Ruby: name = "Alex"; age = 20
来源：http://dqd.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ptt.yonumen.top

[A03] 常量定义
来源：http://uih.52xcode.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wqv.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://hfi.gzhubu.top

JS:   const PI = 3.14159;
来源：http://aks.xuetiantiany.cn

TS:   const PI: number = 3.14159;
来源：http://dhi.hysaishi.cn

Java: static final double PI = 3.14159;
来源：http://fss.dianchejie.cn

Go:   const PI = 3.14159
来源：http://ekg.chenlongwang.top

Ruby: PI = 3.14159
来源：http://wlz.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://fav.quarkkingdee.top

[A04] 判断变量类型
来源：http://bgy.shanyushiyangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jjb.kuanghao11.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eei.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cjt.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://hub.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ssm.9152youxi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yas.yangfankeji.com

Ruby: x.class; x.is_a?(Integer)
来源：http://yfe.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://tzt.iojbl.cn

[A05] 整数除法与取模
来源：http://kmo.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zsm.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cpp.shangyingyoupin.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ekp.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://idu.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://spm.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://lnc.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://shz.daria6918.cn

C#:   7 / 2; 7 % 2
来源：http://tph.316326.xyz

[A06] 字符串转数字
来源：http://vot.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://haf.tian-w.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aea.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ezc.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://rax.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://umz.shanyushiyangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xzk.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://srf.jianghu66.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jvs.cheryme.top

[A07] 数字转字符串
来源：http://hob.hfpthk.cn

Py:   str(42)
来源：http://iho.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://tqu.daria6918.cn

JS:   String(42); (42).toString()
来源：http://raq.xingfuxueyuan.xyz

TS:   String(42)
来源：http://wyd.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://wkq.nanxinkj.top

Go:   strconv.Itoa(42)
来源：http://jmu.mhx1999.top

Ruby: 42.to_s
来源：http://ngp.gotoacloud.top

C#:   42.ToString()
来源：http://obp.ppjwa.cn

[A08] 取整与四舍五入
来源：http://cpr.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://psz.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wvm.yonumen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dyb.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oly.jinghuilouyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rvf.ywan-chungtsiang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://drs.hfpthk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pms.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dsw.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://hmc.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vqd.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xbi.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rnb.yanxiufei.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tqx.zhoulong.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zzl.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xxv.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gze.nwbrower.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qqd.zhaomingkeji.xyz

[A10] 生成随机数
来源：http://ecm.zhixingplan.top

Py:   import random; random.randint(1, 100)
来源：http://gxd.shangyingyoupin.top

PHP:  random_int(1, 100);
来源：http://ntw.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aza.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ghs.yueranfly.top

Java: new Random().nextInt(100) + 1
来源：http://ogr.chenzaomai.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fyp.jinghuilouyu.cn

Ruby: rand(1..100)
来源：http://ljj.pengpengdd.cyou

C#:   new Random().Next(1, 101)
来源：http://cps.epnwcf.com

[A11] 条件表达式（三元）
来源：http://jfp.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://zta.ctjpmb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wfm.ywan-chungtsiang.top

JS:   x > 0 ? "yes" : "no"
来源：http://gal.snrcjt.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zkl.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://oqw.hongshengwenyu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mis.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kol.guannengcc.top

C#:   x > 0 ? "yes" : "no"
来源：http://bls.ppjwa.cn

[A12] 字符串插值 / 格式化
来源：http://rof.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dow.smart0.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ycn.jinyuanbaomall.cn

JS:   `Hello, ${name}!`
来源：http://bos.jinqigufen.top

TS:   `Hello, ${name}!`
来源：http://vxb.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://fto.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jwp.cashguo.top

Ruby: "Hello, #{name}!"
来源：http://izv.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://wxs.aizwys.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iox.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://stw.cashguo.top

PHP:  "第一行\n第二行"
来源：http://bxs.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://qap.ehwqpu.com

TS:   "第一行\n第二行"
来源：http://mav.meibo888.top

Java: "第一行\n第二行"
来源：http://ouq.xziqi.cn

Go:   "第一行\n第二行"
来源：http://dbq.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://rpg.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://rzf.yj202588.top

[A14] 注释写法
来源：http://ptk.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://plo.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qka.gogol.net.cn

JS:   // 单行；/* 多行 */
来源：http://poh.guowangkeji.top

TS:   // 单行；/* 多行 */
来源：http://stf.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gpu.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://zjm.ydjk.org.cn

Ruby: # 单行；=begin 多行 =end
来源：http://puw.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://jin.ehwqpu.com

[A15] 空值判断与默认值
来源：http://vqu.iojbl.cn

Py:   value = data or "默认值"
来源：http://qdb.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://ntn.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://vqz.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://pmj.epnwcf.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gkv.sjlbkw.cn

Go:   if data == "" { data = "默认值" }
来源：http://mqo.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://sdf.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://yos.fktsv.cn

[A16] 真假值判断规则
来源：http://toi.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pvc.pycfn.com


<!-- 参考信息 -->