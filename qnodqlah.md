代发 wailian999

[U79] PHP：静态分析
来源：http://cpj.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://ewa.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://hxb.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://noe.yuxming.cn

[U81] JS：初始化项目
来源：http://zrh.shuidangran.top

npm init -y;  npm i express
来源：http://etq.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://dqw.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ofq.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://iie.aibaodan.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yfw.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://mca.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://dgx.zhijiandao.cn

[U85] JS：可选链
来源：http://zdb.pengpengdd.cyou

a?.b?.c
来源：http://ndh.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://tix.sufxvd.cn

a ?? b
来源：http://viw.fzhhl.top

[U87] JS：解构默认值
来源：http://nxt.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://wmm.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://kzz.uphjek.com

{ ...a, ...b }
来源：http://chl.zdbjq.cn

[U89] JS：数组去重
来源：http://jzl.zhiwuduotai.top

[...new Set(arr)]
来源：http://yoh.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://wxq.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://nhb.daria6918.cn

[U91] JS：对象键值遍历
来源：http://ldq.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://not.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://wks.bjfxy.top

structuredClone(obj)
来源：http://bxm.zhixingplan.top

[U93] JS：模板字符串
来源：http://euf.jqgfzy.top

`共 ${n} 条`
来源：http://xps.sufxvd.cn

[U94] JS：箭头函数
来源：http://iob.vqdsnc.cn

const double = x => x * 2;
来源：http://hfr.cdnleiting.top

[U95] JS：Promise 包装
来源：http://sgg.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://yvp.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://qin.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gwc.jlsjyb.cn

[U97] JS：并发请求
来源：http://dmg.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://vop.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://zlo.wangshuangyany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xnk.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://xaw.daria6918.cn

el.addEventListener("click", e => {})
来源：http://fwg.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://pwz.quarkkingdee.top

document.querySelector(".item")
来源：http://rfg.gaohongyu789.top

[U101] JS：classList 操作
来源：http://vsx.xuanzx.com

el.classList.toggle("active")
来源：http://xov.hywenlv.cn

[U102] JS：本地存储
来源：http://qoo.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ekk.daria6918.cn

[U103] JS：定时器
来源：http://amu.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dqm.gaohongyu789.top

[U104] JS：防抖
来源：http://kaq.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rio.mhx1999.top

[U105] JS：节流
来源：http://amo.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://usk.ehwqpu.com

[U106] JS：日期格式化
来源：http://tqa.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://knw.jyoumei.cn

[U107] JS：数字千分位
来源：http://tet.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ziu.ehwqpu.com

[U108] JS：随机整数
来源：http://ice.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tus.hnxiangtu.top

[U109] JS：数组分组
来源：http://vrs.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://fdv.yuxming.cn

[U110] JS：数组分块
来源：http://lmo.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gkq.redwolf501.top

[U111] JS：对象转 Map
来源：http://dvl.chenlongwang.top

new Map(Object.entries(obj))
来源：http://zwe.xuanzx.com

[U112] JS：字符串补位
来源：http://vwl.fktsv.cn

"7".padStart(3, "0")
来源：http://whf.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://mxw.cucudq.cn

s.replaceAll("a", "b")
来源：http://bav.yonumen.top

[U114] JS：JSON 深比较
来源：http://bli.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hgj.ydzc1.top

[U115] JS：生成 UUID
来源：http://bvp.havefunace.top

crypto.randomUUID()
来源：http://okh.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://dmd.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://vei.hywenlv.cn

[U117] JS：单元测试
来源：http://huo.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://kkn.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://dnm.yj202588.top

npm i -D vite;  npx vite
来源：http://ssm.quarkkingdee.top

[U119] JS：生产构建
来源：http://uyc.chenlongwang.top

npx vite build
来源：http://hnq.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://zys.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://itl.kuanghao11.cn

================================================================================
来源：http://fmx.shanyushiyangtech.top

统计汇总
来源：http://kzh.zdbjq.cn

================================================================================
来源：http://qst.andypj.xyz

按语言统计（条）：
来源：http://loj.316326.xyz

Python ......... 252
来源：http://moa.sxryk.cn

PHP ............ 252
来源：http://dmo.ppjwa.cn

JavaScript ..... 252
来源：http://spm.zhongyouzk.top

TypeScript ..... 212
来源：http://aas.gotoacloud.top

Java ........... 212
来源：http://rjf.fktsv.cn

Go ............. 212
来源：http://ejd.yueranfly.top

Ruby ........... 212
来源：http://awn.jyoumei.cn

C# ............. 212
来源：http://dst.epnwcf.com

C .............. 30
来源：http://kdp.iojbl.cn

C++ ............ 30
来源：http://sxw.jinqigfzy.top

SQL ............ 90
来源：http://dhe.ybcxt.top

Bash ........... 80
来源：http://uaq.sxryk.cn

Kotlin ......... 15
来源：http://nge.shanyushiyangkeji.top

Swift .......... 15
来源：http://hav.pycfn.com

Lua ............ 10
来源：http://tik.guannengcc.top

Perl ........... 10
来源：http://fkl.tanke756.top

Scala .......... 10
来源：http://lpm.shuidangran.top

------------------------------------
来源：http://ros.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://thb.sxryk.cn

按章节统计：
来源：http://chl.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nor.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cat.yvedp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ubl.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nmh.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sfc.meibo888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://trx.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ecn.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rfg.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gai.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mql.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://njk.yj20258.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wvw.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vpc.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uad.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qhp.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ose.hysaishi.cn

Q SQL 专题                              90
来源：http://njg.smart0.xyz

R Bash 专题                             80
来源：http://jur.ybcxt.top

S C / C++ 专题                          60
来源：http://mcv.chenzaomai.com

T 其他语言补充                          60
来源：http://ted.hywenlv.cn

U 高频实用片段                         120
来源：http://eat.redwolf501.top

------------------------------------
来源：http://vrk.zhongyouzk.top

合计                                  2106 条
来源：http://fke.havefunace.top

--------------------------------------------------------------------------------
来源：http://coi.tanke756.top

使用提醒
来源：http://ssd.aizwys.cn

--------------------------------------------------------------------------------
来源：http://plz.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bjv.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pwi.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ynh.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zkb.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cgs.meibo888.top

—— 文件结束 ——
来源：http://yfh.wangdashe.top

================================================================================
来源：http://got.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://nwv.zhongyouzk.top

Common Programming Examples Cheat Book
来源：http://fyv.aizwys.cn

================================================================================
来源：http://pov.9152youxi.cn

【收录内容】
来源：http://dls.uphjek.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://uth.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jyy.pycfn.com

SQL · Bash · C · C++
来源：http://vds.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lht.snrcjt.cn

【使用说明】
来源：http://lys.andypj.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ruy.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fop.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://paz.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aqz.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vhd.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nde.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://igz.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ndt.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lqz.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tva.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pvf.ydzc1.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ing.hysaishi.cn

【文件统计】
来源：http://jlu.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qus.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://xzj.bbcook.cn

目  录
来源：http://obg.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://hkn.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ikw.jinqigfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xuv.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qsd.hnxiangtu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xog.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yxq.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qah.ctjpmb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yjy.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vid.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qwe.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wgc.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oag.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://izs.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gml.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uvu.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pdl.aibaodan.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://she.yongpay.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wwv.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://usp.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fai.zhaomingkeji.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vud.sweek.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hjl.pycfn.com

================================================================================
来源：http://gnp.yongpay.top

A. 基础语法与类型
来源：http://opc.jlsjyb.cn

================================================================================
来源：http://ulf.daria6918.cn

[A01] Hello World
来源：http://rxa.52xcode.cn

Py:   print("Hello, World!")
来源：http://iax.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://bcu.uphjek.com

JS:   console.log("Hello, World!");
来源：http://ycq.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lct.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://ayu.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://lsc.havefunace.top

Ruby: puts "Hello, World!"
来源：http://eya.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ric.xuanzx.com

[A02] 变量声明与赋值
来源：http://taq.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uwh.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sbr.nwbrower.top

JS:   let name = "Alex"; const age = 20;
来源：http://bis.yvedp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wvu.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://egs.hcnkem.com

Go:   name := "Alex"; age := 20
来源：http://qrb.jinqigfzy.top

Ruby: name = "Alex"; age = 20
来源：http://vju.zycfv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://weg.wangshuangyany.cn

[A03] 常量定义
来源：http://fid.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://juj.gotoacloud.top

PHP:  const PI = 3.14159;
来源：http://xla.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://oqs.sjlbkw.cn

TS:   const PI: number = 3.14159;
来源：http://nrn.hfpthk.cn

Java: static final double PI = 3.14159;
来源：http://woo.jianghu66.top

Go:   const PI = 3.14159
来源：http://zhm.fehbvm.com

Ruby: PI = 3.14159
来源：http://jyx.gzhubu.top

C#:   const double PI = 3.14159;
来源：http://bbl.shzxlz.cn

[A04] 判断变量类型
来源：http://bjs.hnqzz.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://fqb.nwbrower.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zdr.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nvk.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://ckr.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ocm.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://kkb.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sgw.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://xhd.c1oappe.top

[A05] 整数除法与取模
来源：http://sds.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tyf.ybcxt.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xsk.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uiy.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hpq.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://qfh.wangshuangyany.cn

Go:   7 / 2; 7 % 2
来源：http://imx.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://wcb.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://uvd.zdbjq.cn

[A06] 字符串转数字
来源：http://dwb.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://fda.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pvn.vehdjk.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://odz.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://zvb.shuidangran.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://upt.sxryk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jpv.aizwys.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://llp.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jsh.aibaodan.cn

[A07] 数字转字符串
来源：http://sgm.zdqjudy.top

Py:   str(42)
来源：http://pik.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://lgt.redwolf501.top

JS:   String(42); (42).toString()
来源：http://xnj.zhongyouzk.top

TS:   String(42)
来源：http://cpl.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://hki.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://cmt.cqqwz.cn

Ruby: 42.to_s
来源：http://xci.chenjidiqi.icu

C#:   42.ToString()
来源：http://jam.ppjwa.cn

[A08] 取整与四舍五入
来源：http://job.havefunace.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tal.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hdv.ivvv.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sph.jqgufenzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ary.nanxuanxn.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://quv.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uml.haohaochexian.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hjp.sufxvd.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cde.zhijiandao.cn

[A09] 绝对值与最大最小值
来源：http://pmk.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vvr.andypj.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lvs.zhiwuduotai.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cbg.sysykeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ssy.yfazqb.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fxh.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uun.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vvg.smart0.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jph.cdnleiting.top

[A10] 生成随机数
来源：http://pps.316326.xyz

Py:   import random; random.randint(1, 100)
来源：http://ndx.zhijiandao.cn

PHP:  random_int(1, 100);
来源：http://tbj.tanke756.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wxl.hammf.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bns.mhx1999.top

Java: new Random().nextInt(100) + 1
来源：http://cyw.jinghuilouyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://srt.hammf.cn

Ruby: rand(1..100)
来源：http://uuu.tarul.cn

C#:   new Random().Next(1, 101)
来源：http://lup.cucudq.cn

[A11] 条件表达式（三元）
来源：http://tsu.gzhubu.top

Py:   "yes" if x > 0 else "no"
来源：http://yws.xinyue.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://pcv.uphjek.com

JS:   x > 0 ? "yes" : "no"
来源：http://zdy.9152youxi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pbo.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://khj.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://idp.kuanghao11.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kwn.jinyuanbaomall.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jag.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://hcy.xylfe.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rnw.sysykeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ewf.meibo888.top

JS:   `Hello, ${name}!`
来源：http://iuo.xuanzx.com

TS:   `Hello, ${name}!`
来源：http://lio.nanxinkj.top

Java: "Hello, %s!".formatted(name)
来源：http://olm.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wbp.nanxinkj.top

Ruby: "Hello, #{name}!"
来源：http://gni.tian-w.cn

C#:   $"Hello, {name}!"
来源：http://zte.jqgufenzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://sen.haohaochexian.top


<!-- 参考信息 -->