代发 wailian999

[U75] PHP：依赖注入
来源：http://afb.ehwqpu.com

composer require psr/container
来源：http://jdi.andypj.xyz

[U76] PHP：简单路由
来源：http://tem.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bof.gotoacloud.top

[U77] PHP：模板渲染
来源：http://fwx.9152youxi.cn

composer require twig/twig
来源：http://hdl.meibo888.top

[U78] PHP：单元测试
来源：http://wid.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://jit.sufxvd.cn

[U79] PHP：静态分析
来源：http://aah.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://hqm.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://dqt.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://daf.bbcook.cn

[U81] JS：初始化项目
来源：http://swd.sufxvd.cn

npm init -y;  npm i express
来源：http://cla.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://hzj.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rfg.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://xfn.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://roy.ydzc1.top

[U84] JS：CommonJS 写法
来源：http://hom.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://frb.sufxvd.cn

[U85] JS：可选链
来源：http://ltz.smart0.xyz

a?.b?.c
来源：http://hnz.xziqi.cn

[U86] JS：空值合并
来源：http://wmi.hesvh.cn

a ?? b
来源：http://fms.uphjek.com

[U87] JS：解构默认值
来源：http://pvp.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://aqp.tianlin.xyz

[U88] JS：对象展开合并
来源：http://edn.feifeiyinyue.top

{ ...a, ...b }
来源：http://ona.zdqjudy.top

[U89] JS：数组去重
来源：http://sfo.pycfn.com

[...new Set(arr)]
来源：http://ooa.yuanzhike.top

[U90] JS：数字数组排序
来源：http://ypf.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://lbu.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://jde.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://txh.c1oappe.top

[U92] JS：深拷贝
来源：http://yam.cqqwz.cn

structuredClone(obj)
来源：http://nla.havefunace.top

[U93] JS：模板字符串
来源：http://ljw.sjlbkw.cn

`共 ${n} 条`
来源：http://dbw.vqdsnc.cn

[U94] JS：箭头函数
来源：http://ict.fehbvm.com

const double = x => x * 2;
来源：http://tjo.ydzc1.top

[U95] JS：Promise 包装
来源：http://emt.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://bxv.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://ytd.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yht.zhengqikj.top

[U97] JS：并发请求
来源：http://ipa.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xoo.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://sdy.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lvi.xziqi.cn

[U99] JS：事件监听
来源：http://xrl.hammf.cn

el.addEventListener("click", e => {})
来源：http://blu.guannengcc.top

[U100] JS：DOM 查询
来源：http://sni.dashuyun.cn

document.querySelector(".item")
来源：http://rja.chenzaomai.com

[U101] JS：classList 操作
来源：http://acn.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://qvu.ivvv.top

[U102] JS：本地存储
来源：http://lni.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jtc.yj20258888.top

[U103] JS：定时器
来源：http://iao.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aim.jinqigfzy.top

[U104] JS：防抖
来源：http://icj.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnw.vqdsnc.cn

[U105] JS：节流
来源：http://isf.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sbz.hesvh.cn

[U106] JS：日期格式化
来源：http://anx.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ftb.xziqi.cn

[U107] JS：数字千分位
来源：http://avq.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wsx.ydzc1.top

[U108] JS：随机整数
来源：http://mjy.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wry.yanxiufei.cn

[U109] JS：数组分组
来源：http://klh.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://seq.cheryme.top

[U110] JS：数组分块
来源：http://oln.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://idp.dianchejie.cn

[U111] JS：对象转 Map
来源：http://bqw.uphjek.com

new Map(Object.entries(obj))
来源：http://pbk.iojbl.cn

[U112] JS：字符串补位
来源：http://whq.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://ijq.ehwqpu.com

[U113] JS：正则替换全部
来源：http://bbb.guowangkeji.top

s.replaceAll("a", "b")
来源：http://hci.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://bhs.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nqs.hammf.cn

[U115] JS：生成 UUID
来源：http://ujf.haohaochexian.top

crypto.randomUUID()
来源：http://dah.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://afm.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://coa.hywenlv.cn

[U117] JS：单元测试
来源：http://njw.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://nbl.mhx1999.top

[U118] JS：开发服务器
来源：http://yst.cqqwz.cn

npm i -D vite;  npx vite
来源：http://mlv.sufxvd.cn

[U119] JS：生产构建
来源：http://cwr.cashguo.top

npx vite build
来源：http://zww.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://hpl.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://ash.snrcjt.cn

================================================================================
来源：http://qtw.wangshuangyany.cn

统计汇总
来源：http://uyy.vehdjk.com

================================================================================
来源：http://cyy.gogol.net.cn

按语言统计（条）：
来源：http://ztz.nwbrower.top

Python ......... 252
来源：http://vqb.gogol.net.cn

PHP ............ 252
来源：http://upw.haohaochexian.top

JavaScript ..... 252
来源：http://psa.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://lws.zhiwuduotai.top

Java ........... 212
来源：http://bpy.xuetiantiany.cn

Go ............. 212
来源：http://dvx.epnwcf.com

Ruby ........... 212
来源：http://rxn.yuxming.cn

C# ............. 212
来源：http://snb.dianchejie.cn

C .............. 30
来源：http://hgh.hammf.cn

C++ ............ 30
来源：http://ikd.ydjk.org.cn

SQL ............ 90
来源：http://ghg.chenlongwang.top

Bash ........... 80
来源：http://cwa.yj20258888.top

Kotlin ......... 15
来源：http://upa.hammf.cn

Swift .......... 15
来源：http://eui.jinghuilouyu.cn

Lua ............ 10
来源：http://oad.shzxlz.cn

Perl ........... 10
来源：http://zfg.bbcook.cn

Scala .......... 10
来源：http://vfm.yonumen.top

------------------------------------
来源：http://jyc.tanke756.top

合计 ........... 2106 条
来源：http://wkf.hnxiangtu.top

按章节统计：
来源：http://mme.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lmt.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://beg.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yjq.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dcr.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fna.fanxiaobao.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ckf.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eem.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bya.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://avq.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mkx.fehbvm.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lfs.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mlg.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cyg.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xki.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vlx.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iuz.52xcode.cn

Q SQL 专题                              90
来源：http://axq.uphjek.com

R Bash 专题                             80
来源：http://oqr.jinqigufen.top

S C / C++ 专题                          60
来源：http://jrz.wangshuangyany.cn

T 其他语言补充                          60
来源：http://hmk.bjfxy.top

U 高频实用片段                         120
来源：http://rwn.c1oappe.top

------------------------------------
来源：http://xnr.ctjpmb.com

合计                                  2106 条
来源：http://kxr.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://vnu.jinyuanbaomall.cn

使用提醒
来源：http://gpr.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://huq.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nus.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cwz.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fvb.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://epp.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://syf.hcnkem.com

—— 文件结束 ——
来源：http://zdo.gotoacloud.top

================================================================================
来源：http://dyn.havefunace.top

程序语言常见例子速查手册（2024 版）
来源：http://jgg.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://nnc.gogol.net.cn

================================================================================
来源：http://zmj.316326.xyz

【收录内容】
来源：http://pqz.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pdg.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wai.gogol.net.cn

SQL · Bash · C · C++
来源：http://sqf.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zjd.jinyuanbaomall.cn

【使用说明】
来源：http://hps.sweek.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ksx.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ijb.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rzm.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vup.tarul.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kcm.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ysu.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mrk.hammf.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://diq.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ajg.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ouk.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rxr.guannengcc.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oot.svipenyu.cn

【文件统计】
来源：http://zlc.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ugx.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://hxs.fktsv.cn

目  录
来源：http://yzh.c1oappe.top

--------------------------------------------------------------------------------
来源：http://waf.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aze.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jny.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kup.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pwl.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oma.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eig.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dqy.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://czi.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tib.zhijiandao.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lqn.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nbl.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jsv.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ggg.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cab.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mur.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bdk.dianchejie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zaj.smart0.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://bbk.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bev.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xoe.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uct.dianchejie.cn

================================================================================
来源：http://dqz.bjfxy.top

A. 基础语法与类型
来源：http://txu.nanxuanxn.top

================================================================================
来源：http://krf.hongshengwenyu.top

[A01] Hello World
来源：http://gcx.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://qhz.xylfe.cn

PHP:  echo "Hello, World!";
来源：http://gnu.hammf.cn

JS:   console.log("Hello, World!");
来源：http://xpp.nanxinkj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://emm.havefunace.top

Java: System.out.println("Hello, World!");
来源：http://qsp.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://pna.pengpengdd.cyou

Ruby: puts "Hello, World!"
来源：http://fte.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://oqn.yfazqb.com

[A02] 变量声明与赋值
来源：http://xav.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tgq.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ckf.chenjidiqi.icu

JS:   let name = "Alex"; const age = 20;
来源：http://kwn.mhx1999.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gqq.daxiang520.top

Java: String name = "Alex"; int age = 20;
来源：http://hub.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://fne.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://eyu.jyoumei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://egb.jinghuilouyu.cn

[A03] 常量定义
来源：http://kfi.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wog.yuanzhike.top

PHP:  const PI = 3.14159;
来源：http://lic.tianlin.xyz

JS:   const PI = 3.14159;
来源：http://ifw.jianghu66.top

TS:   const PI: number = 3.14159;
来源：http://aqj.feifeiyinyue.top

Java: static final double PI = 3.14159;
来源：http://kxe.haohaochexian.top

Go:   const PI = 3.14159
来源：http://wce.cashguo.top

Ruby: PI = 3.14159
来源：http://ewj.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://umx.tianlin.xyz

[A04] 判断变量类型
来源：http://xff.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hvk.chenlongwang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ldz.sxryk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bir.nanxinkj.top

TS:   typeof x; x instanceof Date
来源：http://vmp.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qri.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://dum.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://twn.zdbjq.cn

C#:   x.GetType().Name; x is int
来源：http://amr.guannengcc.top

[A05] 整数除法与取模
来源：http://nia.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mwy.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zyb.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pqr.jianghu66.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xsz.svipenyu.cn

Java: 7 / 2; 7 % 2
来源：http://btg.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://nxu.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://brm.guannengcc.top

C#:   7 / 2; 7 % 2
来源：http://pac.jqgfzy.top

[A06] 字符串转数字
来源：http://ssc.kuanghao11.cn

Py:   int("42"); float("3.14")
来源：http://aby.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mwn.meibo888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xbp.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://laa.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lkv.ybcxt.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ebh.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jzi.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ehx.guannengcc.top

[A07] 数字转字符串
来源：http://gzd.zhongyouzk.top

Py:   str(42)
来源：http://oqc.fehbvm.com

PHP:  (string) 42; strval(42)
来源：http://pea.jinqigfzy.top

JS:   String(42); (42).toString()
来源：http://qqy.9152youxi.cn

TS:   String(42)
来源：http://lie.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mun.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://ryx.sysykeji.top

Ruby: 42.to_s
来源：http://dwx.fehbvm.com

C#:   42.ToString()
来源：http://jxa.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://npc.cqqwz.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hey.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ojb.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://llq.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uwo.fengsongda.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://enn.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ooi.yonumen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://obs.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xwi.jinqigfzy.top

[A09] 绝对值与最大最小值
来源：http://fwt.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dzm.zhaomingkeji.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hik.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rrz.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://glr.bjfxy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://izm.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tmm.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gvj.hywenlv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qrc.fzhhl.top

[A10] 生成随机数
来源：http://wjf.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://qce.fengsongda.top

PHP:  random_int(1, 100);
来源：http://hvm.tianlin.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blp.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://drc.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://reu.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yhu.xylfe.cn

Ruby: rand(1..100)
来源：http://ywy.ydzc1.top

C#:   new Random().Next(1, 101)
来源：http://ara.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://htu.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://tzp.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://aov.0kj1m.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fxj.nwbrower.top

TS:   x > 0 ? "yes" : "no"
来源：http://kmg.9152youxi.cn

Java: x > 0 ? "yes" : "no"
来源：http://yoc.ctjpmb.com

Go:   // 无三元运算符，需用 if 语句
来源：http://mxm.cdnleiting.top

Ruby: x > 0 ? "yes" : "no"
来源：http://whq.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pbf.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://dsu.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pwr.iojbl.cn


<!-- 参考信息 -->