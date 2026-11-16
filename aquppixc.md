代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://but.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://onb.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://mpm.bjfxy.top

module.exports = { a };  const { a } = require("./m");
来源：http://wlw.ydjk.org.cn

[U85] JS：可选链
来源：http://bex.wangshuangyany.cn

a?.b?.c
来源：http://ryt.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://mjk.pycfn.com

a ?? b
来源：http://eak.yfazqb.com

[U87] JS：解构默认值
来源：http://lcg.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://oqj.yueranfly.top

[U88] JS：对象展开合并
来源：http://oxf.havefunace.top

{ ...a, ...b }
来源：http://vgw.sysykeji.top

[U89] JS：数组去重
来源：http://rgu.shzxlz.cn

[...new Set(arr)]
来源：http://ura.ivvv.top

[U90] JS：数字数组排序
来源：http://uxn.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://kej.fehbvm.com

[U91] JS：对象键值遍历
来源：http://mjx.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vvw.chenzaomai.com

[U92] JS：深拷贝
来源：http://yvt.ydjk.org.cn

structuredClone(obj)
来源：http://dtj.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://idm.jianghu66.top

`共 ${n} 条`
来源：http://rtm.zdqjudy.top

[U94] JS：箭头函数
来源：http://tdc.mhx1999.top

const double = x => x * 2;
来源：http://wus.ppjwa.cn

[U95] JS：Promise 包装
来源：http://jel.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://jcw.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://fcs.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xbx.kuanghao11.cn

[U97] JS：并发请求
来源：http://eud.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qca.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://txj.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pdf.tianlin.xyz

[U99] JS：事件监听
来源：http://agb.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://yaj.chenlongwang.top

[U100] JS：DOM 查询
来源：http://zpu.yuxming.cn

document.querySelector(".item")
来源：http://ghj.shzxlz.cn

[U101] JS：classList 操作
来源：http://gdo.aizwys.cn

el.classList.toggle("active")
来源：http://tgt.yangfankeji.com

[U102] JS：本地存储
来源：http://lip.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gso.cdnleiting.top

[U103] JS：定时器
来源：http://ocj.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xgn.yuanzhike.top

[U104] JS：防抖
来源：http://mzn.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://shq.fanxiaobao.xyz

[U105] JS：节流
来源：http://elj.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://efe.gaohongyu789.top

[U106] JS：日期格式化
来源：http://oll.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bdq.yj202588.top

[U107] JS：数字千分位
来源：http://qyr.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://onc.yj202588.top

[U108] JS：随机整数
来源：http://vtt.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jtp.hammf.cn

[U109] JS：数组分组
来源：http://skz.epnwcf.com

Object.groupBy(arr, x => x.type)
来源：http://dyd.nwbrower.top

[U110] JS：数组分块
来源：http://mlw.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qlk.xylfe.cn

[U111] JS：对象转 Map
来源：http://qcj.zycfv.cn

new Map(Object.entries(obj))
来源：http://zef.yanxiufei.cn

[U112] JS：字符串补位
来源：http://ehp.chenlongwang.top

"7".padStart(3, "0")
来源：http://iny.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://gcr.yfazqb.com

s.replaceAll("a", "b")
来源：http://xil.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://ugk.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://frp.316326.xyz

[U115] JS：生成 UUID
来源：http://jpm.ydzc1.top

crypto.randomUUID()
来源：http://izz.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://pol.ppjwa.cn

/** @param {string} name */ function f(name) {}
来源：http://ncm.hammf.cn

[U117] JS：单元测试
来源：http://ygs.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://kkh.fehbvm.com

[U118] JS：开发服务器
来源：http://ktp.zdqjudy.top

npm i -D vite;  npx vite
来源：http://qod.haohaochexian.top

[U119] JS：生产构建
来源：http://cuf.jinyuanbaomall.cn

npx vite build
来源：http://scj.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://dsb.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://lud.cashguo.top

================================================================================
来源：http://wjw.tarul.cn

统计汇总
来源：http://maw.iojbl.cn

================================================================================
来源：http://ufi.gotoacloud.top

按语言统计（条）：
来源：http://oja.hesvh.cn

Python ......... 252
来源：http://jck.bbcook.cn

PHP ............ 252
来源：http://ozd.kuanghao11.cn

JavaScript ..... 252
来源：http://est.aibaodan.cn

TypeScript ..... 212
来源：http://aim.daxiang520.top

Java ........... 212
来源：http://djo.yuxming.cn

Go ............. 212
来源：http://pir.zhoulong.xyz

Ruby ........... 212
来源：http://fuw.sxryk.cn

C# ............. 212
来源：http://ing.xinyue.icu

C .............. 30
来源：http://evo.daria6918.cn

C++ ............ 30
来源：http://aob.fktsv.cn

SQL ............ 90
来源：http://ofd.yj202588.top

Bash ........... 80
来源：http://ebc.shangyingyoupin.top

Kotlin ......... 15
来源：http://bvr.yfazqb.com

Swift .......... 15
来源：http://mdy.shangyingyoupin.top

Lua ............ 10
来源：http://apw.vehdjk.com

Perl ........... 10
来源：http://fis.chenlongwang.top

Scala .......... 10
来源：http://rvd.guowangkeji.top

------------------------------------
来源：http://leo.xingfuxueyuan.xyz

合计 ........... 2106 条
来源：http://loj.shzxlz.cn

按章节统计：
来源：http://mhg.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fit.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yib.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lzv.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vin.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fll.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rvu.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jvv.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mpx.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rri.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bxa.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ffj.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://irf.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kek.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yxe.gzhubu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bpt.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pur.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://hlt.nanxinkj.top

R Bash 专题                             80
来源：http://pyp.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://qjy.hcnkem.com

T 其他语言补充                          60
来源：http://sky.bjfxy.top

U 高频实用片段                         120
来源：http://oot.jinqigufen.top

------------------------------------
来源：http://cao.jiagoushi.top

合计                                  2106 条
来源：http://keg.hcnkem.com

--------------------------------------------------------------------------------
来源：http://qsn.chenzaomai.com

使用提醒
来源：http://snh.yj20258.top

--------------------------------------------------------------------------------
来源：http://yti.xziqi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rgs.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qto.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wpn.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://umq.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kky.hesvh.cn

—— 文件结束 ——
来源：http://yfo.ehwqpu.com

================================================================================
来源：http://wuj.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://tzl.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://mwg.yuanzhike.top

================================================================================
来源：http://jcu.cheryme.top

【收录内容】
来源：http://vvb.yfazqb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://iyw.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uug.sysykeji.top

SQL · Bash · C · C++
来源：http://ckq.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wym.zdbjq.cn

【使用说明】
来源：http://bbe.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yja.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://imv.nanxinkj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://htr.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kkw.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iog.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://akn.zhijiandao.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://msv.andypj.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iqe.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yhq.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cfv.hesvh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pcp.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jay.feifeiyinyue.top

【文件统计】
来源：http://nha.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cgi.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://ykn.bbcook.cn

目  录
来源：http://ymn.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://kab.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pcy.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tun.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kig.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wrm.vqdsnc.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vmr.kuanghao11.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://svf.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ryv.xylfe.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iog.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://odr.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://flo.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lgj.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eho.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pws.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iee.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kbf.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eft.gaohongyu789.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ylq.wangshuangyany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xmv.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jct.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vgo.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vzf.nanxuanxn.top

================================================================================
来源：http://xth.quarkkingdee.top

A. 基础语法与类型
来源：http://vmh.hysaishi.cn

================================================================================
来源：http://ioi.fehbvm.com

[A01] Hello World
来源：http://sva.uphjek.com

Py:   print("Hello, World!")
来源：http://kbu.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://hpx.ydjk.org.cn

JS:   console.log("Hello, World!");
来源：http://zkp.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xwp.hesvh.cn

Java: System.out.println("Hello, World!");
来源：http://fws.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://bcl.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://nnr.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kma.chenzaomai.com

[A02] 变量声明与赋值
来源：http://hqm.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mqp.jinyuanbaomall.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ico.ydzc1.top

JS:   let name = "Alex"; const age = 20;
来源：http://num.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gsp.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://oib.gogol.net.cn

Go:   name := "Alex"; age := 20
来源：http://lti.xuetiantiany.cn

Ruby: name = "Alex"; age = 20
来源：http://nky.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://hds.zhoulong.xyz

[A03] 常量定义
来源：http://ydj.shanyushiyangtech.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fer.sjlbkw.cn

PHP:  const PI = 3.14159;
来源：http://qig.zhaomingkeji.xyz

JS:   const PI = 3.14159;
来源：http://rvh.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://cbz.fktsv.cn

Java: static final double PI = 3.14159;
来源：http://jpb.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://lit.xziqi.cn

Ruby: PI = 3.14159
来源：http://uev.jyoumei.cn

C#:   const double PI = 3.14159;
来源：http://rqm.zhiwuduotai.top

[A04] 判断变量类型
来源：http://gzt.aibaodan.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wkn.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jta.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yne.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://cdn.jinyuanbaomall.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://awz.redwolf501.top

Go:   reflect.TypeOf(x).Name()
来源：http://wyl.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cjl.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://exo.cheryme.top

[A05] 整数除法与取模
来源：http://lzb.hfpthk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jns.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xdj.hammf.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vtd.hammf.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xlv.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://aip.sufxvd.cn

Go:   7 / 2; 7 % 2
来源：http://glp.svipenyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ovm.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://otd.pengpengdd.cyou

[A06] 字符串转数字
来源：http://tbz.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://pva.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bat.daria6918.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nay.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://puq.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lgn.jinqigufen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iks.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fgs.chenlongwang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bke.shanyushiyangtech.top

[A07] 数字转字符串
来源：http://nbs.dianchejie.cn

Py:   str(42)
来源：http://bsg.jqgfzy.top

PHP:  (string) 42; strval(42)
来源：http://nvw.52xcode.cn

JS:   String(42); (42).toString()
来源：http://amt.jqgfzy.top

TS:   String(42)
来源：http://rid.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://dsn.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://jfc.chenzaomai.com

Ruby: 42.to_s
来源：http://mjh.ctjpmb.com

C#:   42.ToString()
来源：http://rus.cdnleiting.top

[A08] 取整与四舍五入
来源：http://ore.jyoumei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fnz.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ixz.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ghs.jinyuanbaomall.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vko.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gms.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pub.9152youxi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://whl.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cbf.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://dnt.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xyj.hesvh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zwk.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qsk.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rxi.zhengqikj.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://egp.hcnkem.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pul.shanyushiyangtech.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dir.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://upw.hongshengwenyu.top

[A10] 生成随机数
来源：http://rpu.dianchejie.cn

Py:   import random; random.randint(1, 100)
来源：http://zot.jinghuilouyu.cn

PHP:  random_int(1, 100);
来源：http://ric.zhaomingkeji.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nmg.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xba.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://rpw.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vcw.0kj1m.cn

Ruby: rand(1..100)
来源：http://njc.yj202588.top

C#:   new Random().Next(1, 101)
来源：http://ucj.yj202588.top

[A11] 条件表达式（三元）
来源：http://oqm.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://wgc.nanxuanxn.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yqd.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dxy.nanxinkj.top

TS:   x > 0 ? "yes" : "no"
来源：http://wnn.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://hin.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jgm.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://njp.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://pko.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://lmn.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pre.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vpa.yj202588.top

JS:   `Hello, ${name}!`
来源：http://mji.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://got.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://aox.zdqjudy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://oqk.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://mve.bjfxy.top

C#:   $"Hello, {name}!"
来源：http://hio.nanxinkj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://aup.redwolf501.top

Py:   "第一行\n第二行"
来源：http://ltl.nanxuanxn.top

PHP:  "第一行\n第二行"
来源：http://gkd.tarul.cn

JS:   "第一行\n第二行"
来源：http://rqr.daria6918.cn

TS:   "第一行\n第二行"
来源：http://oeh.guannengcc.top

Java: "第一行\n第二行"
来源：http://jok.xuetiantiany.cn

Go:   "第一行\n第二行"
来源：http://yxw.ehwqpu.com

Ruby: "第一行\n第二行"
来源：http://zlq.fktsv.cn

C#:   "第一行\n第二行"
来源：http://vhi.meibo888.top


<!-- 参考信息 -->