代发 wailian999

[U91] JS：对象键值遍历
来源：http://qtp.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zqw.cheryme.top

[U92] JS：深拷贝
来源：http://uwi.shuidangran.top

structuredClone(obj)
来源：http://kyx.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://jya.pengpengdd.cyou

`共 ${n} 条`
来源：http://edm.daria6918.cn

[U94] JS：箭头函数
来源：http://zek.ybcxt.top

const double = x => x * 2;
来源：http://sqn.hywenlv.cn

[U95] JS：Promise 包装
来源：http://lys.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://wzd.fehbvm.com

[U96] JS：async/await 与异常
来源：http://qwb.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ksk.9152youxi.cn

[U97] JS：并发请求
来源：http://nto.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lxp.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://kzd.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://euv.zhijiandao.cn

[U99] JS：事件监听
来源：http://ntm.hnqzz.top

el.addEventListener("click", e => {})
来源：http://hsk.ybcxt.top

[U100] JS：DOM 查询
来源：http://etg.yanxiufei.cn

document.querySelector(".item")
来源：http://ljb.yuanzhike.top

[U101] JS：classList 操作
来源：http://vbe.shzxlz.cn

el.classList.toggle("active")
来源：http://oqa.kuanghao11.cn

[U102] JS：本地存储
来源：http://atj.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fmz.meibo888.top

[U103] JS：定时器
来源：http://xeu.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iww.sweek.top

[U104] JS：防抖
来源：http://zuv.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfr.svipenyu.cn

[U105] JS：节流
来源：http://zfx.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vhm.smart0.xyz

[U106] JS：日期格式化
来源：http://jkd.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uyn.xinyue.icu

[U107] JS：数字千分位
来源：http://yni.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ltc.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://nnz.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fcb.zhixingplan.top

[U109] JS：数组分组
来源：http://dgk.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://dzp.shangyingyoupin.top

[U110] JS：数组分块
来源：http://uhr.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pek.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://cfk.bjfxy.top

new Map(Object.entries(obj))
来源：http://xda.hysaishi.cn

[U112] JS：字符串补位
来源：http://sbt.mhx1999.top

"7".padStart(3, "0")
来源：http://hhp.tian-w.cn

[U113] JS：正则替换全部
来源：http://ecy.zdbjq.cn

s.replaceAll("a", "b")
来源：http://sba.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://ysn.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wsq.yanxiufei.cn

[U115] JS：生成 UUID
来源：http://thf.zdbjq.cn

crypto.randomUUID()
来源：http://rwg.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://joj.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://hsi.zycfv.cn

[U117] JS：单元测试
来源：http://avk.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://loy.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://tdv.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://bsb.xylfe.cn

[U119] JS：生产构建
来源：http://xpc.52xcode.cn

npx vite build
来源：http://wss.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://hhu.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://iul.sjlbkw.cn

================================================================================
来源：http://aac.ybcxt.top

统计汇总
来源：http://etv.yj20258888.top

================================================================================
来源：http://zso.jlsjyb.cn

按语言统计（条）：
来源：http://qos.andypj.xyz

Python ......... 252
来源：http://sgx.gzhubu.top

PHP ............ 252
来源：http://yut.zycfv.cn

JavaScript ..... 252
来源：http://sfo.jianghu66.top

TypeScript ..... 212
来源：http://cqe.chenjidiqi.icu

Java ........... 212
来源：http://ibv.xingfuxueyuan.xyz

Go ............. 212
来源：http://bnt.yanxiufei.cn

Ruby ........... 212
来源：http://ojh.52xcode.cn

C# ............. 212
来源：http://uos.hesvh.cn

C .............. 30
来源：http://igc.c1oappe.top

C++ ............ 30
来源：http://nwf.cashguo.top

SQL ............ 90
来源：http://ako.zdbjq.cn

Bash ........... 80
来源：http://olw.aibaodan.cn

Kotlin ......... 15
来源：http://slx.wangdashe.top

Swift .......... 15
来源：http://qer.zhaomingkeji.xyz

Lua ............ 10
来源：http://gql.ybcxt.top

Perl ........... 10
来源：http://oqg.daria6918.cn

Scala .......... 10
来源：http://pbk.52xcode.cn

------------------------------------
来源：http://lfa.tian-w.cn

合计 ........... 2106 条
来源：http://jxp.dianchejie.cn

按章节统计：
来源：http://slp.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zkk.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xos.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://psn.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://utf.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eeb.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uww.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://prj.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jdp.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ssq.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yro.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oek.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uzk.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ldd.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cld.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oso.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jwy.vehdjk.com

Q SQL 专题                              90
来源：http://vji.chenzaomai.com

R Bash 专题                             80
来源：http://kow.quarkkingdee.top

S C / C++ 专题                          60
来源：http://yhm.zhixingplan.top

T 其他语言补充                          60
来源：http://ckz.gogol.net.cn

U 高频实用片段                         120
来源：http://ofh.316326.xyz

------------------------------------
来源：http://gbm.xuanzx.com

合计                                  2106 条
来源：http://vqd.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://mrt.sxryk.cn

使用提醒
来源：http://djw.guannengcc.top

--------------------------------------------------------------------------------
来源：http://rlk.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bes.xziqi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qzc.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kkp.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rbo.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zgr.aizwys.cn

—— 文件结束 ——
来源：http://iuf.jianghu66.top

================================================================================
来源：http://xfi.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://rda.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://car.pycfn.com

================================================================================
来源：http://aab.havefunace.top

【收录内容】
来源：http://sys.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bxl.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xmp.gotoacloud.top

SQL · Bash · C · C++
来源：http://iuh.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dku.bjfxy.top

【使用说明】
来源：http://pzd.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wvn.tianlin.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cmk.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lgo.zhaomingkeji.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qwm.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uur.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cmr.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wfp.guannengcc.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bgg.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uvm.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cyg.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zps.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tbn.epnwcf.com

【文件统计】
来源：http://pbd.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nix.yj202588.top

--------------------------------------------------------------------------------
来源：http://asm.tanke756.top

目  录
来源：http://gii.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://atr.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qxb.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ujk.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pfz.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ago.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wpk.gzhubu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mkh.ctjpmb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qmf.fehbvm.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sfz.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qzc.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xrh.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://twb.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uhi.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eco.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jro.svipenyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jpj.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lxp.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bbc.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://nwp.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://snh.yj202588.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ulu.yj20258.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tej.hongshengwenyu.top

================================================================================
来源：http://gko.shanyushiyangkeji.top

A. 基础语法与类型
来源：http://owe.xuetiantiany.cn

================================================================================
来源：http://saw.cashguo.top

[A01] Hello World
来源：http://zfq.snrcjt.cn

Py:   print("Hello, World!")
来源：http://upo.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://tbu.zhaomingkeji.xyz

JS:   console.log("Hello, World!");
来源：http://kas.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kle.sweek.top

Java: System.out.println("Hello, World!");
来源：http://imu.xuanzx.com

Go:   fmt.Println("Hello, World!")
来源：http://emx.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://enn.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mcw.chenzaomai.com

[A02] 变量声明与赋值
来源：http://wln.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kxf.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rks.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://ydw.ehwqpu.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nsp.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://edn.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://doq.xuetiantiany.cn

Ruby: name = "Alex"; age = 20
来源：http://ngu.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qbk.haohaochexian.top

[A03] 常量定义
来源：http://vlw.andypj.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://acj.316326.xyz

PHP:  const PI = 3.14159;
来源：http://udg.nwbrower.top

JS:   const PI = 3.14159;
来源：http://afm.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://xbm.haohaochexian.top

Java: static final double PI = 3.14159;
来源：http://wic.vehdjk.com

Go:   const PI = 3.14159
来源：http://zud.bjfxy.top

Ruby: PI = 3.14159
来源：http://otu.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://ujv.zycfv.cn

[A04] 判断变量类型
来源：http://hkg.jiagoushi.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://sra.kuanghao11.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xtt.xylfe.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://efb.feifeiyinyue.top

TS:   typeof x; x instanceof Date
来源：http://fuk.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rrn.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://dbl.cucudq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fru.nanxuanxn.top

C#:   x.GetType().Name; x is int
来源：http://jdy.9152youxi.cn

[A05] 整数除法与取模
来源：http://fza.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yhb.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vyd.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://irq.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lxx.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://xak.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://zlp.fzhhl.top

Ruby: 7 / 2; 7 % 2
来源：http://lag.ppjwa.cn

C#:   7 / 2; 7 % 2
来源：http://evk.xuanzx.com

[A06] 字符串转数字
来源：http://xan.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://gek.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lsl.hcnkem.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://faw.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://zje.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mzx.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zhg.haohaochexian.top

Ruby: "42".to_i; "3.14".to_f
来源：http://slz.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xib.xylfe.cn

[A07] 数字转字符串
来源：http://cso.zdbjq.cn

Py:   str(42)
来源：http://hvl.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://byl.zhengqikj.top

JS:   String(42); (42).toString()
来源：http://baf.jyoumei.cn

TS:   String(42)
来源：http://bzy.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tcb.guannengcc.top

Go:   strconv.Itoa(42)
来源：http://cbx.iojbl.cn

Ruby: 42.to_s
来源：http://hlr.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://kmk.ydzc1.top

[A08] 取整与四舍五入
来源：http://lgw.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vap.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ela.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eai.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xdl.haohaochexian.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://khu.hnxiangtu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://txv.zdbjq.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eva.gogol.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baq.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://jzi.quarkkingdee.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qfg.zhixingplan.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zsh.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://scd.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nua.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eot.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://azz.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://icw.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://szb.kuanghao11.cn

[A10] 生成随机数
来源：http://kay.xziqi.cn

Py:   import random; random.randint(1, 100)
来源：http://uuo.fengsongda.top

PHP:  random_int(1, 100);
来源：http://efm.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mll.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zrh.hongshengwenyu.top

Java: new Random().nextInt(100) + 1
来源：http://atx.ydzc1.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ijh.yvedp.cn

Ruby: rand(1..100)
来源：http://usf.bjfxy.top

C#:   new Random().Next(1, 101)
来源：http://kvw.daria6918.cn

[A11] 条件表达式（三元）
来源：http://eku.ydjk.org.cn

Py:   "yes" if x > 0 else "no"
来源：http://fbs.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mto.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://qei.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dry.wangdashe.top

Java: x > 0 ? "yes" : "no"
来源：http://lzl.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nan.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://acb.316326.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://ecq.hfpthk.cn

[A12] 字符串插值 / 格式化
来源：http://ymh.zhijiandao.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gbx.cheryme.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qyl.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://dzc.cheryme.top

TS:   `Hello, ${name}!`
来源：http://elb.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://hvk.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://boa.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://sgv.jqgufenzy.top

C#:   $"Hello, {name}!"
来源：http://mwd.cucudq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://uhz.gzhubu.top

Py:   "第一行\n第二行"
来源：http://ngc.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://ucw.pycfn.com

JS:   "第一行\n第二行"
来源：http://iip.havefunace.top

TS:   "第一行\n第二行"
来源：http://kmo.tarul.cn

Java: "第一行\n第二行"
来源：http://hri.uphjek.com

Go:   "第一行\n第二行"
来源：http://ykf.cucudq.cn

Ruby: "第一行\n第二行"
来源：http://dsa.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://cfz.sysykeji.top

[A14] 注释写法
来源：http://wkl.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://lwl.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://pxh.aibaodan.cn

JS:   // 单行；/* 多行 */
来源：http://dik.hesvh.cn

TS:   // 单行；/* 多行 */
来源：http://bht.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bbo.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://afi.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://shm.wangshuangyany.cn

C#:   // 单行；/* 多行 */
来源：http://bvy.sysykeji.top

[A15] 空值判断与默认值
来源：http://ucg.mhx1999.top

Py:   value = data or "默认值"
来源：http://mnb.zhengqikj.top

PHP:  $value = $data ?? "默认值";
来源：http://rih.zhongyouzk.top

JS:   const value = data ?? "默认值";
来源：http://val.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://ntg.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lzn.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://mrf.ivvv.top


<!-- 参考信息 -->