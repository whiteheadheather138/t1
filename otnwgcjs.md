代发 wailian999

[U81] JS：初始化项目
来源：http://ewc.cashguo.top

npm init -y;  npm i express
来源：http://qow.pycfn.com

[U82] JS：package.json 脚本
来源：http://nzz.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://auq.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://yku.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wuw.uphjek.com

[U84] JS：CommonJS 写法
来源：http://ucm.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ysj.jqgufenzy.top

[U85] JS：可选链
来源：http://gyl.tanke756.top

a?.b?.c
来源：http://czf.quarkkingdee.top

[U86] JS：空值合并
来源：http://jku.zhiwuduotai.top

a ?? b
来源：http://mfz.ybcxt.top

[U87] JS：解构默认值
来源：http://bgr.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://xvp.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://ejw.uphjek.com

{ ...a, ...b }
来源：http://ieu.fengsongda.top

[U89] JS：数组去重
来源：http://qpv.yj20258888.top

[...new Set(arr)]
来源：http://vyy.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://pit.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://syz.hcnkem.com

[U91] JS：对象键值遍历
来源：http://ddt.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iaf.zhijiandao.cn

[U92] JS：深拷贝
来源：http://xjo.hcnkem.com

structuredClone(obj)
来源：http://ybb.ybcxt.top

[U93] JS：模板字符串
来源：http://dbu.c1oappe.top

`共 ${n} 条`
来源：http://iwa.shzxlz.cn

[U94] JS：箭头函数
来源：http://tkm.sxryk.cn

const double = x => x * 2;
来源：http://hpl.xylfe.cn

[U95] JS：Promise 包装
来源：http://fus.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://ytx.xinyue.icu

[U96] JS：async/await 与异常
来源：http://mdl.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dny.sweek.top

[U97] JS：并发请求
来源：http://exu.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uni.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://trd.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://chs.quarkkingdee.top

[U99] JS：事件监听
来源：http://iof.guannengcc.top

el.addEventListener("click", e => {})
来源：http://ibt.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://wmq.hfpthk.cn

document.querySelector(".item")
来源：http://wml.wangdashe.top

[U101] JS：classList 操作
来源：http://spe.ctjpmb.com

el.classList.toggle("active")
来源：http://mow.yj202588.top

[U102] JS：本地存储
来源：http://exs.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kqf.fktsv.cn

[U103] JS：定时器
来源：http://pjt.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lir.jiagoushi.top

[U104] JS：防抖
来源：http://vzf.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujm.jianghu66.top

[U105] JS：节流
来源：http://thm.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://boq.52xcode.cn

[U106] JS：日期格式化
来源：http://zst.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tmh.fehbvm.com

[U107] JS：数字千分位
来源：http://xzm.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vds.jqgfzy.top

[U108] JS：随机整数
来源：http://xed.ydjk.org.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pjy.redwolf501.top

[U109] JS：数组分组
来源：http://ijk.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://xqo.yj202588.top

[U110] JS：数组分块
来源：http://lvt.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bue.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://lbd.pycfn.com

new Map(Object.entries(obj))
来源：http://lvv.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://wvg.nwbrower.top

"7".padStart(3, "0")
来源：http://wyo.gzhubu.top

[U113] JS：正则替换全部
来源：http://vbz.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://lwo.dianchejie.cn

[U114] JS：JSON 深比较
来源：http://xsy.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aja.guowangkeji.top

[U115] JS：生成 UUID
来源：http://rik.yanxiufei.cn

crypto.randomUUID()
来源：http://rwr.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://jmg.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://dpq.havefunace.top

[U117] JS：单元测试
来源：http://izi.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://iel.smart0.xyz

[U118] JS：开发服务器
来源：http://yah.zhixingplan.top

npm i -D vite;  npx vite
来源：http://aec.fktsv.cn

[U119] JS：生产构建
来源：http://zhp.zhengqikj.top

npx vite build
来源：http://gcu.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://rxl.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://nzo.jinghuilouyu.cn

================================================================================
来源：http://kls.smart0.xyz

统计汇总
来源：http://fpg.zhiwuduotai.top

================================================================================
来源：http://myi.cdnleiting.top

按语言统计（条）：
来源：http://mlm.zhijiandao.cn

Python ......... 252
来源：http://kan.zhaomingkeji.xyz

PHP ............ 252
来源：http://inc.chenjidiqi.icu

JavaScript ..... 252
来源：http://bdm.shuidangran.top

TypeScript ..... 212
来源：http://sva.tarul.cn

Java ........... 212
来源：http://kur.cashguo.top

Go ............. 212
来源：http://ezj.ybcxt.top

Ruby ........... 212
来源：http://ywt.yfazqb.com

C# ............. 212
来源：http://vzl.xziqi.cn

C .............. 30
来源：http://cks.hfpthk.cn

C++ ............ 30
来源：http://dda.sufxvd.cn

SQL ............ 90
来源：http://sia.daria6918.cn

Bash ........... 80
来源：http://fue.zdbjq.cn

Kotlin ......... 15
来源：http://xfp.svipenyu.cn

Swift .......... 15
来源：http://roe.jinqigfzy.top

Lua ............ 10
来源：http://sls.nanxuanxn.top

Perl ........... 10
来源：http://zec.ctjpmb.com

Scala .......... 10
来源：http://zqy.mhx1999.top

------------------------------------
来源：http://fci.zhongyouzk.top

合计 ........... 2106 条
来源：http://mog.zdbjq.cn

按章节统计：
来源：http://coq.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yva.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fap.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mbi.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uzm.fanxiaobao.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rwa.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xnm.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ooq.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fmr.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wwk.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xjd.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ehg.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gkr.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fbx.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ykl.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xyl.shangyingyoupin.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nae.xziqi.cn

Q SQL 专题                              90
来源：http://doy.epnwcf.com

R Bash 专题                             80
来源：http://bat.cucudq.cn

S C / C++ 专题                          60
来源：http://xyj.ehwqpu.com

T 其他语言补充                          60
来源：http://wtz.redwolf501.top

U 高频实用片段                         120
来源：http://ezw.guowangkeji.top

------------------------------------
来源：http://bvb.c1oappe.top

合计                                  2106 条
来源：http://hdb.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://csp.mhx1999.top

使用提醒
来源：http://pnd.pycfn.com

--------------------------------------------------------------------------------
来源：http://vpc.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://acv.pengpengdd.cyou

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qfu.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://taq.chenzaomai.com

在旧版本上使用前请先确认语法支持情况。
来源：http://llb.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://epn.zhoulong.xyz

—— 文件结束 ——
来源：http://lgq.ctjpmb.com

================================================================================
来源：http://alr.aizwys.cn

程序语言常见例子速查手册（2024 版）
来源：http://fel.yuxming.cn

Common Programming Examples Cheat Book
来源：http://bdz.ywan-chungtsiang.top

================================================================================
来源：http://gty.gaohongyu789.top

【收录内容】
来源：http://vzb.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vqh.sweek.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cjl.ydjk.org.cn

SQL · Bash · C · C++
来源：http://hnw.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tyh.zhoulong.xyz

【使用说明】
来源：http://lir.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cbw.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kzr.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rjs.yongpay.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dml.cdnleiting.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jxu.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ldc.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mbp.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gyc.jlsjyb.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tcw.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ovv.ywan-chungtsiang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jsq.pycfn.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bbu.svipenyu.cn

【文件统计】
来源：http://rhh.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://knr.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://ipb.jyoumei.cn

目  录
来源：http://npn.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://dia.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iun.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://owe.xziqi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jgw.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mbt.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nfk.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zqz.yongpay.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aje.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sxc.jinghuilouyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wxr.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://clq.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nqh.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ysm.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mtd.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bjs.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ywq.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cfe.bjfxy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tbm.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fao.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yew.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qja.chenjidiqi.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qsh.xingfuxueyuan.xyz

================================================================================
来源：http://ocb.yonumen.top

A. 基础语法与类型
来源：http://zja.nanxinkj.top

================================================================================
来源：http://cqj.meibo888.top

[A01] Hello World
来源：http://dlc.hysaishi.cn

Py:   print("Hello, World!")
来源：http://ver.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://yuc.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://jep.yuanzhike.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dii.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://hwq.yangfankeji.com

Go:   fmt.Println("Hello, World!")
来源：http://kaa.sweek.top

Ruby: puts "Hello, World!"
来源：http://wbf.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cim.sufxvd.cn

[A02] 变量声明与赋值
来源：http://ggg.aizwys.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oke.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://abv.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://xzi.jinyuanbaomall.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vmc.nanxinkj.top

Java: String name = "Alex"; int age = 20;
来源：http://sus.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://afx.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://xfx.zhengqikj.top

C#:   string name = "Alex"; int age = 20;
来源：http://ajf.52xcode.cn

[A03] 常量定义
来源：http://dfn.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://itt.hysaishi.cn

PHP:  const PI = 3.14159;
来源：http://dad.fzhhl.top

JS:   const PI = 3.14159;
来源：http://jyk.sweek.top

TS:   const PI: number = 3.14159;
来源：http://hsi.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://gnd.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://psk.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://ptg.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://cuv.cqqwz.cn

[A04] 判断变量类型
来源：http://tmh.cucudq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cpb.hcnkem.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://itm.cashguo.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lxj.fehbvm.com

TS:   typeof x; x instanceof Date
来源：http://qio.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ngu.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gfh.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://jru.9152youxi.cn

C#:   x.GetType().Name; x is int
来源：http://wag.cdnleiting.top

[A05] 整数除法与取模
来源：http://yro.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wbl.redwolf501.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wee.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tci.52xcode.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ams.hesvh.cn

Java: 7 / 2; 7 % 2
来源：http://llx.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://tee.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://fpw.shanyushiyangtech.top

C#:   7 / 2; 7 % 2
来源：http://wrg.aibaodan.cn

[A06] 字符串转数字
来源：http://dod.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://bhm.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mck.xingfuxueyuan.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hml.jinyuanbaomall.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hbs.gaohongyu789.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://isy.tanke756.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rbp.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uub.epnwcf.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cfi.jinqigufen.top

[A07] 数字转字符串
来源：http://gjp.fzhhl.top

Py:   str(42)
来源：http://crx.tian-w.cn

PHP:  (string) 42; strval(42)
来源：http://qjj.jianghu66.top

JS:   String(42); (42).toString()
来源：http://rhy.hammf.cn

TS:   String(42)
来源：http://lqb.xziqi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wbh.jinyuanbaomall.cn

Go:   strconv.Itoa(42)
来源：http://rrf.chenzaomai.com

Ruby: 42.to_s
来源：http://uyi.gotoacloud.top

C#:   42.ToString()
来源：http://wch.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://qqv.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://awh.gotoacloud.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bsy.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qti.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wyb.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uub.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wmv.sweek.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wvn.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hlf.zdqjudy.top

[A09] 绝对值与最大最小值
来源：http://ghw.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tpx.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://opi.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xjx.daria6918.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rll.sysykeji.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://drf.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nsz.yongpay.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bhu.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tnn.shangyingyoupin.top

[A10] 生成随机数
来源：http://jgn.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://mnj.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://dmh.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xrd.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://scv.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://wxw.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qnk.gzhubu.top

Ruby: rand(1..100)
来源：http://vwg.bbcook.cn

C#:   new Random().Next(1, 101)
来源：http://oth.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://wvt.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://gdl.hywenlv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vpv.guannengcc.top

JS:   x > 0 ? "yes" : "no"
来源：http://rve.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gry.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://fyj.shzxlz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ivh.fengsongda.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ssc.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://buw.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://ajw.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ipa.pycfn.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gzk.ywan-chungtsiang.top

JS:   `Hello, ${name}!`
来源：http://iiw.yongpay.top

TS:   `Hello, ${name}!`
来源：http://mdf.shuidangran.top

Java: "Hello, %s!".formatted(name)
来源：http://nku.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qoh.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://yfj.zhengqikj.top

C#:   $"Hello, {name}!"
来源：http://iog.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://kqo.iojbl.cn

Py:   "第一行\n第二行"
来源：http://nww.ydjk.org.cn

PHP:  "第一行\n第二行"
来源：http://dbh.ybcxt.top

JS:   "第一行\n第二行"
来源：http://xlf.hcnkem.com

TS:   "第一行\n第二行"
来源：http://hcl.c1oappe.top


<!-- 参考信息 -->