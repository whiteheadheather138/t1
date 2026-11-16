代发 wailian999

[U77] PHP：模板渲染
来源：http://uzw.dianchejie.cn

composer require twig/twig
来源：http://sso.jinqigfzy.top

[U78] PHP：单元测试
来源：http://lpy.yj20258.top

composer require --dev phpunit/phpunit
来源：http://umb.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://nie.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://wyu.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://nst.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gew.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://dfr.gzhubu.top

npm init -y;  npm i express
来源：http://vxy.yvedp.cn

[U82] JS：package.json 脚本
来源：http://soh.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dyy.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://qwi.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://neg.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://got.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iro.gotoacloud.top

[U85] JS：可选链
来源：http://sjf.fktsv.cn

a?.b?.c
来源：http://aqg.yongpay.top

[U86] JS：空值合并
来源：http://yrj.yj202588.top

a ?? b
来源：http://xyg.sjlbkw.cn

[U87] JS：解构默认值
来源：http://paa.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://ojs.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://utt.jinghuilouyu.cn

{ ...a, ...b }
来源：http://bwc.jinghuilouyu.cn

[U89] JS：数组去重
来源：http://nsb.zhixingplan.top

[...new Set(arr)]
来源：http://cud.smart0.xyz

[U90] JS：数字数组排序
来源：http://umc.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://ymr.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://zvb.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uer.bbcook.cn

[U92] JS：深拷贝
来源：http://dvh.uphjek.com

structuredClone(obj)
来源：http://ekt.birdmap.top

[U93] JS：模板字符串
来源：http://uzr.epnwcf.com

`共 ${n} 条`
来源：http://zjx.yuxming.cn

[U94] JS：箭头函数
来源：http://art.fanxiaobao.xyz

const double = x => x * 2;
来源：http://zuf.xinyue.icu

[U95] JS：Promise 包装
来源：http://wen.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://cih.hammf.cn

[U96] JS：async/await 与异常
来源：http://qkz.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zkh.xziqi.cn

[U97] JS：并发请求
来源：http://vex.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vsi.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://vjg.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ctm.hongshengwenyu.top

[U99] JS：事件监听
来源：http://rbc.yj20258.top

el.addEventListener("click", e => {})
来源：http://cvq.ppjwa.cn

[U100] JS：DOM 查询
来源：http://dtz.shzxlz.cn

document.querySelector(".item")
来源：http://ytn.hywenlv.cn

[U101] JS：classList 操作
来源：http://ouu.feifeiyinyue.top

el.classList.toggle("active")
来源：http://fbi.ppjwa.cn

[U102] JS：本地存储
来源：http://ehw.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mgt.xylfe.cn

[U103] JS：定时器
来源：http://duc.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zub.epnwcf.com

[U104] JS：防抖
来源：http://bni.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ulm.yueranfly.top

[U105] JS：节流
来源：http://bav.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bqc.guannengcc.top

[U106] JS：日期格式化
来源：http://hgc.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://txt.nwbrower.top

[U107] JS：数字千分位
来源：http://rjm.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ldq.shangyingyoupin.top

[U108] JS：随机整数
来源：http://qqc.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://igm.dianchejie.cn

[U109] JS：数组分组
来源：http://ewf.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://qaq.cashguo.top

[U110] JS：数组分块
来源：http://njk.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gqk.vehdjk.com

[U111] JS：对象转 Map
来源：http://maa.cashguo.top

new Map(Object.entries(obj))
来源：http://pcm.cashguo.top

[U112] JS：字符串补位
来源：http://cwt.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://ati.yj20258888.top

[U113] JS：正则替换全部
来源：http://gbj.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://dol.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://vof.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fli.xinyue.icu

[U115] JS：生成 UUID
来源：http://ykn.daria6918.cn

crypto.randomUUID()
来源：http://fdw.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://qtm.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://qpe.snrcjt.cn

[U117] JS：单元测试
来源：http://ojc.yj202588.top

npm i -D vitest;  npx vitest
来源：http://xud.tarul.cn

[U118] JS：开发服务器
来源：http://aab.zhengqikj.top

npm i -D vite;  npx vite
来源：http://ory.52xcode.cn

[U119] JS：生产构建
来源：http://een.daria6918.cn

npx vite build
来源：http://bfj.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://gfv.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://etf.mhx1999.top

================================================================================
来源：http://oad.havefunace.top

统计汇总
来源：http://vxj.shzxlz.cn

================================================================================
来源：http://pgr.yj202588.top

按语言统计（条）：
来源：http://kmx.shangyingyoupin.top

Python ......... 252
来源：http://zfb.yvedp.cn

PHP ............ 252
来源：http://vna.ivvv.top

JavaScript ..... 252
来源：http://wad.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://jaz.chenlongwang.top

Java ........... 212
来源：http://box.jinyuanbaomall.cn

Go ............. 212
来源：http://yly.svipenyu.cn

Ruby ........... 212
来源：http://vtc.yangfankeji.com

C# ............. 212
来源：http://lda.sxryk.cn

C .............. 30
来源：http://iqo.yuxming.cn

C++ ............ 30
来源：http://kig.vehdjk.com

SQL ............ 90
来源：http://dhb.fzhhl.top

Bash ........... 80
来源：http://ayr.aizwys.cn

Kotlin ......... 15
来源：http://iyr.tianlin.xyz

Swift .......... 15
来源：http://otf.ehwqpu.com

Lua ............ 10
来源：http://bhv.yangfankeji.com

Perl ........... 10
来源：http://aet.chenzaomai.com

Scala .......... 10
来源：http://gjl.fehbvm.com

------------------------------------
来源：http://nzt.vqdsnc.cn

合计 ........... 2106 条
来源：http://ika.guowangkeji.top

按章节统计：
来源：http://ecs.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hba.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dju.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fmr.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oqw.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xki.zhiwuduotai.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sow.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nyk.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://svv.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qeq.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wdh.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hqo.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ghm.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fqz.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ejr.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bkc.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dnn.zhijiandao.cn

Q SQL 专题                              90
来源：http://wka.jinqigfzy.top

R Bash 专题                             80
来源：http://loi.fengsongda.top

S C / C++ 专题                          60
来源：http://dvc.gotoacloud.top

T 其他语言补充                          60
来源：http://spe.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://wyi.zhiwuduotai.top

------------------------------------
来源：http://dnc.birdmap.top

合计                                  2106 条
来源：http://tkt.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://hqz.chenlongwang.top

使用提醒
来源：http://rfl.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://dvw.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://koq.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ims.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://awo.jqgfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hax.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wer.dashuyun.cn

—— 文件结束 ——
来源：http://oit.xuetiantiany.cn

================================================================================
来源：http://pmr.cashguo.top

程序语言常见例子速查手册（2024 版）
来源：http://afm.sysykeji.top

Common Programming Examples Cheat Book
来源：http://ecm.nanxuanxn.top

================================================================================
来源：http://ggm.yongpay.top

【收录内容】
来源：http://cfa.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dbv.mhx1999.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dxm.ybcxt.top

SQL · Bash · C · C++
来源：http://euz.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fad.fktsv.cn

【使用说明】
来源：http://mvc.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qho.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://swk.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://god.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://csz.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ecg.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yws.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tlp.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eds.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cjs.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nyo.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ppd.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tfd.sxryk.cn

【文件统计】
来源：http://dbs.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nyg.havefunace.top

--------------------------------------------------------------------------------
来源：http://lou.jqgfzy.top

目  录
来源：http://bqq.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://svu.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lmh.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wtu.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fnt.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bxx.vehdjk.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ztb.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aem.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xpz.hywenlv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cqx.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tuc.zhengqikj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hdf.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tyr.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://enh.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zul.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uiq.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iuy.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kjt.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wcr.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oqj.ppjwa.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ivc.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ioa.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lxv.yongpay.top

================================================================================
来源：http://wdn.pengpengdd.cyou

A. 基础语法与类型
来源：http://gdc.jyoumei.cn

================================================================================
来源：http://xht.tian-w.cn

[A01] Hello World
来源：http://baa.shanyushiyangkeji.top

Py:   print("Hello, World!")
来源：http://srf.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://uln.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://yvz.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zsm.fanxiaobao.xyz

Java: System.out.println("Hello, World!");
来源：http://zab.zhixingplan.top

Go:   fmt.Println("Hello, World!")
来源：http://ieo.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://tdo.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://djn.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://flo.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fjm.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://wif.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://azg.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pqk.daxiang520.top

Java: String name = "Alex"; int age = 20;
来源：http://vqe.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://lhi.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://emq.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lre.aizwys.cn

[A03] 常量定义
来源：http://csk.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iye.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://ols.sjlbkw.cn

JS:   const PI = 3.14159;
来源：http://geb.yueranfly.top

TS:   const PI: number = 3.14159;
来源：http://bdh.chenlongwang.top

Java: static final double PI = 3.14159;
来源：http://rua.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://inc.xinyue.icu

Ruby: PI = 3.14159
来源：http://mef.zhoulong.xyz

C#:   const double PI = 3.14159;
来源：http://wlc.ctjpmb.com

[A04] 判断变量类型
来源：http://oaj.feifeiyinyue.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ohj.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pfr.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hwl.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://qhc.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fft.9152youxi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bom.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jsh.guowangkeji.top

C#:   x.GetType().Name; x is int
来源：http://hlc.ywan-chungtsiang.top

[A05] 整数除法与取模
来源：http://vof.jianghu66.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vjk.havefunace.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jfq.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xdx.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nfw.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://dkc.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://xtv.hnqzz.top

Ruby: 7 / 2; 7 % 2
来源：http://muj.fktsv.cn

C#:   7 / 2; 7 % 2
来源：http://wac.tanke756.top

[A06] 字符串转数字
来源：http://tjl.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://zzx.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rzp.sufxvd.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lbh.vehdjk.com

TS:   parseInt("42", 10); Number("42")
来源：http://asg.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ccm.pycfn.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ugh.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://evu.yj20258888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uco.hnqzz.top

[A07] 数字转字符串
来源：http://zfy.hesvh.cn

Py:   str(42)
来源：http://zcc.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://qud.guannengcc.top

JS:   String(42); (42).toString()
来源：http://lxx.tianlin.xyz

TS:   String(42)
来源：http://wvm.hnqzz.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oxz.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://rap.yj20258888.top

Ruby: 42.to_s
来源：http://kgm.iojbl.cn

C#:   42.ToString()
来源：http://jyk.zhongyouzk.top

[A08] 取整与四舍五入
来源：http://jpy.vqdsnc.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bkg.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jsp.chenjidiqi.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sxh.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vgs.aizwys.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hqb.hfpthk.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nkg.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yva.dianchejie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iyc.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://hue.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gel.yj20258888.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://prk.0kj1m.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jxg.nwbrower.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://znd.feifeiyinyue.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://doc.sysykeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zbn.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ekx.ydjk.org.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://upu.jqgufenzy.top

[A10] 生成随机数
来源：http://iaq.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://biv.cqqwz.cn

PHP:  random_int(1, 100);
来源：http://qwr.yvedp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mkv.52xcode.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://scl.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://tcr.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wrd.aizwys.cn

Ruby: rand(1..100)
来源：http://blo.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://fel.xingfuxueyuan.xyz

[A11] 条件表达式（三元）
来源：http://zmm.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://xsg.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ytn.vqdsnc.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jxi.epnwcf.com

TS:   x > 0 ? "yes" : "no"
来源：http://qrw.pycfn.com

Java: x > 0 ? "yes" : "no"
来源：http://lrx.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yau.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://otc.bjfxy.top

C#:   x > 0 ? "yes" : "no"
来源：http://mgk.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://lzz.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dvh.aibaodan.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pau.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://mmn.sufxvd.cn

TS:   `Hello, ${name}!`
来源：http://rgu.iojbl.cn

Java: "Hello, %s!".formatted(name)
来源：http://mbe.yj20258.top


<!-- 参考信息 -->