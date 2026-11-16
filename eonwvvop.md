代发 wailian999

[U87] JS：解构默认值
来源：http://jzl.shzxlz.cn

const { a = 1, b = 2 } = obj;
来源：http://bzy.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://dtg.birdmap.top

{ ...a, ...b }
来源：http://ovf.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://jve.316326.xyz

[...new Set(arr)]
来源：http://ybb.snrcjt.cn

[U90] JS：数字数组排序
来源：http://qsf.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://gzj.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://tdw.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://csp.tianlin.xyz

[U92] JS：深拷贝
来源：http://bne.hesvh.cn

structuredClone(obj)
来源：http://pgu.hesvh.cn

[U93] JS：模板字符串
来源：http://zfo.bbcook.cn

`共 ${n} 条`
来源：http://leu.zdbjq.cn

[U94] JS：箭头函数
来源：http://hwi.fehbvm.com

const double = x => x * 2;
来源：http://ess.smart0.xyz

[U95] JS：Promise 包装
来源：http://nmr.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://plg.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://nfa.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nkc.shuidangran.top

[U97] JS：并发请求
来源：http://yqq.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://irm.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://hih.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vbp.tian-w.cn

[U99] JS：事件监听
来源：http://tjg.daria6918.cn

el.addEventListener("click", e => {})
来源：http://vun.hysaishi.cn

[U100] JS：DOM 查询
来源：http://bpr.sufxvd.cn

document.querySelector(".item")
来源：http://evu.fengsongda.top

[U101] JS：classList 操作
来源：http://nul.tian-w.cn

el.classList.toggle("active")
来源：http://eth.chenlongwang.top

[U102] JS：本地存储
来源：http://wtv.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://wrw.sysykeji.top

[U103] JS：定时器
来源：http://pxh.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jra.zhixingplan.top

[U104] JS：防抖
来源：http://rwm.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xrq.nanxuanxn.top

[U105] JS：节流
来源：http://zrh.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rna.jyoumei.cn

[U106] JS：日期格式化
来源：http://ecb.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fvx.jyoumei.cn

[U107] JS：数字千分位
来源：http://ycw.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://akd.yanxiufei.cn

[U108] JS：随机整数
来源：http://edc.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vkl.aizwys.cn

[U109] JS：数组分组
来源：http://tzi.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://rxw.zhixingplan.top

[U110] JS：数组分块
来源：http://xxm.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nxy.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://xcx.cucudq.cn

new Map(Object.entries(obj))
来源：http://kwi.sxryk.cn

[U112] JS：字符串补位
来源：http://acr.ivvv.top

"7".padStart(3, "0")
来源：http://tww.sxryk.cn

[U113] JS：正则替换全部
来源：http://mws.yuxming.cn

s.replaceAll("a", "b")
来源：http://vwo.nwbrower.top

[U114] JS：JSON 深比较
来源：http://kxn.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcn.yj20258.top

[U115] JS：生成 UUID
来源：http://jil.jqgufenzy.top

crypto.randomUUID()
来源：http://kqb.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://kwd.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://jcg.cdnleiting.top

[U117] JS：单元测试
来源：http://kra.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://ltq.yj20258.top

[U118] JS：开发服务器
来源：http://owf.yj20258.top

npm i -D vite;  npx vite
来源：http://ogy.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://aam.bbcook.cn

npx vite build
来源：http://emj.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://xnz.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://lkp.zdbjq.cn

================================================================================
来源：http://bho.nanxinkj.top

统计汇总
来源：http://wrg.tarul.cn

================================================================================
来源：http://jyy.havefunace.top

按语言统计（条）：
来源：http://fbi.nanxuanxn.top

Python ......... 252
来源：http://tzp.tarul.cn

PHP ............ 252
来源：http://nnf.ydjk.org.cn

JavaScript ..... 252
来源：http://yoz.feifeiyinyue.top

TypeScript ..... 212
来源：http://rka.kuanghao11.cn

Java ........... 212
来源：http://ufn.sxryk.cn

Go ............. 212
来源：http://qji.wangshuangyany.cn

Ruby ........... 212
来源：http://rhv.shzxlz.cn

C# ............. 212
来源：http://pzn.nanxuanxn.top

C .............. 30
来源：http://poq.tarul.cn

C++ ............ 30
来源：http://yfy.zhijiandao.cn

SQL ............ 90
来源：http://iur.fengsongda.top

Bash ........... 80
来源：http://vfn.0kj1m.cn

Kotlin ......... 15
来源：http://bre.fktsv.cn

Swift .......... 15
来源：http://vja.shanyushiyangkeji.top

Lua ............ 10
来源：http://hus.vqdsnc.cn

Perl ........... 10
来源：http://tik.meibo888.top

Scala .......... 10
来源：http://avl.jinyuanbaomall.cn

------------------------------------
来源：http://xms.ctjpmb.com

合计 ........... 2106 条
来源：http://fdt.fehbvm.com

按章节统计：
来源：http://aey.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://adr.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qsc.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rag.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fxk.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yin.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ajb.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kmb.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zvo.zhijiandao.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ghp.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xld.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jka.yj20258.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bbt.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hse.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pjs.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mss.jyoumei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://txc.jqgufenzy.top

Q SQL 专题                              90
来源：http://obk.sxryk.cn

R Bash 专题                             80
来源：http://wca.hnxiangtu.top

S C / C++ 专题                          60
来源：http://oqu.ehwqpu.com

T 其他语言补充                          60
来源：http://sif.dianchejie.cn

U 高频实用片段                         120
来源：http://kei.zhiwuduotai.top

------------------------------------
来源：http://zyj.sxryk.cn

合计                                  2106 条
来源：http://fjk.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://lqe.jinghuilouyu.cn

使用提醒
来源：http://alp.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://evk.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rxf.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uat.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qmv.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sbm.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qnm.xuetiantiany.cn

—— 文件结束 ——
来源：http://evs.yvedp.cn

================================================================================
来源：http://mpc.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://tvd.daxiang520.top

Common Programming Examples Cheat Book
来源：http://qxi.tanke756.top

================================================================================
来源：http://wrn.ydzc1.top

【收录内容】
来源：http://zlr.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://upp.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tpj.cucudq.cn

SQL · Bash · C · C++
来源：http://tgl.ppjwa.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pop.kuanghao11.cn

【使用说明】
来源：http://ckf.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://itw.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cif.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jxn.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kuz.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://tiz.jqgfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zwm.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eqk.dianchejie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pbr.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cgh.cheryme.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qpp.tian-w.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lbw.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nmd.haohaochexian.top

【文件统计】
来源：http://jxs.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://don.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://lak.fktsv.cn

目  录
来源：http://neo.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://fjh.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xru.yfazqb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gtp.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hob.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://faj.cucudq.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://llw.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ski.yfazqb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bul.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ypf.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kzw.xylfe.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rhs.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kqp.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kzl.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tzz.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zqk.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zgv.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fvm.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://chz.snrcjt.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hca.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rko.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kha.tarul.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bhb.hcnkem.com

================================================================================
来源：http://vpc.hcnkem.com

A. 基础语法与类型
来源：http://nkm.dashuyun.cn

================================================================================
来源：http://iyk.nanxuanxn.top

[A01] Hello World
来源：http://xnm.nanxinkj.top

Py:   print("Hello, World!")
来源：http://hkb.hongshengwenyu.top

PHP:  echo "Hello, World!";
来源：http://ezv.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://wlq.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hrt.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://dxh.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://mot.ehwqpu.com

Ruby: puts "Hello, World!"
来源：http://iwb.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vdz.zdqjudy.top

[A02] 变量声明与赋值
来源：http://pec.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tfx.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dcb.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://npa.birdmap.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://psa.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://noa.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://dla.0kj1m.cn

Ruby: name = "Alex"; age = 20
来源：http://fij.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jbx.xinyue.icu

[A03] 常量定义
来源：http://lre.fengsongda.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ccc.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://jif.zycfv.cn

JS:   const PI = 3.14159;
来源：http://gig.cdnleiting.top

TS:   const PI: number = 3.14159;
来源：http://rsg.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://bmc.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://xzq.pycfn.com

Ruby: PI = 3.14159
来源：http://sdt.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://wou.chenjidiqi.icu

[A04] 判断变量类型
来源：http://gep.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wid.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ebk.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xbp.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://qwi.sweek.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uxa.shangyingyoupin.top

Go:   reflect.TypeOf(x).Name()
来源：http://fof.jinyuanbaomall.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mld.jlsjyb.cn

C#:   x.GetType().Name; x is int
来源：http://gtw.gogol.net.cn

[A05] 整数除法与取模
来源：http://wxv.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dzm.yj202588.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://all.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bbf.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mcv.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://ttn.jinyuanbaomall.cn

Go:   7 / 2; 7 % 2
来源：http://tve.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://rqf.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://obh.aibaodan.cn

[A06] 字符串转数字
来源：http://hxm.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://nbn.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fci.jianghu66.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rmg.zdqjudy.top

TS:   parseInt("42", 10); Number("42")
来源：http://bvk.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uxo.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jgh.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vyy.zhoulong.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jtb.fzhhl.top

[A07] 数字转字符串
来源：http://lrf.ppjwa.cn

Py:   str(42)
来源：http://doq.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://gxv.yonumen.top

JS:   String(42); (42).toString()
来源：http://lex.xuetiantiany.cn

TS:   String(42)
来源：http://kcb.52xcode.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gkk.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://qwa.yj202588.top

Ruby: 42.to_s
来源：http://hia.pycfn.com

C#:   42.ToString()
来源：http://dki.feifeiyinyue.top

[A08] 取整与四舍五入
来源：http://kic.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kxa.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gie.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sql.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dze.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rne.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jfv.xingfuxueyuan.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://iru.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lud.jlsjyb.cn

[A09] 绝对值与最大最小值
来源：http://gvt.xylfe.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zxu.gaohongyu789.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zro.svipenyu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://miy.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://znu.bjfxy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yzi.xziqi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xuc.daxiang520.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yif.ywan-chungtsiang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fsq.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://ozw.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://yyn.xziqi.cn

PHP:  random_int(1, 100);
来源：http://ued.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eha.yueranfly.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://edx.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://cnz.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zdk.hysaishi.cn

Ruby: rand(1..100)
来源：http://tvc.haohaochexian.top

C#:   new Random().Next(1, 101)
来源：http://wqi.yueranfly.top

[A11] 条件表达式（三元）
来源：http://jpu.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://ofd.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ffk.jinqigufen.top

JS:   x > 0 ? "yes" : "no"
来源：http://xad.guowangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://tjg.jinghuilouyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://yty.guowangkeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://iuy.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pjq.quarkkingdee.top

C#:   x > 0 ? "yes" : "no"
来源：http://tkt.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://sdm.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xjn.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rkx.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://pcv.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://vsl.yueranfly.top

Java: "Hello, %s!".formatted(name)
来源：http://uev.yangfankeji.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ekw.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://mqq.chenlongwang.top

C#:   $"Hello, {name}!"
来源：http://jye.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://uiu.xuanzx.com

Py:   "第一行\n第二行"
来源：http://uct.redwolf501.top

PHP:  "第一行\n第二行"
来源：http://jfs.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://ikl.hongshengwenyu.top

TS:   "第一行\n第二行"
来源：http://wum.quarkkingdee.top

Java: "第一行\n第二行"
来源：http://ihs.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://dht.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://bzq.fengsongda.top

C#:   "第一行\n第二行"
来源：http://mvq.mhx1999.top

[A14] 注释写法
来源：http://scj.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ayz.nwbrower.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iuu.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://zok.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://elx.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pav.zdbjq.cn

Go:   // 单行；/* 多行 */
来源：http://mkm.gotoacloud.top

Ruby: # 单行；=begin 多行 =end
来源：http://qbo.yj202588.top


<!-- 参考信息 -->