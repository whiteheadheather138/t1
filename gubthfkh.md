代发 wailian999

[U79] PHP：静态分析
来源：http://bpf.uphjek.com

composer require --dev phpstan/phpstan
来源：http://jwk.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://hqj.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://gev.fengsongda.top

[U81] JS：初始化项目
来源：http://utf.zdbjq.cn

npm init -y;  npm i express
来源：http://xbj.sweek.top

[U82] JS：package.json 脚本
来源：http://hml.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sum.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://ubv.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pfy.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://ise.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://vvd.jianghu66.top

[U85] JS：可选链
来源：http://oty.dianchejie.cn

a?.b?.c
来源：http://cob.yueranfly.top

[U86] JS：空值合并
来源：http://ldq.sweek.top

a ?? b
来源：http://vli.ydjk.org.cn

[U87] JS：解构默认值
来源：http://nxb.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://sgm.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://nap.yanxiufei.cn

{ ...a, ...b }
来源：http://smk.fktsv.cn

[U89] JS：数组去重
来源：http://ppe.daxiang520.top

[...new Set(arr)]
来源：http://rjn.andypj.xyz

[U90] JS：数字数组排序
来源：http://xje.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://pll.fzhhl.top

[U91] JS：对象键值遍历
来源：http://ltn.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wyi.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://nai.guannengcc.top

structuredClone(obj)
来源：http://rhz.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://daj.xziqi.cn

`共 ${n} 条`
来源：http://rmt.cqqwz.cn

[U94] JS：箭头函数
来源：http://idm.yongpay.top

const double = x => x * 2;
来源：http://lrg.nwbrower.top

[U95] JS：Promise 包装
来源：http://zap.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://qfb.tanke756.top

[U96] JS：async/await 与异常
来源：http://jlh.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://giv.sjlbkw.cn

[U97] JS：并发请求
来源：http://czs.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xzm.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://dre.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eal.0kj1m.cn

[U99] JS：事件监听
来源：http://kqn.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://hlx.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://kbp.xylfe.cn

document.querySelector(".item")
来源：http://xvw.iojbl.cn

[U101] JS：classList 操作
来源：http://zii.vehdjk.com

el.classList.toggle("active")
来源：http://qdn.jinqigfzy.top

[U102] JS：本地存储
来源：http://cfk.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vua.aibaodan.cn

[U103] JS：定时器
来源：http://mwi.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wxx.shangyingyoupin.top

[U104] JS：防抖
来源：http://gjd.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ouq.smart0.xyz

[U105] JS：节流
来源：http://sku.gzhubu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xqy.vqdsnc.cn

[U106] JS：日期格式化
来源：http://yxo.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dia.9152youxi.cn

[U107] JS：数字千分位
来源：http://org.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zio.jianghu66.top

[U108] JS：随机整数
来源：http://jgt.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jzo.cashguo.top

[U109] JS：数组分组
来源：http://iqk.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://dpi.jyoumei.cn

[U110] JS：数组分块
来源：http://ltq.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vxe.yj20258888.top

[U111] JS：对象转 Map
来源：http://yuo.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://igv.quarkkingdee.top

[U112] JS：字符串补位
来源：http://kqc.fengsongda.top

"7".padStart(3, "0")
来源：http://yfu.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://oyl.c1oappe.top

s.replaceAll("a", "b")
来源：http://dwh.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://rgh.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dnb.cheryme.top

[U115] JS：生成 UUID
来源：http://ovn.ybcxt.top

crypto.randomUUID()
来源：http://joa.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://fle.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://hop.ppjwa.cn

[U117] JS：单元测试
来源：http://box.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://egy.xinyue.icu

[U118] JS：开发服务器
来源：http://ncb.iojbl.cn

npm i -D vite;  npx vite
来源：http://pdo.pengpengdd.cyou

[U119] JS：生产构建
来源：http://btx.hywenlv.cn

npx vite build
来源：http://jum.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://dxj.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://jhy.daria6918.cn

================================================================================
来源：http://xlf.yfazqb.com

统计汇总
来源：http://lor.hysaishi.cn

================================================================================
来源：http://nap.fehbvm.com

按语言统计（条）：
来源：http://nsm.yueranfly.top

Python ......... 252
来源：http://wsy.aizwys.cn

PHP ............ 252
来源：http://mju.jqgufenzy.top

JavaScript ..... 252
来源：http://zlu.pycfn.com

TypeScript ..... 212
来源：http://tgy.xylfe.cn

Java ........... 212
来源：http://brw.jianghu66.top

Go ............. 212
来源：http://wur.andypj.xyz

Ruby ........... 212
来源：http://ccb.cdnleiting.top

C# ............. 212
来源：http://guf.316326.xyz

C .............. 30
来源：http://vel.quarkkingdee.top

C++ ............ 30
来源：http://fgf.daria6918.cn

SQL ............ 90
来源：http://syn.52xcode.cn

Bash ........... 80
来源：http://sxu.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://adt.snrcjt.cn

Swift .......... 15
来源：http://sbt.chenlongwang.top

Lua ............ 10
来源：http://ihj.jinghuilouyu.cn

Perl ........... 10
来源：http://bkx.pycfn.com

Scala .......... 10
来源：http://okr.daxiang520.top

------------------------------------
来源：http://fbv.yanxiufei.cn

合计 ........... 2106 条
来源：http://xds.yueranfly.top

按章节统计：
来源：http://saw.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://udk.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tlv.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fti.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zfu.xylfe.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fgf.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nla.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xag.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cch.nwbrower.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qzq.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bml.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://snu.hesvh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ncj.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vbf.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://swr.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xsg.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jyf.yvedp.cn

Q SQL 专题                              90
来源：http://cyd.fzhhl.top

R Bash 专题                             80
来源：http://evd.jinqigfzy.top

S C / C++ 专题                          60
来源：http://ylr.meibo888.top

T 其他语言补充                          60
来源：http://can.zhiwuduotai.top

U 高频实用片段                         120
来源：http://qbl.meibo888.top

------------------------------------
来源：http://aud.jinqigfzy.top

合计                                  2106 条
来源：http://bfn.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://tdr.wangshuangyany.cn

使用提醒
来源：http://rjt.yj202588.top

--------------------------------------------------------------------------------
来源：http://rlm.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hkq.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rml.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tev.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tka.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://luw.bjfxy.top

—— 文件结束 ——
来源：http://xws.zhoulong.xyz

================================================================================
来源：http://obn.jqgfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://mxr.zycfv.cn

Common Programming Examples Cheat Book
来源：http://aug.zhijiandao.cn

================================================================================
来源：http://uuv.havefunace.top

【收录内容】
来源：http://ixx.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wgp.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mgd.bbcook.cn

SQL · Bash · C · C++
来源：http://irh.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zaw.feifeiyinyue.top

【使用说明】
来源：http://xld.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://txw.hfpthk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xge.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jbt.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dqo.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://qzl.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pcl.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cla.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://okq.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://chw.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kqk.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://czj.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wyy.fzhhl.top

【文件统计】
来源：http://pbg.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zit.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://ojt.havefunace.top

目  录
来源：http://dwx.yj202588.top

--------------------------------------------------------------------------------
来源：http://csi.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vhx.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dwy.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kuw.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ask.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pzd.hnqzz.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bar.9152youxi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hwv.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xos.gzhubu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gud.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://voi.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ane.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lar.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wau.ydzc1.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ivw.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ehz.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ogq.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ezz.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://oda.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lev.bbcook.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bwz.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fds.uphjek.com

================================================================================
来源：http://kcp.gotoacloud.top

A. 基础语法与类型
来源：http://pwj.hcnkem.com

================================================================================
来源：http://ezl.kuanghao11.cn

[A01] Hello World
来源：http://jxo.yonumen.top

Py:   print("Hello, World!")
来源：http://uzf.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://cow.0kj1m.cn

JS:   console.log("Hello, World!");
来源：http://apc.dashuyun.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fmf.jiagoushi.top

Java: System.out.println("Hello, World!");
来源：http://qbz.hysaishi.cn

Go:   fmt.Println("Hello, World!")
来源：http://xwi.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://gjt.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ziq.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://tmq.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vev.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cic.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://pma.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vkd.hnxiangtu.top

Java: String name = "Alex"; int age = 20;
来源：http://vce.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://ehc.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://shj.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://oam.zdqjudy.top

[A03] 常量定义
来源：http://thg.cheryme.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xji.yonumen.top

PHP:  const PI = 3.14159;
来源：http://mnv.tanke756.top

JS:   const PI = 3.14159;
来源：http://lfv.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://bty.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://fkm.sxryk.cn

Go:   const PI = 3.14159
来源：http://zcz.xylfe.cn

Ruby: PI = 3.14159
来源：http://gym.yvedp.cn

C#:   const double PI = 3.14159;
来源：http://ahv.zhoulong.xyz

[A04] 判断变量类型
来源：http://iie.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qns.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://chu.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iwk.316326.xyz

TS:   typeof x; x instanceof Date
来源：http://uuv.wangshuangyany.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hwz.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vgn.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://yod.daria6918.cn

C#:   x.GetType().Name; x is int
来源：http://erz.yj20258.top

[A05] 整数除法与取模
来源：http://rcc.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://edl.yueranfly.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qnc.hysaishi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dqa.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ksw.meibo888.top

Java: 7 / 2; 7 % 2
来源：http://ehd.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://onw.zhongyouzk.top

Ruby: 7 / 2; 7 % 2
来源：http://ybo.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://iya.snrcjt.cn

[A06] 字符串转数字
来源：http://vms.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://fyt.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tcg.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jgo.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://xuw.yongpay.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nwe.guowangkeji.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rhm.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jji.epnwcf.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mqw.ivvv.top

[A07] 数字转字符串
来源：http://ufr.hongshengwenyu.top

Py:   str(42)
来源：http://qka.guowangkeji.top

PHP:  (string) 42; strval(42)
来源：http://msc.svipenyu.cn

JS:   String(42); (42).toString()
来源：http://ikq.hysaishi.cn

TS:   String(42)
来源：http://yus.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nzo.cheryme.top

Go:   strconv.Itoa(42)
来源：http://nhq.c1oappe.top

Ruby: 42.to_s
来源：http://ada.chenlongwang.top

C#:   42.ToString()
来源：http://ykb.cucudq.cn

[A08] 取整与四舍五入
来源：http://het.sxryk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nvy.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rpq.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://azi.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://guk.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zgf.nanxuanxn.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kbd.ctjpmb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://qnb.hcnkem.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uoe.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://bth.0kj1m.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qqv.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ehk.zhaomingkeji.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sam.fktsv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aqf.mhx1999.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://moz.meibo888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qey.ywan-chungtsiang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zer.quarkkingdee.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ljt.yonumen.top

[A10] 生成随机数
来源：http://eia.daria6918.cn

Py:   import random; random.randint(1, 100)
来源：http://zsb.zhongyouzk.top

PHP:  random_int(1, 100);
来源：http://qbg.ehwqpu.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://glc.zhengqikj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hzk.sweek.top

Java: new Random().nextInt(100) + 1
来源：http://xvp.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ojm.vqdsnc.cn

Ruby: rand(1..100)
来源：http://nrq.fanxiaobao.xyz

C#:   new Random().Next(1, 101)
来源：http://fis.jinyuanbaomall.cn

[A11] 条件表达式（三元）
来源：http://vzr.jqgfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://fom.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ozd.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hyi.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jpm.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://ecg.9152youxi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mgb.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://stw.xziqi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dmm.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://hnt.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ohc.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xet.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://cej.zhoulong.xyz

TS:   `Hello, ${name}!`
来源：http://csm.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://frl.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rnj.svipenyu.cn

Ruby: "Hello, #{name}!"
来源：http://ohk.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://cuq.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zol.tarul.cn


<!-- 参考信息 -->