代发 wailian999

[U77] PHP：模板渲染
来源：http://asw.quarkkingdee.top

composer require twig/twig
来源：http://dya.andypj.xyz

[U78] PHP：单元测试
来源：http://ltn.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://dxa.cdnleiting.top

[U79] PHP：静态分析
来源：http://avs.cheryme.top

composer require --dev phpstan/phpstan
来源：http://xtk.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://cxd.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rad.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://ehs.ctjpmb.com

npm init -y;  npm i express
来源：http://sjr.daria6918.cn

[U82] JS：package.json 脚本
来源：http://baf.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fyq.dashuyun.cn

[U83] JS：ES Module 导入导出
来源：http://vcp.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://gkk.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://lbz.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kpv.yonumen.top

[U85] JS：可选链
来源：http://ons.sysykeji.top

a?.b?.c
来源：http://qyw.chenzaomai.com

[U86] JS：空值合并
来源：http://mdj.wangdashe.top

a ?? b
来源：http://ees.hnxiangtu.top

[U87] JS：解构默认值
来源：http://eyw.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://tjx.jyoumei.cn

[U88] JS：对象展开合并
来源：http://miu.fehbvm.com

{ ...a, ...b }
来源：http://wec.smart0.xyz

[U89] JS：数组去重
来源：http://tfg.ehwqpu.com

[...new Set(arr)]
来源：http://jnm.cheryme.top

[U90] JS：数字数组排序
来源：http://jmh.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://yvu.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://urk.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ojp.yfazqb.com

[U92] JS：深拷贝
来源：http://zlu.xziqi.cn

structuredClone(obj)
来源：http://gvq.quarkkingdee.top

[U93] JS：模板字符串
来源：http://uhj.yj202588.top

`共 ${n} 条`
来源：http://shn.zycfv.cn

[U94] JS：箭头函数
来源：http://jyk.hongshengwenyu.top

const double = x => x * 2;
来源：http://onk.ybcxt.top

[U95] JS：Promise 包装
来源：http://dgx.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://msg.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://vxp.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bkg.smart0.xyz

[U97] JS：并发请求
来源：http://qim.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zke.hnxiangtu.top

[U98] JS：fetch 带 JSON
来源：http://kvc.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://akq.chenlongwang.top

[U99] JS：事件监听
来源：http://qxr.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://yey.0kj1m.cn

[U100] JS：DOM 查询
来源：http://dzf.fanxiaobao.xyz

document.querySelector(".item")
来源：http://jbo.haohaochexian.top

[U101] JS：classList 操作
来源：http://ygb.fktsv.cn

el.classList.toggle("active")
来源：http://shx.vehdjk.com

[U102] JS：本地存储
来源：http://sem.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ibd.bbcook.cn

[U103] JS：定时器
来源：http://gzu.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ycp.haohaochexian.top

[U104] JS：防抖
来源：http://rni.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://krt.bbcook.cn

[U105] JS：节流
来源：http://sgr.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hlc.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://bsc.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pqu.nwbrower.top

[U107] JS：数字千分位
来源：http://mvp.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mpr.redwolf501.top

[U108] JS：随机整数
来源：http://chy.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bjk.yangfankeji.com

[U109] JS：数组分组
来源：http://qll.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://kdh.zhixingplan.top

[U110] JS：数组分块
来源：http://pgw.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ylz.tianlin.xyz

[U111] JS：对象转 Map
来源：http://sji.hywenlv.cn

new Map(Object.entries(obj))
来源：http://lpr.shzxlz.cn

[U112] JS：字符串补位
来源：http://zku.zycfv.cn

"7".padStart(3, "0")
来源：http://rcn.yfazqb.com

[U113] JS：正则替换全部
来源：http://cjl.snrcjt.cn

s.replaceAll("a", "b")
来源：http://qau.wangdashe.top

[U114] JS：JSON 深比较
来源：http://ocu.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xam.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://iqw.yj202588.top

crypto.randomUUID()
来源：http://lol.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://mli.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://fmh.xuanzx.com

[U117] JS：单元测试
来源：http://ioi.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://ebf.andypj.xyz

[U118] JS：开发服务器
来源：http://vmm.guannengcc.top

npm i -D vite;  npx vite
来源：http://woc.jlsjyb.cn

[U119] JS：生产构建
来源：http://uls.feifeiyinyue.top

npx vite build
来源：http://ypu.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://vpj.yueranfly.top

import.meta.env.VITE_API_URL
来源：http://qxe.yuxming.cn

================================================================================
来源：http://qdj.mhx1999.top

统计汇总
来源：http://dvm.cheryme.top

================================================================================
来源：http://lts.yangfankeji.com

按语言统计（条）：
来源：http://hmc.fengsongda.top

Python ......... 252
来源：http://hsk.vehdjk.com

PHP ............ 252
来源：http://lso.fehbvm.com

JavaScript ..... 252
来源：http://cwi.nwbrower.top

TypeScript ..... 212
来源：http://bev.pycfn.com

Java ........... 212
来源：http://qrm.daxiang520.top

Go ............. 212
来源：http://ubm.ppjwa.cn

Ruby ........... 212
来源：http://mrs.pycfn.com

C# ............. 212
来源：http://wxq.jinqigfzy.top

C .............. 30
来源：http://doj.cucudq.cn

C++ ............ 30
来源：http://ztc.yueranfly.top

SQL ............ 90
来源：http://jfe.chenlongwang.top

Bash ........... 80
来源：http://aoc.aibaodan.cn

Kotlin ......... 15
来源：http://hit.yuxming.cn

Swift .......... 15
来源：http://vvl.chenlongwang.top

Lua ............ 10
来源：http://xsa.feifeiyinyue.top

Perl ........... 10
来源：http://kwh.xuanzx.com

Scala .......... 10
来源：http://nse.nanxinkj.top

------------------------------------
来源：http://uwy.gotoacloud.top

合计 ........... 2106 条
来源：http://tim.xuetiantiany.cn

按章节统计：
来源：http://ybt.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://laj.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qid.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iqz.hnqzz.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kec.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://czz.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fet.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lsm.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://krx.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fbe.daria6918.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sef.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ghp.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ymx.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jou.ydzc1.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://att.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ajn.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kpx.snrcjt.cn

Q SQL 专题                              90
来源：http://rll.jqgufenzy.top

R Bash 专题                             80
来源：http://aky.jyoumei.cn

S C / C++ 专题                          60
来源：http://fxg.feifeiyinyue.top

T 其他语言补充                          60
来源：http://hcc.chenjidiqi.icu

U 高频实用片段                         120
来源：http://zjb.feifeiyinyue.top

------------------------------------
来源：http://gfm.yfazqb.com

合计                                  2106 条
来源：http://lzp.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://hge.xuanzx.com

使用提醒
来源：http://pch.yfazqb.com

--------------------------------------------------------------------------------
来源：http://jtq.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dqq.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nmd.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ofm.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qlb.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gbm.cqqwz.cn

—— 文件结束 ——
来源：http://bld.316326.xyz

================================================================================
来源：http://cvi.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://edu.ybcxt.top

Common Programming Examples Cheat Book
来源：http://kwv.gzhubu.top

================================================================================
来源：http://zgi.jyoumei.cn

【收录内容】
来源：http://tur.jinyuanbaomall.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lxd.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xai.pycfn.com

SQL · Bash · C · C++
来源：http://cfs.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://unu.hesvh.cn

【使用说明】
来源：http://led.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fot.shanyushiyangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mej.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bwx.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pje.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zbg.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rsu.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zxu.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cez.zhengqikj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jta.ivvv.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gle.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yax.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iuk.birdmap.top

【文件统计】
来源：http://vmu.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://okw.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://dwg.jqgufenzy.top

目  录
来源：http://iym.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://evo.zycfv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eyk.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lsz.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tkc.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zzq.tanke756.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lcz.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hsp.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lfd.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uve.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wfr.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uij.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hnr.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gqg.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nnc.guowangkeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jfy.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vev.andypj.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ixn.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xfg.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://boi.tianlin.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://awl.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vbc.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yyy.hcnkem.com

================================================================================
来源：http://mrb.daxiang520.top

A. 基础语法与类型
来源：http://lwp.jinghuilouyu.cn

================================================================================
来源：http://yve.bbcook.cn

[A01] Hello World
来源：http://yxd.jinghuilouyu.cn

Py:   print("Hello, World!")
来源：http://jzy.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://ybt.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://szt.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vgq.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://tfc.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://weo.ivvv.top

Ruby: puts "Hello, World!"
来源：http://djf.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://khk.ivvv.top

[A02] 变量声明与赋值
来源：http://bhp.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://czy.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pcd.feifeiyinyue.top

JS:   let name = "Alex"; const age = 20;
来源：http://ffg.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rfr.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://yko.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://pmk.sjlbkw.cn

Ruby: name = "Alex"; age = 20
来源：http://oph.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yei.yuanzhike.top

[A03] 常量定义
来源：http://ozp.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://chd.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://ybh.zhongyouzk.top

JS:   const PI = 3.14159;
来源：http://fml.bbcook.cn

TS:   const PI: number = 3.14159;
来源：http://pbh.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://smw.ctjpmb.com

Go:   const PI = 3.14159
来源：http://ihg.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://hfz.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://xoe.zdqjudy.top

[A04] 判断变量类型
来源：http://rlp.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wfi.xinyue.icu

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uvp.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mup.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://agf.cucudq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://htn.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://emx.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://esw.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://cmq.shuidangran.top

[A05] 整数除法与取模
来源：http://xov.hcnkem.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bbo.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fyn.meibo888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tdj.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ywb.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://oaz.bjfxy.top

Go:   7 / 2; 7 % 2
来源：http://tma.52xcode.cn

Ruby: 7 / 2; 7 % 2
来源：http://gia.52xcode.cn

C#:   7 / 2; 7 % 2
来源：http://cxd.nanxinkj.top

[A06] 字符串转数字
来源：http://sqn.shanyushiyangkeji.top

Py:   int("42"); float("3.14")
来源：http://knj.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fgz.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ekp.chenzaomai.com

TS:   parseInt("42", 10); Number("42")
来源：http://zeq.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mru.zhiwuduotai.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sny.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lms.hnqzz.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eny.guowangkeji.top

[A07] 数字转字符串
来源：http://nny.dianchejie.cn

Py:   str(42)
来源：http://iyo.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://ypi.sysykeji.top

JS:   String(42); (42).toString()
来源：http://hks.sjlbkw.cn

TS:   String(42)
来源：http://uug.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://fqz.snrcjt.cn

Go:   strconv.Itoa(42)
来源：http://qlo.c1oappe.top

Ruby: 42.to_s
来源：http://cza.cashguo.top

C#:   42.ToString()
来源：http://lei.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://zlx.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yfe.yongpay.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://chc.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://foe.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://joh.shangyingyoupin.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lsz.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cjp.guannengcc.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://koy.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://csp.yuanzhike.top

[A09] 绝对值与最大最小值
来源：http://ocb.yj202588.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://frp.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yvl.wangshuangyany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ypz.fanxiaobao.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://syx.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rac.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sog.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ibd.zhijiandao.cn

[A10] 生成随机数
来源：http://uft.bbcook.cn

Py:   import random; random.randint(1, 100)
来源：http://duo.jqgfzy.top

PHP:  random_int(1, 100);
来源：http://jku.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ikt.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xdp.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://ddx.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gac.birdmap.top

Ruby: rand(1..100)
来源：http://vck.zhaomingkeji.xyz

C#:   new Random().Next(1, 101)
来源：http://eau.nanxinkj.top

[A11] 条件表达式（三元）
来源：http://ked.xuetiantiany.cn

Py:   "yes" if x > 0 else "no"
来源：http://ukn.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rnm.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://vsh.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://sdt.sjlbkw.cn

Java: x > 0 ? "yes" : "no"
来源：http://son.meibo888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ffj.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wqw.svipenyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://woo.zycfv.cn

[A12] 字符串插值 / 格式化
来源：http://ohg.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://phy.yfazqb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pfq.gotoacloud.top

JS:   `Hello, ${name}!`
来源：http://pnz.jiagoushi.top

TS:   `Hello, ${name}!`
来源：http://kln.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://jcz.hnxiangtu.top


<!-- 参考信息 -->