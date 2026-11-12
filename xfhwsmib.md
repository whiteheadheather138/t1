代发 wailian999

[U79] PHP：静态分析
来源：http://kzl.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://yng.xuanzx.com

[U80] PHP：代码规范修复
来源：http://nqd.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://mht.yfazqb.com

[U81] JS：初始化项目
来源：http://qkb.fzhhl.top

npm init -y;  npm i express
来源：http://kim.yongpay.top

[U82] JS：package.json 脚本
来源：http://qad.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://glp.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://jla.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://aew.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://lve.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ham.kuanghao11.cn

[U85] JS：可选链
来源：http://nnx.hammf.cn

a?.b?.c
来源：http://zet.tianlin.xyz

[U86] JS：空值合并
来源：http://waz.epnwcf.com

a ?? b
来源：http://wjw.jlsjyb.cn

[U87] JS：解构默认值
来源：http://bpe.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://qzi.9152youxi.cn

[U88] JS：对象展开合并
来源：http://zbo.pycfn.com

{ ...a, ...b }
来源：http://vpj.fktsv.cn

[U89] JS：数组去重
来源：http://dzg.jqgfzy.top

[...new Set(arr)]
来源：http://yca.hysaishi.cn

[U90] JS：数字数组排序
来源：http://yyx.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://zce.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://bke.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cig.sxryk.cn

[U92] JS：深拷贝
来源：http://rvs.wangdashe.top

structuredClone(obj)
来源：http://ebv.guannengcc.top

[U93] JS：模板字符串
来源：http://epw.fengsongda.top

`共 ${n} 条`
来源：http://eqg.ppjwa.cn

[U94] JS：箭头函数
来源：http://zlz.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://gjb.havefunace.top

[U95] JS：Promise 包装
来源：http://krv.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://xab.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://jmy.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xzx.xuetiantiany.cn

[U97] JS：并发请求
来源：http://gmq.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tts.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://qua.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aey.sxryk.cn

[U99] JS：事件监听
来源：http://jrl.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://zfx.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://jyd.yj20258.top

document.querySelector(".item")
来源：http://flz.xziqi.cn

[U101] JS：classList 操作
来源：http://qcf.hammf.cn

el.classList.toggle("active")
来源：http://svg.hnqzz.top

[U102] JS：本地存储
来源：http://xni.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mqz.316326.xyz

[U103] JS：定时器
来源：http://zpn.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aij.smart0.xyz

[U104] JS：防抖
来源：http://emg.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtn.hammf.cn

[U105] JS：节流
来源：http://vrn.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ywe.guowangkeji.top

[U106] JS：日期格式化
来源：http://tqf.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zov.gzhubu.top

[U107] JS：数字千分位
来源：http://zbo.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uli.cqqwz.cn

[U108] JS：随机整数
来源：http://tix.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aqz.xziqi.cn

[U109] JS：数组分组
来源：http://sce.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://ymd.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://yta.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dtz.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://kxe.mhx1999.top

new Map(Object.entries(obj))
来源：http://ayi.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://gvl.xinyue.icu

"7".padStart(3, "0")
来源：http://iqm.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://hyc.ppjwa.cn

s.replaceAll("a", "b")
来源：http://tle.epnwcf.com

[U114] JS：JSON 深比较
来源：http://nnc.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cwv.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://aon.cucudq.cn

crypto.randomUUID()
来源：http://cbr.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://vcd.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://xco.shzxlz.cn

[U117] JS：单元测试
来源：http://iti.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://myb.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://msj.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://evt.yfazqb.com

[U119] JS：生产构建
来源：http://yem.chenlongwang.top

npx vite build
来源：http://vkx.smart0.xyz

[U120] JS：读取环境变量（Vite）
来源：http://zqs.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://zlv.ctjpmb.com

================================================================================
来源：http://lzb.jqgfzy.top

统计汇总
来源：http://ova.fanxiaobao.xyz

================================================================================
来源：http://gzl.tian-w.cn

按语言统计（条）：
来源：http://pgp.hywenlv.cn

Python ......... 252
来源：http://shk.yueranfly.top

PHP ............ 252
来源：http://npy.shzxlz.cn

JavaScript ..... 252
来源：http://zhd.fktsv.cn

TypeScript ..... 212
来源：http://bid.guowangkeji.top

Java ........... 212
来源：http://yoo.aizwys.cn

Go ............. 212
来源：http://nwj.vqdsnc.cn

Ruby ........... 212
来源：http://kfn.nwbrower.top

C# ............. 212
来源：http://yzb.zhijiandao.cn

C .............. 30
来源：http://sdb.yuanzhike.top

C++ ............ 30
来源：http://xia.chenzaomai.com

SQL ............ 90
来源：http://uwh.yangfankeji.com

Bash ........... 80
来源：http://vli.tanke756.top

Kotlin ......... 15
来源：http://sry.hysaishi.cn

Swift .......... 15
来源：http://wok.gaohongyu789.top

Lua ............ 10
来源：http://vmu.sysykeji.top

Perl ........... 10
来源：http://gvd.pycfn.com

Scala .......... 10
来源：http://leg.yvedp.cn

------------------------------------
来源：http://wor.snrcjt.cn

合计 ........... 2106 条
来源：http://hbi.hywenlv.cn

按章节统计：
来源：http://uyp.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lrm.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://njt.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ewu.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ghk.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iay.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gsj.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oef.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wuv.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zzr.nwbrower.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cjr.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mjf.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rdf.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yuh.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kiy.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://unk.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zdp.fengsongda.top

Q SQL 专题                              90
来源：http://pps.yueranfly.top

R Bash 专题                             80
来源：http://bbr.shuidangran.top

S C / C++ 专题                          60
来源：http://yaq.redwolf501.top

T 其他语言补充                          60
来源：http://sor.pengpengdd.cyou

U 高频实用片段                         120
来源：http://tgw.quarkkingdee.top

------------------------------------
来源：http://dka.ehwqpu.com

合计                                  2106 条
来源：http://smo.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://gsv.mhx1999.top

使用提醒
来源：http://gpv.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://fot.zhoulong.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://elw.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lcu.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fmc.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://loy.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://urf.cucudq.cn

—— 文件结束 ——
来源：http://oez.quarkkingdee.top

================================================================================
来源：http://vlt.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://muu.ivvv.top

Common Programming Examples Cheat Book
来源：http://nai.yanxiufei.cn

================================================================================
来源：http://xad.cucudq.cn

【收录内容】
来源：http://euk.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bav.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rao.tanke756.top

SQL · Bash · C · C++
来源：http://vyf.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nim.zhaomingkeji.xyz

【使用说明】
来源：http://onr.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jku.pengpengdd.cyou

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rgd.sufxvd.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fls.nanxuanxn.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://psj.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cdz.yonumen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lcr.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://exv.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zkq.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lbt.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cvj.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tjv.yj202588.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qso.ppjwa.cn

【文件统计】
来源：http://qly.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hse.tarul.cn

--------------------------------------------------------------------------------
来源：http://uxy.jinqigfzy.top

目  录
来源：http://hkm.sxryk.cn

--------------------------------------------------------------------------------
来源：http://psi.sweek.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hiq.ywan-chungtsiang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bic.zhengqikj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nko.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dni.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ddj.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dsv.hfpthk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nri.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://csr.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yeq.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mng.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kvj.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gpb.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bxo.nanxinkj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ews.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vkm.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jrp.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lml.tanke756.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vhm.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cke.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhr.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rlm.xuanzx.com

================================================================================
来源：http://pxp.dianchejie.cn

A. 基础语法与类型
来源：http://sfe.yfazqb.com

================================================================================
来源：http://ryf.52xcode.cn

[A01] Hello World
来源：http://cio.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://opd.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://wzm.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://ynb.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ups.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://kox.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://eks.jinghuilouyu.cn

Ruby: puts "Hello, World!"
来源：http://fda.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fsg.52xcode.cn

[A02] 变量声明与赋值
来源：http://zid.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rxg.kuanghao11.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sls.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://dzf.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://chn.xuanzx.com

Java: String name = "Alex"; int age = 20;
来源：http://mpo.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://ocg.jqgfzy.top

Ruby: name = "Alex"; age = 20
来源：http://kib.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fag.bjfxy.top

[A03] 常量定义
来源：http://mhx.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yiz.aizwys.cn

PHP:  const PI = 3.14159;
来源：http://bjp.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://mxx.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://rfg.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://ppj.yj202588.top

Go:   const PI = 3.14159
来源：http://ahn.fengsongda.top

Ruby: PI = 3.14159
来源：http://mkb.yuanzhike.top

C#:   const double PI = 3.14159;
来源：http://wih.cashguo.top

[A04] 判断变量类型
来源：http://csd.meibo888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mgy.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cqq.zhaomingkeji.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blp.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://lbp.zhiwuduotai.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://btk.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ghw.yj20258888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xda.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://anb.hywenlv.cn

[A05] 整数除法与取模
来源：http://civ.jinqigfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gac.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ebg.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vbx.shangyingyoupin.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uxt.hywenlv.cn

Java: 7 / 2; 7 % 2
来源：http://uxm.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://uar.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://kcy.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://byl.chenzaomai.com

[A06] 字符串转数字
来源：http://ekx.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://lqz.cucudq.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ndw.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ntz.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://ilc.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ceu.feifeiyinyue.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hwy.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pon.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sje.jianghu66.top

[A07] 数字转字符串
来源：http://pvh.316326.xyz

Py:   str(42)
来源：http://zne.ydzc1.top

PHP:  (string) 42; strval(42)
来源：http://axt.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://zjp.aizwys.cn

TS:   String(42)
来源：http://srd.guannengcc.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://okf.sysykeji.top

Go:   strconv.Itoa(42)
来源：http://jrm.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://yvj.tanke756.top

C#:   42.ToString()
来源：http://pla.svipenyu.cn

[A08] 取整与四舍五入
来源：http://lpe.xziqi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oja.hywenlv.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aoc.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gmt.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://arg.yj20258888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qzm.jinqigfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xnk.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hem.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://buw.quarkkingdee.top

[A09] 绝对值与最大最小值
来源：http://daq.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vkc.yj20258888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vrz.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mge.daxiang520.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nlt.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mlo.yueranfly.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gqr.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vay.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xpt.cashguo.top

[A10] 生成随机数
来源：http://ltk.redwolf501.top

Py:   import random; random.randint(1, 100)
来源：http://zqu.hcnkem.com

PHP:  random_int(1, 100);
来源：http://nzg.zycfv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lxc.xziqi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zvq.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://tai.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zzd.hysaishi.cn

Ruby: rand(1..100)
来源：http://dvi.pengpengdd.cyou

C#:   new Random().Next(1, 101)
来源：http://uee.ywan-chungtsiang.top

[A11] 条件表达式（三元）
来源：http://rvo.xuetiantiany.cn

Py:   "yes" if x > 0 else "no"
来源：http://yoi.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fgv.shangyingyoupin.top

JS:   x > 0 ? "yes" : "no"
来源：http://cdo.jqgufenzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://vcb.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://fkz.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jkb.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ltr.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gzd.gotoacloud.top

[A12] 字符串插值 / 格式化
来源：http://gfq.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qqb.zhaomingkeji.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://quz.cheryme.top

JS:   `Hello, ${name}!`
来源：http://van.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://wda.yuanzhike.top

Java: "Hello, %s!".formatted(name)
来源：http://sum.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wrd.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://abs.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://ojr.vqdsnc.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zsm.jinqigfzy.top


<!-- 参考信息 -->