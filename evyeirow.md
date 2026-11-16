代发 wailian999

[U85] JS：可选链
来源：http://byr.dianchejie.cn

a?.b?.c
来源：http://jfx.zhixingplan.top

[U86] JS：空值合并
来源：http://lqm.hysaishi.cn

a ?? b
来源：http://wcl.daxiang520.top

[U87] JS：解构默认值
来源：http://oto.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://dcc.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://vdz.shanyushiyangtech.top

{ ...a, ...b }
来源：http://yzo.ctjpmb.com

[U89] JS：数组去重
来源：http://sht.epnwcf.com

[...new Set(arr)]
来源：http://zmx.jyoumei.cn

[U90] JS：数字数组排序
来源：http://mwu.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://msh.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://niu.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ygy.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://uat.sweek.top

structuredClone(obj)
来源：http://avx.zhixingplan.top

[U93] JS：模板字符串
来源：http://zxm.hysaishi.cn

`共 ${n} 条`
来源：http://eyu.yangfankeji.com

[U94] JS：箭头函数
来源：http://wgz.gaohongyu789.top

const double = x => x * 2;
来源：http://bsc.tanke756.top

[U95] JS：Promise 包装
来源：http://vef.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://pwl.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://xdm.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://upz.0kj1m.cn

[U97] JS：并发请求
来源：http://njs.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rji.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://evq.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mfe.yonumen.top

[U99] JS：事件监听
来源：http://stq.xylfe.cn

el.addEventListener("click", e => {})
来源：http://rrs.zhixingplan.top

[U100] JS：DOM 查询
来源：http://syx.chenlongwang.top

document.querySelector(".item")
来源：http://fgr.svipenyu.cn

[U101] JS：classList 操作
来源：http://lnc.nanxuanxn.top

el.classList.toggle("active")
来源：http://lrk.aizwys.cn

[U102] JS：本地存储
来源：http://umn.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://mgj.dianchejie.cn

[U103] JS：定时器
来源：http://wbr.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ymp.316326.xyz

[U104] JS：防抖
来源：http://tzq.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwz.yongpay.top

[U105] JS：节流
来源：http://lsm.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pnk.daxiang520.top

[U106] JS：日期格式化
来源：http://wxo.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://abm.jinqigufen.top

[U107] JS：数字千分位
来源：http://bgz.fktsv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nrp.jiagoushi.top

[U108] JS：随机整数
来源：http://ins.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eku.gogol.net.cn

[U109] JS：数组分组
来源：http://aoh.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://ibg.andypj.xyz

[U110] JS：数组分块
来源：http://sxn.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kou.ppjwa.cn

[U111] JS：对象转 Map
来源：http://ejf.yueranfly.top

new Map(Object.entries(obj))
来源：http://nph.snrcjt.cn

[U112] JS：字符串补位
来源：http://phj.sufxvd.cn

"7".padStart(3, "0")
来源：http://xvv.yfazqb.com

[U113] JS：正则替换全部
来源：http://oqj.chenzaomai.com

s.replaceAll("a", "b")
来源：http://fxs.birdmap.top

[U114] JS：JSON 深比较
来源：http://tas.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pbv.fengsongda.top

[U115] JS：生成 UUID
来源：http://wcm.yuxming.cn

crypto.randomUUID()
来源：http://slu.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://nka.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://drk.jyoumei.cn

[U117] JS：单元测试
来源：http://kot.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://ndu.hfpthk.cn

[U118] JS：开发服务器
来源：http://zyn.ybcxt.top

npm i -D vite;  npx vite
来源：http://zin.svipenyu.cn

[U119] JS：生产构建
来源：http://exb.bbcook.cn

npx vite build
来源：http://ret.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://isb.sweek.top

import.meta.env.VITE_API_URL
来源：http://byf.hywenlv.cn

================================================================================
来源：http://wyz.zhongyouzk.top

统计汇总
来源：http://hbg.zhengqikj.top

================================================================================
来源：http://yfx.cashguo.top

按语言统计（条）：
来源：http://cxt.wangdashe.top

Python ......... 252
来源：http://nul.zhaomingkeji.xyz

PHP ............ 252
来源：http://ryj.gotoacloud.top

JavaScript ..... 252
来源：http://wte.redwolf501.top

TypeScript ..... 212
来源：http://pto.bbcook.cn

Java ........... 212
来源：http://bkn.sweek.top

Go ............. 212
来源：http://bvd.ydjk.org.cn

Ruby ........... 212
来源：http://vxj.ydjk.org.cn

C# ............. 212
来源：http://moq.hywenlv.cn

C .............. 30
来源：http://cro.haohaochexian.top

C++ ............ 30
来源：http://wgb.pengpengdd.cyou

SQL ............ 90
来源：http://eda.xuetiantiany.cn

Bash ........... 80
来源：http://srh.kuanghao11.cn

Kotlin ......... 15
来源：http://pzq.hfpthk.cn

Swift .......... 15
来源：http://wir.zhaomingkeji.xyz

Lua ............ 10
来源：http://obm.jinyuanbaomall.cn

Perl ........... 10
来源：http://ovv.jinqigfzy.top

Scala .......... 10
来源：http://tto.kuanghao11.cn

------------------------------------
来源：http://rer.yongpay.top

合计 ........... 2106 条
来源：http://fvq.jinqigfzy.top

按章节统计：
来源：http://vlc.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rod.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qvv.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kxj.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bwh.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iim.chenlongwang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kqv.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://omj.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kre.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sul.gotoacloud.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wew.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lcq.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fkv.ybcxt.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ipt.yj20258.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zze.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aod.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mhk.zhixingplan.top

Q SQL 专题                              90
来源：http://ciy.xinyue.icu

R Bash 专题                             80
来源：http://ant.svipenyu.cn

S C / C++ 专题                          60
来源：http://bnw.fzhhl.top

T 其他语言补充                          60
来源：http://qkb.316326.xyz

U 高频实用片段                         120
来源：http://vwm.tarul.cn

------------------------------------
来源：http://ivn.birdmap.top

合计                                  2106 条
来源：http://mvg.yj20258.top

--------------------------------------------------------------------------------
来源：http://jes.shanyushiyangtech.top

使用提醒
来源：http://huv.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://grm.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kyx.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://goq.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ykh.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jsp.cashguo.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lbq.yj202588.top

—— 文件结束 ——
来源：http://shu.ivvv.top

================================================================================
来源：http://lbi.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://nii.aizwys.cn

Common Programming Examples Cheat Book
来源：http://gcy.jinqigfzy.top

================================================================================
来源：http://hhy.ivvv.top

【收录内容】
来源：http://lcc.jlsjyb.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dvj.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pgo.fengsongda.top

SQL · Bash · C · C++
来源：http://gwk.yuanzhike.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yed.yonumen.top

【使用说明】
来源：http://lae.vqdsnc.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gkz.pycfn.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eov.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://okc.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ktd.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://upx.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eol.hnqzz.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uui.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oeu.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uwh.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bwc.cqqwz.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xpk.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wjf.ybcxt.top

【文件统计】
来源：http://ogv.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uyw.316326.xyz

--------------------------------------------------------------------------------
来源：http://hkp.hesvh.cn

目  录
来源：http://fxj.hesvh.cn

--------------------------------------------------------------------------------
来源：http://gld.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jcx.zhongyouzk.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fqd.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yjj.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://isb.nwbrower.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xcf.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cjy.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yea.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vbc.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yyg.wangdashe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aha.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nxv.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ngb.kuanghao11.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://umf.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yvt.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mzx.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rgi.zhaomingkeji.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pkd.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xzo.hysaishi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nia.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hot.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ewe.yj20258888.top

================================================================================
来源：http://ibj.hongshengwenyu.top

A. 基础语法与类型
来源：http://kzo.xuetiantiany.cn

================================================================================
来源：http://fem.hongshengwenyu.top

[A01] Hello World
来源：http://tih.tianlin.xyz

Py:   print("Hello, World!")
来源：http://mqz.hammf.cn

PHP:  echo "Hello, World!";
来源：http://oxo.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://haw.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fxw.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://arg.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://orq.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://pbf.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://efh.jiagoushi.top

[A02] 变量声明与赋值
来源：http://sek.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jfa.zhixingplan.top

PHP:  $name = "Alex"; $age = 20;
来源：http://vdr.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ila.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ndf.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://zgt.sweek.top

Go:   name := "Alex"; age := 20
来源：http://oio.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://jam.ywan-chungtsiang.top

C#:   string name = "Alex"; int age = 20;
来源：http://gve.shangyingyoupin.top

[A03] 常量定义
来源：http://yle.yj20258.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lof.shanyushiyangkeji.top

PHP:  const PI = 3.14159;
来源：http://laq.zhengqikj.top

JS:   const PI = 3.14159;
来源：http://lqw.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://loa.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://euk.gaohongyu789.top

Go:   const PI = 3.14159
来源：http://hxg.epnwcf.com

Ruby: PI = 3.14159
来源：http://svv.zhaomingkeji.xyz

C#:   const double PI = 3.14159;
来源：http://yon.fengsongda.top

[A04] 判断变量类型
来源：http://pis.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sdz.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kqy.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gio.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://oxv.cqqwz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://brm.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rne.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://gcr.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://gen.fktsv.cn

[A05] 整数除法与取模
来源：http://enh.pycfn.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xds.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://elt.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ukz.shzxlz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lcg.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://nym.xingfuxueyuan.xyz

Go:   7 / 2; 7 % 2
来源：http://fyi.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://jxh.ivvv.top

C#:   7 / 2; 7 % 2
来源：http://hvd.yongpay.top

[A06] 字符串转数字
来源：http://zag.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://ihp.hywenlv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pxd.jianghu66.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jvi.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://ufw.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yrc.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ava.hnqzz.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fhp.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mav.wangshuangyany.cn

[A07] 数字转字符串
来源：http://hbc.ehwqpu.com

Py:   str(42)
来源：http://cko.zhoulong.xyz

PHP:  (string) 42; strval(42)
来源：http://vuz.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://cyd.sufxvd.cn

TS:   String(42)
来源：http://jdr.feifeiyinyue.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pns.hongshengwenyu.top

Go:   strconv.Itoa(42)
来源：http://yar.xinyue.icu

Ruby: 42.to_s
来源：http://uoa.guannengcc.top

C#:   42.ToString()
来源：http://yet.0kj1m.cn

[A08] 取整与四舍五入
来源：http://ioo.hnxiangtu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nre.yuxming.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ire.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zdz.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hoi.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://emd.chenjidiqi.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rzk.quarkkingdee.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gvl.hfpthk.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zlb.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://iht.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dya.shanyushiyangtech.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tme.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rgg.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ddp.sweek.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qri.zdqjudy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oft.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zfl.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tiu.sweek.top

[A10] 生成随机数
来源：http://fcu.zdbjq.cn

Py:   import random; random.randint(1, 100)
来源：http://cjx.meibo888.top

PHP:  random_int(1, 100);
来源：http://lzy.yj202588.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://onw.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ezk.guowangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://kap.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gsq.c1oappe.top

Ruby: rand(1..100)
来源：http://utc.zhiwuduotai.top

C#:   new Random().Next(1, 101)
来源：http://qxg.fengsongda.top

[A11] 条件表达式（三元）
来源：http://vja.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://pfs.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://wqz.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://qmr.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oft.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://wsw.jianghu66.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ivj.tanke756.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ejp.fehbvm.com

C#:   x > 0 ? "yes" : "no"
来源：http://igb.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://fhb.tianlin.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vqw.vqdsnc.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uwx.meibo888.top

JS:   `Hello, ${name}!`
来源：http://zev.shzxlz.cn

TS:   `Hello, ${name}!`
来源：http://xko.zhixingplan.top

Java: "Hello, %s!".formatted(name)
来源：http://nnf.sufxvd.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ctv.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://ucl.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://hfw.yongpay.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hxk.zhixingplan.top

Py:   "第一行\n第二行"
来源：http://dgr.tianlin.xyz

PHP:  "第一行\n第二行"
来源：http://ris.jinqigfzy.top

JS:   "第一行\n第二行"
来源：http://nax.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://yay.sxryk.cn

Java: "第一行\n第二行"
来源：http://rno.gaohongyu789.top

Go:   "第一行\n第二行"
来源：http://ssf.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://umi.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://pja.snrcjt.cn

[A14] 注释写法
来源：http://xzu.zhaomingkeji.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://pjj.cashguo.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jho.jqgfzy.top

JS:   // 单行；/* 多行 */
来源：http://ldc.birdmap.top


<!-- 参考信息 -->