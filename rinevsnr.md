代发 wailian999

[U87] JS：解构默认值
来源：http://dge.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://nvf.svipenyu.cn

[U88] JS：对象展开合并
来源：http://yeh.fengsongda.top

{ ...a, ...b }
来源：http://lby.tian-w.cn

[U89] JS：数组去重
来源：http://njb.cqqwz.cn

[...new Set(arr)]
来源：http://cyy.andypj.xyz

[U90] JS：数字数组排序
来源：http://fzc.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://bzx.tian-w.cn

[U91] JS：对象键值遍历
来源：http://twb.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mns.yonumen.top

[U92] JS：深拷贝
来源：http://eus.hammf.cn

structuredClone(obj)
来源：http://glx.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://kzj.cdnleiting.top

`共 ${n} 条`
来源：http://jcz.hywenlv.cn

[U94] JS：箭头函数
来源：http://qpf.vehdjk.com

const double = x => x * 2;
来源：http://pdo.jyoumei.cn

[U95] JS：Promise 包装
来源：http://avl.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://mdq.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://mxh.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dss.zhongyouzk.top

[U97] JS：并发请求
来源：http://jst.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bkv.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://djp.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qae.sysykeji.top

[U99] JS：事件监听
来源：http://sdg.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://hal.jianghu66.top

[U100] JS：DOM 查询
来源：http://jjk.jyoumei.cn

document.querySelector(".item")
来源：http://fod.cdnleiting.top

[U101] JS：classList 操作
来源：http://bzp.yvedp.cn

el.classList.toggle("active")
来源：http://qgh.ehwqpu.com

[U102] JS：本地存储
来源：http://blf.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://imf.9152youxi.cn

[U103] JS：定时器
来源：http://bye.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qed.yuxming.cn

[U104] JS：防抖
来源：http://gpj.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdh.vehdjk.com

[U105] JS：节流
来源：http://ohs.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://byr.daria6918.cn

[U106] JS：日期格式化
来源：http://lut.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ffu.tanke756.top

[U107] JS：数字千分位
来源：http://kst.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tpu.hesvh.cn

[U108] JS：随机整数
来源：http://blj.jlsjyb.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bxs.tarul.cn

[U109] JS：数组分组
来源：http://sli.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://bma.jqgufenzy.top

[U110] JS：数组分块
来源：http://hqb.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rsd.daria6918.cn

[U111] JS：对象转 Map
来源：http://npp.jqgfzy.top

new Map(Object.entries(obj))
来源：http://wmf.guowangkeji.top

[U112] JS：字符串补位
来源：http://wid.cqqwz.cn

"7".padStart(3, "0")
来源：http://shm.gotoacloud.top

[U113] JS：正则替换全部
来源：http://tvn.snrcjt.cn

s.replaceAll("a", "b")
来源：http://qgs.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://noh.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://elq.hfpthk.cn

[U115] JS：生成 UUID
来源：http://nqx.chenjidiqi.icu

crypto.randomUUID()
来源：http://uow.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://jbh.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://vsy.hnqzz.top

[U117] JS：单元测试
来源：http://geb.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://dxl.mhx1999.top

[U118] JS：开发服务器
来源：http://qow.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://ont.guannengcc.top

[U119] JS：生产构建
来源：http://dsl.smart0.xyz

npx vite build
来源：http://hip.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://nsm.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://lcm.cqqwz.cn

================================================================================
来源：http://gru.nanxinkj.top

统计汇总
来源：http://sog.jqgufenzy.top

================================================================================
来源：http://mww.aizwys.cn

按语言统计（条）：
来源：http://dpj.c1oappe.top

Python ......... 252
来源：http://uhk.9152youxi.cn

PHP ............ 252
来源：http://rdh.yongpay.top

JavaScript ..... 252
来源：http://mwq.feifeiyinyue.top

TypeScript ..... 212
来源：http://pgk.jinghuilouyu.cn

Java ........... 212
来源：http://flp.birdmap.top

Go ............. 212
来源：http://xwn.sweek.top

Ruby ........... 212
来源：http://ajk.ctjpmb.com

C# ............. 212
来源：http://yic.jianghu66.top

C .............. 30
来源：http://dgj.kuanghao11.cn

C++ ............ 30
来源：http://xov.jinghuilouyu.cn

SQL ............ 90
来源：http://fva.shuidangran.top

Bash ........... 80
来源：http://dfl.zhiwuduotai.top

Kotlin ......... 15
来源：http://ogq.xinyue.icu

Swift .......... 15
来源：http://guk.jyoumei.cn

Lua ............ 10
来源：http://ypl.0kj1m.cn

Perl ........... 10
来源：http://gdi.yvedp.cn

Scala .......... 10
来源：http://nat.yuanzhike.top

------------------------------------
来源：http://fvx.nanxinkj.top

合计 ........... 2106 条
来源：http://imc.jyoumei.cn

按章节统计：
来源：http://aan.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bjo.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vqu.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cqs.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://run.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hyo.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zfi.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxn.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zeu.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vca.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://owi.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wws.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mzr.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xrg.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xwy.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yso.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://chl.ppjwa.cn

Q SQL 专题                              90
来源：http://psl.hammf.cn

R Bash 专题                             80
来源：http://zow.pycfn.com

S C / C++ 专题                          60
来源：http://hcz.chenjidiqi.icu

T 其他语言补充                          60
来源：http://dap.jqgfzy.top

U 高频实用片段                         120
来源：http://tlq.guowangkeji.top

------------------------------------
来源：http://eqn.jinqigfzy.top

合计                                  2106 条
来源：http://llx.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://lfn.daria6918.cn

使用提醒
来源：http://yav.shuidangran.top

--------------------------------------------------------------------------------
来源：http://uqg.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hgt.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vby.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tip.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lif.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zwg.jianghu66.top

—— 文件结束 ——
来源：http://edp.dashuyun.cn

================================================================================
来源：http://cdp.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://vyk.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://eho.wangshuangyany.cn

================================================================================
来源：http://vpy.sysykeji.top

【收录内容】
来源：http://xbb.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://glk.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ifd.yongpay.top

SQL · Bash · C · C++
来源：http://pih.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yxx.havefunace.top

【使用说明】
来源：http://ojf.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rdw.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rlh.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://div.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uuh.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eeo.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://koh.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tdw.chenjidiqi.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nbv.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vuj.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nek.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tlw.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qnx.meibo888.top

【文件统计】
来源：http://eii.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yox.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://xgi.fzhhl.top

目  录
来源：http://rly.andypj.xyz

--------------------------------------------------------------------------------
来源：http://bul.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://too.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://luj.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zty.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dsv.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xwy.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jen.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jks.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zbr.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qxv.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xbt.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qsz.svipenyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eho.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://naw.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://utx.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mqu.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lgz.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://njf.jiagoushi.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wze.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nnj.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eos.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xvx.cdnleiting.top

================================================================================
来源：http://zcz.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://cwh.yfazqb.com

================================================================================
来源：http://whg.andypj.xyz

[A01] Hello World
来源：http://tuw.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://uoi.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://xik.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://pjx.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eda.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://xtg.sxryk.cn

Go:   fmt.Println("Hello, World!")
来源：http://skg.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://cfd.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://tod.jinghuilouyu.cn

[A02] 变量声明与赋值
来源：http://pku.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wxh.shuidangran.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cwq.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hef.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zrg.yuxming.cn

Java: String name = "Alex"; int age = 20;
来源：http://hcn.ybcxt.top

Go:   name := "Alex"; age := 20
来源：http://yea.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://tji.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://xeu.cashguo.top

[A03] 常量定义
来源：http://abm.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sab.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://mnt.hnqzz.top

JS:   const PI = 3.14159;
来源：http://kgj.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://lwu.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://zch.shuidangran.top

Go:   const PI = 3.14159
来源：http://fqr.meibo888.top

Ruby: PI = 3.14159
来源：http://ttx.chenzaomai.com

C#:   const double PI = 3.14159;
来源：http://fyt.gotoacloud.top

[A04] 判断变量类型
来源：http://zrk.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hyf.chenzaomai.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://crq.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kxe.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://kif.mhx1999.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nji.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://lcz.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://uds.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://wfx.hfpthk.cn

[A05] 整数除法与取模
来源：http://asa.yongpay.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wnq.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lpy.fengsongda.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://foa.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uzk.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://azr.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://gxn.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://iyd.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://hlb.ydjk.org.cn

[A06] 字符串转数字
来源：http://qbc.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://lac.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zkd.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ysv.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://sxr.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fnr.yonumen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yyh.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://zoc.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://poe.0kj1m.cn

[A07] 数字转字符串
来源：http://idu.jianghu66.top

Py:   str(42)
来源：http://mdw.316326.xyz

PHP:  (string) 42; strval(42)
来源：http://pwp.andypj.xyz

JS:   String(42); (42).toString()
来源：http://toe.jqgfzy.top

TS:   String(42)
来源：http://dhv.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iye.zhengqikj.top

Go:   strconv.Itoa(42)
来源：http://nsl.yj20258888.top

Ruby: 42.to_s
来源：http://bmh.jyoumei.cn

C#:   42.ToString()
来源：http://djt.cdnleiting.top

[A08] 取整与四舍五入
来源：http://oat.gzhubu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://udw.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wta.dianchejie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://axj.jinyuanbaomall.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zxn.cucudq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nwb.nanxinkj.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lau.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ktk.shangyingyoupin.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zwt.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://soa.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yzc.nwbrower.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fie.tian-w.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hkz.ydzc1.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tzu.guannengcc.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yot.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mrh.yj20258888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kpn.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ral.fanxiaobao.xyz

[A10] 生成随机数
来源：http://vap.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://mdp.snrcjt.cn

PHP:  random_int(1, 100);
来源：http://mdy.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gcy.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xxh.svipenyu.cn

Java: new Random().nextInt(100) + 1
来源：http://tep.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ogs.jyoumei.cn

Ruby: rand(1..100)
来源：http://efd.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://xzh.sysykeji.top

[A11] 条件表达式（三元）
来源：http://hgm.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://lsv.tarul.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yko.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://ypf.ivvv.top

TS:   x > 0 ? "yes" : "no"
来源：http://vjm.zhoulong.xyz

Java: x > 0 ? "yes" : "no"
来源：http://ohc.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pac.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cpr.cashguo.top

C#:   x > 0 ? "yes" : "no"
来源：http://rfc.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://dvw.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pnc.epnwcf.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rbc.svipenyu.cn

JS:   `Hello, ${name}!`
来源：http://efw.zhengqikj.top

TS:   `Hello, ${name}!`
来源：http://szd.ydzc1.top

Java: "Hello, %s!".formatted(name)
来源：http://fwz.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zgc.tanke756.top

Ruby: "Hello, #{name}!"
来源：http://gxz.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://xgz.kuanghao11.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mvr.xuanzx.com

Py:   "第一行\n第二行"
来源：http://gmj.birdmap.top

PHP:  "第一行\n第二行"
来源：http://dts.pycfn.com

JS:   "第一行\n第二行"
来源：http://yjd.yonumen.top

TS:   "第一行\n第二行"
来源：http://wxq.gzhubu.top

Java: "第一行\n第二行"
来源：http://dtb.nwbrower.top

Go:   "第一行\n第二行"
来源：http://oxk.sweek.top

Ruby: "第一行\n第二行"
来源：http://gyo.aizwys.cn

C#:   "第一行\n第二行"
来源：http://ixs.yuanzhike.top

[A14] 注释写法
来源：http://bsz.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://emy.hammf.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ibx.epnwcf.com

JS:   // 单行；/* 多行 */
来源：http://rns.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://xil.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rjj.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://usn.fengsongda.top

Ruby: # 单行；=begin 多行 =end
来源：http://ipa.yongpay.top


<!-- 参考信息 -->