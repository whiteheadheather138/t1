代发 wailian999

[U85] JS：可选链
来源：http://otn.kuanghao11.cn

a?.b?.c
来源：http://ozb.pycfn.com

[U86] JS：空值合并
来源：http://oux.gzhubu.top

a ?? b
来源：http://zjf.aizwys.cn

[U87] JS：解构默认值
来源：http://jrc.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://iey.birdmap.top

[U88] JS：对象展开合并
来源：http://zjo.jianghu66.top

{ ...a, ...b }
来源：http://ngu.yvedp.cn

[U89] JS：数组去重
来源：http://aew.chenzaomai.com

[...new Set(arr)]
来源：http://qnc.guowangkeji.top

[U90] JS：数字数组排序
来源：http://bca.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://mjx.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://exd.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uss.xziqi.cn

[U92] JS：深拷贝
来源：http://qsx.52xcode.cn

structuredClone(obj)
来源：http://szo.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://wqf.yonumen.top

`共 ${n} 条`
来源：http://xvr.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://jaa.shzxlz.cn

const double = x => x * 2;
来源：http://aze.cashguo.top

[U95] JS：Promise 包装
来源：http://msv.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://vub.hnqzz.top

[U96] JS：async/await 与异常
来源：http://xqb.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://szw.cqqwz.cn

[U97] JS：并发请求
来源：http://dfc.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eyl.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://xxj.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kgh.aizwys.cn

[U99] JS：事件监听
来源：http://srq.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://dad.9152youxi.cn

[U100] JS：DOM 查询
来源：http://gxu.jinghuilouyu.cn

document.querySelector(".item")
来源：http://fsa.ivvv.top

[U101] JS：classList 操作
来源：http://vfc.sufxvd.cn

el.classList.toggle("active")
来源：http://yhz.sysykeji.top

[U102] JS：本地存储
来源：http://bds.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ujn.chenlongwang.top

[U103] JS：定时器
来源：http://kca.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aqi.sufxvd.cn

[U104] JS：防抖
来源：http://ami.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qvp.ivvv.top

[U105] JS：节流
来源：http://tng.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hzj.tanke756.top

[U106] JS：日期格式化
来源：http://xsz.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bkg.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://bhi.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sco.zdbjq.cn

[U108] JS：随机整数
来源：http://uva.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fio.shuidangran.top

[U109] JS：数组分组
来源：http://deb.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://zex.zycfv.cn

[U110] JS：数组分块
来源：http://iha.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tcp.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://cjv.bbcook.cn

new Map(Object.entries(obj))
来源：http://mov.zdbjq.cn

[U112] JS：字符串补位
来源：http://huk.gaohongyu789.top

"7".padStart(3, "0")
来源：http://wrr.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://mzh.meibo888.top

s.replaceAll("a", "b")
来源：http://nsd.52xcode.cn

[U114] JS：JSON 深比较
来源：http://fzx.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yow.bjfxy.top

[U115] JS：生成 UUID
来源：http://omm.zhengqikj.top

crypto.randomUUID()
来源：http://kkm.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://oip.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://xje.redwolf501.top

[U117] JS：单元测试
来源：http://cni.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://idv.cdnleiting.top

[U118] JS：开发服务器
来源：http://jrk.fzhhl.top

npm i -D vite;  npx vite
来源：http://sbm.aizwys.cn

[U119] JS：生产构建
来源：http://apy.xingfuxueyuan.xyz

npx vite build
来源：http://wnq.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://txz.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://ctq.zhoulong.xyz

================================================================================
来源：http://orw.jinqigfzy.top

统计汇总
来源：http://dti.quarkkingdee.top

================================================================================
来源：http://fsd.fanxiaobao.xyz

按语言统计（条）：
来源：http://ygm.zhengqikj.top

Python ......... 252
来源：http://hrj.ydzc1.top

PHP ............ 252
来源：http://hpz.hywenlv.cn

JavaScript ..... 252
来源：http://jhy.xuanzx.com

TypeScript ..... 212
来源：http://pnx.xingfuxueyuan.xyz

Java ........... 212
来源：http://smi.hnqzz.top

Go ............. 212
来源：http://qdk.aizwys.cn

Ruby ........... 212
来源：http://gcf.shanyushiyangkeji.top

C# ............. 212
来源：http://jio.birdmap.top

C .............. 30
来源：http://wrn.dashuyun.cn

C++ ............ 30
来源：http://aff.0kj1m.cn

SQL ............ 90
来源：http://mmy.dianchejie.cn

Bash ........... 80
来源：http://kgd.daxiang520.top

Kotlin ......... 15
来源：http://jab.fehbvm.com

Swift .......... 15
来源：http://zth.uphjek.com

Lua ............ 10
来源：http://dmv.jinqigufen.top

Perl ........... 10
来源：http://ljt.zhixingplan.top

Scala .......... 10
来源：http://jaa.jqgufenzy.top

------------------------------------
来源：http://cuz.hywenlv.cn

合计 ........... 2106 条
来源：http://pca.guowangkeji.top

按章节统计：
来源：http://xqr.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ypi.yj202588.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bzm.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://edp.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ijl.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yzo.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://knw.pengpengdd.cyou

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://acc.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://feg.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mxf.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://atx.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fvq.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jcl.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ohr.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ejw.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tir.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ito.xylfe.cn

Q SQL 专题                              90
来源：http://bnz.aizwys.cn

R Bash 专题                             80
来源：http://qun.bbcook.cn

S C / C++ 专题                          60
来源：http://tyy.cdnleiting.top

T 其他语言补充                          60
来源：http://gkn.hfpthk.cn

U 高频实用片段                         120
来源：http://jgd.nanxinkj.top

------------------------------------
来源：http://rcs.sysykeji.top

合计                                  2106 条
来源：http://pbo.52xcode.cn

--------------------------------------------------------------------------------
来源：http://txr.hnqzz.top

使用提醒
来源：http://tih.daxiang520.top

--------------------------------------------------------------------------------
来源：http://ceh.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yor.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mcc.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rrf.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jsv.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cpm.zhengqikj.top

—— 文件结束 ——
来源：http://wcq.zhaomingkeji.xyz

================================================================================
来源：http://mkk.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://djw.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://uws.sweek.top

================================================================================
来源：http://nbi.hcnkem.com

【收录内容】
来源：http://fbk.yonumen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hjy.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fxg.hnxiangtu.top

SQL · Bash · C · C++
来源：http://hxw.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tne.dashuyun.cn

【使用说明】
来源：http://eev.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iso.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ude.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ycl.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fvv.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fyq.cqqwz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://azv.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ifj.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fjw.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fnk.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nak.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://niy.0kj1m.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zjr.haohaochexian.top

【文件统计】
来源：http://szd.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xkm.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://bck.vehdjk.com

目  录
来源：http://uhi.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://khs.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wdb.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vic.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iiv.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tao.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://exk.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pen.pycfn.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://apo.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mqx.chenjidiqi.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gzn.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lgf.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zug.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xgc.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cbe.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qxb.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://stn.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bys.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rgx.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ppz.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tnd.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ilo.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eyx.tianlin.xyz

================================================================================
来源：http://tzv.jinghuilouyu.cn

A. 基础语法与类型
来源：http://bei.hnqzz.top

================================================================================
来源：http://jhw.yuanzhike.top

[A01] Hello World
来源：http://mhp.zycfv.cn

Py:   print("Hello, World!")
来源：http://tlu.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://pjy.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://qxu.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://frq.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://bkr.xuetiantiany.cn

Go:   fmt.Println("Hello, World!")
来源：http://gkg.yonumen.top

Ruby: puts "Hello, World!"
来源：http://hvw.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ptg.yj20258888.top

[A02] 变量声明与赋值
来源：http://vde.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ajq.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vcp.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://hnd.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://atv.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://bfe.snrcjt.cn

Go:   name := "Alex"; age := 20
来源：http://dwc.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://fpd.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://edv.sufxvd.cn

[A03] 常量定义
来源：http://cxe.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eie.iojbl.cn

PHP:  const PI = 3.14159;
来源：http://ypz.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://ctx.birdmap.top

TS:   const PI: number = 3.14159;
来源：http://mku.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://bwu.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://bpx.yangfankeji.com

Ruby: PI = 3.14159
来源：http://jvu.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://ukj.guannengcc.top

[A04] 判断变量类型
来源：http://mwt.wangshuangyany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://twj.redwolf501.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xsf.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oja.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://vcw.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://izs.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://zla.0kj1m.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kzg.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://phm.ppjwa.cn

[A05] 整数除法与取模
来源：http://knu.tarul.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rbz.bjfxy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hxh.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://abq.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ghl.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://hqd.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://hhs.yj20258888.top

Ruby: 7 / 2; 7 % 2
来源：http://azi.yonumen.top

C#:   7 / 2; 7 % 2
来源：http://gou.gzhubu.top

[A06] 字符串转数字
来源：http://yfv.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://cwd.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gyg.svipenyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yhq.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tvr.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tiq.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ihy.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kir.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iyy.fktsv.cn

[A07] 数字转字符串
来源：http://nae.hongshengwenyu.top

Py:   str(42)
来源：http://jiq.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://zyz.yuxming.cn

JS:   String(42); (42).toString()
来源：http://nyg.chenzaomai.com

TS:   String(42)
来源：http://ozq.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vyf.cashguo.top

Go:   strconv.Itoa(42)
来源：http://usz.xuetiantiany.cn

Ruby: 42.to_s
来源：http://kiy.shangyingyoupin.top

C#:   42.ToString()
来源：http://tgx.yueranfly.top

[A08] 取整与四舍五入
来源：http://arv.pengpengdd.cyou

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sza.daria6918.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gsl.yangfankeji.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gsg.mhx1999.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sgg.wangdashe.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vok.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bko.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wus.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blm.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://cnn.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fns.shzxlz.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vrr.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kuw.cqqwz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nag.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iyv.aizwys.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fvp.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wne.iojbl.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dwg.tanke756.top

[A10] 生成随机数
来源：http://zrx.zhixingplan.top

Py:   import random; random.randint(1, 100)
来源：http://cdg.hywenlv.cn

PHP:  random_int(1, 100);
来源：http://fnq.shanyushiyangtech.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kbu.gaohongyu789.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nlb.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://nyk.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ezc.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://tpc.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://enm.wangshuangyany.cn

[A11] 条件表达式（三元）
来源：http://kxg.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://lcz.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://eqh.kuanghao11.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zad.ehwqpu.com

TS:   x > 0 ? "yes" : "no"
来源：http://wqi.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://gte.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://irb.hywenlv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xik.tarul.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oga.snrcjt.cn

[A12] 字符串插值 / 格式化
来源：http://ehg.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aym.cdnleiting.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xuj.yongpay.top

JS:   `Hello, ${name}!`
来源：http://qvz.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://qzv.0kj1m.cn

Java: "Hello, %s!".formatted(name)
来源：http://wti.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pda.zhiwuduotai.top

Ruby: "Hello, #{name}!"
来源：http://fyy.zhaomingkeji.xyz

C#:   $"Hello, {name}!"
来源：http://sjs.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://ipw.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://fwj.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://hul.hnqzz.top

JS:   "第一行\n第二行"
来源：http://fqw.yanxiufei.cn

TS:   "第一行\n第二行"
来源：http://fvr.fktsv.cn

Java: "第一行\n第二行"
来源：http://jli.52xcode.cn

Go:   "第一行\n第二行"
来源：http://jrf.snrcjt.cn

Ruby: "第一行\n第二行"
来源：http://obv.yj20258888.top

C#:   "第一行\n第二行"
来源：http://ojm.quarkkingdee.top

[A14] 注释写法
来源：http://oir.chenzaomai.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://smd.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://cuu.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://hfs.bbcook.cn


<!-- 参考信息 -->