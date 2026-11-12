代发 wailian999

[U91] JS：对象键值遍历
来源：http://jth.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kjc.nwbrower.top

[U92] JS：深拷贝
来源：http://bry.chenlongwang.top

structuredClone(obj)
来源：http://nuo.vehdjk.com

[U93] JS：模板字符串
来源：http://ony.hcnkem.com

`共 ${n} 条`
来源：http://xwv.vqdsnc.cn

[U94] JS：箭头函数
来源：http://gdt.wangshuangyany.cn

const double = x => x * 2;
来源：http://uly.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://yhg.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://ien.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://ikc.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://etp.pengpengdd.cyou

[U97] JS：并发请求
来源：http://jzf.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qtn.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://mjp.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mkn.jiagoushi.top

[U99] JS：事件监听
来源：http://sfy.ybcxt.top

el.addEventListener("click", e => {})
来源：http://pdq.sweek.top

[U100] JS：DOM 查询
来源：http://cvu.fengsongda.top

document.querySelector(".item")
来源：http://vzz.cdnleiting.top

[U101] JS：classList 操作
来源：http://vpm.cqqwz.cn

el.classList.toggle("active")
来源：http://bls.bjfxy.top

[U102] JS：本地存储
来源：http://zmd.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zrg.ydzc1.top

[U103] JS：定时器
来源：http://gxd.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mis.ydjk.org.cn

[U104] JS：防抖
来源：http://gia.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwd.shangyingyoupin.top

[U105] JS：节流
来源：http://jbz.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zrd.jqgufenzy.top

[U106] JS：日期格式化
来源：http://bxg.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jmu.gzhubu.top

[U107] JS：数字千分位
来源：http://mut.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://chn.nwbrower.top

[U108] JS：随机整数
来源：http://txn.snrcjt.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ild.ehwqpu.com

[U109] JS：数组分组
来源：http://ofp.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://yza.tianlin.xyz

[U110] JS：数组分块
来源：http://hxr.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://trw.tanke756.top

[U111] JS：对象转 Map
来源：http://ctg.epnwcf.com

new Map(Object.entries(obj))
来源：http://iva.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://cps.andypj.xyz

"7".padStart(3, "0")
来源：http://yrj.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://gpx.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://ura.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://pnu.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kig.jinqigufen.top

[U115] JS：生成 UUID
来源：http://efa.hcnkem.com

crypto.randomUUID()
来源：http://hik.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://ksz.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://bix.cucudq.cn

[U117] JS：单元测试
来源：http://ohx.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://ejl.sxryk.cn

[U118] JS：开发服务器
来源：http://slu.yvedp.cn

npm i -D vite;  npx vite
来源：http://enl.nwbrower.top

[U119] JS：生产构建
来源：http://agy.ywan-chungtsiang.top

npx vite build
来源：http://ozt.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://yck.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://nys.nanxuanxn.top

================================================================================
来源：http://amq.meibo888.top

统计汇总
来源：http://usp.havefunace.top

================================================================================
来源：http://fkb.fzhhl.top

按语言统计（条）：
来源：http://jia.jinqigufen.top

Python ......... 252
来源：http://ylg.zhijiandao.cn

PHP ............ 252
来源：http://exg.snrcjt.cn

JavaScript ..... 252
来源：http://dxx.uphjek.com

TypeScript ..... 212
来源：http://czt.9152youxi.cn

Java ........... 212
来源：http://fol.jlsjyb.cn

Go ............. 212
来源：http://gmb.jinyuanbaomall.cn

Ruby ........... 212
来源：http://mne.ctjpmb.com

C# ............. 212
来源：http://rme.hnqzz.top

C .............. 30
来源：http://rzm.wangdashe.top

C++ ............ 30
来源：http://pkh.yj20258.top

SQL ............ 90
来源：http://fsj.daria6918.cn

Bash ........... 80
来源：http://myi.yj20258888.top

Kotlin ......... 15
来源：http://dyk.chenlongwang.top

Swift .......... 15
来源：http://lgf.jinqigfzy.top

Lua ............ 10
来源：http://ltu.ybcxt.top

Perl ........... 10
来源：http://mmi.hcnkem.com

Scala .......... 10
来源：http://ugv.fehbvm.com

------------------------------------
来源：http://omd.hesvh.cn

合计 ........... 2106 条
来源：http://koj.aibaodan.cn

按章节统计：
来源：http://npc.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hxz.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://svu.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xin.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yar.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gdb.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://beh.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://naw.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddt.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://riu.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yjx.nanxuanxn.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oee.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hjf.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mqz.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hnt.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vtw.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://six.zhongyouzk.top

Q SQL 专题                              90
来源：http://wxl.yangfankeji.com

R Bash 专题                             80
来源：http://lub.zhengqikj.top

S C / C++ 专题                          60
来源：http://ttp.sxryk.cn

T 其他语言补充                          60
来源：http://sjs.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://sxt.hcnkem.com

------------------------------------
来源：http://fiw.xinyue.icu

合计                                  2106 条
来源：http://hns.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://zjj.andypj.xyz

使用提醒
来源：http://khc.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://ffo.redwolf501.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xpb.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mnp.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iqw.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://quf.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hkq.yj20258.top

—— 文件结束 ——
来源：http://zgz.yuxming.cn

================================================================================
来源：http://dfe.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://jzc.sysykeji.top

Common Programming Examples Cheat Book
来源：http://rrs.xinyue.icu

================================================================================
来源：http://mno.guannengcc.top

【收录内容】
来源：http://sdc.yvedp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vlj.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dja.yfazqb.com

SQL · Bash · C · C++
来源：http://yei.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lih.zhaomingkeji.xyz

【使用说明】
来源：http://zbl.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cxx.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ljc.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qpb.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tlg.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lfe.c1oappe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zyt.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pgn.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dcn.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tvv.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bwu.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bzb.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fzh.cheryme.top

【文件统计】
来源：http://har.quarkkingdee.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://itt.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://lou.sysykeji.top

目  录
来源：http://hjy.yj202588.top

--------------------------------------------------------------------------------
来源：http://pks.yongpay.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dgl.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://smo.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pgr.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dub.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lts.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ufz.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://idg.sxryk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zwp.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tkx.bbcook.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://avo.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ynx.jinqigufen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ywa.jqgufenzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iob.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://okm.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://btw.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bfc.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ynl.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jft.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xxi.cucudq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dli.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pme.quarkkingdee.top

================================================================================
来源：http://sth.xziqi.cn

A. 基础语法与类型
来源：http://gyo.ywan-chungtsiang.top

================================================================================
来源：http://pib.316326.xyz

[A01] Hello World
来源：http://egw.yuanzhike.top

Py:   print("Hello, World!")
来源：http://cxp.ivvv.top

PHP:  echo "Hello, World!";
来源：http://mnw.iojbl.cn

JS:   console.log("Hello, World!");
来源：http://jke.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jdz.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://faz.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://vds.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://kzp.wangshuangyany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rda.sweek.top

[A02] 变量声明与赋值
来源：http://ugm.nanxinkj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tuk.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://jdj.yj20258888.top

JS:   let name = "Alex"; const age = 20;
来源：http://jwn.sysykeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bjc.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://you.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://gny.yangfankeji.com

Ruby: name = "Alex"; age = 20
来源：http://bvd.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aly.aizwys.cn

[A03] 常量定义
来源：http://dgz.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://izm.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://gpg.bjfxy.top

JS:   const PI = 3.14159;
来源：http://swo.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://jjt.sxryk.cn

Java: static final double PI = 3.14159;
来源：http://vja.jiagoushi.top

Go:   const PI = 3.14159
来源：http://fxh.bjfxy.top

Ruby: PI = 3.14159
来源：http://yav.mhx1999.top

C#:   const double PI = 3.14159;
来源：http://tin.kuanghao11.cn

[A04] 判断变量类型
来源：http://vmh.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gzd.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ffe.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ofs.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://ldr.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ifl.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hck.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://apl.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://evb.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://jot.feifeiyinyue.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gam.jqgufenzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uld.xuanzx.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iel.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jen.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://lwo.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://xyi.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://aaz.gzhubu.top

C#:   7 / 2; 7 % 2
来源：http://woo.dianchejie.cn

[A06] 字符串转数字
来源：http://cko.feifeiyinyue.top

Py:   int("42"); float("3.14")
来源：http://akh.shanyushiyangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dcq.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bjw.yfazqb.com

TS:   parseInt("42", 10); Number("42")
来源：http://uah.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nub.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://viz.yj202588.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nrj.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rxq.yvedp.cn

[A07] 数字转字符串
来源：http://dbo.jinqigufen.top

Py:   str(42)
来源：http://uiz.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://tjd.snrcjt.cn

JS:   String(42); (42).toString()
来源：http://cnq.yonumen.top

TS:   String(42)
来源：http://gxm.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wep.dianchejie.cn

Go:   strconv.Itoa(42)
来源：http://ppf.uphjek.com

Ruby: 42.to_s
来源：http://qwc.ydzc1.top

C#:   42.ToString()
来源：http://aeu.xylfe.cn

[A08] 取整与四舍五入
来源：http://iwh.chenjidiqi.icu

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fbi.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iid.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gyv.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baf.gaohongyu789.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bax.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ais.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://emx.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://alm.haohaochexian.top

[A09] 绝对值与最大最小值
来源：http://mww.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hek.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xgu.vqdsnc.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lus.svipenyu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mno.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://taw.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kax.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fos.meibo888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zct.chenzaomai.com

[A10] 生成随机数
来源：http://cer.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://iah.ctjpmb.com

PHP:  random_int(1, 100);
来源：http://opl.iojbl.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sxn.ctjpmb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vuz.hywenlv.cn

Java: new Random().nextInt(100) + 1
来源：http://guf.fzhhl.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jfp.sjlbkw.cn

Ruby: rand(1..100)
来源：http://dqf.hammf.cn

C#:   new Random().Next(1, 101)
来源：http://qim.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://nsm.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://dcu.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fkx.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://zwg.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hfm.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://qox.fehbvm.com

Go:   // 无三元运算符，需用 if 语句
来源：http://dlp.shuidangran.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pog.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://swm.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://udn.hfpthk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://adt.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pxh.bbcook.cn

JS:   `Hello, ${name}!`
来源：http://abh.wangshuangyany.cn

TS:   `Hello, ${name}!`
来源：http://chh.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://con.bjfxy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nkh.gzhubu.top

Ruby: "Hello, #{name}!"
来源：http://cew.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://exw.birdmap.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hlv.yuxming.cn

Py:   "第一行\n第二行"
来源：http://dej.iojbl.cn

PHP:  "第一行\n第二行"
来源：http://kha.aizwys.cn

JS:   "第一行\n第二行"
来源：http://ngl.birdmap.top

TS:   "第一行\n第二行"
来源：http://mak.cheryme.top

Java: "第一行\n第二行"
来源：http://yqf.zdqjudy.top

Go:   "第一行\n第二行"
来源：http://vhg.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://cxy.yvedp.cn

C#:   "第一行\n第二行"
来源：http://gjb.haohaochexian.top

[A14] 注释写法
来源：http://llx.uphjek.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://ucf.meibo888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wow.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://hnw.vehdjk.com

TS:   // 单行；/* 多行 */
来源：http://zwa.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ysk.sxryk.cn

Go:   // 单行；/* 多行 */
来源：http://kic.hywenlv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xjo.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://lkx.ybcxt.top

[A15] 空值判断与默认值
来源：http://mjd.zdbjq.cn

Py:   value = data or "默认值"
来源：http://gtt.ybcxt.top

PHP:  $value = $data ?? "默认值";
来源：http://ete.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://nfy.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://vjr.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vwc.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://nhh.vehdjk.com


<!-- 参考信息 -->