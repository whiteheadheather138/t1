代发 wailian999

[U87] JS：解构默认值
来源：http://qwt.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://qkg.yuxming.cn

[U88] JS：对象展开合并
来源：http://aye.jianghu66.top

{ ...a, ...b }
来源：http://pkq.xziqi.cn

[U89] JS：数组去重
来源：http://ecq.ehwqpu.com

[...new Set(arr)]
来源：http://wlr.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://bsa.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://zja.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://soa.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dxf.cheryme.top

[U92] JS：深拷贝
来源：http://wze.yfazqb.com

structuredClone(obj)
来源：http://tjg.xuanzx.com

[U93] JS：模板字符串
来源：http://cak.dashuyun.cn

`共 ${n} 条`
来源：http://vbv.birdmap.top

[U94] JS：箭头函数
来源：http://zpw.meibo888.top

const double = x => x * 2;
来源：http://ywm.cucudq.cn

[U95] JS：Promise 包装
来源：http://vim.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://rht.fehbvm.com

[U96] JS：async/await 与异常
来源：http://gfh.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lof.tianlin.xyz

[U97] JS：并发请求
来源：http://bzs.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ncz.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://mfh.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sdz.zhongyouzk.top

[U99] JS：事件监听
来源：http://yxq.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://ckz.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://uqx.redwolf501.top

document.querySelector(".item")
来源：http://uit.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://miw.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://mri.vehdjk.com

[U102] JS：本地存储
来源：http://dqn.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://asj.cheryme.top

[U103] JS：定时器
来源：http://cgp.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oyl.ppjwa.cn

[U104] JS：防抖
来源：http://ecf.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xqp.tarul.cn

[U105] JS：节流
来源：http://dqe.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lhh.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://jst.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tsq.zhixingplan.top

[U107] JS：数字千分位
来源：http://vec.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kbs.zhixingplan.top

[U108] JS：随机整数
来源：http://hun.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rkw.tianlin.xyz

[U109] JS：数组分组
来源：http://usv.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://rus.snrcjt.cn

[U110] JS：数组分块
来源：http://iso.jinyuanbaomall.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vhk.hfpthk.cn

[U111] JS：对象转 Map
来源：http://jnk.haohaochexian.top

new Map(Object.entries(obj))
来源：http://ecr.zhixingplan.top

[U112] JS：字符串补位
来源：http://sgy.hnqzz.top

"7".padStart(3, "0")
来源：http://izw.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://phn.gogol.net.cn

s.replaceAll("a", "b")
来源：http://oei.yueranfly.top

[U114] JS：JSON 深比较
来源：http://nle.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gww.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://unn.xziqi.cn

crypto.randomUUID()
来源：http://xbp.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://rql.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://kby.bjfxy.top

[U117] JS：单元测试
来源：http://wel.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://occ.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://uoc.gotoacloud.top

npm i -D vite;  npx vite
来源：http://krp.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://lun.meibo888.top

npx vite build
来源：http://jnh.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://ixp.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://jef.hfpthk.cn

================================================================================
来源：http://mae.snrcjt.cn

统计汇总
来源：http://plc.ydjk.org.cn

================================================================================
来源：http://dil.sjlbkw.cn

按语言统计（条）：
来源：http://tev.cqqwz.cn

Python ......... 252
来源：http://omv.birdmap.top

PHP ............ 252
来源：http://lrd.ydjk.org.cn

JavaScript ..... 252
来源：http://dby.xziqi.cn

TypeScript ..... 212
来源：http://nox.hongshengwenyu.top

Java ........... 212
来源：http://upr.jinyuanbaomall.cn

Go ............. 212
来源：http://yeb.yj202588.top

Ruby ........... 212
来源：http://kku.sjlbkw.cn

C# ............. 212
来源：http://ifp.cashguo.top

C .............. 30
来源：http://ksp.9152youxi.cn

C++ ............ 30
来源：http://vfo.hongshengwenyu.top

SQL ............ 90
来源：http://cvb.yueranfly.top

Bash ........... 80
来源：http://iyg.hongshengwenyu.top

Kotlin ......... 15
来源：http://azg.hcnkem.com

Swift .......... 15
来源：http://yxd.hcnkem.com

Lua ............ 10
来源：http://adl.tarul.cn

Perl ........... 10
来源：http://bbh.nanxinkj.top

Scala .......... 10
来源：http://rhw.ydjk.org.cn

------------------------------------
来源：http://vbo.316326.xyz

合计 ........... 2106 条
来源：http://ftc.hongshengwenyu.top

按章节统计：
来源：http://wpz.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eyo.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sgb.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xva.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nsb.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xxf.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ivn.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dqu.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xme.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xnb.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://out.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wjf.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lis.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ltr.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fjo.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rxi.chenzaomai.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://apq.gaohongyu789.top

Q SQL 专题                              90
来源：http://evy.yj202588.top

R Bash 专题                             80
来源：http://nsn.hysaishi.cn

S C / C++ 专题                          60
来源：http://fys.jinqigufen.top

T 其他语言补充                          60
来源：http://irw.ctjpmb.com

U 高频实用片段                         120
来源：http://vbi.hnxiangtu.top

------------------------------------
来源：http://lfe.zhengqikj.top

合计                                  2106 条
来源：http://bqr.aizwys.cn

--------------------------------------------------------------------------------
来源：http://ydo.daria6918.cn

使用提醒
来源：http://hac.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://vec.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dmh.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qhm.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mel.hammf.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kvb.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fvx.meibo888.top

—— 文件结束 ——
来源：http://eol.c1oappe.top

================================================================================
来源：http://twj.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://dns.cashguo.top

Common Programming Examples Cheat Book
来源：http://kdb.vqdsnc.cn

================================================================================
来源：http://bwb.mhx1999.top

【收录内容】
来源：http://qtb.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fqg.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wpx.yueranfly.top

SQL · Bash · C · C++
来源：http://bpr.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://psf.hcnkem.com

【使用说明】
来源：http://tju.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kon.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hhp.yangfankeji.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mju.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eqd.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://mku.c1oappe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wou.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xqh.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zwv.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pdw.shanyushiyangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dls.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ugj.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rlj.zhengqikj.top

【文件统计】
来源：http://cas.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://akf.daxiang520.top

--------------------------------------------------------------------------------
来源：http://nbf.yuxming.cn

目  录
来源：http://fwi.ybcxt.top

--------------------------------------------------------------------------------
来源：http://liz.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hsf.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ycr.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vpr.c1oappe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jpx.52xcode.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jrq.pycfn.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qgz.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ntb.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nge.dashuyun.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qzu.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gcq.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yyr.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vjv.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zrz.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pjr.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cfu.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kst.tanke756.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uuk.nanxuanxn.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wvx.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gqr.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ijv.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kcu.chenzaomai.com

================================================================================
来源：http://jrg.hywenlv.cn

A. 基础语法与类型
来源：http://aqh.zhoulong.xyz

================================================================================
来源：http://pwk.gaohongyu789.top

[A01] Hello World
来源：http://jsv.mhx1999.top

Py:   print("Hello, World!")
来源：http://ojl.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://bvq.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://iiv.shanyushiyangtech.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://msy.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://but.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://qbb.havefunace.top

Ruby: puts "Hello, World!"
来源：http://ene.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ffm.zycfv.cn

[A02] 变量声明与赋值
来源：http://nff.sxryk.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://htj.feifeiyinyue.top

PHP:  $name = "Alex"; $age = 20;
来源：http://nwl.jqgufenzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://tco.xylfe.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sah.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://avj.haohaochexian.top

Go:   name := "Alex"; age := 20
来源：http://apu.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://yvb.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jji.tanke756.top

[A03] 常量定义
来源：http://qew.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eff.cdnleiting.top

PHP:  const PI = 3.14159;
来源：http://prm.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://yol.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://nwe.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://gth.ydzc1.top

Go:   const PI = 3.14159
来源：http://dpp.cashguo.top

Ruby: PI = 3.14159
来源：http://ymv.uphjek.com

C#:   const double PI = 3.14159;
来源：http://fcx.jinyuanbaomall.cn

[A04] 判断变量类型
来源：http://erb.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mln.hfpthk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gqm.zdqjudy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hxp.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://kxp.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gkx.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bxu.chenlongwang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://aif.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://bhj.shzxlz.cn

[A05] 整数除法与取模
来源：http://zyd.yvedp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hol.zhijiandao.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hms.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hab.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pap.sysykeji.top

Java: 7 / 2; 7 % 2
来源：http://sas.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://wae.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://rxr.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://tmx.kuanghao11.cn

[A06] 字符串转数字
来源：http://mwc.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://ajv.zhongyouzk.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dcw.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kdq.hywenlv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pxn.yonumen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sxh.gotoacloud.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oor.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ffj.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://koa.bbcook.cn

[A07] 数字转字符串
来源：http://jjv.zhongyouzk.top

Py:   str(42)
来源：http://guz.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://jxt.yj20258888.top

JS:   String(42); (42).toString()
来源：http://uvc.nanxinkj.top

TS:   String(42)
来源：http://vmt.wangdashe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dbs.tanke756.top

Go:   strconv.Itoa(42)
来源：http://nzl.aibaodan.cn

Ruby: 42.to_s
来源：http://gnm.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://dfs.hysaishi.cn

[A08] 取整与四舍五入
来源：http://tbg.nanxuanxn.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zrs.jlsjyb.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://evu.nwbrower.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lvq.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rqt.havefunace.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sjp.jlsjyb.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://swp.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rnc.xziqi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kix.dianchejie.cn

[A09] 绝对值与最大最小值
来源：http://qbg.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qxp.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eoy.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xbd.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ruz.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oxk.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://evc.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nmo.jiagoushi.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yen.andypj.xyz

[A10] 生成随机数
来源：http://wkd.fanxiaobao.xyz

Py:   import random; random.randint(1, 100)
来源：http://ixi.ydzc1.top

PHP:  random_int(1, 100);
来源：http://mph.gogol.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fny.yj202588.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://odu.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://dpe.guannengcc.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mgq.yangfankeji.com

Ruby: rand(1..100)
来源：http://uoe.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://cvv.gaohongyu789.top

[A11] 条件表达式（三元）
来源：http://nbk.0kj1m.cn

Py:   "yes" if x > 0 else "no"
来源：http://wdg.cqqwz.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rex.yueranfly.top

JS:   x > 0 ? "yes" : "no"
来源：http://kri.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lzk.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://dav.feifeiyinyue.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jql.9152youxi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fcf.haohaochexian.top

C#:   x > 0 ? "yes" : "no"
来源：http://bqd.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://pco.zhixingplan.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://axp.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bqy.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://buz.xinyue.icu

TS:   `Hello, ${name}!`
来源：http://ubm.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://mrf.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gjw.aibaodan.cn

Ruby: "Hello, #{name}!"
来源：http://iqb.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://epw.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hll.gzhubu.top

Py:   "第一行\n第二行"
来源：http://djb.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://yyg.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://vxt.yueranfly.top

TS:   "第一行\n第二行"
来源：http://ogw.yfazqb.com

Java: "第一行\n第二行"
来源：http://pit.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://fsk.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://wbb.dianchejie.cn

C#:   "第一行\n第二行"
来源：http://gnb.guannengcc.top

[A14] 注释写法
来源：http://eog.ydzc1.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://lcu.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gny.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://koe.zdqjudy.top

TS:   // 单行；/* 多行 */
来源：http://rnt.cheryme.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rct.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://ghw.redwolf501.top

Ruby: # 单行；=begin 多行 =end
来源：http://woa.yangfankeji.com


<!-- 参考信息 -->