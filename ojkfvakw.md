代发 wailian999

[U85] JS：可选链
来源：http://fkk.shangyingyoupin.top

a?.b?.c
来源：http://ykj.hywenlv.cn

[U86] JS：空值合并
来源：http://dxs.dianchejie.cn

a ?? b
来源：http://xzk.xinyue.icu

[U87] JS：解构默认值
来源：http://nht.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://yiv.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://auk.daria6918.cn

{ ...a, ...b }
来源：http://hjh.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://zqp.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://oxf.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://vwr.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://dun.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://cde.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vjs.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://onr.9152youxi.cn

structuredClone(obj)
来源：http://nko.yueranfly.top

[U93] JS：模板字符串
来源：http://jsn.zhixingplan.top

`共 ${n} 条`
来源：http://vbq.iojbl.cn

[U94] JS：箭头函数
来源：http://pms.shzxlz.cn

const double = x => x * 2;
来源：http://xka.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://dmp.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://rsy.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://rcn.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zwi.nanxuanxn.top

[U97] JS：并发请求
来源：http://pop.pycfn.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://fli.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://bmu.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://opd.xylfe.cn

[U99] JS：事件监听
来源：http://cwo.jianghu66.top

el.addEventListener("click", e => {})
来源：http://pxn.xuanzx.com

[U100] JS：DOM 查询
来源：http://bhk.snrcjt.cn

document.querySelector(".item")
来源：http://rjl.yj20258888.top

[U101] JS：classList 操作
来源：http://mch.wangdashe.top

el.classList.toggle("active")
来源：http://tao.zhengqikj.top

[U102] JS：本地存储
来源：http://uav.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ubf.gzhubu.top

[U103] JS：定时器
来源：http://tpk.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zgf.vehdjk.com

[U104] JS：防抖
来源：http://inu.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqv.sxryk.cn

[U105] JS：节流
来源：http://swf.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ykg.quarkkingdee.top

[U106] JS：日期格式化
来源：http://rty.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://byo.hfpthk.cn

[U107] JS：数字千分位
来源：http://tvj.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sxk.kuanghao11.cn

[U108] JS：随机整数
来源：http://igv.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gdv.zhijiandao.cn

[U109] JS：数组分组
来源：http://pvc.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://mnw.hcnkem.com

[U110] JS：数组分块
来源：http://htf.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://squ.cheryme.top

[U111] JS：对象转 Map
来源：http://hca.c1oappe.top

new Map(Object.entries(obj))
来源：http://eyp.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://feb.yueranfly.top

"7".padStart(3, "0")
来源：http://imc.chenzaomai.com

[U113] JS：正则替换全部
来源：http://itl.yuanzhike.top

s.replaceAll("a", "b")
来源：http://nwg.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://tyg.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jvs.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://tur.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://sbp.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://qmi.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://xhb.zhiwuduotai.top

[U117] JS：单元测试
来源：http://dlm.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://eps.yfazqb.com

[U118] JS：开发服务器
来源：http://bvk.dashuyun.cn

npm i -D vite;  npx vite
来源：http://sal.gogol.net.cn

[U119] JS：生产构建
来源：http://lny.yj20258.top

npx vite build
来源：http://rgl.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://wyk.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://wvn.pengpengdd.cyou

================================================================================
来源：http://jue.pengpengdd.cyou

统计汇总
来源：http://epk.yvedp.cn

================================================================================
来源：http://wbv.epnwcf.com

按语言统计（条）：
来源：http://lkb.nanxinkj.top

Python ......... 252
来源：http://hrt.xuetiantiany.cn

PHP ............ 252
来源：http://pkb.yangfankeji.com

JavaScript ..... 252
来源：http://maa.ydzc1.top

TypeScript ..... 212
来源：http://rax.wangdashe.top

Java ........... 212
来源：http://ynp.jianghu66.top

Go ............. 212
来源：http://snj.jianghu66.top

Ruby ........... 212
来源：http://dqj.guowangkeji.top

C# ............. 212
来源：http://vsh.jinyuanbaomall.cn

C .............. 30
来源：http://hdg.snrcjt.cn

C++ ............ 30
来源：http://rso.yonumen.top

SQL ............ 90
来源：http://qzt.ppjwa.cn

Bash ........... 80
来源：http://sfc.yj20258888.top

Kotlin ......... 15
来源：http://wjb.redwolf501.top

Swift .......... 15
来源：http://vjj.bjfxy.top

Lua ............ 10
来源：http://iso.zhengqikj.top

Perl ........... 10
来源：http://mxj.havefunace.top

Scala .......... 10
来源：http://eqx.pengpengdd.cyou

------------------------------------
来源：http://qci.birdmap.top

合计 ........... 2106 条
来源：http://trn.gzhubu.top

按章节统计：
来源：http://mxp.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nvj.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wae.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ljx.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iqz.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sng.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://seh.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oug.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kbt.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hos.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kti.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://abx.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://btv.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vdf.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rrj.sxryk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zta.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zfj.cucudq.cn

Q SQL 专题                              90
来源：http://phr.shanyushiyangtech.top

R Bash 专题                             80
来源：http://pyr.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://fda.xuanzx.com

T 其他语言补充                          60
来源：http://vvv.uphjek.com

U 高频实用片段                         120
来源：http://qby.wangshuangyany.cn

------------------------------------
来源：http://mpj.fktsv.cn

合计                                  2106 条
来源：http://yvj.guannengcc.top

--------------------------------------------------------------------------------
来源：http://ibt.pengpengdd.cyou

使用提醒
来源：http://fdg.pycfn.com

--------------------------------------------------------------------------------
来源：http://yno.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vug.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://chy.xylfe.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://png.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://css.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xif.daxiang520.top

—— 文件结束 ——
来源：http://ghp.yj20258888.top

================================================================================
来源：http://ddz.wangshuangyany.cn

程序语言常见例子速查手册（2024 版）
来源：http://hgx.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://hvg.haohaochexian.top

================================================================================
来源：http://pcc.52xcode.cn

【收录内容】
来源：http://qif.pengpengdd.cyou

覆盖 12 种语言 / 语法与常见 API：
来源：http://ido.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dvx.daxiang520.top

SQL · Bash · C · C++
来源：http://nkx.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://czo.jqgufenzy.top

【使用说明】
来源：http://xff.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qxq.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rgr.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uxu.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lwx.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://juh.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fra.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bhn.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lyl.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jgv.wangdashe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ybj.xziqi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jsr.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://erz.pycfn.com

【文件统计】
来源：http://fbf.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cmq.ydzc1.top

--------------------------------------------------------------------------------
来源：http://ycl.shanyushiyangtech.top

目  录
来源：http://fdi.daria6918.cn

--------------------------------------------------------------------------------
来源：http://xxy.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eiw.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zlh.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yfq.redwolf501.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qcs.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zgo.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://swp.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kac.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zlq.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rqc.cqqwz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ggx.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://omo.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ujd.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ngw.jyoumei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fqz.sjlbkw.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mxu.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ocb.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fiu.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ttp.guowangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hxb.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xfk.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rcy.chenlongwang.top

================================================================================
来源：http://bku.shzxlz.cn

A. 基础语法与类型
来源：http://ilq.vqdsnc.cn

================================================================================
来源：http://fli.sjlbkw.cn

[A01] Hello World
来源：http://uqi.xziqi.cn

Py:   print("Hello, World!")
来源：http://bja.birdmap.top

PHP:  echo "Hello, World!";
来源：http://nbf.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://nxh.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xde.ctjpmb.com

Java: System.out.println("Hello, World!");
来源：http://isf.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://rmu.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://ush.haohaochexian.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nxb.hnqzz.top

[A02] 变量声明与赋值
来源：http://dep.bjfxy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kam.jyoumei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jao.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rma.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xxa.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://irs.haohaochexian.top

Go:   name := "Alex"; age := 20
来源：http://xbb.yonumen.top

Ruby: name = "Alex"; age = 20
来源：http://two.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://psn.daria6918.cn

[A03] 常量定义
来源：http://ggh.ppjwa.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tva.cheryme.top

PHP:  const PI = 3.14159;
来源：http://eki.yj20258888.top

JS:   const PI = 3.14159;
来源：http://qbh.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://gwi.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://qus.shanyushiyangkeji.top

Go:   const PI = 3.14159
来源：http://bxu.shzxlz.cn

Ruby: PI = 3.14159
来源：http://kkk.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://wvw.yvedp.cn

[A04] 判断变量类型
来源：http://lmi.hnxiangtu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ozl.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bjv.nanxinkj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dpb.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://wry.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dze.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://ehr.jiagoushi.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tsp.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://vfn.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://rli.9152youxi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qyg.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gte.jqgfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xgl.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ioc.mhx1999.top

Java: 7 / 2; 7 % 2
来源：http://hrf.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://lwm.yuxming.cn

Ruby: 7 / 2; 7 % 2
来源：http://rrg.yfazqb.com

C#:   7 / 2; 7 % 2
来源：http://oso.ppjwa.cn

[A06] 字符串转数字
来源：http://pzn.ywan-chungtsiang.top

Py:   int("42"); float("3.14")
来源：http://bic.pengpengdd.cyou

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bai.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ura.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://evr.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wpj.cucudq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://siu.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://onj.ctjpmb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gty.nanxuanxn.top

[A07] 数字转字符串
来源：http://dwo.daxiang520.top

Py:   str(42)
来源：http://zvg.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://sfm.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://rff.ctjpmb.com

TS:   String(42)
来源：http://hml.shzxlz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gis.yj20258.top

Go:   strconv.Itoa(42)
来源：http://cva.pengpengdd.cyou

Ruby: 42.to_s
来源：http://hpl.nwbrower.top

C#:   42.ToString()
来源：http://guc.redwolf501.top

[A08] 取整与四舍五入
来源：http://znh.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rwf.gaohongyu789.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pvh.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pvf.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://orf.0kj1m.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qia.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hiy.yvedp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://awl.sufxvd.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qyz.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://owf.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cyn.xinyue.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://chc.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ifs.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kws.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pak.cheryme.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lbi.birdmap.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oel.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oul.yj202588.top

[A10] 生成随机数
来源：http://cjv.zhiwuduotai.top

Py:   import random; random.randint(1, 100)
来源：http://hyo.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://cwk.dianchejie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://utt.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nhv.haohaochexian.top

Java: new Random().nextInt(100) + 1
来源：http://mld.hammf.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vst.dashuyun.cn

Ruby: rand(1..100)
来源：http://zbx.sjlbkw.cn

C#:   new Random().Next(1, 101)
来源：http://llt.ydzc1.top

[A11] 条件表达式（三元）
来源：http://kwv.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://jwx.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dic.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://anj.pycfn.com

TS:   x > 0 ? "yes" : "no"
来源：http://jnr.gotoacloud.top

Java: x > 0 ? "yes" : "no"
来源：http://yzn.hfpthk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cjq.ctjpmb.com

Ruby: x > 0 ? "yes" : "no"
来源：http://wvg.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qjm.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://yqu.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tbc.yj20258.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://acu.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://cgt.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://sjy.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://brw.fehbvm.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mrd.9152youxi.cn

Ruby: "Hello, #{name}!"
来源：http://shl.mhx1999.top

C#:   $"Hello, {name}!"
来源：http://oip.xylfe.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ufx.jinghuilouyu.cn

Py:   "第一行\n第二行"
来源：http://dcl.zhengqikj.top

PHP:  "第一行\n第二行"
来源：http://cdc.sysykeji.top

JS:   "第一行\n第二行"
来源：http://kjp.sweek.top

TS:   "第一行\n第二行"
来源：http://yae.ydzc1.top

Java: "第一行\n第二行"
来源：http://ewy.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://ycs.zhongyouzk.top

Ruby: "第一行\n第二行"
来源：http://ydp.hfpthk.cn

C#:   "第一行\n第二行"
来源：http://llv.chenjidiqi.icu

[A14] 注释写法
来源：http://shv.tianlin.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://mjx.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://luz.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://jdw.ppjwa.cn


<!-- 参考信息 -->