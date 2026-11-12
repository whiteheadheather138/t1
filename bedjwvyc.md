代发 wailian999

[U91] JS：对象键值遍历
来源：http://ptp.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mrg.hnxiangtu.top

[U92] JS：深拷贝
来源：http://aar.yueranfly.top

structuredClone(obj)
来源：http://bht.jqgfzy.top

[U93] JS：模板字符串
来源：http://vmq.xylfe.cn

`共 ${n} 条`
来源：http://uvu.chenlongwang.top

[U94] JS：箭头函数
来源：http://wuu.dashuyun.cn

const double = x => x * 2;
来源：http://edo.daria6918.cn

[U95] JS：Promise 包装
来源：http://onb.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://bmq.yongpay.top

[U96] JS：async/await 与异常
来源：http://fhn.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bbb.chenlongwang.top

[U97] JS：并发请求
来源：http://qkp.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kkt.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://djf.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eyw.havefunace.top

[U99] JS：事件监听
来源：http://pjp.fzhhl.top

el.addEventListener("click", e => {})
来源：http://anu.hesvh.cn

[U100] JS：DOM 查询
来源：http://dip.daria6918.cn

document.querySelector(".item")
来源：http://zdd.gogol.net.cn

[U101] JS：classList 操作
来源：http://syc.sjlbkw.cn

el.classList.toggle("active")
来源：http://jed.ehwqpu.com

[U102] JS：本地存储
来源：http://dfr.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://whu.dashuyun.cn

[U103] JS：定时器
来源：http://cor.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nvi.fehbvm.com

[U104] JS：防抖
来源：http://ank.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqt.yanxiufei.cn

[U105] JS：节流
来源：http://wyr.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oub.fktsv.cn

[U106] JS：日期格式化
来源：http://upo.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zkt.hcnkem.com

[U107] JS：数字千分位
来源：http://gng.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ala.wangdashe.top

[U108] JS：随机整数
来源：http://gsm.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://psg.ydzc1.top

[U109] JS：数组分组
来源：http://cnk.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://zqr.yonumen.top

[U110] JS：数组分块
来源：http://bsb.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fuk.cqqwz.cn

[U111] JS：对象转 Map
来源：http://cgv.sxryk.cn

new Map(Object.entries(obj))
来源：http://fph.chenlongwang.top

[U112] JS：字符串补位
来源：http://iol.jianghu66.top

"7".padStart(3, "0")
来源：http://frh.sysykeji.top

[U113] JS：正则替换全部
来源：http://xxy.chenlongwang.top

s.replaceAll("a", "b")
来源：http://ouk.meibo888.top

[U114] JS：JSON 深比较
来源：http://wbi.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mai.cucudq.cn

[U115] JS：生成 UUID
来源：http://bbk.ydjk.org.cn

crypto.randomUUID()
来源：http://upp.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://rbr.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://yyz.chenzaomai.com

[U117] JS：单元测试
来源：http://qkf.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://qgs.xziqi.cn

[U118] JS：开发服务器
来源：http://jrb.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://jiy.yj20258.top

[U119] JS：生产构建
来源：http://ame.wangdashe.top

npx vite build
来源：http://niq.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://grn.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://mjx.0kj1m.cn

================================================================================
来源：http://clk.ywan-chungtsiang.top

统计汇总
来源：http://wan.iojbl.cn

================================================================================
来源：http://yzd.yj20258888.top

按语言统计（条）：
来源：http://cth.yuanzhike.top

Python ......... 252
来源：http://myj.gogol.net.cn

PHP ............ 252
来源：http://osj.ydjk.org.cn

JavaScript ..... 252
来源：http://gbt.tanke756.top

TypeScript ..... 212
来源：http://lph.havefunace.top

Java ........... 212
来源：http://ord.52xcode.cn

Go ............. 212
来源：http://axo.redwolf501.top

Ruby ........... 212
来源：http://fmm.mhx1999.top

C# ............. 212
来源：http://jeo.chenlongwang.top

C .............. 30
来源：http://rao.ydzc1.top

C++ ............ 30
来源：http://xwl.jinyuanbaomall.cn

SQL ............ 90
来源：http://awu.guowangkeji.top

Bash ........... 80
来源：http://khu.svipenyu.cn

Kotlin ......... 15
来源：http://pks.bbcook.cn

Swift .......... 15
来源：http://evk.yangfankeji.com

Lua ............ 10
来源：http://qab.jianghu66.top

Perl ........... 10
来源：http://iwv.bbcook.cn

Scala .......... 10
来源：http://sgr.jiagoushi.top

------------------------------------
来源：http://oxn.ydzc1.top

合计 ........... 2106 条
来源：http://edi.hnxiangtu.top

按章节统计：
来源：http://bos.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uum.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cbx.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ayk.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fsk.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gut.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xxb.aibaodan.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hsf.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ipu.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cit.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://txd.zhengqikj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://afo.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xul.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pso.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://otk.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oju.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://idy.hammf.cn

Q SQL 专题                              90
来源：http://cdi.jlsjyb.cn

R Bash 专题                             80
来源：http://nni.bjfxy.top

S C / C++ 专题                          60
来源：http://phm.shuidangran.top

T 其他语言补充                          60
来源：http://dlk.zhixingplan.top

U 高频实用片段                         120
来源：http://jrr.hnxiangtu.top

------------------------------------
来源：http://wzw.cdnleiting.top

合计                                  2106 条
来源：http://gxb.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://fdd.jiagoushi.top

使用提醒
来源：http://tny.tian-w.cn

--------------------------------------------------------------------------------
来源：http://mor.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oed.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fxo.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bqa.meibo888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://aox.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://trg.redwolf501.top

—— 文件结束 ——
来源：http://rkt.jinyuanbaomall.cn

================================================================================
来源：http://ysv.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://erf.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://lqv.yuanzhike.top

================================================================================
来源：http://jkq.fehbvm.com

【收录内容】
来源：http://kls.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ywa.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xew.ppjwa.cn

SQL · Bash · C · C++
来源：http://dmi.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zcv.aizwys.cn

【使用说明】
来源：http://ntu.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bqp.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aog.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wda.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rxa.sweek.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zku.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sqx.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cwd.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dbl.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dzt.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vvj.sxryk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hjv.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ihl.xinyue.icu

【文件统计】
来源：http://xti.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nzw.tarul.cn

--------------------------------------------------------------------------------
来源：http://xiw.cashguo.top

目  录
来源：http://mem.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://blo.sxryk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tnv.ywan-chungtsiang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://slm.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yae.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wnc.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ysw.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://geu.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kbf.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jen.daria6918.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vmc.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hxn.quarkkingdee.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ibk.ehwqpu.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xee.aibaodan.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rsd.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hec.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ajd.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jev.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kpr.yfazqb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ynd.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://prv.dashuyun.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kps.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xbb.zhongyouzk.top

================================================================================
来源：http://sdb.xziqi.cn

A. 基础语法与类型
来源：http://iqn.hnqzz.top

================================================================================
来源：http://gvs.sweek.top

[A01] Hello World
来源：http://rrx.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://ciq.yonumen.top

PHP:  echo "Hello, World!";
来源：http://vrm.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://hur.svipenyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nyf.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://wfs.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://ikv.zycfv.cn

Ruby: puts "Hello, World!"
来源：http://kfj.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wrq.havefunace.top

[A02] 变量声明与赋值
来源：http://mid.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tnm.zhixingplan.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bpj.yueranfly.top

JS:   let name = "Alex"; const age = 20;
来源：http://dxv.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ekg.vqdsnc.cn

Java: String name = "Alex"; int age = 20;
来源：http://pus.sxryk.cn

Go:   name := "Alex"; age := 20
来源：http://kwf.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://xbf.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://tpw.gaohongyu789.top

[A03] 常量定义
来源：http://egl.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://szp.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://sib.tian-w.cn

JS:   const PI = 3.14159;
来源：http://ore.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://mhn.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://jfg.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://onq.sweek.top

Ruby: PI = 3.14159
来源：http://asl.cheryme.top

C#:   const double PI = 3.14159;
来源：http://dim.zhengqikj.top

[A04] 判断变量类型
来源：http://hgg.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wmn.yvedp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dgf.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hct.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://oey.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://whk.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://hjf.sjlbkw.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tvj.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://brt.svipenyu.cn

[A05] 整数除法与取模
来源：http://atg.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vah.jyoumei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://job.bbcook.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pjq.52xcode.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wfm.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://uda.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://hkx.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://whz.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://tmu.nwbrower.top

[A06] 字符串转数字
来源：http://jyb.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://kbw.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uvs.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://psz.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://eiy.guannengcc.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vfc.52xcode.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://icd.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://uti.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xvg.zhongyouzk.top

[A07] 数字转字符串
来源：http://xgg.ydzc1.top

Py:   str(42)
来源：http://oce.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://mzq.tian-w.cn

JS:   String(42); (42).toString()
来源：http://jxn.zhengqikj.top

TS:   String(42)
来源：http://hfh.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://azn.cheryme.top

Go:   strconv.Itoa(42)
来源：http://pek.pycfn.com

Ruby: 42.to_s
来源：http://xna.daxiang520.top

C#:   42.ToString()
来源：http://ruz.gogol.net.cn

[A08] 取整与四舍五入
来源：http://zwd.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zue.aibaodan.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nha.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mjf.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xbd.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qab.hongshengwenyu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mno.haohaochexian.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ghc.snrcjt.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tnk.c1oappe.top

[A09] 绝对值与最大最小值
来源：http://ikh.nwbrower.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blm.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zhy.c1oappe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yhw.snrcjt.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jkd.shanyushiyangkeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sbo.yanxiufei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://omz.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ocp.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tkk.cheryme.top

[A10] 生成随机数
来源：http://jhw.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://uhv.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://ejn.meibo888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uue.vehdjk.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tub.ppjwa.cn

Java: new Random().nextInt(100) + 1
来源：http://lre.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://coi.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://yxt.ydjk.org.cn

C#:   new Random().Next(1, 101)
来源：http://oib.vqdsnc.cn

[A11] 条件表达式（三元）
来源：http://bes.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://nbq.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fzj.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pem.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://mik.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://pqa.yueranfly.top

Go:   // 无三元运算符，需用 if 语句
来源：http://juh.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://pqg.0kj1m.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eqv.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://aeo.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vls.gogol.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vzk.smart0.xyz

JS:   `Hello, ${name}!`
来源：http://jap.shanyushiyangkeji.top

TS:   `Hello, ${name}!`
来源：http://arx.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://jvy.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ino.yuxming.cn

Ruby: "Hello, #{name}!"
来源：http://inn.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://rib.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://wcu.ybcxt.top

Py:   "第一行\n第二行"
来源：http://xiu.redwolf501.top

PHP:  "第一行\n第二行"
来源：http://hcm.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://qob.ivvv.top

TS:   "第一行\n第二行"
来源：http://abu.aibaodan.cn

Java: "第一行\n第二行"
来源：http://pdz.yuanzhike.top

Go:   "第一行\n第二行"
来源：http://ahe.ydzc1.top

Ruby: "第一行\n第二行"
来源：http://doc.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://nhq.ybcxt.top

[A14] 注释写法
来源：http://llc.gogol.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ntb.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://tti.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://gpl.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://vvm.jlsjyb.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kvb.yueranfly.top

Go:   // 单行；/* 多行 */
来源：http://smk.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://xsb.gzhubu.top

C#:   // 单行；/* 多行 */
来源：http://zmh.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://nbw.hongshengwenyu.top

Py:   value = data or "默认值"
来源：http://heq.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://dsq.yj20258.top

JS:   const value = data ?? "默认值";
来源：http://pis.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://uqw.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qor.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://thl.ehwqpu.com


<!-- 参考信息 -->