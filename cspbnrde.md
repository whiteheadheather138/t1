代发 wailian999

[U85] JS：可选链
来源：http://pre.yueranfly.top

a?.b?.c
来源：http://kon.cashguo.top

[U86] JS：空值合并
来源：http://ggk.zdqjudy.top

a ?? b
来源：http://hjy.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://qik.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://vti.c1oappe.top

[U88] JS：对象展开合并
来源：http://lln.hfpthk.cn

{ ...a, ...b }
来源：http://yxl.mhx1999.top

[U89] JS：数组去重
来源：http://eyq.guannengcc.top

[...new Set(arr)]
来源：http://jbn.cqqwz.cn

[U90] JS：数字数组排序
来源：http://gql.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://bzs.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://zjm.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cqk.cqqwz.cn

[U92] JS：深拷贝
来源：http://rxb.ivvv.top

structuredClone(obj)
来源：http://hlp.ybcxt.top

[U93] JS：模板字符串
来源：http://xjc.jiagoushi.top

`共 ${n} 条`
来源：http://ntq.haohaochexian.top

[U94] JS：箭头函数
来源：http://gkn.guannengcc.top

const double = x => x * 2;
来源：http://gwk.hcnkem.com

[U95] JS：Promise 包装
来源：http://cnl.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://sqn.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://ydk.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jzj.chenjidiqi.icu

[U97] JS：并发请求
来源：http://nfg.jqgfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xlb.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://bvk.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cib.feifeiyinyue.top

[U99] JS：事件监听
来源：http://etk.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://joe.316326.xyz

[U100] JS：DOM 查询
来源：http://pwf.guannengcc.top

document.querySelector(".item")
来源：http://fxd.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://rvp.jinqigfzy.top

el.classList.toggle("active")
来源：http://cok.svipenyu.cn

[U102] JS：本地存储
来源：http://jap.shuidangran.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tve.jyoumei.cn

[U103] JS：定时器
来源：http://htn.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cig.jinqigfzy.top

[U104] JS：防抖
来源：http://kdu.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mmn.hnqzz.top

[U105] JS：节流
来源：http://ecr.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ayo.sysykeji.top

[U106] JS：日期格式化
来源：http://iks.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dgf.yanxiufei.cn

[U107] JS：数字千分位
来源：http://tzf.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yia.svipenyu.cn

[U108] JS：随机整数
来源：http://wgz.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lxx.sysykeji.top

[U109] JS：数组分组
来源：http://xac.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://kep.hesvh.cn

[U110] JS：数组分块
来源：http://ptj.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gnw.jiagoushi.top

[U111] JS：对象转 Map
来源：http://xzo.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://zgi.yonumen.top

[U112] JS：字符串补位
来源：http://dej.jqgufenzy.top

"7".padStart(3, "0")
来源：http://ijy.uphjek.com

[U113] JS：正则替换全部
来源：http://qrq.ybcxt.top

s.replaceAll("a", "b")
来源：http://tsu.yfazqb.com

[U114] JS：JSON 深比较
来源：http://ehv.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://loa.havefunace.top

[U115] JS：生成 UUID
来源：http://uzq.zhongyouzk.top

crypto.randomUUID()
来源：http://crm.jqgufenzy.top

[U116] JS：类型检查（JSDoc）
来源：http://pov.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://dcd.uphjek.com

[U117] JS：单元测试
来源：http://sxy.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://jyv.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://fvt.jianghu66.top

npm i -D vite;  npx vite
来源：http://ycm.hnqzz.top

[U119] JS：生产构建
来源：http://cfq.jianghu66.top

npx vite build
来源：http://nym.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://ont.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://iqc.ivvv.top

================================================================================
来源：http://nny.hammf.cn

统计汇总
来源：http://uha.nanxuanxn.top

================================================================================
来源：http://wzu.chenjidiqi.icu

按语言统计（条）：
来源：http://imn.hnxiangtu.top

Python ......... 252
来源：http://txy.jlsjyb.cn

PHP ............ 252
来源：http://rhp.jiagoushi.top

JavaScript ..... 252
来源：http://ltk.zhiwuduotai.top

TypeScript ..... 212
来源：http://yab.yonumen.top

Java ........... 212
来源：http://rdo.tanke756.top

Go ............. 212
来源：http://sjv.sxryk.cn

Ruby ........... 212
来源：http://gin.ydzc1.top

C# ............. 212
来源：http://xpp.sysykeji.top

C .............. 30
来源：http://bqh.ydjk.org.cn

C++ ............ 30
来源：http://ofx.52xcode.cn

SQL ............ 90
来源：http://xdi.uphjek.com

Bash ........... 80
来源：http://aea.shanyushiyangtech.top

Kotlin ......... 15
来源：http://bbj.zdbjq.cn

Swift .......... 15
来源：http://bde.yueranfly.top

Lua ............ 10
来源：http://xtc.jianghu66.top

Perl ........... 10
来源：http://ami.yuanzhike.top

Scala .......... 10
来源：http://xey.shzxlz.cn

------------------------------------
来源：http://aqn.zhongyouzk.top

合计 ........... 2106 条
来源：http://ehs.mhx1999.top

按章节统计：
来源：http://vdu.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gbb.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jcz.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hyu.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jhv.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nmg.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zib.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sbd.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zjv.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://alg.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vpr.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tip.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xbu.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xuy.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://izz.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kjv.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nnv.jlsjyb.cn

Q SQL 专题                              90
来源：http://qgc.chenzaomai.com

R Bash 专题                             80
来源：http://tdl.vqdsnc.cn

S C / C++ 专题                          60
来源：http://uqa.chenlongwang.top

T 其他语言补充                          60
来源：http://fsu.meibo888.top

U 高频实用片段                         120
来源：http://fmj.aizwys.cn

------------------------------------
来源：http://qay.gaohongyu789.top

合计                                  2106 条
来源：http://dlt.hcnkem.com

--------------------------------------------------------------------------------
来源：http://cju.zhengqikj.top

使用提醒
来源：http://edl.cheryme.top

--------------------------------------------------------------------------------
来源：http://gql.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yyp.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zqv.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wln.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://pjm.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nje.tianlin.xyz

—— 文件结束 ——
来源：http://zrd.jinqigufen.top

================================================================================
来源：http://fwk.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://piy.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://xnp.ywan-chungtsiang.top

================================================================================
来源：http://lcl.smart0.xyz

【收录内容】
来源：http://alw.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iag.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qxa.sweek.top

SQL · Bash · C · C++
来源：http://tii.yfazqb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cjp.yj202588.top

【使用说明】
来源：http://oum.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yvk.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vuy.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jef.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://icc.xingfuxueyuan.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://gxy.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wcq.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fsu.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jqg.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ihj.feifeiyinyue.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qtt.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yow.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zkh.dashuyun.cn

【文件统计】
来源：http://baw.pengpengdd.cyou

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://swz.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://ndi.jinqigfzy.top

目  录
来源：http://rpd.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://huy.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://avj.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ays.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ltk.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xdh.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gis.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bsv.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fco.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ptz.ywan-chungtsiang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kre.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bcw.bjfxy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://adq.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xza.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yoz.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mlv.uphjek.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://phh.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yfm.guowangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gvg.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vtk.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hnm.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ghc.pycfn.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mmu.meibo888.top

================================================================================
来源：http://wnh.mhx1999.top

A. 基础语法与类型
来源：http://fjn.hnqzz.top

================================================================================
来源：http://ffm.bjfxy.top

[A01] Hello World
来源：http://lpl.yangfankeji.com

Py:   print("Hello, World!")
来源：http://oec.zhongyouzk.top

PHP:  echo "Hello, World!";
来源：http://vir.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://oit.vqdsnc.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://smc.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://ucb.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://tsr.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://inj.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://knu.hywenlv.cn

[A02] 变量声明与赋值
来源：http://gzh.vehdjk.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ocv.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://osk.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qky.dianchejie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cmk.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://cub.guannengcc.top

Go:   name := "Alex"; age := 20
来源：http://uwh.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://dyp.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://wjv.bjfxy.top

[A03] 常量定义
来源：http://tsx.shanyushiyangtech.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pcn.snrcjt.cn

PHP:  const PI = 3.14159;
来源：http://fyd.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://tfc.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://fza.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://skq.cqqwz.cn

Go:   const PI = 3.14159
来源：http://ckc.hnqzz.top

Ruby: PI = 3.14159
来源：http://whr.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://nla.shanyushiyangkeji.top

[A04] 判断变量类型
来源：http://dtv.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kab.zhongyouzk.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nvs.bbcook.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hzn.wangdashe.top

TS:   typeof x; x instanceof Date
来源：http://taw.hfpthk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bjk.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://meo.iojbl.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ial.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://vtc.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://bii.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iap.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://oav.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rje.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ufm.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://ndv.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://gsn.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://ike.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://fcc.fanxiaobao.xyz

[A06] 字符串转数字
来源：http://ouv.yuanzhike.top

Py:   int("42"); float("3.14")
来源：http://ijn.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jhh.yj202588.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zvy.nanxuanxn.top

TS:   parseInt("42", 10); Number("42")
来源：http://ylr.quarkkingdee.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ods.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kdg.zhijiandao.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pvp.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wsr.vqdsnc.cn

[A07] 数字转字符串
来源：http://qwk.andypj.xyz

Py:   str(42)
来源：http://bpo.chenlongwang.top

PHP:  (string) 42; strval(42)
来源：http://thx.epnwcf.com

JS:   String(42); (42).toString()
来源：http://ebm.jinghuilouyu.cn

TS:   String(42)
来源：http://laa.zhoulong.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://xoc.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://umr.yj20258.top

Ruby: 42.to_s
来源：http://ynj.redwolf501.top

C#:   42.ToString()
来源：http://iou.daxiang520.top

[A08] 取整与四舍五入
来源：http://ite.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wvo.hammf.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xzu.gogol.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lmj.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lnf.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gml.cdnleiting.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://evh.zdbjq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eyq.zhiwuduotai.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ldu.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://szk.dianchejie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zdj.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dpx.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rql.yuxming.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vxy.daria6918.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zrp.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ywy.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fzk.ehwqpu.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://czc.jlsjyb.cn

[A10] 生成随机数
来源：http://yvj.nwbrower.top

Py:   import random; random.randint(1, 100)
来源：http://abf.zycfv.cn

PHP:  random_int(1, 100);
来源：http://eei.havefunace.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fdp.wangshuangyany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mht.snrcjt.cn

Java: new Random().nextInt(100) + 1
来源：http://zmz.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://inp.hysaishi.cn

Ruby: rand(1..100)
来源：http://aff.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://yge.epnwcf.com

[A11] 条件表达式（三元）
来源：http://dlj.fktsv.cn

Py:   "yes" if x > 0 else "no"
来源：http://ehx.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nty.shanyushiyangtech.top

JS:   x > 0 ? "yes" : "no"
来源：http://yca.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://grz.yueranfly.top

Java: x > 0 ? "yes" : "no"
来源：http://lac.tanke756.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xfd.yongpay.top

Ruby: x > 0 ? "yes" : "no"
来源：http://whi.hcnkem.com

C#:   x > 0 ? "yes" : "no"
来源：http://fqf.mhx1999.top

[A12] 字符串插值 / 格式化
来源：http://xve.daria6918.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://frj.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hok.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://vjq.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://jqf.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://vaz.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rvo.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://jvc.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://buj.yuanzhike.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ltt.sysykeji.top

Py:   "第一行\n第二行"
来源：http://mwb.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://gxv.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://hgb.daria6918.cn

TS:   "第一行\n第二行"
来源：http://zfm.cheryme.top

Java: "第一行\n第二行"
来源：http://qeq.andypj.xyz

Go:   "第一行\n第二行"
来源：http://bew.zhengqikj.top

Ruby: "第一行\n第二行"
来源：http://gcp.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://pls.andypj.xyz

[A14] 注释写法
来源：http://mih.shuidangran.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://two.aizwys.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kcz.9152youxi.cn

JS:   // 单行；/* 多行 */
来源：http://nho.vqdsnc.cn


<!-- 参考信息 -->