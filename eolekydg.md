代发 wailian999

[U77] PHP：模板渲染
来源：http://yvv.hcnkem.com

composer require twig/twig
来源：http://viv.316326.xyz

[U78] PHP：单元测试
来源：http://bxo.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://pec.zhijiandao.cn

[U79] PHP：静态分析
来源：http://kkk.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://kaj.vehdjk.com

[U80] PHP：代码规范修复
来源：http://oas.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tpm.xziqi.cn

[U81] JS：初始化项目
来源：http://bqv.yangfankeji.com

npm init -y;  npm i express
来源：http://nzi.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://xrp.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gzh.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://pto.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nso.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://jbq.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tca.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://tpg.tian-w.cn

a?.b?.c
来源：http://qcc.fehbvm.com

[U86] JS：空值合并
来源：http://qdc.meibo888.top

a ?? b
来源：http://igg.andypj.xyz

[U87] JS：解构默认值
来源：http://eti.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://kif.hammf.cn

[U88] JS：对象展开合并
来源：http://ljk.ivvv.top

{ ...a, ...b }
来源：http://sev.yj202588.top

[U89] JS：数组去重
来源：http://ars.xinyue.icu

[...new Set(arr)]
来源：http://tss.zycfv.cn

[U90] JS：数字数组排序
来源：http://npl.mhx1999.top

[...arr].sort((a, b) => a - b)
来源：http://tbb.fengsongda.top

[U91] JS：对象键值遍历
来源：http://tzv.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cat.ehwqpu.com

[U92] JS：深拷贝
来源：http://onz.ctjpmb.com

structuredClone(obj)
来源：http://rdf.havefunace.top

[U93] JS：模板字符串
来源：http://ibz.guowangkeji.top

`共 ${n} 条`
来源：http://krf.yj20258888.top

[U94] JS：箭头函数
来源：http://uox.quarkkingdee.top

const double = x => x * 2;
来源：http://clh.xziqi.cn

[U95] JS：Promise 包装
来源：http://lqx.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://agv.havefunace.top

[U96] JS：async/await 与异常
来源：http://muc.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iss.redwolf501.top

[U97] JS：并发请求
来源：http://ges.yj20258888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qnj.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://ybq.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fyt.52xcode.cn

[U99] JS：事件监听
来源：http://kli.nwbrower.top

el.addEventListener("click", e => {})
来源：http://hai.bjfxy.top

[U100] JS：DOM 查询
来源：http://utx.yuanzhike.top

document.querySelector(".item")
来源：http://kuw.guannengcc.top

[U101] JS：classList 操作
来源：http://kfu.cucudq.cn

el.classList.toggle("active")
来源：http://kad.wangdashe.top

[U102] JS：本地存储
来源：http://oqq.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nzd.pycfn.com

[U103] JS：定时器
来源：http://ezy.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ehp.mhx1999.top

[U104] JS：防抖
来源：http://doa.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://erk.guowangkeji.top

[U105] JS：节流
来源：http://mnq.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xtb.yuanzhike.top

[U106] JS：日期格式化
来源：http://ljp.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nub.shzxlz.cn

[U107] JS：数字千分位
来源：http://bxl.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xpb.hysaishi.cn

[U108] JS：随机整数
来源：http://lyr.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cfv.hfpthk.cn

[U109] JS：数组分组
来源：http://mxj.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://vvu.redwolf501.top

[U110] JS：数组分块
来源：http://htz.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qki.xinyue.icu

[U111] JS：对象转 Map
来源：http://kpv.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://hsv.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://ntz.yueranfly.top

"7".padStart(3, "0")
来源：http://rqo.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://lcd.yj20258.top

s.replaceAll("a", "b")
来源：http://goi.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://nok.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uwb.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://rmv.yuxming.cn

crypto.randomUUID()
来源：http://fln.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://hpd.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://dsv.zycfv.cn

[U117] JS：单元测试
来源：http://xzr.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://yss.316326.xyz

[U118] JS：开发服务器
来源：http://mdn.nwbrower.top

npm i -D vite;  npx vite
来源：http://tiy.kuanghao11.cn

[U119] JS：生产构建
来源：http://gxe.cashguo.top

npx vite build
来源：http://ufv.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://eci.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://hud.ywan-chungtsiang.top

================================================================================
来源：http://anm.sweek.top

统计汇总
来源：http://wcy.cashguo.top

================================================================================
来源：http://rzu.ppjwa.cn

按语言统计（条）：
来源：http://xsn.fanxiaobao.xyz

Python ......... 252
来源：http://cnt.sweek.top

PHP ............ 252
来源：http://xnj.pengpengdd.cyou

JavaScript ..... 252
来源：http://kja.xylfe.cn

TypeScript ..... 212
来源：http://lbp.zycfv.cn

Java ........... 212
来源：http://quz.xziqi.cn

Go ............. 212
来源：http://yzc.316326.xyz

Ruby ........... 212
来源：http://ybb.daxiang520.top

C# ............. 212
来源：http://pqq.ctjpmb.com

C .............. 30
来源：http://gxm.hywenlv.cn

C++ ............ 30
来源：http://dpf.pycfn.com

SQL ............ 90
来源：http://pwj.yonumen.top

Bash ........... 80
来源：http://teu.iojbl.cn

Kotlin ......... 15
来源：http://uel.feifeiyinyue.top

Swift .......... 15
来源：http://ohm.yj20258888.top

Lua ............ 10
来源：http://ltz.havefunace.top

Perl ........... 10
来源：http://rmp.iojbl.cn

Scala .......... 10
来源：http://qjs.daxiang520.top

------------------------------------
来源：http://cgo.cqqwz.cn

合计 ........... 2106 条
来源：http://wdw.shuidangran.top

按章节统计：
来源：http://dcs.gaohongyu789.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hso.yj20258888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yly.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uua.hnqzz.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gxc.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oec.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://asg.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vzn.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gtw.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gch.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fso.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rdc.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zgx.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hds.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wph.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://emb.vqdsnc.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aqf.andypj.xyz

Q SQL 专题                              90
来源：http://dnb.hywenlv.cn

R Bash 专题                             80
来源：http://llt.andypj.xyz

S C / C++ 专题                          60
来源：http://cnc.yj20258888.top

T 其他语言补充                          60
来源：http://zqb.andypj.xyz

U 高频实用片段                         120
来源：http://mmk.yueranfly.top

------------------------------------
来源：http://xyi.sweek.top

合计                                  2106 条
来源：http://owk.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://mxr.shuidangran.top

使用提醒
来源：http://bvy.c1oappe.top

--------------------------------------------------------------------------------
来源：http://xei.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fxy.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vmp.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://woy.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kri.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mox.ydjk.org.cn

—— 文件结束 ——
来源：http://vph.316326.xyz

================================================================================
来源：http://rkg.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://rhi.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://avc.gogol.net.cn

================================================================================
来源：http://wjy.shuidangran.top

【收录内容】
来源：http://cyq.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://biu.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bjj.ctjpmb.com

SQL · Bash · C · C++
来源：http://mlb.wangdashe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kai.shzxlz.cn

【使用说明】
来源：http://wcn.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rnx.tian-w.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mog.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://noj.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rqv.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dxj.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fxb.hammf.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dmw.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jhr.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://div.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sux.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://twi.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dax.sufxvd.cn

【文件统计】
来源：http://xap.andypj.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://evg.havefunace.top

--------------------------------------------------------------------------------
来源：http://sdy.aizwys.cn

目  录
来源：http://opf.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://cqo.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qiw.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iyy.c1oappe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hzf.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vuk.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://skz.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gne.0kj1m.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hci.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zdt.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ayj.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://suy.zycfv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lab.daria6918.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gyi.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://srl.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nus.uphjek.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jmy.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yck.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rnr.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kad.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uuu.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eky.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yne.cucudq.cn

================================================================================
来源：http://ksv.hywenlv.cn

A. 基础语法与类型
来源：http://zpf.zhiwuduotai.top

================================================================================
来源：http://eih.316326.xyz

[A01] Hello World
来源：http://gsy.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://yyf.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://opy.aibaodan.cn

JS:   console.log("Hello, World!");
来源：http://ooh.hysaishi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ybj.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://qwz.zhijiandao.cn

Go:   fmt.Println("Hello, World!")
来源：http://jad.haohaochexian.top

Ruby: puts "Hello, World!"
来源：http://rhm.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ihn.snrcjt.cn

[A02] 变量声明与赋值
来源：http://snc.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xfs.wangdashe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hcv.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://zue.jianghu66.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ydu.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://qto.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://rxo.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://ghz.fehbvm.com

C#:   string name = "Alex"; int age = 20;
来源：http://ymu.hesvh.cn

[A03] 常量定义
来源：http://waw.fktsv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tzg.zhongyouzk.top

PHP:  const PI = 3.14159;
来源：http://gkr.c1oappe.top

JS:   const PI = 3.14159;
来源：http://eqm.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://eir.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://tck.nanxuanxn.top

Go:   const PI = 3.14159
来源：http://yog.birdmap.top

Ruby: PI = 3.14159
来源：http://ceo.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://qjo.cdnleiting.top

[A04] 判断变量类型
来源：http://oqo.zhengqikj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pfu.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qju.shanyushiyangtech.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mxk.shanyushiyangtech.top

TS:   typeof x; x instanceof Date
来源：http://pwg.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dji.yanxiufei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://htv.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://jmb.yongpay.top

C#:   x.GetType().Name; x is int
来源：http://pfq.tian-w.cn

[A05] 整数除法与取模
来源：http://ysy.gzhubu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ozs.kuanghao11.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tjt.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fhv.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://crs.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://rej.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://cxh.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://bxs.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://kyi.bjfxy.top

[A06] 字符串转数字
来源：http://tck.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://kox.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wpn.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rqq.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://swn.zhengqikj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://odi.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kai.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bpl.wangdashe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wef.ydzc1.top

[A07] 数字转字符串
来源：http://tgd.aizwys.cn

Py:   str(42)
来源：http://rca.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://kjx.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://dtj.yueranfly.top

TS:   String(42)
来源：http://iqd.jlsjyb.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uvp.zhongyouzk.top

Go:   strconv.Itoa(42)
来源：http://cvf.zycfv.cn

Ruby: 42.to_s
来源：http://dtt.sysykeji.top

C#:   42.ToString()
来源：http://sqt.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://wji.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fuf.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vmu.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jtd.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ima.hywenlv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ywe.yongpay.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pnb.shuidangran.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://itc.ppjwa.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://far.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://jzj.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pxm.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vkl.cqqwz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kln.sweek.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mlj.c1oappe.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zqd.jinqigfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pma.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wzj.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jnm.fzhhl.top

[A10] 生成随机数
来源：http://nfa.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://cgs.ehwqpu.com

PHP:  random_int(1, 100);
来源：http://mum.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bct.hnxiangtu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tli.hnxiangtu.top

Java: new Random().nextInt(100) + 1
来源：http://jim.yonumen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dhf.cashguo.top

Ruby: rand(1..100)
来源：http://soe.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://kqs.yj202588.top

[A11] 条件表达式（三元）
来源：http://pni.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://ymq.fanxiaobao.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ufv.52xcode.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cxc.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ghn.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://ykb.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://txd.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zhs.daxiang520.top

C#:   x > 0 ? "yes" : "no"
来源：http://pyn.jqgufenzy.top

[A12] 字符串插值 / 格式化
来源：http://wur.andypj.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pzp.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hxp.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://kei.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://fuf.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://rhb.haohaochexian.top


<!-- 参考信息 -->