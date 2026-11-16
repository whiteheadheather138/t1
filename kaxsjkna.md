代发 wailian999

[U91] JS：对象键值遍历
来源：http://zyb.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://atj.sjlbkw.cn

[U92] JS：深拷贝
来源：http://qcn.aizwys.cn

structuredClone(obj)
来源：http://wcr.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://rhq.yj202588.top

`共 ${n} 条`
来源：http://zgl.hnxiangtu.top

[U94] JS：箭头函数
来源：http://elb.vehdjk.com

const double = x => x * 2;
来源：http://vpq.yfazqb.com

[U95] JS：Promise 包装
来源：http://beo.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://ovl.yonumen.top

[U96] JS：async/await 与异常
来源：http://kpr.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ymc.epnwcf.com

[U97] JS：并发请求
来源：http://kfq.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rbi.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://ctu.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mzm.xylfe.cn

[U99] JS：事件监听
来源：http://tkn.redwolf501.top

el.addEventListener("click", e => {})
来源：http://ezp.tarul.cn

[U100] JS：DOM 查询
来源：http://gfh.cashguo.top

document.querySelector(".item")
来源：http://kzb.epnwcf.com

[U101] JS：classList 操作
来源：http://uht.ctjpmb.com

el.classList.toggle("active")
来源：http://ufb.jqgufenzy.top

[U102] JS：本地存储
来源：http://vni.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dav.tarul.cn

[U103] JS：定时器
来源：http://ean.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fwb.hammf.cn

[U104] JS：防抖
来源：http://zci.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzj.gzhubu.top

[U105] JS：节流
来源：http://byk.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qjr.zdbjq.cn

[U106] JS：日期格式化
来源：http://xcx.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kvo.sufxvd.cn

[U107] JS：数字千分位
来源：http://zfi.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://syp.jqgufenzy.top

[U108] JS：随机整数
来源：http://lns.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gev.jinqigufen.top

[U109] JS：数组分组
来源：http://dzf.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://peb.zdbjq.cn

[U110] JS：数组分块
来源：http://lmm.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nob.tian-w.cn

[U111] JS：对象转 Map
来源：http://xkr.cqqwz.cn

new Map(Object.entries(obj))
来源：http://alj.9152youxi.cn

[U112] JS：字符串补位
来源：http://fvt.uphjek.com

"7".padStart(3, "0")
来源：http://hrf.gogol.net.cn

[U113] JS：正则替换全部
来源：http://qiz.jinqigufen.top

s.replaceAll("a", "b")
来源：http://dxv.xuanzx.com

[U114] JS：JSON 深比较
来源：http://lcr.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://klv.zhengqikj.top

[U115] JS：生成 UUID
来源：http://ooi.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://rbe.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://bzn.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://kmq.cashguo.top

[U117] JS：单元测试
来源：http://xji.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://ggv.hammf.cn

[U118] JS：开发服务器
来源：http://awn.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://cpv.hnqzz.top

[U119] JS：生产构建
来源：http://ofu.jqgfzy.top

npx vite build
来源：http://wcv.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://lwc.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://ysx.hywenlv.cn

================================================================================
来源：http://gjy.guannengcc.top

统计汇总
来源：http://clk.hammf.cn

================================================================================
来源：http://tro.sweek.top

按语言统计（条）：
来源：http://mtd.birdmap.top

Python ......... 252
来源：http://ccn.xingfuxueyuan.xyz

PHP ............ 252
来源：http://koh.ppjwa.cn

JavaScript ..... 252
来源：http://noe.yanxiufei.cn

TypeScript ..... 212
来源：http://vxf.havefunace.top

Java ........... 212
来源：http://mqp.sysykeji.top

Go ............. 212
来源：http://btf.9152youxi.cn

Ruby ........... 212
来源：http://rsn.wangdashe.top

C# ............. 212
来源：http://dfx.daxiang520.top

C .............. 30
来源：http://afx.shangyingyoupin.top

C++ ............ 30
来源：http://zvq.hfpthk.cn

SQL ............ 90
来源：http://yrh.dashuyun.cn

Bash ........... 80
来源：http://ldd.nwbrower.top

Kotlin ......... 15
来源：http://hsi.yanxiufei.cn

Swift .......... 15
来源：http://irw.yuanzhike.top

Lua ............ 10
来源：http://fcv.ivvv.top

Perl ........... 10
来源：http://wfs.chenjidiqi.icu

Scala .......... 10
来源：http://zud.svipenyu.cn

------------------------------------
来源：http://uai.chenzaomai.com

合计 ........... 2106 条
来源：http://twh.mhx1999.top

按章节统计：
来源：http://cek.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cqr.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wbt.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hea.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fuw.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uew.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jpc.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rzp.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lzn.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://erf.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vby.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nzo.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qsu.shzxlz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://krv.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blj.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mdu.chenlongwang.top

Q SQL 专题                              90
来源：http://ufe.jinghuilouyu.cn

R Bash 专题                             80
来源：http://not.haohaochexian.top

S C / C++ 专题                          60
来源：http://zaa.xylfe.cn

T 其他语言补充                          60
来源：http://has.hfpthk.cn

U 高频实用片段                         120
来源：http://mzf.uphjek.com

------------------------------------
来源：http://nea.zdbjq.cn

合计                                  2106 条
来源：http://ffu.c1oappe.top

--------------------------------------------------------------------------------
来源：http://ntc.dianchejie.cn

使用提醒
来源：http://iaf.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://hka.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ajt.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vqg.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ran.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fww.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yvf.mhx1999.top

—— 文件结束 ——
来源：http://gwd.mhx1999.top

================================================================================
来源：http://kzm.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://czz.meibo888.top

Common Programming Examples Cheat Book
来源：http://bnq.yongpay.top

================================================================================
来源：http://yvg.guowangkeji.top

【收录内容】
来源：http://tya.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ugr.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://thj.yangfankeji.com

SQL · Bash · C · C++
来源：http://auz.zdbjq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tfc.jlsjyb.cn

【使用说明】
来源：http://wto.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ymm.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rbm.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lpj.cqqwz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bbn.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dja.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gvw.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qon.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://naa.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ctw.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vqm.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iob.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ppp.xuetiantiany.cn

【文件统计】
来源：http://dqk.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sbe.cashguo.top

--------------------------------------------------------------------------------
来源：http://woz.gaohongyu789.top

目  录
来源：http://dwg.redwolf501.top

--------------------------------------------------------------------------------
来源：http://emo.ppjwa.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xuc.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bgx.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ffn.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zyw.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rub.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gtg.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lsg.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fra.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tpj.c1oappe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rnj.epnwcf.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://amo.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rwq.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vri.vqdsnc.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zaw.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gfe.fanxiaobao.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vnp.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wdj.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eew.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xyk.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://djo.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ugs.ybcxt.top

================================================================================
来源：http://ybb.hfpthk.cn

A. 基础语法与类型
来源：http://jpg.shuidangran.top

================================================================================
来源：http://mkk.shangyingyoupin.top

[A01] Hello World
来源：http://rhk.9152youxi.cn

Py:   print("Hello, World!")
来源：http://ojt.hcnkem.com

PHP:  echo "Hello, World!";
来源：http://dea.fehbvm.com

JS:   console.log("Hello, World!");
来源：http://uhy.fzhhl.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ydr.cashguo.top

Java: System.out.println("Hello, World!");
来源：http://prs.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://jdm.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://gum.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://btx.vehdjk.com

[A02] 变量声明与赋值
来源：http://jqr.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eop.yanxiufei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kns.fengsongda.top

JS:   let name = "Alex"; const age = 20;
来源：http://ppa.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qvd.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://bxb.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://uvw.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://nrx.chenlongwang.top

C#:   string name = "Alex"; int age = 20;
来源：http://unf.chenjidiqi.icu

[A03] 常量定义
来源：http://eqt.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lep.pycfn.com

PHP:  const PI = 3.14159;
来源：http://vmz.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://eyl.nwbrower.top

TS:   const PI: number = 3.14159;
来源：http://zmi.ybcxt.top

Java: static final double PI = 3.14159;
来源：http://eou.zhixingplan.top

Go:   const PI = 3.14159
来源：http://eig.fengsongda.top

Ruby: PI = 3.14159
来源：http://ukf.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://znc.sweek.top

[A04] 判断变量类型
来源：http://lnh.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gwr.birdmap.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uwe.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yja.yvedp.cn

TS:   typeof x; x instanceof Date
来源：http://ttn.jianghu66.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://maw.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://swd.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tod.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://xil.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://jvd.jqgfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vgi.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zvh.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://syp.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rgi.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://hmo.zhaomingkeji.xyz

Go:   7 / 2; 7 % 2
来源：http://vbc.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://ilh.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://hxc.yuxming.cn

[A06] 字符串转数字
来源：http://yhk.quarkkingdee.top

Py:   int("42"); float("3.14")
来源：http://dvf.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nhs.vqdsnc.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wbj.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pxi.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ryd.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zxd.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ytz.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://omd.hnxiangtu.top

[A07] 数字转字符串
来源：http://gdn.feifeiyinyue.top

Py:   str(42)
来源：http://qhx.aibaodan.cn

PHP:  (string) 42; strval(42)
来源：http://lds.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://wsy.jlsjyb.cn

TS:   String(42)
来源：http://kes.hnqzz.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ymp.guowangkeji.top

Go:   strconv.Itoa(42)
来源：http://mbu.nanxuanxn.top

Ruby: 42.to_s
来源：http://avb.fengsongda.top

C#:   42.ToString()
来源：http://eqo.yongpay.top

[A08] 取整与四舍五入
来源：http://mpi.jinghuilouyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://csh.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://eys.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hif.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ppj.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tns.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nvv.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kbj.chenjidiqi.icu

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://huy.cucudq.cn

[A09] 绝对值与最大最小值
来源：http://okp.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ttn.havefunace.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://doi.vehdjk.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://efo.dianchejie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qax.uphjek.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dtm.yuxming.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qip.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vqc.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aoz.kuanghao11.cn

[A10] 生成随机数
来源：http://wis.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://kel.uphjek.com

PHP:  random_int(1, 100);
来源：http://biu.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vnq.hammf.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bpk.cheryme.top

Java: new Random().nextInt(100) + 1
来源：http://gvy.yuanzhike.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yet.zhoulong.xyz

Ruby: rand(1..100)
来源：http://gei.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://gdn.fengsongda.top

[A11] 条件表达式（三元）
来源：http://qrf.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://vei.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qga.fktsv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ljy.fktsv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dau.mhx1999.top

Java: x > 0 ? "yes" : "no"
来源：http://aoi.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lyz.hnqzz.top

Ruby: x > 0 ? "yes" : "no"
来源：http://htw.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jwc.zhongyouzk.top

[A12] 字符串插值 / 格式化
来源：http://mfn.wangdashe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fii.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bxn.ivvv.top

JS:   `Hello, ${name}!`
来源：http://irb.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://tjh.xuanzx.com

Java: "Hello, %s!".formatted(name)
来源：http://rbc.yvedp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pwo.yuanzhike.top

Ruby: "Hello, #{name}!"
来源：http://udt.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://izf.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://njl.nanxuanxn.top

Py:   "第一行\n第二行"
来源：http://zmv.9152youxi.cn

PHP:  "第一行\n第二行"
来源：http://iju.yangfankeji.com

JS:   "第一行\n第二行"
来源：http://rss.mhx1999.top

TS:   "第一行\n第二行"
来源：http://guw.fktsv.cn

Java: "第一行\n第二行"
来源：http://dok.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://cur.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://bjd.52xcode.cn

C#:   "第一行\n第二行"
来源：http://kws.ctjpmb.com

[A14] 注释写法
来源：http://dnj.hongshengwenyu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://agj.sweek.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://bnm.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://tdr.cheryme.top

TS:   // 单行；/* 多行 */
来源：http://vfu.dianchejie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rty.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://six.dianchejie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ols.hywenlv.cn

C#:   // 单行；/* 多行 */
来源：http://cpy.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://yrw.sweek.top

Py:   value = data or "默认值"
来源：http://qvi.pengpengdd.cyou

PHP:  $value = $data ?? "默认值";
来源：http://yok.cheryme.top

JS:   const value = data ?? "默认值";
来源：http://pza.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://xgh.nwbrower.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://byy.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://eiy.epnwcf.com


<!-- 参考信息 -->