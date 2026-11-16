代发 wailian999

[U91] JS：对象键值遍历
来源：http://muh.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xii.ivvv.top

[U92] JS：深拷贝
来源：http://rgv.cucudq.cn

structuredClone(obj)
来源：http://ghm.xuanzx.com

[U93] JS：模板字符串
来源：http://ptb.uphjek.com

`共 ${n} 条`
来源：http://obe.daxiang520.top

[U94] JS：箭头函数
来源：http://ual.shanyushiyangtech.top

const double = x => x * 2;
来源：http://ixi.zhengqikj.top

[U95] JS：Promise 包装
来源：http://jgl.yonumen.top

new Promise((resolve, reject) => {})
来源：http://hri.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://law.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oem.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://hxv.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://zhe.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://qcl.yonumen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://srb.yanxiufei.cn

[U99] JS：事件监听
来源：http://bjj.smart0.xyz

el.addEventListener("click", e => {})
来源：http://xvj.hcnkem.com

[U100] JS：DOM 查询
来源：http://xsq.vehdjk.com

document.querySelector(".item")
来源：http://yuc.yj20258888.top

[U101] JS：classList 操作
来源：http://dwz.hesvh.cn

el.classList.toggle("active")
来源：http://axu.sysykeji.top

[U102] JS：本地存储
来源：http://soz.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ewy.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://uag.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jqv.sufxvd.cn

[U104] JS：防抖
来源：http://kcx.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://urm.snrcjt.cn

[U105] JS：节流
来源：http://sez.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ugj.yj20258888.top

[U106] JS：日期格式化
来源：http://jtr.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xmv.hysaishi.cn

[U107] JS：数字千分位
来源：http://key.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ixi.ivvv.top

[U108] JS：随机整数
来源：http://lun.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://akh.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://drc.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://kga.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://bfr.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfl.yfazqb.com

[U111] JS：对象转 Map
来源：http://fnu.0kj1m.cn

new Map(Object.entries(obj))
来源：http://jcp.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://otu.hcnkem.com

"7".padStart(3, "0")
来源：http://qot.ehwqpu.com

[U113] JS：正则替换全部
来源：http://rxv.hcnkem.com

s.replaceAll("a", "b")
来源：http://vsz.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://opd.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xxh.yangfankeji.com

[U115] JS：生成 UUID
来源：http://ylc.yuanzhike.top

crypto.randomUUID()
来源：http://nqn.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://zwt.meibo888.top

/** @param {string} name */ function f(name) {}
来源：http://hnv.yonumen.top

[U117] JS：单元测试
来源：http://cie.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://ezb.chenzaomai.com

[U118] JS：开发服务器
来源：http://ssi.shzxlz.cn

npm i -D vite;  npx vite
来源：http://yid.sxryk.cn

[U119] JS：生产构建
来源：http://qzb.tianlin.xyz

npx vite build
来源：http://odr.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://qve.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://cwd.tianlin.xyz

================================================================================
来源：http://xjs.yvedp.cn

统计汇总
来源：http://lds.ydjk.org.cn

================================================================================
来源：http://ffu.aibaodan.cn

按语言统计（条）：
来源：http://ofj.316326.xyz

Python ......... 252
来源：http://okn.guannengcc.top

PHP ............ 252
来源：http://fhq.yueranfly.top

JavaScript ..... 252
来源：http://pim.vqdsnc.cn

TypeScript ..... 212
来源：http://zel.tarul.cn

Java ........... 212
来源：http://bej.zdbjq.cn

Go ............. 212
来源：http://dvc.sxryk.cn

Ruby ........... 212
来源：http://pad.52xcode.cn

C# ............. 212
来源：http://dnq.andypj.xyz

C .............. 30
来源：http://hrt.hnqzz.top

C++ ............ 30
来源：http://jov.shzxlz.cn

SQL ............ 90
来源：http://jdv.ctjpmb.com

Bash ........... 80
来源：http://mlp.yj20258.top

Kotlin ......... 15
来源：http://enb.shanyushiyangtech.top

Swift .......... 15
来源：http://pxd.shanyushiyangkeji.top

Lua ............ 10
来源：http://wtp.pycfn.com

Perl ........... 10
来源：http://zde.wangshuangyany.cn

Scala .......... 10
来源：http://qso.guowangkeji.top

------------------------------------
来源：http://dtf.xinyue.icu

合计 ........... 2106 条
来源：http://zhd.yuxming.cn

按章节统计：
来源：http://otx.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nta.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jcc.ctjpmb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://let.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sib.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ftx.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gfa.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gbj.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vna.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bsk.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iup.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pdj.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://teq.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tng.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hua.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://thj.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ryw.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://ywk.aizwys.cn

R Bash 专题                             80
来源：http://ich.ydjk.org.cn

S C / C++ 专题                          60
来源：http://ooq.zycfv.cn

T 其他语言补充                          60
来源：http://fhu.sysykeji.top

U 高频实用片段                         120
来源：http://zmr.sysykeji.top

------------------------------------
来源：http://zqi.xinyue.icu

合计                                  2106 条
来源：http://goi.mhx1999.top

--------------------------------------------------------------------------------
来源：http://ftn.ybcxt.top

使用提醒
来源：http://lzz.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://dlg.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://llj.yangfankeji.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kii.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ati.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://srr.tianlin.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yjr.ywan-chungtsiang.top

—— 文件结束 ——
来源：http://gbg.haohaochexian.top

================================================================================
来源：http://vya.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://ycw.jianghu66.top

Common Programming Examples Cheat Book
来源：http://ect.wangshuangyany.cn

================================================================================
来源：http://otl.ehwqpu.com

【收录内容】
来源：http://kun.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://efm.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://msl.yangfankeji.com

SQL · Bash · C · C++
来源：http://tqk.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ztq.hnqzz.top

【使用说明】
来源：http://tyw.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jca.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cen.yfazqb.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pwk.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://egt.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nkd.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nwv.dianchejie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hhq.zhongyouzk.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fzi.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dqb.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://azb.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jni.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nkl.zdbjq.cn

【文件统计】
来源：http://whv.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ocg.yongpay.top

--------------------------------------------------------------------------------
来源：http://wtm.hcnkem.com

目  录
来源：http://wpn.sxryk.cn

--------------------------------------------------------------------------------
来源：http://xce.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zmm.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gsa.fehbvm.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gly.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vlf.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fev.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://opg.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vsi.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pqf.ppjwa.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vrx.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gps.redwolf501.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tus.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bul.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lpj.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://apz.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://aod.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bgy.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jyr.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://yqz.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zqf.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zds.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tij.jinqigufen.top

================================================================================
来源：http://vcq.smart0.xyz

A. 基础语法与类型
来源：http://tzg.gogol.net.cn

================================================================================
来源：http://lqk.xziqi.cn

[A01] Hello World
来源：http://xuu.nwbrower.top

Py:   print("Hello, World!")
来源：http://aus.cdnleiting.top

PHP:  echo "Hello, World!";
来源：http://cnv.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://tlt.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://skt.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://aqr.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://foy.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://ezz.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cof.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://vit.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nkp.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gvv.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://igj.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://smb.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://qog.jqgfzy.top

Go:   name := "Alex"; age := 20
来源：http://soe.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://pia.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wxj.yanxiufei.cn

[A03] 常量定义
来源：http://rda.fktsv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nqq.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://wsf.zhiwuduotai.top

JS:   const PI = 3.14159;
来源：http://giw.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://zty.c1oappe.top

Java: static final double PI = 3.14159;
来源：http://kvh.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://csq.316326.xyz

Ruby: PI = 3.14159
来源：http://wcb.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://ewa.cdnleiting.top

[A04] 判断变量类型
来源：http://qnu.yueranfly.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://tkv.jyoumei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://btx.yueranfly.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qic.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://wwr.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wcg.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://rcw.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rns.hfpthk.cn

C#:   x.GetType().Name; x is int
来源：http://ixz.hnqzz.top

[A05] 整数除法与取模
来源：http://iev.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://flb.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ceg.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lil.haohaochexian.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hlx.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://fhf.guowangkeji.top

Go:   7 / 2; 7 % 2
来源：http://aar.jianghu66.top

Ruby: 7 / 2; 7 % 2
来源：http://mwc.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://rjb.sweek.top

[A06] 字符串转数字
来源：http://xbd.sweek.top

Py:   int("42"); float("3.14")
来源：http://exg.uphjek.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ygz.zhongyouzk.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lgn.zhiwuduotai.top

TS:   parseInt("42", 10); Number("42")
来源：http://juj.gogol.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gus.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iqc.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dbo.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://whk.daria6918.cn

[A07] 数字转字符串
来源：http://hvu.xuetiantiany.cn

Py:   str(42)
来源：http://eqc.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://auo.hammf.cn

JS:   String(42); (42).toString()
来源：http://qnc.yangfankeji.com

TS:   String(42)
来源：http://gqv.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gui.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://ify.zhongyouzk.top

Ruby: 42.to_s
来源：http://ibi.sjlbkw.cn

C#:   42.ToString()
来源：http://ebw.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://iwz.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://npy.zhengqikj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gjt.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lqx.yj20258888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lcl.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qka.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ukh.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://byi.svipenyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://szb.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://kno.yanxiufei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wuc.sweek.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hvv.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nsf.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ntw.jlsjyb.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fbj.hongshengwenyu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://boo.vehdjk.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ffv.zhongyouzk.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aka.havefunace.top

[A10] 生成随机数
来源：http://rbv.zdbjq.cn

Py:   import random; random.randint(1, 100)
来源：http://pta.ivvv.top

PHP:  random_int(1, 100);
来源：http://kii.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kcm.epnwcf.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wbm.xuetiantiany.cn

Java: new Random().nextInt(100) + 1
来源：http://ahx.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wsw.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://cml.ppjwa.cn

C#:   new Random().Next(1, 101)
来源：http://xwh.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://rvh.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://eab.guannengcc.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jvs.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://pus.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://bkw.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://pqa.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tni.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yie.nwbrower.top

C#:   x > 0 ? "yes" : "no"
来源：http://fmy.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://kqf.jlsjyb.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aby.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://buh.meibo888.top

JS:   `Hello, ${name}!`
来源：http://emh.yj20258.top

TS:   `Hello, ${name}!`
来源：http://kdu.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://djm.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://svy.sweek.top

Ruby: "Hello, #{name}!"
来源：http://cqx.sweek.top

C#:   $"Hello, {name}!"
来源：http://jom.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://noz.aibaodan.cn

Py:   "第一行\n第二行"
来源：http://gat.chenlongwang.top

PHP:  "第一行\n第二行"
来源：http://iwc.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://hkb.hcnkem.com

TS:   "第一行\n第二行"
来源：http://ddh.jqgufenzy.top

Java: "第一行\n第二行"
来源：http://tin.sysykeji.top

Go:   "第一行\n第二行"
来源：http://osr.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://qky.sysykeji.top

C#:   "第一行\n第二行"
来源：http://ehe.redwolf501.top

[A14] 注释写法
来源：http://wjj.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mxq.epnwcf.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://bkr.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://cgd.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://boi.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wie.316326.xyz

Go:   // 单行；/* 多行 */
来源：http://qfv.pycfn.com

Ruby: # 单行；=begin 多行 =end
来源：http://afv.guowangkeji.top

C#:   // 单行；/* 多行 */
来源：http://tqm.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://dlc.sjlbkw.cn

Py:   value = data or "默认值"
来源：http://tjj.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://gsj.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://keo.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://msn.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qju.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://ukw.jinyuanbaomall.cn


<!-- 参考信息 -->