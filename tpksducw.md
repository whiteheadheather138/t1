代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://ndr.hammf.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mlb.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://dts.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://kgb.pengpengdd.cyou

[U85] JS：可选链
来源：http://dzg.cdnleiting.top

a?.b?.c
来源：http://fiy.cashguo.top

[U86] JS：空值合并
来源：http://jrp.guowangkeji.top

a ?? b
来源：http://rsk.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://kuj.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://tqa.jiagoushi.top

[U88] JS：对象展开合并
来源：http://fnv.tian-w.cn

{ ...a, ...b }
来源：http://ejx.9152youxi.cn

[U89] JS：数组去重
来源：http://xyu.shuidangran.top

[...new Set(arr)]
来源：http://zuw.gotoacloud.top

[U90] JS：数字数组排序
来源：http://tes.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://uxf.kuanghao11.cn

[U91] JS：对象键值遍历
来源：http://mjb.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ilc.gotoacloud.top

[U92] JS：深拷贝
来源：http://sow.ywan-chungtsiang.top

structuredClone(obj)
来源：http://poe.hammf.cn

[U93] JS：模板字符串
来源：http://yuk.hesvh.cn

`共 ${n} 条`
来源：http://cep.0kj1m.cn

[U94] JS：箭头函数
来源：http://qkw.fengsongda.top

const double = x => x * 2;
来源：http://mab.sufxvd.cn

[U95] JS：Promise 包装
来源：http://juo.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://uxj.shuidangran.top

[U96] JS：async/await 与异常
来源：http://jnb.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mby.ppjwa.cn

[U97] JS：并发请求
来源：http://knq.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tgf.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://txv.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vgx.smart0.xyz

[U99] JS：事件监听
来源：http://jsu.zhoulong.xyz

el.addEventListener("click", e => {})
来源：http://dvl.cucudq.cn

[U100] JS：DOM 查询
来源：http://tok.yuanzhike.top

document.querySelector(".item")
来源：http://fjy.bjfxy.top

[U101] JS：classList 操作
来源：http://act.guannengcc.top

el.classList.toggle("active")
来源：http://cxm.cqqwz.cn

[U102] JS：本地存储
来源：http://qyy.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bdb.hongshengwenyu.top

[U103] JS：定时器
来源：http://sbj.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wto.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://uwl.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bdv.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://aah.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fhw.aizwys.cn

[U106] JS：日期格式化
来源：http://eyu.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://prt.gogol.net.cn

[U107] JS：数字千分位
来源：http://bie.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://joa.mhx1999.top

[U108] JS：随机整数
来源：http://zvc.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lqx.zhongyouzk.top

[U109] JS：数组分组
来源：http://hdz.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://cyw.zdqjudy.top

[U110] JS：数组分块
来源：http://ovv.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xua.fktsv.cn

[U111] JS：对象转 Map
来源：http://dgn.fktsv.cn

new Map(Object.entries(obj))
来源：http://cqo.hesvh.cn

[U112] JS：字符串补位
来源：http://vsn.gotoacloud.top

"7".padStart(3, "0")
来源：http://pet.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://xcn.hysaishi.cn

s.replaceAll("a", "b")
来源：http://akh.aizwys.cn

[U114] JS：JSON 深比较
来源：http://nas.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wgt.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://kae.daxiang520.top

crypto.randomUUID()
来源：http://vkl.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://umw.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://mta.fehbvm.com

[U117] JS：单元测试
来源：http://zyu.ctjpmb.com

npm i -D vitest;  npx vitest
来源：http://omr.yfazqb.com

[U118] JS：开发服务器
来源：http://dfb.yj202588.top

npm i -D vite;  npx vite
来源：http://rjn.ppjwa.cn

[U119] JS：生产构建
来源：http://wud.9152youxi.cn

npx vite build
来源：http://yse.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://kvk.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://dch.redwolf501.top

================================================================================
来源：http://xhk.cashguo.top

统计汇总
来源：http://wsx.zycfv.cn

================================================================================
来源：http://rmv.svipenyu.cn

按语言统计（条）：
来源：http://rnx.zhixingplan.top

Python ......... 252
来源：http://irr.dashuyun.cn

PHP ............ 252
来源：http://jbz.sufxvd.cn

JavaScript ..... 252
来源：http://awt.redwolf501.top

TypeScript ..... 212
来源：http://ool.smart0.xyz

Java ........... 212
来源：http://bxs.sufxvd.cn

Go ............. 212
来源：http://ohs.xuanzx.com

Ruby ........... 212
来源：http://ljy.iojbl.cn

C# ............. 212
来源：http://zow.svipenyu.cn

C .............. 30
来源：http://mbb.xuetiantiany.cn

C++ ............ 30
来源：http://eoc.redwolf501.top

SQL ............ 90
来源：http://gft.xziqi.cn

Bash ........... 80
来源：http://clg.shzxlz.cn

Kotlin ......... 15
来源：http://gcd.chenzaomai.com

Swift .......... 15
来源：http://rrc.yanxiufei.cn

Lua ............ 10
来源：http://toi.sxryk.cn

Perl ........... 10
来源：http://wck.aizwys.cn

Scala .......... 10
来源：http://utn.xuetiantiany.cn

------------------------------------
来源：http://dwk.nanxuanxn.top

合计 ........... 2106 条
来源：http://nbb.sxryk.cn

按章节统计：
来源：http://wqb.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ntt.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hrh.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gji.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wgq.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dbb.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xqb.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vpi.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://era.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ahp.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gxd.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ted.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lkd.xuanzx.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vem.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gqe.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pfz.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gja.pengpengdd.cyou

Q SQL 专题                              90
来源：http://hdl.hnxiangtu.top

R Bash 专题                             80
来源：http://otg.sxryk.cn

S C / C++ 专题                          60
来源：http://vmv.yj20258.top

T 其他语言补充                          60
来源：http://ogw.wangshuangyany.cn

U 高频实用片段                         120
来源：http://pam.bjfxy.top

------------------------------------
来源：http://rkd.quarkkingdee.top

合计                                  2106 条
来源：http://xsa.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://bcp.chenjidiqi.icu

使用提醒
来源：http://wgh.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://xaa.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://erm.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tdv.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vnw.andypj.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://yfl.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ytz.cucudq.cn

—— 文件结束 ——
来源：http://qyd.hfpthk.cn

================================================================================
来源：http://rfd.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://ewu.316326.xyz

Common Programming Examples Cheat Book
来源：http://qnw.cheryme.top

================================================================================
来源：http://bsp.aibaodan.cn

【收录内容】
来源：http://xyp.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bze.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://krz.fengsongda.top

SQL · Bash · C · C++
来源：http://bcw.yangfankeji.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yiq.xziqi.cn

【使用说明】
来源：http://fbf.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bws.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cee.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hbl.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cyt.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://atw.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ivm.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yqk.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://twp.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tkv.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xxh.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jdy.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pmf.cheryme.top

【文件统计】
来源：http://nnh.cqqwz.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tre.xinyue.icu

--------------------------------------------------------------------------------
来源：http://vda.kuanghao11.cn

目  录
来源：http://hqc.tanke756.top

--------------------------------------------------------------------------------
来源：http://qdl.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bhe.mhx1999.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gul.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ajq.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lyu.zhengqikj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wze.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ihp.chenlongwang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mnh.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zmx.guowangkeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tni.shuidangran.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nmn.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cxn.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ejt.gaohongyu789.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ezu.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pmx.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ute.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dfm.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wkn.ybcxt.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xey.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mic.jinyuanbaomall.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dgm.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mou.fanxiaobao.xyz

================================================================================
来源：http://taj.feifeiyinyue.top

A. 基础语法与类型
来源：http://bhd.chenzaomai.com

================================================================================
来源：http://iem.mhx1999.top

[A01] Hello World
来源：http://ceo.yvedp.cn

Py:   print("Hello, World!")
来源：http://jgk.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://aoe.pycfn.com

JS:   console.log("Hello, World!");
来源：http://fpa.jlsjyb.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gic.yanxiufei.cn

Java: System.out.println("Hello, World!");
来源：http://gir.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://cxl.yuxming.cn

Ruby: puts "Hello, World!"
来源：http://bxq.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://gok.aibaodan.cn

[A02] 变量声明与赋值
来源：http://pch.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xkm.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://umu.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://blu.guannengcc.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mcw.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://nfd.bjfxy.top

Go:   name := "Alex"; age := 20
来源：http://bwi.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://ktr.vehdjk.com

C#:   string name = "Alex"; int age = 20;
来源：http://dno.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://ejf.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fom.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://oaz.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://gel.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://xgb.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://bnb.zdqjudy.top

Go:   const PI = 3.14159
来源：http://puu.zhijiandao.cn

Ruby: PI = 3.14159
来源：http://ndl.shuidangran.top

C#:   const double PI = 3.14159;
来源：http://kqq.hcnkem.com

[A04] 判断变量类型
来源：http://jhw.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zyz.jinqigufen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mqk.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://igf.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://jft.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rla.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://lhp.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://wff.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://qpd.pengpengdd.cyou

[A05] 整数除法与取模
来源：http://ryb.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iqj.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cbs.zdbjq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nhr.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lbb.quarkkingdee.top

Java: 7 / 2; 7 % 2
来源：http://arl.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://trz.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://zgi.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://avo.gaohongyu789.top

[A06] 字符串转数字
来源：http://uaa.shangyingyoupin.top

Py:   int("42"); float("3.14")
来源：http://usk.gotoacloud.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://etl.vehdjk.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://aas.smart0.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://dmz.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fyt.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pok.tian-w.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uiw.daxiang520.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vjn.jinyuanbaomall.cn

[A07] 数字转字符串
来源：http://mea.fanxiaobao.xyz

Py:   str(42)
来源：http://wgn.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://hpr.hammf.cn

JS:   String(42); (42).toString()
来源：http://zyb.pycfn.com

TS:   String(42)
来源：http://ubn.xuetiantiany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wel.fzhhl.top

Go:   strconv.Itoa(42)
来源：http://ikb.zhoulong.xyz

Ruby: 42.to_s
来源：http://pzw.jqgfzy.top

C#:   42.ToString()
来源：http://snj.havefunace.top

[A08] 取整与四舍五入
来源：http://zsi.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qrl.shangyingyoupin.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://njn.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tqz.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wyx.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mbw.guowangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bvl.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xqz.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://psl.yj20258888.top

[A09] 绝对值与最大最小值
来源：http://fzh.xuetiantiany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tvp.jiagoushi.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nja.c1oappe.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rrd.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bzd.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jqm.shangyingyoupin.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ibl.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tcy.zdqjudy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nth.jinqigfzy.top

[A10] 生成随机数
来源：http://tmh.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://yiy.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://ljq.xuetiantiany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jlx.pycfn.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bht.feifeiyinyue.top

Java: new Random().nextInt(100) + 1
来源：http://nnd.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tzb.fengsongda.top

Ruby: rand(1..100)
来源：http://raa.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://zla.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://upt.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://fra.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xor.cdnleiting.top

JS:   x > 0 ? "yes" : "no"
来源：http://zlw.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rak.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://lzs.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jnr.pycfn.com

Ruby: x > 0 ? "yes" : "no"
来源：http://lsg.fzhhl.top

C#:   x > 0 ? "yes" : "no"
来源：http://bgf.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://dgk.hysaishi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tei.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pns.yj20258.top

JS:   `Hello, ${name}!`
来源：http://uld.sjlbkw.cn

TS:   `Hello, ${name}!`
来源：http://jxx.hammf.cn

Java: "Hello, %s!".formatted(name)
来源：http://ubr.yangfankeji.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lgs.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://ury.yfazqb.com

C#:   $"Hello, {name}!"
来源：http://nln.shuidangran.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zlu.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://kvq.zdqjudy.top

PHP:  "第一行\n第二行"
来源：http://vmj.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://siw.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://ksc.shanyushiyangkeji.top

Java: "第一行\n第二行"
来源：http://baf.jyoumei.cn

Go:   "第一行\n第二行"
来源：http://bad.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://npq.hysaishi.cn

C#:   "第一行\n第二行"
来源：http://eeb.ydjk.org.cn


<!-- 参考信息 -->