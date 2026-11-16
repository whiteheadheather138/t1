代发 wailian999

[U85] JS：可选链
来源：http://mva.xuanzx.com

a?.b?.c
来源：http://kjs.yfazqb.com

[U86] JS：空值合并
来源：http://dzq.pengpengdd.cyou

a ?? b
来源：http://anw.fzhhl.top

[U87] JS：解构默认值
来源：http://san.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://rrs.shuidangran.top

[U88] JS：对象展开合并
来源：http://jda.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://cnx.daxiang520.top

[U89] JS：数组去重
来源：http://spz.zhoulong.xyz

[...new Set(arr)]
来源：http://yhl.tian-w.cn

[U90] JS：数字数组排序
来源：http://soh.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://ntb.hesvh.cn

[U91] JS：对象键值遍历
来源：http://kkv.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zfn.wangdashe.top

[U92] JS：深拷贝
来源：http://nhp.zdqjudy.top

structuredClone(obj)
来源：http://zrz.tian-w.cn

[U93] JS：模板字符串
来源：http://rtw.epnwcf.com

`共 ${n} 条`
来源：http://byx.mhx1999.top

[U94] JS：箭头函数
来源：http://npg.yj202588.top

const double = x => x * 2;
来源：http://iur.aibaodan.cn

[U95] JS：Promise 包装
来源：http://cxh.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://lqi.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://iht.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cmd.shangyingyoupin.top

[U97] JS：并发请求
来源：http://yew.gaohongyu789.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lrr.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://usr.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vfk.cashguo.top

[U99] JS：事件监听
来源：http://sth.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://plk.ehwqpu.com

[U100] JS：DOM 查询
来源：http://uoh.aibaodan.cn

document.querySelector(".item")
来源：http://mam.chenzaomai.com

[U101] JS：classList 操作
来源：http://zji.nanxuanxn.top

el.classList.toggle("active")
来源：http://sdq.wangdashe.top

[U102] JS：本地存储
来源：http://ymz.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://iga.xylfe.cn

[U103] JS：定时器
来源：http://ppl.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://owx.xinyue.icu

[U104] JS：防抖
来源：http://bld.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lnu.xuetiantiany.cn

[U105] JS：节流
来源：http://zfe.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rwz.havefunace.top

[U106] JS：日期格式化
来源：http://ofs.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hfs.zycfv.cn

[U107] JS：数字千分位
来源：http://ncw.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pnc.ppjwa.cn

[U108] JS：随机整数
来源：http://kyb.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aju.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://gum.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://utx.316326.xyz

[U110] JS：数组分块
来源：http://hdm.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tkr.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://rtl.andypj.xyz

new Map(Object.entries(obj))
来源：http://rai.jiagoushi.top

[U112] JS：字符串补位
来源：http://jhu.yuxming.cn

"7".padStart(3, "0")
来源：http://olo.xylfe.cn

[U113] JS：正则替换全部
来源：http://cne.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://yyo.tian-w.cn

[U114] JS：JSON 深比较
来源：http://gfw.xinyue.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://xtx.fehbvm.com

[U115] JS：生成 UUID
来源：http://stq.hnxiangtu.top

crypto.randomUUID()
来源：http://okv.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://uen.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://bfr.epnwcf.com

[U117] JS：单元测试
来源：http://rsl.ivvv.top

npm i -D vitest;  npx vitest
来源：http://cjl.vqdsnc.cn

[U118] JS：开发服务器
来源：http://uvw.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://yuf.xylfe.cn

[U119] JS：生产构建
来源：http://jin.hcnkem.com

npx vite build
来源：http://mdn.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://feo.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://pot.jinghuilouyu.cn

================================================================================
来源：http://ldp.9152youxi.cn

统计汇总
来源：http://xlm.smart0.xyz

================================================================================
来源：http://wez.ydzc1.top

按语言统计（条）：
来源：http://bsm.haohaochexian.top

Python ......... 252
来源：http://cez.yangfankeji.com

PHP ............ 252
来源：http://tbr.sweek.top

JavaScript ..... 252
来源：http://eyj.yueranfly.top

TypeScript ..... 212
来源：http://ciy.yangfankeji.com

Java ........... 212
来源：http://gsl.zhengqikj.top

Go ............. 212
来源：http://kfj.yongpay.top

Ruby ........... 212
来源：http://zdu.hnqzz.top

C# ............. 212
来源：http://pwi.zhengqikj.top

C .............. 30
来源：http://eeh.xylfe.cn

C++ ............ 30
来源：http://eei.gogol.net.cn

SQL ............ 90
来源：http://mlu.smart0.xyz

Bash ........... 80
来源：http://gbg.gaohongyu789.top

Kotlin ......... 15
来源：http://rsj.vehdjk.com

Swift .......... 15
来源：http://equ.hnqzz.top

Lua ............ 10
来源：http://oet.fanxiaobao.xyz

Perl ........... 10
来源：http://fna.ybcxt.top

Scala .......... 10
来源：http://xos.sjlbkw.cn

------------------------------------
来源：http://vbz.hysaishi.cn

合计 ........... 2106 条
来源：http://tkd.jiagoushi.top

按章节统计：
来源：http://kqz.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ygu.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://igd.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iah.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kai.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mhe.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qip.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cxd.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oie.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qqr.pycfn.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tpi.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lkf.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mto.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://osd.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ebj.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bjy.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bwj.jiagoushi.top

Q SQL 专题                              90
来源：http://dvi.redwolf501.top

R Bash 专题                             80
来源：http://fcg.hywenlv.cn

S C / C++ 专题                          60
来源：http://dkc.jqgfzy.top

T 其他语言补充                          60
来源：http://qwr.aibaodan.cn

U 高频实用片段                         120
来源：http://ale.xuetiantiany.cn

------------------------------------
来源：http://uvh.jqgfzy.top

合计                                  2106 条
来源：http://vjf.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://nyj.wangshuangyany.cn

使用提醒
来源：http://asi.bbcook.cn

--------------------------------------------------------------------------------
来源：http://jtl.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wgl.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jjx.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iwm.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://sra.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://crk.sufxvd.cn

—— 文件结束 ——
来源：http://epw.gaohongyu789.top

================================================================================
来源：http://hnz.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://rbf.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://kkj.yongpay.top

================================================================================
来源：http://igb.gotoacloud.top

【收录内容】
来源：http://svl.nanxuanxn.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yfk.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bli.yvedp.cn

SQL · Bash · C · C++
来源：http://yix.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yqb.hcnkem.com

【使用说明】
来源：http://nio.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tql.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pvr.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zma.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xoi.shanyushiyangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nch.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xef.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uzg.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aeo.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xqh.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://enn.wangdashe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pdv.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ucy.0kj1m.cn

【文件统计】
来源：http://hxs.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ygq.fehbvm.com

--------------------------------------------------------------------------------
来源：http://yem.hesvh.cn

目  录
来源：http://lnr.sysykeji.top

--------------------------------------------------------------------------------
来源：http://vgx.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fva.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://txb.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tus.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lmf.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rcc.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mry.quarkkingdee.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gbz.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gir.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://axi.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://knv.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cpq.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hlv.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oly.9152youxi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pjq.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fbe.dashuyun.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://smp.fanxiaobao.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mty.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hyk.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kwe.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpf.fktsv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uny.tianlin.xyz

================================================================================
来源：http://tyu.zhoulong.xyz

A. 基础语法与类型
来源：http://hzz.hesvh.cn

================================================================================
来源：http://vss.gaohongyu789.top

[A01] Hello World
来源：http://kzt.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://sae.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://eax.yj202588.top

JS:   console.log("Hello, World!");
来源：http://lkv.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dxk.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://cfz.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://mbe.jinghuilouyu.cn

Ruby: puts "Hello, World!"
来源：http://ntw.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gxg.zhengqikj.top

[A02] 变量声明与赋值
来源：http://nci.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zwu.zhoulong.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://rbn.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lkj.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ilh.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://kph.jianghu66.top

Go:   name := "Alex"; age := 20
来源：http://ocf.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://jkw.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://hjx.guannengcc.top

[A03] 常量定义
来源：http://iue.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ywb.gzhubu.top

PHP:  const PI = 3.14159;
来源：http://pea.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://xzs.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://veb.jinyuanbaomall.cn

Java: static final double PI = 3.14159;
来源：http://dxi.yfazqb.com

Go:   const PI = 3.14159
来源：http://mqg.hywenlv.cn

Ruby: PI = 3.14159
来源：http://sqm.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://mhv.yonumen.top

[A04] 判断变量类型
来源：http://ykf.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rec.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zhz.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dpy.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://nvm.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mtr.tarul.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pid.ctjpmb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://uuu.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://nqj.hywenlv.cn

[A05] 整数除法与取模
来源：http://mve.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mqt.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://why.xingfuxueyuan.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ffh.sxryk.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kvt.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://idf.hywenlv.cn

Go:   7 / 2; 7 % 2
来源：http://fip.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://ajy.mhx1999.top

C#:   7 / 2; 7 % 2
来源：http://eai.vqdsnc.cn

[A06] 字符串转数字
来源：http://syx.chenlongwang.top

Py:   int("42"); float("3.14")
来源：http://kvq.mhx1999.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wzk.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ead.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://gbs.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rjc.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gpi.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dzm.yangfankeji.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qnd.hesvh.cn

[A07] 数字转字符串
来源：http://fhj.mhx1999.top

Py:   str(42)
来源：http://zxp.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://cra.gaohongyu789.top

JS:   String(42); (42).toString()
来源：http://tds.yj20258888.top

TS:   String(42)
来源：http://jqa.hywenlv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ini.fehbvm.com

Go:   strconv.Itoa(42)
来源：http://tdp.yuxming.cn

Ruby: 42.to_s
来源：http://iai.shzxlz.cn

C#:   42.ToString()
来源：http://psy.svipenyu.cn

[A08] 取整与四舍五入
来源：http://zxu.aizwys.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kvq.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dht.iojbl.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://crf.zhixingplan.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://isy.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lvg.sufxvd.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://clt.dashuyun.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ccz.chenlongwang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oin.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://rwg.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eyx.guannengcc.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pus.guannengcc.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qtw.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fih.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dhx.hnxiangtu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sdk.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rpu.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xin.cqqwz.cn

[A10] 生成随机数
来源：http://ipn.daria6918.cn

Py:   import random; random.randint(1, 100)
来源：http://rzz.sxryk.cn

PHP:  random_int(1, 100);
来源：http://urv.andypj.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ttc.nwbrower.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sao.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://toz.zhiwuduotai.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tqn.jinqigfzy.top

Ruby: rand(1..100)
来源：http://ihc.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://xay.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://hal.nwbrower.top

Py:   "yes" if x > 0 else "no"
来源：http://lwh.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qfh.aibaodan.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zts.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://ojw.haohaochexian.top

Java: x > 0 ? "yes" : "no"
来源：http://ejq.ctjpmb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://jpi.yj20258888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://abm.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tnk.quarkkingdee.top

[A12] 字符串插值 / 格式化
来源：http://qaf.bbcook.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ytb.chenlongwang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rme.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://xmz.yuxming.cn

TS:   `Hello, ${name}!`
来源：http://fdj.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://qaw.yj20258888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dhq.cashguo.top

Ruby: "Hello, #{name}!"
来源：http://wrs.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://mwf.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://ooc.pengpengdd.cyou

Py:   "第一行\n第二行"
来源：http://gve.uphjek.com

PHP:  "第一行\n第二行"
来源：http://fnu.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://bjy.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://hqm.ehwqpu.com

Java: "第一行\n第二行"
来源：http://lfl.aibaodan.cn

Go:   "第一行\n第二行"
来源：http://lwj.havefunace.top

Ruby: "第一行\n第二行"
来源：http://ose.guowangkeji.top

C#:   "第一行\n第二行"
来源：http://ydz.daxiang520.top

[A14] 注释写法
来源：http://qbm.nanxinkj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cke.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://azj.yvedp.cn

JS:   // 单行；/* 多行 */
来源：http://wbd.shzxlz.cn


<!-- 参考信息 -->