代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://skd.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://bak.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://rdy.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cin.jyoumei.cn

[U85] JS：可选链
来源：http://bzf.zdqjudy.top

a?.b?.c
来源：http://yvb.haohaochexian.top

[U86] JS：空值合并
来源：http://tke.yj20258888.top

a ?? b
来源：http://tyj.yanxiufei.cn

[U87] JS：解构默认值
来源：http://adk.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://ere.guannengcc.top

[U88] JS：对象展开合并
来源：http://kbk.vqdsnc.cn

{ ...a, ...b }
来源：http://odn.zhiwuduotai.top

[U89] JS：数组去重
来源：http://aav.hnxiangtu.top

[...new Set(arr)]
来源：http://cpa.c1oappe.top

[U90] JS：数字数组排序
来源：http://rcn.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://kru.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://sbg.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bjh.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://gwz.jianghu66.top

structuredClone(obj)
来源：http://ysu.cqqwz.cn

[U93] JS：模板字符串
来源：http://gsy.gogol.net.cn

`共 ${n} 条`
来源：http://loh.jlsjyb.cn

[U94] JS：箭头函数
来源：http://rcr.wangshuangyany.cn

const double = x => x * 2;
来源：http://vif.tianlin.xyz

[U95] JS：Promise 包装
来源：http://lyj.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://hnx.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://ubo.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ktt.dianchejie.cn

[U97] JS：并发请求
来源：http://tgf.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://grq.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://cge.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wmz.havefunace.top

[U99] JS：事件监听
来源：http://rmr.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://daq.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://qvm.wangdashe.top

document.querySelector(".item")
来源：http://vtf.ivvv.top

[U101] JS：classList 操作
来源：http://eej.yueranfly.top

el.classList.toggle("active")
来源：http://xhq.jinqigfzy.top

[U102] JS：本地存储
来源：http://nxn.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vct.zhixingplan.top

[U103] JS：定时器
来源：http://ztv.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pxd.zhijiandao.cn

[U104] JS：防抖
来源：http://qim.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kct.yuanzhike.top

[U105] JS：节流
来源：http://jsk.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vjq.meibo888.top

[U106] JS：日期格式化
来源：http://xqf.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eoc.tanke756.top

[U107] JS：数字千分位
来源：http://pos.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ezx.yangfankeji.com

[U108] JS：随机整数
来源：http://xnm.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jor.fktsv.cn

[U109] JS：数组分组
来源：http://ivx.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://xhd.vqdsnc.cn

[U110] JS：数组分块
来源：http://ctj.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://akr.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://rej.zdbjq.cn

new Map(Object.entries(obj))
来源：http://nku.dianchejie.cn

[U112] JS：字符串补位
来源：http://ssb.fengsongda.top

"7".padStart(3, "0")
来源：http://epm.iojbl.cn

[U113] JS：正则替换全部
来源：http://vpe.bjfxy.top

s.replaceAll("a", "b")
来源：http://swn.xinyue.icu

[U114] JS：JSON 深比较
来源：http://mir.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wrh.snrcjt.cn

[U115] JS：生成 UUID
来源：http://bkh.hnxiangtu.top

crypto.randomUUID()
来源：http://vyc.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://hot.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://muk.zhixingplan.top

[U117] JS：单元测试
来源：http://xtd.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://wqz.sufxvd.cn

[U118] JS：开发服务器
来源：http://dzf.haohaochexian.top

npm i -D vite;  npx vite
来源：http://ctc.gogol.net.cn

[U119] JS：生产构建
来源：http://ica.shangyingyoupin.top

npx vite build
来源：http://ddl.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://bnr.ivvv.top

import.meta.env.VITE_API_URL
来源：http://xoj.jinqigufen.top

================================================================================
来源：http://qgw.bjfxy.top

统计汇总
来源：http://mmh.jianghu66.top

================================================================================
来源：http://ihx.52xcode.cn

按语言统计（条）：
来源：http://puy.daxiang520.top

Python ......... 252
来源：http://zeh.shanyushiyangtech.top

PHP ............ 252
来源：http://pef.hongshengwenyu.top

JavaScript ..... 252
来源：http://llh.ctjpmb.com

TypeScript ..... 212
来源：http://gai.yfazqb.com

Java ........... 212
来源：http://yhz.316326.xyz

Go ............. 212
来源：http://rgl.yj20258.top

Ruby ........... 212
来源：http://lrp.xuanzx.com

C# ............. 212
来源：http://kwj.yj20258.top

C .............. 30
来源：http://wre.wangshuangyany.cn

C++ ............ 30
来源：http://bnf.nanxuanxn.top

SQL ............ 90
来源：http://yok.zycfv.cn

Bash ........... 80
来源：http://vdy.jyoumei.cn

Kotlin ......... 15
来源：http://siy.shuidangran.top

Swift .......... 15
来源：http://lfw.zhongyouzk.top

Lua ............ 10
来源：http://xlm.meibo888.top

Perl ........... 10
来源：http://cqv.sxryk.cn

Scala .......... 10
来源：http://tss.havefunace.top

------------------------------------
来源：http://mcm.gaohongyu789.top

合计 ........... 2106 条
来源：http://yhq.redwolf501.top

按章节统计：
来源：http://xqs.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lmo.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xbg.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ozg.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jlt.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mtc.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zli.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hbw.fzhhl.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xwg.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://edr.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vtl.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dms.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jeo.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rnf.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lbv.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://exw.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uxs.dashuyun.cn

Q SQL 专题                              90
来源：http://dmb.feifeiyinyue.top

R Bash 专题                             80
来源：http://qca.yj202588.top

S C / C++ 专题                          60
来源：http://lhg.0kj1m.cn

T 其他语言补充                          60
来源：http://qag.52xcode.cn

U 高频实用片段                         120
来源：http://lom.hammf.cn

------------------------------------
来源：http://oco.hnqzz.top

合计                                  2106 条
来源：http://cuv.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://jyp.fehbvm.com

使用提醒
来源：http://tuu.yfazqb.com

--------------------------------------------------------------------------------
来源：http://ojw.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ron.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wij.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oda.wangdashe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ztd.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jkc.nanxinkj.top

—— 文件结束 ——
来源：http://irr.gotoacloud.top

================================================================================
来源：http://sro.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://brr.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://zyf.aizwys.cn

================================================================================
来源：http://ukk.jqgfzy.top

【收录内容】
来源：http://irv.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jud.nanxinkj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://olx.316326.xyz

SQL · Bash · C · C++
来源：http://cmh.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cuu.yuanzhike.top

【使用说明】
来源：http://cfv.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bzb.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://suy.yj20258.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://umo.jlsjyb.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dxv.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jok.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ovz.zhoulong.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ttc.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zxw.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oqa.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hqh.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ojk.hcnkem.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cbw.shangyingyoupin.top

【文件统计】
来源：http://wtp.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://emr.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://ipk.hfpthk.cn

目  录
来源：http://tro.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://vcw.ppjwa.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://frn.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iib.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://buv.ywan-chungtsiang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hag.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dph.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xjf.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vlp.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gcm.wangdashe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sjq.0kj1m.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://euc.gaohongyu789.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://flr.c1oappe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rwl.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uxf.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://moy.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ftm.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fhj.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xet.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zpe.ctjpmb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://udv.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wod.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lfd.meibo888.top

================================================================================
来源：http://apy.zycfv.cn

A. 基础语法与类型
来源：http://waq.guannengcc.top

================================================================================
来源：http://xqc.andypj.xyz

[A01] Hello World
来源：http://bru.fengsongda.top

Py:   print("Hello, World!")
来源：http://mjv.nwbrower.top

PHP:  echo "Hello, World!";
来源：http://zqq.zhijiandao.cn

JS:   console.log("Hello, World!");
来源：http://slt.tianlin.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://suq.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://uvk.yj202588.top

Go:   fmt.Println("Hello, World!")
来源：http://rft.vehdjk.com

Ruby: puts "Hello, World!"
来源：http://okm.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tms.zdbjq.cn

[A02] 变量声明与赋值
来源：http://skf.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ltu.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://src.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zyp.yongpay.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qkq.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://ofk.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://kls.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://mrg.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://ycs.c1oappe.top

[A03] 常量定义
来源：http://pbf.jiagoushi.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bri.316326.xyz

PHP:  const PI = 3.14159;
来源：http://ewv.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://dti.yuanzhike.top

TS:   const PI: number = 3.14159;
来源：http://eqt.zdbjq.cn

Java: static final double PI = 3.14159;
来源：http://ymb.aibaodan.cn

Go:   const PI = 3.14159
来源：http://xlc.guowangkeji.top

Ruby: PI = 3.14159
来源：http://qyn.zhiwuduotai.top

C#:   const double PI = 3.14159;
来源：http://wyn.guowangkeji.top

[A04] 判断变量类型
来源：http://hzp.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lyv.fehbvm.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yip.ehwqpu.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bvz.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://sjc.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jut.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://hbu.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mun.tian-w.cn

C#:   x.GetType().Name; x is int
来源：http://xbi.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://gmz.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ksb.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hwh.quarkkingdee.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gzm.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lie.ivvv.top

Java: 7 / 2; 7 % 2
来源：http://xih.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://xxr.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://awy.yfazqb.com

C#:   7 / 2; 7 % 2
来源：http://jqr.cheryme.top

[A06] 字符串转数字
来源：http://nfn.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://lgj.pengpengdd.cyou

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://egw.cdnleiting.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tng.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cfc.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ksx.zhaomingkeji.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://het.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pqd.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://unk.fzhhl.top

[A07] 数字转字符串
来源：http://qxv.tian-w.cn

Py:   str(42)
来源：http://jdp.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://ssq.kuanghao11.cn

JS:   String(42); (42).toString()
来源：http://plt.0kj1m.cn

TS:   String(42)
来源：http://haj.wangshuangyany.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hzs.0kj1m.cn

Go:   strconv.Itoa(42)
来源：http://lwl.ywan-chungtsiang.top

Ruby: 42.to_s
来源：http://uey.jqgfzy.top

C#:   42.ToString()
来源：http://vjp.316326.xyz

[A08] 取整与四舍五入
来源：http://jcv.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gma.chenjidiqi.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xmm.zhoulong.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uwt.tianlin.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://avv.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://utz.epnwcf.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pho.xziqi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tig.pycfn.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ams.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://wgm.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://heo.xylfe.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dco.snrcjt.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://adp.nanxinkj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xlv.jinghuilouyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jbc.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pbn.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gtq.xingfuxueyuan.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ohu.yueranfly.top

[A10] 生成随机数
来源：http://dnx.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://saz.xingfuxueyuan.xyz

PHP:  random_int(1, 100);
来源：http://kkb.zhijiandao.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yar.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vbo.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://uuq.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hvp.svipenyu.cn

Ruby: rand(1..100)
来源：http://fol.jinqigfzy.top

C#:   new Random().Next(1, 101)
来源：http://uci.jyoumei.cn

[A11] 条件表达式（三元）
来源：http://whj.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://lon.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://gml.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://kzj.vqdsnc.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oli.zdbjq.cn

Java: x > 0 ? "yes" : "no"
来源：http://mmu.mhx1999.top

Go:   // 无三元运算符，需用 if 语句
来源：http://snf.ehwqpu.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ogo.ppjwa.cn

C#:   x > 0 ? "yes" : "no"
来源：http://toj.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://pwp.316326.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kxg.daxiang520.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hbo.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://eib.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://sfs.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://ddz.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://spw.guowangkeji.top

Ruby: "Hello, #{name}!"
来源：http://wez.mhx1999.top

C#:   $"Hello, {name}!"
来源：http://ohf.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://otc.wangdashe.top

Py:   "第一行\n第二行"
来源：http://exm.xingfuxueyuan.xyz

PHP:  "第一行\n第二行"
来源：http://klz.zycfv.cn

JS:   "第一行\n第二行"
来源：http://qwd.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://nwc.0kj1m.cn

Java: "第一行\n第二行"
来源：http://xaw.fengsongda.top

Go:   "第一行\n第二行"
来源：http://xav.sysykeji.top

Ruby: "第一行\n第二行"
来源：http://wwo.nanxuanxn.top

C#:   "第一行\n第二行"
来源：http://ihe.chenzaomai.com


<!-- 参考信息 -->