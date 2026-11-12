代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://pud.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://sbl.pycfn.com

[U84] JS：CommonJS 写法
来源：http://eqd.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xox.jiagoushi.top

[U85] JS：可选链
来源：http://fvz.jqgufenzy.top

a?.b?.c
来源：http://yhu.epnwcf.com

[U86] JS：空值合并
来源：http://nil.gaohongyu789.top

a ?? b
来源：http://ybv.redwolf501.top

[U87] JS：解构默认值
来源：http://vku.ppjwa.cn

const { a = 1, b = 2 } = obj;
来源：http://zed.ppjwa.cn

[U88] JS：对象展开合并
来源：http://xjt.zhoulong.xyz

{ ...a, ...b }
来源：http://kre.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://xju.yongpay.top

[...new Set(arr)]
来源：http://rzf.zycfv.cn

[U90] JS：数字数组排序
来源：http://bxw.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://usl.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://cly.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://efs.hfpthk.cn

[U92] JS：深拷贝
来源：http://cgq.hnxiangtu.top

structuredClone(obj)
来源：http://xbb.guannengcc.top

[U93] JS：模板字符串
来源：http://yer.gogol.net.cn

`共 ${n} 条`
来源：http://ryn.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://wcq.dashuyun.cn

const double = x => x * 2;
来源：http://epr.jqgfzy.top

[U95] JS：Promise 包装
来源：http://npt.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://fqz.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://ver.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rgk.jinqigufen.top

[U97] JS：并发请求
来源：http://xiv.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gbq.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://efr.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hwg.chenzaomai.com

[U99] JS：事件监听
来源：http://qhf.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://tnr.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://wnp.wangshuangyany.cn

document.querySelector(".item")
来源：http://nmu.nwbrower.top

[U101] JS：classList 操作
来源：http://vfd.yangfankeji.com

el.classList.toggle("active")
来源：http://wgx.dianchejie.cn

[U102] JS：本地存储
来源：http://csn.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lpb.jyoumei.cn

[U103] JS：定时器
来源：http://wjq.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pzs.sjlbkw.cn

[U104] JS：防抖
来源：http://lkh.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://noi.cucudq.cn

[U105] JS：节流
来源：http://vdd.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tmd.sysykeji.top

[U106] JS：日期格式化
来源：http://lbn.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hxj.hnqzz.top

[U107] JS：数字千分位
来源：http://ajq.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hrg.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://jyx.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ktx.hfpthk.cn

[U109] JS：数组分组
来源：http://tri.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://vwr.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://rco.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://snt.guannengcc.top

[U111] JS：对象转 Map
来源：http://tiq.xziqi.cn

new Map(Object.entries(obj))
来源：http://yss.yongpay.top

[U112] JS：字符串补位
来源：http://ods.ctjpmb.com

"7".padStart(3, "0")
来源：http://kwi.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://lpa.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://xfm.tarul.cn

[U114] JS：JSON 深比较
来源：http://gjd.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cuu.redwolf501.top

[U115] JS：生成 UUID
来源：http://jwe.xuanzx.com

crypto.randomUUID()
来源：http://ajn.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://bcd.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://rwl.cqqwz.cn

[U117] JS：单元测试
来源：http://voy.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://kbh.zhixingplan.top

[U118] JS：开发服务器
来源：http://hni.vehdjk.com

npm i -D vite;  npx vite
来源：http://nxg.fzhhl.top

[U119] JS：生产构建
来源：http://xgh.quarkkingdee.top

npx vite build
来源：http://bog.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://fxi.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://zff.ywan-chungtsiang.top

================================================================================
来源：http://whq.fktsv.cn

统计汇总
来源：http://gna.hongshengwenyu.top

================================================================================
来源：http://zax.hfpthk.cn

按语言统计（条）：
来源：http://fbt.hesvh.cn

Python ......... 252
来源：http://xtm.mhx1999.top

PHP ............ 252
来源：http://bwg.chenzaomai.com

JavaScript ..... 252
来源：http://vgg.jqgufenzy.top

TypeScript ..... 212
来源：http://jvl.cqqwz.cn

Java ........... 212
来源：http://wpm.gotoacloud.top

Go ............. 212
来源：http://ssp.ydjk.org.cn

Ruby ........... 212
来源：http://nzi.fengsongda.top

C# ............. 212
来源：http://cji.bbcook.cn

C .............. 30
来源：http://qdk.tanke756.top

C++ ............ 30
来源：http://vuu.yj202588.top

SQL ............ 90
来源：http://rew.sweek.top

Bash ........... 80
来源：http://ieu.aibaodan.cn

Kotlin ......... 15
来源：http://gyy.zhiwuduotai.top

Swift .......... 15
来源：http://smc.daria6918.cn

Lua ............ 10
来源：http://ycg.uphjek.com

Perl ........... 10
来源：http://ioe.cqqwz.cn

Scala .......... 10
来源：http://esi.jinqigfzy.top

------------------------------------
来源：http://pze.hywenlv.cn

合计 ........... 2106 条
来源：http://whj.yvedp.cn

按章节统计：
来源：http://wcy.aizwys.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iol.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://omz.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xsa.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zaw.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sds.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rgg.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://skf.jinghuilouyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iob.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vbn.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jjg.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hlq.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://txk.jlsjyb.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yje.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bgq.52xcode.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uzs.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://usl.zdqjudy.top

Q SQL 专题                              90
来源：http://jwt.zhengqikj.top

R Bash 专题                             80
来源：http://psz.svipenyu.cn

S C / C++ 专题                          60
来源：http://qbq.tianlin.xyz

T 其他语言补充                          60
来源：http://ham.tanke756.top

U 高频实用片段                         120
来源：http://tvz.yfazqb.com

------------------------------------
来源：http://mal.gaohongyu789.top

合计                                  2106 条
来源：http://svb.yj20258888.top

--------------------------------------------------------------------------------
来源：http://myv.zhongyouzk.top

使用提醒
来源：http://vde.yfazqb.com

--------------------------------------------------------------------------------
来源：http://zcu.smart0.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://suo.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bve.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bap.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wcq.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nsj.hnxiangtu.top

—— 文件结束 ——
来源：http://bag.ctjpmb.com

================================================================================
来源：http://tfd.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://xhj.xziqi.cn

Common Programming Examples Cheat Book
来源：http://vet.uphjek.com

================================================================================
来源：http://kba.tian-w.cn

【收录内容】
来源：http://snw.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://aad.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cgd.jinqigufen.top

SQL · Bash · C · C++
来源：http://epg.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pdd.ybcxt.top

【使用说明】
来源：http://ter.tanke756.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ijo.zdbjq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kzh.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bdn.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gfo.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xdy.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qjm.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qzg.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://saj.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wme.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tht.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xpd.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mov.ydzc1.top

【文件统计】
来源：http://hgn.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fxe.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://lcf.hesvh.cn

目  录
来源：http://tyc.52xcode.cn

--------------------------------------------------------------------------------
来源：http://dsn.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aup.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qdk.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dup.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rye.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xcf.52xcode.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ump.uphjek.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dqs.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kxm.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qgn.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jnu.cheryme.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wxi.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://phf.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xzu.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://njx.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zhl.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zyr.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ujq.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bpn.zhaomingkeji.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vlq.ctjpmb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://awc.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qyh.zhixingplan.top

================================================================================
来源：http://soh.jinqigufen.top

A. 基础语法与类型
来源：http://hba.fanxiaobao.xyz

================================================================================
来源：http://hgh.ppjwa.cn

[A01] Hello World
来源：http://mof.redwolf501.top

Py:   print("Hello, World!")
来源：http://zra.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://kxa.hnxiangtu.top

JS:   console.log("Hello, World!");
来源：http://tkc.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dxr.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://hmg.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://dhl.sjlbkw.cn

Ruby: puts "Hello, World!"
来源：http://oia.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://izg.316326.xyz

[A02] 变量声明与赋值
来源：http://xld.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aps.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wbu.nwbrower.top

JS:   let name = "Alex"; const age = 20;
来源：http://qsi.vqdsnc.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gop.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://btd.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://rjk.hywenlv.cn

Ruby: name = "Alex"; age = 20
来源：http://mty.yonumen.top

C#:   string name = "Alex"; int age = 20;
来源：http://acq.andypj.xyz

[A03] 常量定义
来源：http://uqo.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tdw.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://xeq.ivvv.top

JS:   const PI = 3.14159;
来源：http://xci.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://sgy.shzxlz.cn

Java: static final double PI = 3.14159;
来源：http://riz.uphjek.com

Go:   const PI = 3.14159
来源：http://xem.xinyue.icu

Ruby: PI = 3.14159
来源：http://lxa.cashguo.top

C#:   const double PI = 3.14159;
来源：http://uxy.sjlbkw.cn

[A04] 判断变量类型
来源：http://vvo.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://txs.chenjidiqi.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ebs.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ijj.ivvv.top

TS:   typeof x; x instanceof Date
来源：http://dyo.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gum.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bmk.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bvj.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://gks.jinqigfzy.top

[A05] 整数除法与取模
来源：http://xbs.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qae.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://knh.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pat.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vxj.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://vqs.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://axu.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://jbf.shuidangran.top

C#:   7 / 2; 7 % 2
来源：http://nnr.daxiang520.top

[A06] 字符串转数字
来源：http://fxj.pengpengdd.cyou

Py:   int("42"); float("3.14")
来源：http://wbm.wangdashe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zev.gotoacloud.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ntl.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sku.yj20258.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ice.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xam.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://eaj.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ndd.jinqigfzy.top

[A07] 数字转字符串
来源：http://pjh.yueranfly.top

Py:   str(42)
来源：http://cbo.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://tgu.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://raa.aizwys.cn

TS:   String(42)
来源：http://kbr.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://jvl.yj202588.top

Go:   strconv.Itoa(42)
来源：http://czp.zhijiandao.cn

Ruby: 42.to_s
来源：http://iph.hesvh.cn

C#:   42.ToString()
来源：http://eaa.hammf.cn

[A08] 取整与四舍五入
来源：http://nmx.daxiang520.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bus.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hfl.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tpk.dianchejie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ssd.cdnleiting.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nwp.yvedp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rqh.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ons.daxiang520.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sge.dashuyun.cn

[A09] 绝对值与最大最小值
来源：http://bul.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mqz.daxiang520.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://atu.tarul.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bhl.tanke756.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://txb.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cpl.jyoumei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gez.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nmk.jlsjyb.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mzp.hfpthk.cn

[A10] 生成随机数
来源：http://zrt.hnxiangtu.top

Py:   import random; random.randint(1, 100)
来源：http://jfy.wangdashe.top

PHP:  random_int(1, 100);
来源：http://pux.ydzc1.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gtv.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tfa.hesvh.cn

Java: new Random().nextInt(100) + 1
来源：http://kta.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qun.xinyue.icu

Ruby: rand(1..100)
来源：http://dnm.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://bda.52xcode.cn

[A11] 条件表达式（三元）
来源：http://lwr.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://tzd.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://grz.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://wlj.gzhubu.top

TS:   x > 0 ? "yes" : "no"
来源：http://ubv.yanxiufei.cn

Java: x > 0 ? "yes" : "no"
来源：http://iog.jiagoushi.top

Go:   // 无三元运算符，需用 if 语句
来源：http://baq.ydzc1.top

Ruby: x > 0 ? "yes" : "no"
来源：http://knz.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://ecg.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://cnr.shangyingyoupin.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cix.sxryk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://alh.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://spu.cashguo.top

TS:   `Hello, ${name}!`
来源：http://hkk.316326.xyz

Java: "Hello, %s!".formatted(name)
来源：http://bpn.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rxn.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://hoz.cucudq.cn

C#:   $"Hello, {name}!"
来源：http://laa.nanxinkj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cpq.svipenyu.cn

Py:   "第一行\n第二行"
来源：http://lzh.dashuyun.cn

PHP:  "第一行\n第二行"
来源：http://vvv.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://dkg.guannengcc.top

TS:   "第一行\n第二行"
来源：http://ujb.vehdjk.com

Java: "第一行\n第二行"
来源：http://ola.hcnkem.com

Go:   "第一行\n第二行"
来源：http://xxw.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://tgl.epnwcf.com

C#:   "第一行\n第二行"
来源：http://vwz.nwbrower.top


<!-- 参考信息 -->