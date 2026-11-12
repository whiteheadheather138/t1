代发 wailian999

[U85] JS：可选链
来源：http://ogs.tarul.cn

a?.b?.c
来源：http://peo.hysaishi.cn

[U86] JS：空值合并
来源：http://grp.sjlbkw.cn

a ?? b
来源：http://udc.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://wcs.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://muq.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://pys.yfazqb.com

{ ...a, ...b }
来源：http://ohg.zhixingplan.top

[U89] JS：数组去重
来源：http://rgk.iojbl.cn

[...new Set(arr)]
来源：http://bec.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://jsv.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://wyh.jianghu66.top

[U91] JS：对象键值遍历
来源：http://dke.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vog.fzhhl.top

[U92] JS：深拷贝
来源：http://lqt.yangfankeji.com

structuredClone(obj)
来源：http://jjl.andypj.xyz

[U93] JS：模板字符串
来源：http://vvg.jinqigfzy.top

`共 ${n} 条`
来源：http://iil.redwolf501.top

[U94] JS：箭头函数
来源：http://sqp.snrcjt.cn

const double = x => x * 2;
来源：http://oyz.yanxiufei.cn

[U95] JS：Promise 包装
来源：http://iel.316326.xyz

new Promise((resolve, reject) => {})
来源：http://osh.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://gcq.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://esm.hcnkem.com

[U97] JS：并发请求
来源：http://eag.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://aad.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://mps.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sqt.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://esh.yuxming.cn

el.addEventListener("click", e => {})
来源：http://shs.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://nrr.birdmap.top

document.querySelector(".item")
来源：http://jbi.yuxming.cn

[U101] JS：classList 操作
来源：http://pem.uphjek.com

el.classList.toggle("active")
来源：http://gfg.cqqwz.cn

[U102] JS：本地存储
来源：http://ece.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bkv.chenjidiqi.icu

[U103] JS：定时器
来源：http://qgm.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aqa.zhoulong.xyz

[U104] JS：防抖
来源：http://kuf.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuu.bbcook.cn

[U105] JS：节流
来源：http://xyz.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://poj.sweek.top

[U106] JS：日期格式化
来源：http://uma.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pwf.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://ctk.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://koc.cdnleiting.top

[U108] JS：随机整数
来源：http://gos.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ttv.smart0.xyz

[U109] JS：数组分组
来源：http://avd.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://zop.xinyue.icu

[U110] JS：数组分块
来源：http://lie.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sji.zhixingplan.top

[U111] JS：对象转 Map
来源：http://ryp.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://cml.mhx1999.top

[U112] JS：字符串补位
来源：http://moc.daria6918.cn

"7".padStart(3, "0")
来源：http://nre.cashguo.top

[U113] JS：正则替换全部
来源：http://muk.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://kpz.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://etc.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cnp.yueranfly.top

[U115] JS：生成 UUID
来源：http://rho.zhengqikj.top

crypto.randomUUID()
来源：http://dge.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://nlg.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://eje.zhiwuduotai.top

[U117] JS：单元测试
来源：http://mwn.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://zim.xinyue.icu

[U118] JS：开发服务器
来源：http://wif.jqgfzy.top

npm i -D vite;  npx vite
来源：http://kyz.gotoacloud.top

[U119] JS：生产构建
来源：http://zko.zhoulong.xyz

npx vite build
来源：http://ukt.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://fsd.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://kjy.zhengqikj.top

================================================================================
来源：http://ofy.guannengcc.top

统计汇总
来源：http://wjz.ybcxt.top

================================================================================
来源：http://pqf.wangdashe.top

按语言统计（条）：
来源：http://ola.smart0.xyz

Python ......... 252
来源：http://xed.jianghu66.top

PHP ............ 252
来源：http://zzh.shanyushiyangtech.top

JavaScript ..... 252
来源：http://sby.mhx1999.top

TypeScript ..... 212
来源：http://sep.fanxiaobao.xyz

Java ........... 212
来源：http://bnw.dashuyun.cn

Go ............. 212
来源：http://jqj.havefunace.top

Ruby ........... 212
来源：http://wpf.havefunace.top

C# ............. 212
来源：http://gxo.hammf.cn

C .............. 30
来源：http://csy.zhoulong.xyz

C++ ............ 30
来源：http://msi.aibaodan.cn

SQL ............ 90
来源：http://yyj.tanke756.top

Bash ........... 80
来源：http://gih.birdmap.top

Kotlin ......... 15
来源：http://txe.yfazqb.com

Swift .......... 15
来源：http://xss.ybcxt.top

Lua ............ 10
来源：http://edv.vqdsnc.cn

Perl ........... 10
来源：http://ydz.uphjek.com

Scala .......... 10
来源：http://hyk.sjlbkw.cn

------------------------------------
来源：http://hto.yuxming.cn

合计 ........... 2106 条
来源：http://lud.nwbrower.top

按章节统计：
来源：http://ldt.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mrx.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tmv.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jcc.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mca.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wfm.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jvr.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vds.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ysy.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qwl.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://znv.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lms.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jtz.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://syh.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ljq.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zbf.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tuk.gotoacloud.top

Q SQL 专题                              90
来源：http://cdc.yj202588.top

R Bash 专题                             80
来源：http://fuq.yj20258888.top

S C / C++ 专题                          60
来源：http://gww.fehbvm.com

T 其他语言补充                          60
来源：http://duw.hywenlv.cn

U 高频实用片段                         120
来源：http://rja.yj202588.top

------------------------------------
来源：http://nno.dashuyun.cn

合计                                  2106 条
来源：http://sjt.yuxming.cn

--------------------------------------------------------------------------------
来源：http://txc.ydjk.org.cn

使用提醒
来源：http://nun.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://qzp.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vvb.aizwys.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://iqm.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pkh.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wop.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mmc.jinghuilouyu.cn

—— 文件结束 ——
来源：http://aoy.xinyue.icu

================================================================================
来源：http://xnx.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://ksv.316326.xyz

Common Programming Examples Cheat Book
来源：http://rjq.sufxvd.cn

================================================================================
来源：http://xkt.shangyingyoupin.top

【收录内容】
来源：http://qdt.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oxu.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kfl.jlsjyb.cn

SQL · Bash · C · C++
来源：http://hfh.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jqb.hesvh.cn

【使用说明】
来源：http://pmy.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cys.nwbrower.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qnx.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rte.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hwl.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kro.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ghf.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ivp.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vde.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://unp.fengsongda.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pgl.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ixx.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pdr.jlsjyb.cn

【文件统计】
来源：http://vct.fanxiaobao.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mbn.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://nqy.sxryk.cn

目  录
来源：http://xfo.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://cww.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://trn.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bvu.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mtc.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pat.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mvb.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://toz.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xzv.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jae.hnqzz.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ayx.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pfe.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ook.ehwqpu.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pqp.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dme.wangdashe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yjp.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gvc.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qjj.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jbp.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ays.sufxvd.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ocw.sjlbkw.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://idi.pengpengdd.cyou

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jet.gzhubu.top

================================================================================
来源：http://jsj.xziqi.cn

A. 基础语法与类型
来源：http://wxc.kuanghao11.cn

================================================================================
来源：http://dlh.zhongyouzk.top

[A01] Hello World
来源：http://vyr.aizwys.cn

Py:   print("Hello, World!")
来源：http://hjw.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://wgz.aizwys.cn

JS:   console.log("Hello, World!");
来源：http://ofn.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qvs.gzhubu.top

Java: System.out.println("Hello, World!");
来源：http://rzm.yuanzhike.top

Go:   fmt.Println("Hello, World!")
来源：http://pjc.ydjk.org.cn

Ruby: puts "Hello, World!"
来源：http://dbk.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qpx.feifeiyinyue.top

[A02] 变量声明与赋值
来源：http://qve.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://abg.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rqe.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://wmn.dianchejie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uov.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://uuy.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://xqt.jinqigfzy.top

Ruby: name = "Alex"; age = 20
来源：http://srx.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://las.tian-w.cn

[A03] 常量定义
来源：http://oua.zhixingplan.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gmw.mhx1999.top

PHP:  const PI = 3.14159;
来源：http://mhb.zhaomingkeji.xyz

JS:   const PI = 3.14159;
来源：http://hdj.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://sea.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://kov.jianghu66.top

Go:   const PI = 3.14159
来源：http://trw.yonumen.top

Ruby: PI = 3.14159
来源：http://rdr.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://bdh.tianlin.xyz

[A04] 判断变量类型
来源：http://jxs.fengsongda.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gcj.havefunace.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lir.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://reo.ydjk.org.cn

TS:   typeof x; x instanceof Date
来源：http://jop.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eeq.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://ldm.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vfz.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://oyf.ybcxt.top

[A05] 整数除法与取模
来源：http://sxh.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dvo.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vss.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fxb.aibaodan.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lmp.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://klm.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://lph.shangyingyoupin.top

Ruby: 7 / 2; 7 % 2
来源：http://jpl.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://vbk.guowangkeji.top

[A06] 字符串转数字
来源：http://rmu.hesvh.cn

Py:   int("42"); float("3.14")
来源：http://kbg.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mta.vqdsnc.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ier.shangyingyoupin.top

TS:   parseInt("42", 10); Number("42")
来源：http://vck.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fjx.sufxvd.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://spi.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://twy.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dkk.wangdashe.top

[A07] 数字转字符串
来源：http://wfk.zhixingplan.top

Py:   str(42)
来源：http://cjl.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://ekw.bbcook.cn

JS:   String(42); (42).toString()
来源：http://pkl.zhoulong.xyz

TS:   String(42)
来源：http://pqc.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://xjs.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://jnl.cdnleiting.top

Ruby: 42.to_s
来源：http://djz.bbcook.cn

C#:   42.ToString()
来源：http://jfo.bbcook.cn

[A08] 取整与四舍五入
来源：http://wlj.cdnleiting.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ldm.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dij.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ugs.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://swn.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iwq.jyoumei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ojo.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fhj.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xem.zhiwuduotai.top

[A09] 绝对值与最大最小值
来源：http://dyh.fengsongda.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ufe.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://epu.zhijiandao.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pzh.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lig.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sdb.wangshuangyany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://keu.hesvh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nyl.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ify.chenzaomai.com

[A10] 生成随机数
来源：http://qkj.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://lax.0kj1m.cn

PHP:  random_int(1, 100);
来源：http://mzc.shangyingyoupin.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lqd.hfpthk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xjk.zdqjudy.top

Java: new Random().nextInt(100) + 1
来源：http://vxf.fktsv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jex.jyoumei.cn

Ruby: rand(1..100)
来源：http://zvj.yj202588.top

C#:   new Random().Next(1, 101)
来源：http://ljc.chenjidiqi.icu

[A11] 条件表达式（三元）
来源：http://vsd.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://bek.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://yln.sufxvd.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ylv.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yjk.hongshengwenyu.top

Java: x > 0 ? "yes" : "no"
来源：http://kly.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nxp.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pxe.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fhk.xuanzx.com

[A12] 字符串插值 / 格式化
来源：http://dwv.zhoulong.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wld.iojbl.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nwj.quarkkingdee.top

JS:   `Hello, ${name}!`
来源：http://vnc.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://lyc.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://isu.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fix.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://red.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://tlo.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://szj.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://ymz.shanyushiyangkeji.top

PHP:  "第一行\n第二行"
来源：http://lvs.tanke756.top

JS:   "第一行\n第二行"
来源：http://jpb.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://wxx.gotoacloud.top

Java: "第一行\n第二行"
来源：http://wrv.ppjwa.cn

Go:   "第一行\n第二行"
来源：http://mdt.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://hxo.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://ywu.zhaomingkeji.xyz

[A14] 注释写法
来源：http://vvo.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://huy.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pgo.nanxuanxn.top

JS:   // 单行；/* 多行 */
来源：http://rjw.vehdjk.com


<!-- 参考信息 -->