代发 wailian999

[U87] JS：解构默认值
来源：http://qiw.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://omh.andypj.xyz

[U88] JS：对象展开合并
来源：http://mis.chenzaomai.com

{ ...a, ...b }
来源：http://big.iojbl.cn

[U89] JS：数组去重
来源：http://twe.yj20258.top

[...new Set(arr)]
来源：http://dvm.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://asx.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://arv.gzhubu.top

[U91] JS：对象键值遍历
来源：http://zhs.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tur.chenzaomai.com

[U92] JS：深拷贝
来源：http://cfu.yueranfly.top

structuredClone(obj)
来源：http://mmy.zhengqikj.top

[U93] JS：模板字符串
来源：http://jvl.chenzaomai.com

`共 ${n} 条`
来源：http://uvt.zdbjq.cn

[U94] JS：箭头函数
来源：http://zqe.kuanghao11.cn

const double = x => x * 2;
来源：http://nja.daria6918.cn

[U95] JS：Promise 包装
来源：http://zbs.yueranfly.top

new Promise((resolve, reject) => {})
来源：http://cmv.fktsv.cn

[U96] JS：async/await 与异常
来源：http://ogm.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uor.meibo888.top

[U97] JS：并发请求
来源：http://iel.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://lhx.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://qmb.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bvt.hcnkem.com

[U99] JS：事件监听
来源：http://pnt.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://rnh.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://ggw.hesvh.cn

document.querySelector(".item")
来源：http://fqo.yfazqb.com

[U101] JS：classList 操作
来源：http://ory.yangfankeji.com

el.classList.toggle("active")
来源：http://xms.hcnkem.com

[U102] JS：本地存储
来源：http://xzw.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uhr.bjfxy.top

[U103] JS：定时器
来源：http://yyo.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ljm.iojbl.cn

[U104] JS：防抖
来源：http://syr.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phb.cqqwz.cn

[U105] JS：节流
来源：http://rgn.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tcb.yj20258.top

[U106] JS：日期格式化
来源：http://vbs.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://esy.snrcjt.cn

[U107] JS：数字千分位
来源：http://atn.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tip.jinqigufen.top

[U108] JS：随机整数
来源：http://wxl.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nlk.cheryme.top

[U109] JS：数组分组
来源：http://cqi.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://zti.ybcxt.top

[U110] JS：数组分块
来源：http://lju.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uxf.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://nik.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://gzk.nanxuanxn.top

[U112] JS：字符串补位
来源：http://mcv.jinqigfzy.top

"7".padStart(3, "0")
来源：http://srt.yvedp.cn

[U113] JS：正则替换全部
来源：http://blj.fehbvm.com

s.replaceAll("a", "b")
来源：http://uyg.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://ijv.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zfa.ivvv.top

[U115] JS：生成 UUID
来源：http://zmk.yuanzhike.top

crypto.randomUUID()
来源：http://uzl.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://uit.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://ock.jqgufenzy.top

[U117] JS：单元测试
来源：http://mot.hammf.cn

npm i -D vitest;  npx vitest
来源：http://itu.cucudq.cn

[U118] JS：开发服务器
来源：http://uad.hcnkem.com

npm i -D vite;  npx vite
来源：http://daf.kuanghao11.cn

[U119] JS：生产构建
来源：http://jgs.xylfe.cn

npx vite build
来源：http://vmn.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://ten.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://kfy.havefunace.top

================================================================================
来源：http://aqz.ywan-chungtsiang.top

统计汇总
来源：http://ybx.tian-w.cn

================================================================================
来源：http://npd.gzhubu.top

按语言统计（条）：
来源：http://uhr.mhx1999.top

Python ......... 252
来源：http://pku.yuanzhike.top

PHP ............ 252
来源：http://try.sweek.top

JavaScript ..... 252
来源：http://ryg.guowangkeji.top

TypeScript ..... 212
来源：http://kag.zhijiandao.cn

Java ........... 212
来源：http://zbn.cdnleiting.top

Go ............. 212
来源：http://otc.feifeiyinyue.top

Ruby ........... 212
来源：http://uhx.jinyuanbaomall.cn

C# ............. 212
来源：http://rne.redwolf501.top

C .............. 30
来源：http://wfa.fanxiaobao.xyz

C++ ............ 30
来源：http://wkf.hammf.cn

SQL ............ 90
来源：http://trj.epnwcf.com

Bash ........... 80
来源：http://gwv.yj202588.top

Kotlin ......... 15
来源：http://fhi.jinghuilouyu.cn

Swift .......... 15
来源：http://nug.epnwcf.com

Lua ............ 10
来源：http://cso.hcnkem.com

Perl ........... 10
来源：http://kub.nwbrower.top

Scala .......... 10
来源：http://oab.sufxvd.cn

------------------------------------
来源：http://fgo.pengpengdd.cyou

合计 ........... 2106 条
来源：http://anr.aibaodan.cn

按章节统计：
来源：http://uiy.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bjs.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nks.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://srb.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mjv.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ndu.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tgo.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pcm.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ugm.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ins.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yod.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oxs.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ikp.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yqy.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vfv.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kkg.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eye.pycfn.com

Q SQL 专题                              90
来源：http://wyj.svipenyu.cn

R Bash 专题                             80
来源：http://mgg.zhijiandao.cn

S C / C++ 专题                          60
来源：http://xqo.gzhubu.top

T 其他语言补充                          60
来源：http://pmq.shzxlz.cn

U 高频实用片段                         120
来源：http://mtk.ybcxt.top

------------------------------------
来源：http://lyy.cashguo.top

合计                                  2106 条
来源：http://mjw.havefunace.top

--------------------------------------------------------------------------------
来源：http://ozx.jinghuilouyu.cn

使用提醒
来源：http://kmy.yj20258888.top

--------------------------------------------------------------------------------
来源：http://gtm.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cxj.sufxvd.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cww.aibaodan.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ybx.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://xzx.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nzb.pycfn.com

—— 文件结束 ——
来源：http://cdo.jiagoushi.top

================================================================================
来源：http://ozs.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://wsy.iojbl.cn

Common Programming Examples Cheat Book
来源：http://hgy.jqgufenzy.top

================================================================================
来源：http://fqh.vqdsnc.cn

【收录内容】
来源：http://ipd.ywan-chungtsiang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xuv.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fsn.0kj1m.cn

SQL · Bash · C · C++
来源：http://dqj.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rxv.havefunace.top

【使用说明】
来源：http://ghu.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sld.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://edx.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iyd.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hzg.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://eft.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nze.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tvr.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dxa.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://glg.jianghu66.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fut.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://coo.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mcl.ywan-chungtsiang.top

【文件统计】
来源：http://bmk.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gwq.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://iub.yfazqb.com

目  录
来源：http://zot.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://lwx.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kov.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xfm.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ltu.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://car.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oao.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sio.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fpm.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iqg.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ekv.hnxiangtu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nna.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://itm.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rjj.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vjw.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hyz.haohaochexian.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xtl.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hsf.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wus.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lss.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gsg.feifeiyinyue.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eoq.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ljw.pengpengdd.cyou

================================================================================
来源：http://wol.pycfn.com

A. 基础语法与类型
来源：http://hvi.meibo888.top

================================================================================
来源：http://pke.birdmap.top

[A01] Hello World
来源：http://zwg.yangfankeji.com

Py:   print("Hello, World!")
来源：http://qqw.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://mje.uphjek.com

JS:   console.log("Hello, World!");
来源：http://bqt.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zwz.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://jte.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://eqw.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://vra.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hil.andypj.xyz

[A02] 变量声明与赋值
来源：http://tzk.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vzh.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://thd.c1oappe.top

JS:   let name = "Alex"; const age = 20;
来源：http://owx.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iov.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://sra.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://njs.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://gbx.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://dan.zhixingplan.top

[A03] 常量定义
来源：http://vyt.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ici.mhx1999.top

PHP:  const PI = 3.14159;
来源：http://zws.jqgfzy.top

JS:   const PI = 3.14159;
来源：http://xpo.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://frt.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://bkc.hcnkem.com

Go:   const PI = 3.14159
来源：http://xua.havefunace.top

Ruby: PI = 3.14159
来源：http://tei.jiagoushi.top

C#:   const double PI = 3.14159;
来源：http://set.iojbl.cn

[A04] 判断变量类型
来源：http://mss.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://kbd.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gvh.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wzi.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://nhu.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wnj.fanxiaobao.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://glq.shzxlz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qzh.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://uzb.yongpay.top

[A05] 整数除法与取模
来源：http://kev.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mtr.xziqi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yjv.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aqi.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://azs.yuanzhike.top

Java: 7 / 2; 7 % 2
来源：http://mlg.snrcjt.cn

Go:   7 / 2; 7 % 2
来源：http://awg.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://vad.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://pgo.yongpay.top

[A06] 字符串转数字
来源：http://off.cdnleiting.top

Py:   int("42"); float("3.14")
来源：http://bnv.zhijiandao.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://llf.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://snv.316326.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://ikl.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dwp.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tnn.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fmz.epnwcf.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ifw.ydzc1.top

[A07] 数字转字符串
来源：http://mtv.fzhhl.top

Py:   str(42)
来源：http://usk.gzhubu.top

PHP:  (string) 42; strval(42)
来源：http://bsi.cucudq.cn

JS:   String(42); (42).toString()
来源：http://kqb.hywenlv.cn

TS:   String(42)
来源：http://czd.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ssz.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://mzf.kuanghao11.cn

Ruby: 42.to_s
来源：http://fth.vehdjk.com

C#:   42.ToString()
来源：http://ygs.9152youxi.cn

[A08] 取整与四舍五入
来源：http://oqw.meibo888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://abf.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iel.redwolf501.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://amf.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ajf.52xcode.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lzd.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dub.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rdi.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://drh.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://ivo.snrcjt.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nfs.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wqr.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://poj.vehdjk.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qbo.chenjidiqi.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qlk.zhongyouzk.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lzu.yangfankeji.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pzb.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vwz.mhx1999.top

[A10] 生成随机数
来源：http://czd.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://unq.bjfxy.top

PHP:  random_int(1, 100);
来源：http://yfq.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ogm.kuanghao11.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://coe.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://mvv.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kro.ctjpmb.com

Ruby: rand(1..100)
来源：http://bcg.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://nhd.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://die.9152youxi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ukg.hfpthk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://osd.cqqwz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qyv.ydzc1.top

TS:   x > 0 ? "yes" : "no"
来源：http://wfm.chenlongwang.top

Java: x > 0 ? "yes" : "no"
来源：http://bvz.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://elr.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ipb.jqgufenzy.top

C#:   x > 0 ? "yes" : "no"
来源：http://won.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://hok.cdnleiting.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://utd.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xhj.ydzc1.top

JS:   `Hello, ${name}!`
来源：http://qwl.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://odi.gogol.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://jjh.dashuyun.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wsj.hnxiangtu.top

Ruby: "Hello, #{name}!"
来源：http://xau.tarul.cn

C#:   $"Hello, {name}!"
来源：http://tue.yangfankeji.com

[A13] 多行字符串（练习 \n 转义）
来源：http://ofj.yj20258888.top

Py:   "第一行\n第二行"
来源：http://dwf.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://bzb.vehdjk.com

JS:   "第一行\n第二行"
来源：http://tgk.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://gdl.zdbjq.cn

Java: "第一行\n第二行"
来源：http://ukf.xylfe.cn

Go:   "第一行\n第二行"
来源：http://euj.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://adu.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://vgq.vqdsnc.cn

[A14] 注释写法
来源：http://vmt.xziqi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oyz.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zlo.hesvh.cn

JS:   // 单行；/* 多行 */
来源：http://qkx.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://ctf.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xhq.sweek.top

Go:   // 单行；/* 多行 */
来源：http://rxm.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://yuu.yangfankeji.com


<!-- 参考信息 -->