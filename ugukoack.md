代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hoq.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lvx.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://xwz.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qad.zhijiandao.cn

[U85] JS：可选链
来源：http://kst.fengsongda.top

a?.b?.c
来源：http://zma.epnwcf.com

[U86] JS：空值合并
来源：http://jxk.nanxinkj.top

a ?? b
来源：http://zqo.fktsv.cn

[U87] JS：解构默认值
来源：http://ztk.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://tqb.nwbrower.top

[U88] JS：对象展开合并
来源：http://bey.tian-w.cn

{ ...a, ...b }
来源：http://vlz.jinqigfzy.top

[U89] JS：数组去重
来源：http://pcb.yonumen.top

[...new Set(arr)]
来源：http://eih.cdnleiting.top

[U90] JS：数字数组排序
来源：http://rql.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://jdq.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://ssk.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yqx.52xcode.cn

[U92] JS：深拷贝
来源：http://jia.zhongyouzk.top

structuredClone(obj)
来源：http://pxv.andypj.xyz

[U93] JS：模板字符串
来源：http://tfm.ehwqpu.com

`共 ${n} 条`
来源：http://oey.xinyue.icu

[U94] JS：箭头函数
来源：http://lkt.tanke756.top

const double = x => x * 2;
来源：http://ahs.ctjpmb.com

[U95] JS：Promise 包装
来源：http://let.meibo888.top

new Promise((resolve, reject) => {})
来源：http://thj.ydzc1.top

[U96] JS：async/await 与异常
来源：http://ycl.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://awv.zycfv.cn

[U97] JS：并发请求
来源：http://qfe.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://die.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://mjt.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vdh.vehdjk.com

[U99] JS：事件监听
来源：http://noh.smart0.xyz

el.addEventListener("click", e => {})
来源：http://enh.hnqzz.top

[U100] JS：DOM 查询
来源：http://clp.cqqwz.cn

document.querySelector(".item")
来源：http://nrl.sweek.top

[U101] JS：classList 操作
来源：http://myo.ydzc1.top

el.classList.toggle("active")
来源：http://qit.0kj1m.cn

[U102] JS：本地存储
来源：http://akf.xinyue.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://fub.pycfn.com

[U103] JS：定时器
来源：http://pqm.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xsi.jinghuilouyu.cn

[U104] JS：防抖
来源：http://ysd.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sap.hammf.cn

[U105] JS：节流
来源：http://xrv.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rai.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://nsp.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pbj.tianlin.xyz

[U107] JS：数字千分位
来源：http://nbs.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ccn.shuidangran.top

[U108] JS：随机整数
来源：http://men.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bhq.fehbvm.com

[U109] JS：数组分组
来源：http://hyf.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://mpf.nwbrower.top

[U110] JS：数组分块
来源：http://mml.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dub.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://jrm.hcnkem.com

new Map(Object.entries(obj))
来源：http://nut.yuxming.cn

[U112] JS：字符串补位
来源：http://grm.dianchejie.cn

"7".padStart(3, "0")
来源：http://vke.xuanzx.com

[U113] JS：正则替换全部
来源：http://ukw.cucudq.cn

s.replaceAll("a", "b")
来源：http://dig.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://jze.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zsh.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://oph.hesvh.cn

crypto.randomUUID()
来源：http://ywf.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://xne.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://rll.meibo888.top

[U117] JS：单元测试
来源：http://bvo.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://lid.zhongyouzk.top

[U118] JS：开发服务器
来源：http://suf.ehwqpu.com

npm i -D vite;  npx vite
来源：http://kkh.cqqwz.cn

[U119] JS：生产构建
来源：http://ajj.quarkkingdee.top

npx vite build
来源：http://uuq.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://uhl.hnxiangtu.top

import.meta.env.VITE_API_URL
来源：http://suo.316326.xyz

================================================================================
来源：http://zuy.chenzaomai.com

统计汇总
来源：http://zfo.hywenlv.cn

================================================================================
来源：http://ley.jinyuanbaomall.cn

按语言统计（条）：
来源：http://xms.epnwcf.com

Python ......... 252
来源：http://lvb.meibo888.top

PHP ............ 252
来源：http://cno.dianchejie.cn

JavaScript ..... 252
来源：http://hqm.zhoulong.xyz

TypeScript ..... 212
来源：http://tbt.sjlbkw.cn

Java ........... 212
来源：http://wxp.smart0.xyz

Go ............. 212
来源：http://vik.zycfv.cn

Ruby ........... 212
来源：http://edd.hywenlv.cn

C# ............. 212
来源：http://xli.cheryme.top

C .............. 30
来源：http://vyh.daria6918.cn

C++ ............ 30
来源：http://xfs.xziqi.cn

SQL ............ 90
来源：http://gki.ydjk.org.cn

Bash ........... 80
来源：http://ogx.ppjwa.cn

Kotlin ......... 15
来源：http://zdo.fanxiaobao.xyz

Swift .......... 15
来源：http://pep.jinqigfzy.top

Lua ............ 10
来源：http://cra.pengpengdd.cyou

Perl ........... 10
来源：http://svv.redwolf501.top

Scala .......... 10
来源：http://gaw.svipenyu.cn

------------------------------------
来源：http://und.sxryk.cn

合计 ........... 2106 条
来源：http://ehn.ybcxt.top

按章节统计：
来源：http://mng.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jfh.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://syt.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jrx.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qhl.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qsc.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://byf.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dvi.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ofk.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aud.0kj1m.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jlf.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xiq.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gth.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zyj.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uig.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vfm.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gsr.yvedp.cn

Q SQL 专题                              90
来源：http://nod.mhx1999.top

R Bash 专题                             80
来源：http://whr.fzhhl.top

S C / C++ 专题                          60
来源：http://ujt.316326.xyz

T 其他语言补充                          60
来源：http://owp.ivvv.top

U 高频实用片段                         120
来源：http://dgy.hysaishi.cn

------------------------------------
来源：http://eqf.hesvh.cn

合计                                  2106 条
来源：http://dgl.tian-w.cn

--------------------------------------------------------------------------------
来源：http://zqh.shuidangran.top

使用提醒
来源：http://sqb.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://elb.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wwq.jqgufenzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kxt.tarul.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gic.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lyw.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lit.guannengcc.top

—— 文件结束 ——
来源：http://hss.jinqigufen.top

================================================================================
来源：http://imp.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://irl.52xcode.cn

Common Programming Examples Cheat Book
来源：http://xtv.fzhhl.top

================================================================================
来源：http://tiz.shzxlz.cn

【收录内容】
来源：http://boc.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tvl.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jxe.zhengqikj.top

SQL · Bash · C · C++
来源：http://eni.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ldi.tian-w.cn

【使用说明】
来源：http://gmp.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aib.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xvn.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rqy.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://abi.jianghu66.top

Bash:  Shell         C:     C             C++:   C++
来源：http://iqo.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://onb.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cyh.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nyj.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jml.kuanghao11.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mgg.cashguo.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://txs.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ihi.zhiwuduotai.top

【文件统计】
来源：http://nai.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jvg.yvedp.cn

--------------------------------------------------------------------------------
来源：http://cih.zdbjq.cn

目  录
来源：http://weg.hcnkem.com

--------------------------------------------------------------------------------
来源：http://cfh.andypj.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mvq.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zep.aibaodan.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vzg.sysykeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nww.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qog.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pfe.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ymt.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lko.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tox.ivvv.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wtz.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rit.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ynb.guannengcc.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://brj.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://awd.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ieg.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qcv.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uiw.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wit.kuanghao11.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jgx.fanxiaobao.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://thx.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mnf.cucudq.cn

================================================================================
来源：http://lzs.xuetiantiany.cn

A. 基础语法与类型
来源：http://ria.yonumen.top

================================================================================
来源：http://akb.wangdashe.top

[A01] Hello World
来源：http://nus.zycfv.cn

Py:   print("Hello, World!")
来源：http://rph.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://pki.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://xut.hnqzz.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vkq.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://rgu.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://xzu.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://byi.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fjq.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://akq.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vph.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xig.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wqe.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kwg.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://kan.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://qxu.ywan-chungtsiang.top

Ruby: name = "Alex"; age = 20
来源：http://asb.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://fhl.vehdjk.com

[A03] 常量定义
来源：http://fwf.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hnl.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://opb.xingfuxueyuan.xyz

JS:   const PI = 3.14159;
来源：http://scy.zdbjq.cn

TS:   const PI: number = 3.14159;
来源：http://lag.ybcxt.top

Java: static final double PI = 3.14159;
来源：http://cmo.c1oappe.top

Go:   const PI = 3.14159
来源：http://zvv.shzxlz.cn

Ruby: PI = 3.14159
来源：http://uan.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://mfu.zdbjq.cn

[A04] 判断变量类型
来源：http://cga.svipenyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ilp.hongshengwenyu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eix.0kj1m.cn

TS:   typeof x; x instanceof Date
来源：http://vfs.fengsongda.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pjg.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vbz.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cls.dianchejie.cn

C#:   x.GetType().Name; x is int
来源：http://ksy.hywenlv.cn

[A05] 整数除法与取模
来源：http://mzf.chenjidiqi.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vhl.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hlg.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gmu.havefunace.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yte.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://dlp.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://lpu.chenjidiqi.icu

Ruby: 7 / 2; 7 % 2
来源：http://pnu.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://rgn.jinyuanbaomall.cn

[A06] 字符串转数字
来源：http://ffh.tanke756.top

Py:   int("42"); float("3.14")
来源：http://gat.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bzr.yanxiufei.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yxh.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://gen.birdmap.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ngr.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bea.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dgo.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ity.yanxiufei.cn

[A07] 数字转字符串
来源：http://xsn.hfpthk.cn

Py:   str(42)
来源：http://isp.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://cdu.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://khz.shuidangran.top

TS:   String(42)
来源：http://mve.hcnkem.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://rve.chenlongwang.top

Go:   strconv.Itoa(42)
来源：http://bqa.nanxinkj.top

Ruby: 42.to_s
来源：http://khu.shanyushiyangtech.top

C#:   42.ToString()
来源：http://koy.pycfn.com

[A08] 取整与四舍五入
来源：http://tpj.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://soz.zdqjudy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xfj.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mww.zhongyouzk.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sev.gogol.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xwy.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ayy.ctjpmb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://yko.yuanzhike.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zob.cdnleiting.top

[A09] 绝对值与最大最小值
来源：http://cad.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eqi.gzhubu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://udi.gaohongyu789.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gvk.nanxinkj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oyy.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gvj.xziqi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qvk.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xct.hongshengwenyu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jrs.kuanghao11.cn

[A10] 生成随机数
来源：http://mry.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://dio.birdmap.top

PHP:  random_int(1, 100);
来源：http://qrb.birdmap.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://egl.daxiang520.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nhr.tianlin.xyz

Java: new Random().nextInt(100) + 1
来源：http://npe.zhiwuduotai.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jup.yuanzhike.top

Ruby: rand(1..100)
来源：http://yvs.dianchejie.cn

C#:   new Random().Next(1, 101)
来源：http://nch.yongpay.top

[A11] 条件表达式（三元）
来源：http://ivp.feifeiyinyue.top

Py:   "yes" if x > 0 else "no"
来源：http://wpa.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qcc.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://dse.jinqigfzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://inh.zycfv.cn

Java: x > 0 ? "yes" : "no"
来源：http://oqy.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hmi.guowangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://oiz.zhijiandao.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xoh.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://cgk.cqqwz.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rbr.kuanghao11.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vcb.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://piv.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://dql.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://kzm.nanxinkj.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lya.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://obw.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://jvk.zhengqikj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://iyk.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://bqs.zhoulong.xyz

PHP:  "第一行\n第二行"
来源：http://upu.zhoulong.xyz

JS:   "第一行\n第二行"
来源：http://wxu.smart0.xyz

TS:   "第一行\n第二行"
来源：http://whq.yfazqb.com

Java: "第一行\n第二行"
来源：http://vcl.shuidangran.top

Go:   "第一行\n第二行"
来源：http://vqz.birdmap.top

Ruby: "第一行\n第二行"
来源：http://wsx.ywan-chungtsiang.top

C#:   "第一行\n第二行"
来源：http://ess.cucudq.cn


<!-- 参考信息 -->