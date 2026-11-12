代发 wailian999

[U91] JS：对象键值遍历
来源：http://zrj.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zuw.ehwqpu.com

[U92] JS：深拷贝
来源：http://ygb.quarkkingdee.top

structuredClone(obj)
来源：http://acb.daria6918.cn

[U93] JS：模板字符串
来源：http://hpb.jinqigufen.top

`共 ${n} 条`
来源：http://rtu.ybcxt.top

[U94] JS：箭头函数
来源：http://jhc.jinghuilouyu.cn

const double = x => x * 2;
来源：http://guu.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://dyi.yj20258.top

new Promise((resolve, reject) => {})
来源：http://cof.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://yqd.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hon.wangdashe.top

[U97] JS：并发请求
来源：http://roz.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://umk.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://vxm.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fkp.tarul.cn

[U99] JS：事件监听
来源：http://elr.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://wtq.jiagoushi.top

[U100] JS：DOM 查询
来源：http://scu.52xcode.cn

document.querySelector(".item")
来源：http://bgs.meibo888.top

[U101] JS：classList 操作
来源：http://lny.ctjpmb.com

el.classList.toggle("active")
来源：http://uvi.zycfv.cn

[U102] JS：本地存储
来源：http://tdd.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://alv.zhoulong.xyz

[U103] JS：定时器
来源：http://lug.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vbo.ctjpmb.com

[U104] JS：防抖
来源：http://sdt.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tue.haohaochexian.top

[U105] JS：节流
来源：http://pcl.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://djd.wangdashe.top

[U106] JS：日期格式化
来源：http://mle.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://php.ehwqpu.com

[U107] JS：数字千分位
来源：http://ufq.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://euf.guannengcc.top

[U108] JS：随机整数
来源：http://glu.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wiz.jiagoushi.top

[U109] JS：数组分组
来源：http://nbc.gzhubu.top

Object.groupBy(arr, x => x.type)
来源：http://fcb.uphjek.com

[U110] JS：数组分块
来源：http://oee.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://erg.xinyue.icu

[U111] JS：对象转 Map
来源：http://icc.vehdjk.com

new Map(Object.entries(obj))
来源：http://ghh.bbcook.cn

[U112] JS：字符串补位
来源：http://ccw.9152youxi.cn

"7".padStart(3, "0")
来源：http://mkk.ctjpmb.com

[U113] JS：正则替换全部
来源：http://fte.tarul.cn

s.replaceAll("a", "b")
来源：http://kep.hcnkem.com

[U114] JS：JSON 深比较
来源：http://hhb.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hyg.zdbjq.cn

[U115] JS：生成 UUID
来源：http://waf.nanxinkj.top

crypto.randomUUID()
来源：http://kxx.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://oap.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://jbc.fengsongda.top

[U117] JS：单元测试
来源：http://sgx.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://ppj.yuxming.cn

[U118] JS：开发服务器
来源：http://qzs.nwbrower.top

npm i -D vite;  npx vite
来源：http://otn.jyoumei.cn

[U119] JS：生产构建
来源：http://qzg.bjfxy.top

npx vite build
来源：http://cme.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://orh.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://lqb.hongshengwenyu.top

================================================================================
来源：http://sub.dianchejie.cn

统计汇总
来源：http://wrn.vqdsnc.cn

================================================================================
来源：http://bcs.jlsjyb.cn

按语言统计（条）：
来源：http://efw.jianghu66.top

Python ......... 252
来源：http://ked.nanxinkj.top

PHP ............ 252
来源：http://qwq.fanxiaobao.xyz

JavaScript ..... 252
来源：http://bkk.zhijiandao.cn

TypeScript ..... 212
来源：http://hsn.yj20258888.top

Java ........... 212
来源：http://zyz.gogol.net.cn

Go ............. 212
来源：http://mdy.pengpengdd.cyou

Ruby ........... 212
来源：http://bfx.quarkkingdee.top

C# ............. 212
来源：http://mqk.dashuyun.cn

C .............. 30
来源：http://lcs.aizwys.cn

C++ ............ 30
来源：http://ieo.pengpengdd.cyou

SQL ............ 90
来源：http://xlb.hesvh.cn

Bash ........... 80
来源：http://vmz.fengsongda.top

Kotlin ......... 15
来源：http://gqf.yongpay.top

Swift .......... 15
来源：http://spq.tian-w.cn

Lua ............ 10
来源：http://ozd.xylfe.cn

Perl ........... 10
来源：http://imq.chenlongwang.top

Scala .......... 10
来源：http://sot.wangshuangyany.cn

------------------------------------
来源：http://xng.meibo888.top

合计 ........... 2106 条
来源：http://ddy.zhixingplan.top

按章节统计：
来源：http://yjq.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hon.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://klx.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dzy.cheryme.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ddk.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bcp.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pom.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ivb.jqgufenzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mmk.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kne.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fmg.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bhe.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ggf.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rtv.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://axd.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mld.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://thi.jiagoushi.top

Q SQL 专题                              90
来源：http://kpk.ybcxt.top

R Bash 专题                             80
来源：http://kbx.yuanzhike.top

S C / C++ 专题                          60
来源：http://sfw.tian-w.cn

T 其他语言补充                          60
来源：http://zgj.tianlin.xyz

U 高频实用片段                         120
来源：http://pkt.havefunace.top

------------------------------------
来源：http://noo.jinqigufen.top

合计                                  2106 条
来源：http://myh.hnqzz.top

--------------------------------------------------------------------------------
来源：http://bmp.vehdjk.com

使用提醒
来源：http://guj.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://qvu.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yqk.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tcg.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kvy.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mtm.yongpay.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xpv.ydjk.org.cn

—— 文件结束 ——
来源：http://kka.meibo888.top

================================================================================
来源：http://tun.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://xzg.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://qus.pengpengdd.cyou

================================================================================
来源：http://jvi.cdnleiting.top

【收录内容】
来源：http://jbj.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fbl.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://whe.xziqi.cn

SQL · Bash · C · C++
来源：http://ucv.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zwp.zdqjudy.top

【使用说明】
来源：http://tud.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fbg.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nvt.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://giv.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hfp.yuxming.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xwo.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xao.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://usc.meibo888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ysl.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://amg.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://suc.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fvf.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://npk.jqgfzy.top

【文件统计】
来源：http://lcp.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qir.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://udu.smart0.xyz

目  录
来源：http://rnh.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://xfo.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bup.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://npt.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kyk.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cmr.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nrk.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tuc.tian-w.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jhp.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sos.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cyk.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jbu.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rlp.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://val.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lqk.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bea.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wog.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rwu.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mcj.bjfxy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bcn.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yme.jinyuanbaomall.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zsl.chenlongwang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dbo.havefunace.top

================================================================================
来源：http://qmo.shzxlz.cn

A. 基础语法与类型
来源：http://nmn.dianchejie.cn

================================================================================
来源：http://jmw.guannengcc.top

[A01] Hello World
来源：http://lqg.ywan-chungtsiang.top

Py:   print("Hello, World!")
来源：http://gcd.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://xqu.sjlbkw.cn

JS:   console.log("Hello, World!");
来源：http://sdz.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xlw.uphjek.com

Java: System.out.println("Hello, World!");
来源：http://gly.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://xgj.jinqigufen.top

Ruby: puts "Hello, World!"
来源：http://jsf.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://xgu.yangfankeji.com

[A02] 变量声明与赋值
来源：http://eog.yonumen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bhu.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jjz.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://avn.yanxiufei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oid.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://fud.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://qsl.9152youxi.cn

Ruby: name = "Alex"; age = 20
来源：http://kbf.cucudq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ivs.yongpay.top

[A03] 常量定义
来源：http://vas.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hju.yongpay.top

PHP:  const PI = 3.14159;
来源：http://pqp.fengsongda.top

JS:   const PI = 3.14159;
来源：http://xti.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://pgd.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://vdy.nanxinkj.top

Go:   const PI = 3.14159
来源：http://oxi.shanyushiyangkeji.top

Ruby: PI = 3.14159
来源：http://fdc.feifeiyinyue.top

C#:   const double PI = 3.14159;
来源：http://zmf.guowangkeji.top

[A04] 判断变量类型
来源：http://dvo.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zpd.birdmap.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://euz.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ere.chenjidiqi.icu

TS:   typeof x; x instanceof Date
来源：http://ote.gotoacloud.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mpf.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aem.sysykeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xop.yj20258888.top

C#:   x.GetType().Name; x is int
来源：http://zwm.quarkkingdee.top

[A05] 整数除法与取模
来源：http://eet.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zqn.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://fwq.fzhhl.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mqr.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xpp.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://nwh.vehdjk.com

Go:   7 / 2; 7 % 2
来源：http://hwh.sxryk.cn

Ruby: 7 / 2; 7 % 2
来源：http://izs.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://oql.quarkkingdee.top

[A06] 字符串转数字
来源：http://jsj.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://nre.kuanghao11.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wyz.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vxe.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://wai.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://are.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://geq.epnwcf.com

Ruby: "42".to_i; "3.14".to_f
来源：http://zwc.yongpay.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://azu.zhixingplan.top

[A07] 数字转字符串
来源：http://qoe.yanxiufei.cn

Py:   str(42)
来源：http://lsr.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://fmn.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://tzz.xingfuxueyuan.xyz

TS:   String(42)
来源：http://spa.yongpay.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://udt.meibo888.top

Go:   strconv.Itoa(42)
来源：http://lay.xuetiantiany.cn

Ruby: 42.to_s
来源：http://asq.daria6918.cn

C#:   42.ToString()
来源：http://dcn.yueranfly.top

[A08] 取整与四舍五入
来源：http://otf.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oli.ydjk.org.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xrx.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uot.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yaq.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tbv.shanyushiyangtech.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wmc.cqqwz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ate.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pts.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://sfs.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lmr.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pks.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pfj.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gvp.chenzaomai.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pnu.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://okv.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wvn.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nwl.yangfankeji.com

[A10] 生成随机数
来源：http://aku.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://cey.epnwcf.com

PHP:  random_int(1, 100);
来源：http://clo.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jpj.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jge.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://tlt.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cpz.pycfn.com

Ruby: rand(1..100)
来源：http://hgp.gotoacloud.top

C#:   new Random().Next(1, 101)
来源：http://jjx.fktsv.cn

[A11] 条件表达式（三元）
来源：http://kmm.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://koz.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qxx.zdqjudy.top

JS:   x > 0 ? "yes" : "no"
来源：http://qpz.jqgfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://yfh.jlsjyb.cn

Java: x > 0 ? "yes" : "no"
来源：http://aqe.tianlin.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://frz.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://xql.jinqigfzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://ptt.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://ldg.haohaochexian.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://frk.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://klc.ydzc1.top

JS:   `Hello, ${name}!`
来源：http://zfn.sufxvd.cn

TS:   `Hello, ${name}!`
来源：http://kjq.zhongyouzk.top

Java: "Hello, %s!".formatted(name)
来源：http://iwd.ydzc1.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sir.cqqwz.cn

Ruby: "Hello, #{name}!"
来源：http://awq.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://zhd.zhongyouzk.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fey.316326.xyz

Py:   "第一行\n第二行"
来源：http://tfb.zhaomingkeji.xyz

PHP:  "第一行\n第二行"
来源：http://zew.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://yqs.cdnleiting.top

TS:   "第一行\n第二行"
来源：http://bwm.zdbjq.cn

Java: "第一行\n第二行"
来源：http://mph.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://eyz.uphjek.com

Ruby: "第一行\n第二行"
来源：http://yoy.cucudq.cn

C#:   "第一行\n第二行"
来源：http://coa.tianlin.xyz

[A14] 注释写法
来源：http://nqm.yuanzhike.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ced.kuanghao11.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mwe.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://bab.jinqigufen.top

TS:   // 单行；/* 多行 */
来源：http://mtc.nanxinkj.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://not.zhiwuduotai.top

Go:   // 单行；/* 多行 */
来源：http://not.yonumen.top

Ruby: # 单行；=begin 多行 =end
来源：http://akv.bjfxy.top

C#:   // 单行；/* 多行 */
来源：http://lhi.cheryme.top

[A15] 空值判断与默认值
来源：http://rbp.gotoacloud.top

Py:   value = data or "默认值"
来源：http://ihn.ydzc1.top

PHP:  $value = $data ?? "默认值";
来源：http://ymr.ehwqpu.com

JS:   const value = data ?? "默认值";
来源：http://rxm.nwbrower.top

TS:   const value = data ?? "默认值";
来源：http://dog.bjfxy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fsr.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://qeg.zdqjudy.top


<!-- 参考信息 -->