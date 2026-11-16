代发 wailian999

[U85] JS：可选链
来源：http://fke.ybcxt.top

a?.b?.c
来源：http://jjn.cheryme.top

[U86] JS：空值合并
来源：http://cpd.jinqigfzy.top

a ?? b
来源：http://ntj.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://xpy.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://tve.redwolf501.top

[U88] JS：对象展开合并
来源：http://sfs.uphjek.com

{ ...a, ...b }
来源：http://ltk.wangshuangyany.cn

[U89] JS：数组去重
来源：http://dli.xinyue.icu

[...new Set(arr)]
来源：http://ljy.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://foi.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://maj.yueranfly.top

[U91] JS：对象键值遍历
来源：http://uvk.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ywi.guowangkeji.top

[U92] JS：深拷贝
来源：http://xxv.dianchejie.cn

structuredClone(obj)
来源：http://rza.chenzaomai.com

[U93] JS：模板字符串
来源：http://sgo.nwbrower.top

`共 ${n} 条`
来源：http://fcg.316326.xyz

[U94] JS：箭头函数
来源：http://rdv.gotoacloud.top

const double = x => x * 2;
来源：http://qsb.jqgfzy.top

[U95] JS：Promise 包装
来源：http://nmu.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://liy.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://fee.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kbo.chenlongwang.top

[U97] JS：并发请求
来源：http://plz.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dor.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://srg.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rvl.xinyue.icu

[U99] JS：事件监听
来源：http://zoy.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://dhv.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://ejy.gaohongyu789.top

document.querySelector(".item")
来源：http://gzx.cheryme.top

[U101] JS：classList 操作
来源：http://zhd.hnxiangtu.top

el.classList.toggle("active")
来源：http://wue.yuanzhike.top

[U102] JS：本地存储
来源：http://uni.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iud.zhoulong.xyz

[U103] JS：定时器
来源：http://mrm.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hmx.jiagoushi.top

[U104] JS：防抖
来源：http://wmn.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xfr.redwolf501.top

[U105] JS：节流
来源：http://zlq.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yln.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://hhj.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zpb.hywenlv.cn

[U107] JS：数字千分位
来源：http://xzb.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xlu.9152youxi.cn

[U108] JS：随机整数
来源：http://pqu.tarul.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tmu.tarul.cn

[U109] JS：数组分组
来源：http://uvq.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://onj.yuanzhike.top

[U110] JS：数组分块
来源：http://lsh.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xqn.shzxlz.cn

[U111] JS：对象转 Map
来源：http://noi.tarul.cn

new Map(Object.entries(obj))
来源：http://thm.jinqigfzy.top

[U112] JS：字符串补位
来源：http://iki.shuidangran.top

"7".padStart(3, "0")
来源：http://nrr.svipenyu.cn

[U113] JS：正则替换全部
来源：http://gme.tanke756.top

s.replaceAll("a", "b")
来源：http://jhj.yj202588.top

[U114] JS：JSON 深比较
来源：http://vxm.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://bzq.hysaishi.cn

[U115] JS：生成 UUID
来源：http://die.sufxvd.cn

crypto.randomUUID()
来源：http://jfn.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://wrd.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://bny.snrcjt.cn

[U117] JS：单元测试
来源：http://fto.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://lcv.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://tnr.dashuyun.cn

npm i -D vite;  npx vite
来源：http://pqe.sysykeji.top

[U119] JS：生产构建
来源：http://xwf.haohaochexian.top

npx vite build
来源：http://qcg.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://qgu.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://xju.pycfn.com

================================================================================
来源：http://kja.yangfankeji.com

统计汇总
来源：http://dyz.pycfn.com

================================================================================
来源：http://xtx.fengsongda.top

按语言统计（条）：
来源：http://wsy.andypj.xyz

Python ......... 252
来源：http://psi.bbcook.cn

PHP ............ 252
来源：http://hfo.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://kbq.chenjidiqi.icu

TypeScript ..... 212
来源：http://sep.xuetiantiany.cn

Java ........... 212
来源：http://txn.gotoacloud.top

Go ............. 212
来源：http://esr.sufxvd.cn

Ruby ........... 212
来源：http://lrj.hongshengwenyu.top

C# ............. 212
来源：http://bwy.tanke756.top

C .............. 30
来源：http://tnz.epnwcf.com

C++ ............ 30
来源：http://eth.cdnleiting.top

SQL ............ 90
来源：http://ooy.birdmap.top

Bash ........... 80
来源：http://whh.guannengcc.top

Kotlin ......... 15
来源：http://nnv.chenjidiqi.icu

Swift .......... 15
来源：http://vqs.quarkkingdee.top

Lua ............ 10
来源：http://wjq.nanxuanxn.top

Perl ........... 10
来源：http://kvl.zycfv.cn

Scala .......... 10
来源：http://vws.shzxlz.cn

------------------------------------
来源：http://mxh.jinqigfzy.top

合计 ........... 2106 条
来源：http://gxi.tian-w.cn

按章节统计：
来源：http://mkz.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iqi.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://njg.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ajr.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gap.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wzk.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nlt.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fye.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ukc.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://svi.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vqy.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qwv.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fxl.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ena.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hgn.sxryk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bzo.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://prv.xinyue.icu

Q SQL 专题                              90
来源：http://uee.zhengqikj.top

R Bash 专题                             80
来源：http://chl.fzhhl.top

S C / C++ 专题                          60
来源：http://yaj.cheryme.top

T 其他语言补充                          60
来源：http://eoh.jinqigufen.top

U 高频实用片段                         120
来源：http://yym.gogol.net.cn

------------------------------------
来源：http://grm.vehdjk.com

合计                                  2106 条
来源：http://bsc.yonumen.top

--------------------------------------------------------------------------------
来源：http://omq.jinyuanbaomall.cn

使用提醒
来源：http://lpa.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://fbc.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sor.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ypf.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iku.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uuu.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wmf.andypj.xyz

—— 文件结束 ——
来源：http://aav.yuxming.cn

================================================================================
来源：http://rjt.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://khk.hongshengwenyu.top

Common Programming Examples Cheat Book
来源：http://sib.chenzaomai.com

================================================================================
来源：http://qzj.nanxuanxn.top

【收录内容】
来源：http://trl.hfpthk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tqi.dashuyun.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tca.yangfankeji.com

SQL · Bash · C · C++
来源：http://cfi.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lhc.cqqwz.cn

【使用说明】
来源：http://yhn.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eqy.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mpa.zdbjq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jcg.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://igo.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://gmb.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qeo.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wwu.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lvd.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wor.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xgg.uphjek.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ohl.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vbe.birdmap.top

【文件统计】
来源：http://ufn.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gkw.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://upq.bjfxy.top

目  录
来源：http://bbz.yj20258.top

--------------------------------------------------------------------------------
来源：http://zps.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ekt.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nyp.316326.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pic.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zti.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lay.xuanzx.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xgq.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gyb.yj202588.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eyy.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zeg.fengsongda.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://adu.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rwf.sufxvd.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ifx.tian-w.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iam.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uqc.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://diq.ctjpmb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fbx.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jfl.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ffg.ivvv.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qen.zycfv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eof.wangdashe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ngf.yj202588.top

================================================================================
来源：http://yhh.sweek.top

A. 基础语法与类型
来源：http://sia.ehwqpu.com

================================================================================
来源：http://stu.chenzaomai.com

[A01] Hello World
来源：http://vel.epnwcf.com

Py:   print("Hello, World!")
来源：http://lfe.guowangkeji.top

PHP:  echo "Hello, World!";
来源：http://qxe.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://exe.hfpthk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gqq.hysaishi.cn

Java: System.out.println("Hello, World!");
来源：http://fcx.dashuyun.cn

Go:   fmt.Println("Hello, World!")
来源：http://kxx.haohaochexian.top

Ruby: puts "Hello, World!"
来源：http://tmt.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rcy.vehdjk.com

[A02] 变量声明与赋值
来源：http://qhx.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qbj.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://oax.cqqwz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://spg.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fgu.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://fby.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://xjr.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://wdw.zhijiandao.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vyy.smart0.xyz

[A03] 常量定义
来源：http://sbo.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oht.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://dag.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://apq.zhijiandao.cn

TS:   const PI: number = 3.14159;
来源：http://lzb.xingfuxueyuan.xyz

Java: static final double PI = 3.14159;
来源：http://fzs.chenjidiqi.icu

Go:   const PI = 3.14159
来源：http://wdy.andypj.xyz

Ruby: PI = 3.14159
来源：http://ctt.hywenlv.cn

C#:   const double PI = 3.14159;
来源：http://qzn.andypj.xyz

[A04] 判断变量类型
来源：http://uma.xinyue.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://suv.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lql.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fgd.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://bno.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wtt.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://bip.yfazqb.com

Ruby: x.class; x.is_a?(Integer)
来源：http://tqm.vqdsnc.cn

C#:   x.GetType().Name; x is int
来源：http://eva.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://vjp.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pjb.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lzx.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qcq.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mrl.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://ueu.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://btq.xuanzx.com

Ruby: 7 / 2; 7 % 2
来源：http://mze.cashguo.top

C#:   7 / 2; 7 % 2
来源：http://nyr.meibo888.top

[A06] 字符串转数字
来源：http://pqh.andypj.xyz

Py:   int("42"); float("3.14")
来源：http://bkh.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mqr.wangdashe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bss.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://aha.dashuyun.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dxv.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pvp.iojbl.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xlc.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://btu.fengsongda.top

[A07] 数字转字符串
来源：http://xle.aizwys.cn

Py:   str(42)
来源：http://oan.316326.xyz

PHP:  (string) 42; strval(42)
来源：http://jwa.guannengcc.top

JS:   String(42); (42).toString()
来源：http://udu.sweek.top

TS:   String(42)
来源：http://mpm.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ltz.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://hgv.sxryk.cn

Ruby: 42.to_s
来源：http://yfr.xuetiantiany.cn

C#:   42.ToString()
来源：http://fsl.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://tlz.hongshengwenyu.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://upf.kuanghao11.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wcd.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hjf.wangshuangyany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oie.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wpn.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qnz.chenjidiqi.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://snn.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vpy.cdnleiting.top

[A09] 绝对值与最大最小值
来源：http://bjm.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zxv.cdnleiting.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fua.ctjpmb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ecc.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ebm.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ctv.gzhubu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://onb.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://for.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lic.zdbjq.cn

[A10] 生成随机数
来源：http://eoi.nwbrower.top

Py:   import random; random.randint(1, 100)
来源：http://yac.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://aww.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://owi.chenzaomai.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pcb.yuxming.cn

Java: new Random().nextInt(100) + 1
来源：http://pdx.kuanghao11.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cav.gaohongyu789.top

Ruby: rand(1..100)
来源：http://cqx.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://qdt.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://nqa.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://hxw.hcnkem.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://hvu.feifeiyinyue.top

JS:   x > 0 ? "yes" : "no"
来源：http://wyt.yfazqb.com

TS:   x > 0 ? "yes" : "no"
来源：http://qqw.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://tpp.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bhh.aibaodan.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qgd.ppjwa.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rss.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://hof.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dcm.ydjk.org.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dqi.zdqjudy.top

JS:   `Hello, ${name}!`
来源：http://ktc.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://muu.mhx1999.top

Java: "Hello, %s!".formatted(name)
来源：http://xhe.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://glr.zhongyouzk.top

Ruby: "Hello, #{name}!"
来源：http://jmt.dashuyun.cn

C#:   $"Hello, {name}!"
来源：http://goh.kuanghao11.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eld.feifeiyinyue.top

Py:   "第一行\n第二行"
来源：http://pbs.tarul.cn

PHP:  "第一行\n第二行"
来源：http://tgy.ywan-chungtsiang.top

JS:   "第一行\n第二行"
来源：http://irm.yj202588.top

TS:   "第一行\n第二行"
来源：http://mta.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://kkg.yongpay.top

Go:   "第一行\n第二行"
来源：http://dfj.smart0.xyz

Ruby: "第一行\n第二行"
来源：http://wrs.tanke756.top

C#:   "第一行\n第二行"
来源：http://fhm.zhaomingkeji.xyz

[A14] 注释写法
来源：http://ukj.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bgt.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qcu.shangyingyoupin.top

JS:   // 单行；/* 多行 */
来源：http://jes.yj20258.top


<!-- 参考信息 -->