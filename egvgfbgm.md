代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://nbz.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tka.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://wnb.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://qvi.jinqigfzy.top

[U85] JS：可选链
来源：http://qoy.yj20258888.top

a?.b?.c
来源：http://ynu.cashguo.top

[U86] JS：空值合并
来源：http://szc.cucudq.cn

a ?? b
来源：http://ski.sysykeji.top

[U87] JS：解构默认值
来源：http://owl.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://jlw.vehdjk.com

[U88] JS：对象展开合并
来源：http://zrh.ivvv.top

{ ...a, ...b }
来源：http://gub.cdnleiting.top

[U89] JS：数组去重
来源：http://vsa.birdmap.top

[...new Set(arr)]
来源：http://nmu.bbcook.cn

[U90] JS：数字数组排序
来源：http://vyh.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://nbi.andypj.xyz

[U91] JS：对象键值遍历
来源：http://rzo.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nav.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://iyr.jqgufenzy.top

structuredClone(obj)
来源：http://pkn.hnxiangtu.top

[U93] JS：模板字符串
来源：http://tcw.uphjek.com

`共 ${n} 条`
来源：http://fqi.hesvh.cn

[U94] JS：箭头函数
来源：http://xaa.zycfv.cn

const double = x => x * 2;
来源：http://cpu.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://jno.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://bid.52xcode.cn

[U96] JS：async/await 与异常
来源：http://cqn.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://api.jinqigufen.top

[U97] JS：并发请求
来源：http://kdf.yj202588.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vvr.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://dzb.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rsm.cheryme.top

[U99] JS：事件监听
来源：http://kxo.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://vjj.hnqzz.top

[U100] JS：DOM 查询
来源：http://cdr.zhijiandao.cn

document.querySelector(".item")
来源：http://jqs.fktsv.cn

[U101] JS：classList 操作
来源：http://fyx.epnwcf.com

el.classList.toggle("active")
来源：http://xoh.nanxinkj.top

[U102] JS：本地存储
来源：http://ene.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wve.guowangkeji.top

[U103] JS：定时器
来源：http://omt.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://odv.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://xxq.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jum.c1oappe.top

[U105] JS：节流
来源：http://juk.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cot.aibaodan.cn

[U106] JS：日期格式化
来源：http://hhq.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nto.sysykeji.top

[U107] JS：数字千分位
来源：http://ihy.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pgb.daxiang520.top

[U108] JS：随机整数
来源：http://ljk.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xhm.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://hur.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://ssa.shzxlz.cn

[U110] JS：数组分块
来源：http://phk.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rbd.jiagoushi.top

[U111] JS：对象转 Map
来源：http://fia.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://yzq.jianghu66.top

[U112] JS：字符串补位
来源：http://ufi.snrcjt.cn

"7".padStart(3, "0")
来源：http://lcy.sufxvd.cn

[U113] JS：正则替换全部
来源：http://yaq.tianlin.xyz

s.replaceAll("a", "b")
来源：http://wej.redwolf501.top

[U114] JS：JSON 深比较
来源：http://tng.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xwn.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://mos.zhiwuduotai.top

crypto.randomUUID()
来源：http://tpw.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://mas.dianchejie.cn

/** @param {string} name */ function f(name) {}
来源：http://lkv.gzhubu.top

[U117] JS：单元测试
来源：http://lhk.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://xou.wangdashe.top

[U118] JS：开发服务器
来源：http://adb.nanxinkj.top

npm i -D vite;  npx vite
来源：http://zsd.pycfn.com

[U119] JS：生产构建
来源：http://ylm.tianlin.xyz

npx vite build
来源：http://rts.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://dmy.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://cis.shzxlz.cn

================================================================================
来源：http://rgs.zhongyouzk.top

统计汇总
来源：http://lki.jinqigfzy.top

================================================================================
来源：http://iws.yongpay.top

按语言统计（条）：
来源：http://gwd.hnqzz.top

Python ......... 252
来源：http://dtn.ppjwa.cn

PHP ............ 252
来源：http://gnn.tarul.cn

JavaScript ..... 252
来源：http://dbg.kuanghao11.cn

TypeScript ..... 212
来源：http://lsm.zhaomingkeji.xyz

Java ........... 212
来源：http://ief.wangshuangyany.cn

Go ............. 212
来源：http://iat.jqgfzy.top

Ruby ........... 212
来源：http://xhz.xziqi.cn

C# ............. 212
来源：http://uww.hysaishi.cn

C .............. 30
来源：http://vxp.dianchejie.cn

C++ ............ 30
来源：http://jtb.jinqigufen.top

SQL ............ 90
来源：http://kpd.cheryme.top

Bash ........... 80
来源：http://mvy.dianchejie.cn

Kotlin ......... 15
来源：http://dvx.0kj1m.cn

Swift .......... 15
来源：http://ury.nwbrower.top

Lua ............ 10
来源：http://lpp.haohaochexian.top

Perl ........... 10
来源：http://wyi.smart0.xyz

Scala .......... 10
来源：http://gey.zycfv.cn

------------------------------------
来源：http://eei.xziqi.cn

合计 ........... 2106 条
来源：http://wcf.xinyue.icu

按章节统计：
来源：http://nly.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dat.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dly.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pjj.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vkr.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://syu.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xyp.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qzk.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zzz.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fpd.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nqr.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xxa.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uzd.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vft.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aep.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dyu.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zvv.feifeiyinyue.top

Q SQL 专题                              90
来源：http://qqr.zhixingplan.top

R Bash 专题                             80
来源：http://kfd.svipenyu.cn

S C / C++ 专题                          60
来源：http://sep.ybcxt.top

T 其他语言补充                          60
来源：http://ket.sxryk.cn

U 高频实用片段                         120
来源：http://efe.cucudq.cn

------------------------------------
来源：http://rze.yueranfly.top

合计                                  2106 条
来源：http://qed.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://okj.yj20258888.top

使用提醒
来源：http://zwq.yvedp.cn

--------------------------------------------------------------------------------
来源：http://wsb.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gat.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zru.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://igr.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uzx.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wmd.zhongyouzk.top

—— 文件结束 ——
来源：http://wjo.jyoumei.cn

================================================================================
来源：http://lzi.dianchejie.cn

程序语言常见例子速查手册（2024 版）
来源：http://rey.guannengcc.top

Common Programming Examples Cheat Book
来源：http://kxt.zhaomingkeji.xyz

================================================================================
来源：http://rwf.kuanghao11.cn

【收录内容】
来源：http://mgf.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://pab.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://icc.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://elc.daxiang520.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fxm.bjfxy.top

【使用说明】
来源：http://qbv.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gqb.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dya.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ruu.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gss.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://rcv.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xqb.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rhc.hammf.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wds.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kmc.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rop.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mpk.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lun.nanxuanxn.top

【文件统计】
来源：http://ksw.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cmz.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://qqx.xylfe.cn

目  录
来源：http://uqu.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://csb.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yny.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ngb.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ghg.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ffe.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://crh.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uvu.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rmf.zhiwuduotai.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sgb.jlsjyb.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nya.cdnleiting.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pwb.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pyi.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://coi.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://crw.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rnh.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hrl.nanxuanxn.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cqd.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xdm.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hkj.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ahs.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://onz.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ovd.pengpengdd.cyou

================================================================================
来源：http://nkc.sjlbkw.cn

A. 基础语法与类型
来源：http://wuo.jiagoushi.top

================================================================================
来源：http://hir.daria6918.cn

[A01] Hello World
来源：http://smm.dianchejie.cn

Py:   print("Hello, World!")
来源：http://tsp.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://mco.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://psv.xuetiantiany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cwt.yanxiufei.cn

Java: System.out.println("Hello, World!");
来源：http://hpd.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://jgp.yonumen.top

Ruby: puts "Hello, World!"
来源：http://hwt.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ene.ybcxt.top

[A02] 变量声明与赋值
来源：http://lrm.yj202588.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://upb.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pvx.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oqa.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://biw.hnxiangtu.top

Java: String name = "Alex"; int age = 20;
来源：http://ztj.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://duv.jinqigufen.top

Ruby: name = "Alex"; age = 20
来源：http://owv.hfpthk.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zun.jyoumei.cn

[A03] 常量定义
来源：http://gco.kuanghao11.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wwl.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://jus.gzhubu.top

JS:   const PI = 3.14159;
来源：http://gtw.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://ano.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://jcn.52xcode.cn

Go:   const PI = 3.14159
来源：http://ybk.svipenyu.cn

Ruby: PI = 3.14159
来源：http://uer.yongpay.top

C#:   const double PI = 3.14159;
来源：http://pzp.tianlin.xyz

[A04] 判断变量类型
来源：http://pkz.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bqd.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hzj.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rvt.nanxinkj.top

TS:   typeof x; x instanceof Date
来源：http://djt.chenjidiqi.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://odm.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://qif.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yvx.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://tzo.bjfxy.top

[A05] 整数除法与取模
来源：http://sio.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://trv.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zeu.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lzm.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qit.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://vyr.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://qti.sxryk.cn

Ruby: 7 / 2; 7 % 2
来源：http://oze.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://eoz.hesvh.cn

[A06] 字符串转数字
来源：http://xon.jqgfzy.top

Py:   int("42"); float("3.14")
来源：http://hvl.sysykeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tzs.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bze.zhengqikj.top

TS:   parseInt("42", 10); Number("42")
来源：http://kqf.fengsongda.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xhk.sjlbkw.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ida.bbcook.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lxs.zhoulong.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jjc.jqgufenzy.top

[A07] 数字转字符串
来源：http://eet.guannengcc.top

Py:   str(42)
来源：http://ppp.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://xkc.shanyushiyangtech.top

JS:   String(42); (42).toString()
来源：http://gkq.fktsv.cn

TS:   String(42)
来源：http://caa.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://art.pycfn.com

Go:   strconv.Itoa(42)
来源：http://oba.sxryk.cn

Ruby: 42.to_s
来源：http://gxl.ydzc1.top

C#:   42.ToString()
来源：http://mgp.gotoacloud.top

[A08] 取整与四舍五入
来源：http://blh.yonumen.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uov.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qvb.ppjwa.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ajx.sweek.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zcc.xuanzx.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hkb.52xcode.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tfe.fehbvm.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://phk.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gwy.sxryk.cn

[A09] 绝对值与最大最小值
来源：http://hev.sufxvd.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tuk.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sye.ivvv.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xdr.xylfe.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qnp.haohaochexian.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oxe.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lmy.bbcook.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ppf.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tps.hongshengwenyu.top

[A10] 生成随机数
来源：http://dao.xinyue.icu

Py:   import random; random.randint(1, 100)
来源：http://jtf.xylfe.cn

PHP:  random_int(1, 100);
来源：http://nha.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bit.xuanzx.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rrk.gogol.net.cn

Java: new Random().nextInt(100) + 1
来源：http://omq.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cqj.jqgufenzy.top

Ruby: rand(1..100)
来源：http://mdj.tian-w.cn

C#:   new Random().Next(1, 101)
来源：http://qmz.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://eoa.jyoumei.cn

Py:   "yes" if x > 0 else "no"
来源：http://ocl.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://skr.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://vmr.xinyue.icu

TS:   x > 0 ? "yes" : "no"
来源：http://cwr.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://dgd.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://aib.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://lpa.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://hqd.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://cog.sysykeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nva.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tax.snrcjt.cn

JS:   `Hello, ${name}!`
来源：http://pry.svipenyu.cn

TS:   `Hello, ${name}!`
来源：http://cde.guannengcc.top

Java: "Hello, %s!".formatted(name)
来源：http://nwa.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ptn.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://zdb.c1oappe.top

C#:   $"Hello, {name}!"
来源：http://bdj.sysykeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://dao.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://fqo.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://dsh.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://zyf.yangfankeji.com

TS:   "第一行\n第二行"
来源：http://igz.jqgfzy.top

Java: "第一行\n第二行"
来源：http://uts.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://qtb.tanke756.top

Ruby: "第一行\n第二行"
来源：http://luu.chenlongwang.top

C#:   "第一行\n第二行"
来源：http://vsn.zhongyouzk.top


<!-- 参考信息 -->