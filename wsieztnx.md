代发 wailian999

[U75] PHP：依赖注入
来源：http://ofu.tanke756.top

composer require psr/container
来源：http://dru.jlsjyb.cn

[U76] PHP：简单路由
来源：http://wsx.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ifu.hnqzz.top

[U77] PHP：模板渲染
来源：http://nwo.svipenyu.cn

composer require twig/twig
来源：http://juh.fzhhl.top

[U78] PHP：单元测试
来源：http://twu.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://wtr.yanxiufei.cn

[U79] PHP：静态分析
来源：http://ywi.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://bxp.yueranfly.top

[U80] PHP：代码规范修复
来源：http://yvc.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://lsq.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://csy.jlsjyb.cn

npm init -y;  npm i express
来源：http://mpt.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://wuy.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jfz.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://eof.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sla.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://yra.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rwk.wangdashe.top

[U85] JS：可选链
来源：http://hob.yuxming.cn

a?.b?.c
来源：http://oip.c1oappe.top

[U86] JS：空值合并
来源：http://lph.shuidangran.top

a ?? b
来源：http://ngq.jqgfzy.top

[U87] JS：解构默认值
来源：http://ppo.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://nhk.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://ttu.jqgufenzy.top

{ ...a, ...b }
来源：http://ggn.jyoumei.cn

[U89] JS：数组去重
来源：http://rsv.sufxvd.cn

[...new Set(arr)]
来源：http://bup.hcnkem.com

[U90] JS：数字数组排序
来源：http://zkt.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://htt.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://roc.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ozc.yj20258888.top

[U92] JS：深拷贝
来源：http://lxh.fehbvm.com

structuredClone(obj)
来源：http://ndf.jinqigfzy.top

[U93] JS：模板字符串
来源：http://vcl.redwolf501.top

`共 ${n} 条`
来源：http://jiq.52xcode.cn

[U94] JS：箭头函数
来源：http://kyx.andypj.xyz

const double = x => x * 2;
来源：http://zeh.snrcjt.cn

[U95] JS：Promise 包装
来源：http://ugq.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://ojn.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://knr.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://twp.sysykeji.top

[U97] JS：并发请求
来源：http://dvm.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://vog.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://ygx.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wox.mhx1999.top

[U99] JS：事件监听
来源：http://jna.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://gbf.meibo888.top

[U100] JS：DOM 查询
来源：http://jrw.uphjek.com

document.querySelector(".item")
来源：http://pgf.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://xvi.pycfn.com

el.classList.toggle("active")
来源：http://ggh.hongshengwenyu.top

[U102] JS：本地存储
来源：http://ztn.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://fkz.pengpengdd.cyou

[U103] JS：定时器
来源：http://wfd.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ooh.zhijiandao.cn

[U104] JS：防抖
来源：http://mfd.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upt.tianlin.xyz

[U105] JS：节流
来源：http://cym.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wev.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://mgw.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xpz.aizwys.cn

[U107] JS：数字千分位
来源：http://xoy.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://evy.chenjidiqi.icu

[U108] JS：随机整数
来源：http://iyp.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jkx.bbcook.cn

[U109] JS：数组分组
来源：http://ihf.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://zzl.hywenlv.cn

[U110] JS：数组分块
来源：http://mma.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vuj.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://jka.zdbjq.cn

new Map(Object.entries(obj))
来源：http://aoj.daxiang520.top

[U112] JS：字符串补位
来源：http://zqb.chenzaomai.com

"7".padStart(3, "0")
来源：http://jce.guannengcc.top

[U113] JS：正则替换全部
来源：http://tbj.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://yxk.andypj.xyz

[U114] JS：JSON 深比较
来源：http://zsi.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://kih.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://baa.yvedp.cn

crypto.randomUUID()
来源：http://hid.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://eoy.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://kdr.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://caa.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://eyt.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://arc.shuidangran.top

npm i -D vite;  npx vite
来源：http://lzu.yvedp.cn

[U119] JS：生产构建
来源：http://rqf.yj20258.top

npx vite build
来源：http://kmi.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://faq.yj202588.top

import.meta.env.VITE_API_URL
来源：http://mwl.zhengqikj.top

================================================================================
来源：http://drh.nanxinkj.top

统计汇总
来源：http://dmx.316326.xyz

================================================================================
来源：http://jwd.ydzc1.top

按语言统计（条）：
来源：http://vcq.hysaishi.cn

Python ......... 252
来源：http://trs.yj20258888.top

PHP ............ 252
来源：http://grd.ydzc1.top

JavaScript ..... 252
来源：http://wjr.jqgufenzy.top

TypeScript ..... 212
来源：http://pbe.redwolf501.top

Java ........... 212
来源：http://oeu.hysaishi.cn

Go ............. 212
来源：http://bsj.yfazqb.com

Ruby ........... 212
来源：http://zqn.nwbrower.top

C# ............. 212
来源：http://ill.gogol.net.cn

C .............. 30
来源：http://cnd.mhx1999.top

C++ ............ 30
来源：http://gwa.jinyuanbaomall.cn

SQL ............ 90
来源：http://hnh.zhixingplan.top

Bash ........... 80
来源：http://npe.hnqzz.top

Kotlin ......... 15
来源：http://xwv.vehdjk.com

Swift .......... 15
来源：http://pli.hongshengwenyu.top

Lua ............ 10
来源：http://fzd.vehdjk.com

Perl ........... 10
来源：http://ody.shuidangran.top

Scala .......... 10
来源：http://kdh.xylfe.cn

------------------------------------
来源：http://imv.shangyingyoupin.top

合计 ........... 2106 条
来源：http://jjl.vehdjk.com

按章节统计：
来源：http://hpl.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lvk.ydjk.org.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jbl.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aet.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ihn.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dad.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pcd.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ill.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wjh.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ufk.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zzr.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lhe.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lcm.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tgn.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nzd.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lgs.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://smj.nanxuanxn.top

Q SQL 专题                              90
来源：http://rqt.sjlbkw.cn

R Bash 专题                             80
来源：http://kbb.tanke756.top

S C / C++ 专题                          60
来源：http://lni.shzxlz.cn

T 其他语言补充                          60
来源：http://lug.ivvv.top

U 高频实用片段                         120
来源：http://jck.fengsongda.top

------------------------------------
来源：http://iul.jianghu66.top

合计                                  2106 条
来源：http://bfb.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://xcp.smart0.xyz

使用提醒
来源：http://xvr.xinyue.icu

--------------------------------------------------------------------------------
来源：http://qkt.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://txo.iojbl.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lqx.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://whv.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://etw.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://biv.kuanghao11.cn

—— 文件结束 ——
来源：http://knn.feifeiyinyue.top

================================================================================
来源：http://lho.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://sib.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://iqh.wangshuangyany.cn

================================================================================
来源：http://rnt.vehdjk.com

【收录内容】
来源：http://ugu.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://qti.yongpay.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bjd.ehwqpu.com

SQL · Bash · C · C++
来源：http://svp.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mdl.fzhhl.top

【使用说明】
来源：http://ycj.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mim.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eyt.fktsv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hwf.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://prp.vqdsnc.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lwg.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dbw.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nbu.guannengcc.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mqj.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mdg.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://keh.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rac.tanke756.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fnb.svipenyu.cn

【文件统计】
来源：http://pli.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ouy.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://mue.chenjidiqi.icu

目  录
来源：http://ott.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://cvp.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rdm.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kji.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ulu.zhiwuduotai.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mjc.hnxiangtu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eld.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fdh.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ntg.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tqq.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qnz.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ino.jlsjyb.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://puq.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lcd.smart0.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://whz.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://igr.tian-w.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tir.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yst.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vqs.quarkkingdee.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fjp.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xow.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wip.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://srl.shuidangran.top

================================================================================
来源：http://pmd.fengsongda.top

A. 基础语法与类型
来源：http://tma.cqqwz.cn

================================================================================
来源：http://ids.ehwqpu.com

[A01] Hello World
来源：http://jbe.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://jrt.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://rer.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://qfs.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hvv.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://vgn.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://hxz.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://kte.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://nwj.cdnleiting.top

[A02] 变量声明与赋值
来源：http://aju.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qlg.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mvi.sxryk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zbf.zdbjq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://idg.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://mhj.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://tbq.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://ocl.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://qxm.xylfe.cn

[A03] 常量定义
来源：http://gdz.wangdashe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lgu.snrcjt.cn

PHP:  const PI = 3.14159;
来源：http://bzy.daria6918.cn

JS:   const PI = 3.14159;
来源：http://vaq.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://sgu.smart0.xyz

Java: static final double PI = 3.14159;
来源：http://rbp.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://dle.cashguo.top

Ruby: PI = 3.14159
来源：http://jin.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://zwg.yj202588.top

[A04] 判断变量类型
来源：http://exa.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rci.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ibu.jlsjyb.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cxu.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://mtb.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://stp.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://vec.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pbc.cucudq.cn

C#:   x.GetType().Name; x is int
来源：http://jdb.chenzaomai.com

[A05] 整数除法与取模
来源：http://ehk.cucudq.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uwu.ehwqpu.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://lfs.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kex.hesvh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vmx.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://ixv.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://wks.sweek.top

Ruby: 7 / 2; 7 % 2
来源：http://rdi.ydzc1.top

C#:   7 / 2; 7 % 2
来源：http://dwl.hongshengwenyu.top

[A06] 字符串转数字
来源：http://gjs.zdqjudy.top

Py:   int("42"); float("3.14")
来源：http://bbc.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ist.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dqu.gogol.net.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fnf.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rvm.ydjk.org.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cjf.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iys.cqqwz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://spo.epnwcf.com

[A07] 数字转字符串
来源：http://kxi.daria6918.cn

Py:   str(42)
来源：http://rjj.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://qua.dianchejie.cn

JS:   String(42); (42).toString()
来源：http://fqz.shzxlz.cn

TS:   String(42)
来源：http://zmc.iojbl.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pec.dashuyun.cn

Go:   strconv.Itoa(42)
来源：http://toq.gotoacloud.top

Ruby: 42.to_s
来源：http://him.yonumen.top

C#:   42.ToString()
来源：http://fee.haohaochexian.top

[A08] 取整与四舍五入
来源：http://nie.chenlongwang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://csu.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ajm.daxiang520.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ulw.snrcjt.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kig.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fzw.andypj.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gek.jinyuanbaomall.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kgb.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bcs.tanke756.top

[A09] 绝对值与最大最小值
来源：http://xuy.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wvw.sjlbkw.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lol.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gad.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lia.andypj.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://psf.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lnb.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://luu.zhoulong.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aie.daxiang520.top

[A10] 生成随机数
来源：http://yrq.sjlbkw.cn

Py:   import random; random.randint(1, 100)
来源：http://vvi.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://dtm.sufxvd.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rpj.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nia.smart0.xyz

Java: new Random().nextInt(100) + 1
来源：http://qnu.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fug.xylfe.cn

Ruby: rand(1..100)
来源：http://rgy.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://bym.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://tai.jqgufenzy.top

Py:   "yes" if x > 0 else "no"
来源：http://cfw.cucudq.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lax.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://hqa.0kj1m.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gny.yj20258888.top

Java: x > 0 ? "yes" : "no"
来源：http://xmc.chenjidiqi.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://rfh.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ybo.shzxlz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ods.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://evr.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iyz.52xcode.cn


<!-- 参考信息 -->