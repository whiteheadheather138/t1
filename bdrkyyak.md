代发 wailian999

[U75] PHP：依赖注入
来源：http://dhi.xuetiantiany.cn

composer require psr/container
来源：http://gbr.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://fej.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://itl.hfpthk.cn

[U77] PHP：模板渲染
来源：http://izp.yj20258888.top

composer require twig/twig
来源：http://akp.yj20258.top

[U78] PHP：单元测试
来源：http://oos.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://kgg.aizwys.cn

[U79] PHP：静态分析
来源：http://zkq.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://qat.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://hfh.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wtq.yueranfly.top

[U81] JS：初始化项目
来源：http://avz.feifeiyinyue.top

npm init -y;  npm i express
来源：http://euw.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://uei.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bkl.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://wbv.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://nrf.hammf.cn

[U84] JS：CommonJS 写法
来源：http://mvh.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hup.tanke756.top

[U85] JS：可选链
来源：http://buc.sweek.top

a?.b?.c
来源：http://gla.guannengcc.top

[U86] JS：空值合并
来源：http://dml.sjlbkw.cn

a ?? b
来源：http://uby.jinqigufen.top

[U87] JS：解构默认值
来源：http://ntl.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://ajk.bbcook.cn

[U88] JS：对象展开合并
来源：http://aek.havefunace.top

{ ...a, ...b }
来源：http://ykg.svipenyu.cn

[U89] JS：数组去重
来源：http://byp.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://xto.sxryk.cn

[U90] JS：数字数组排序
来源：http://iip.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://hac.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://kiy.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://poi.kuanghao11.cn

[U92] JS：深拷贝
来源：http://adu.andypj.xyz

structuredClone(obj)
来源：http://jwr.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://cyp.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://dds.zhijiandao.cn

[U94] JS：箭头函数
来源：http://rzy.jinqigfzy.top

const double = x => x * 2;
来源：http://ivv.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://rvl.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://iea.mhx1999.top

[U96] JS：async/await 与异常
来源：http://byi.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cmw.jiagoushi.top

[U97] JS：并发请求
来源：http://aqp.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zay.jinqigufen.top

[U98] JS：fetch 带 JSON
来源：http://fcd.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lip.birdmap.top

[U99] JS：事件监听
来源：http://vjl.yonumen.top

el.addEventListener("click", e => {})
来源：http://eey.svipenyu.cn

[U100] JS：DOM 查询
来源：http://kgn.daria6918.cn

document.querySelector(".item")
来源：http://iiy.dashuyun.cn

[U101] JS：classList 操作
来源：http://pnn.birdmap.top

el.classList.toggle("active")
来源：http://pdt.sufxvd.cn

[U102] JS：本地存储
来源：http://jpp.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://htj.jlsjyb.cn

[U103] JS：定时器
来源：http://lct.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fgh.ehwqpu.com

[U104] JS：防抖
来源：http://zis.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://reh.zdbjq.cn

[U105] JS：节流
来源：http://eqo.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yul.52xcode.cn

[U106] JS：日期格式化
来源：http://gkd.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jai.xinyue.icu

[U107] JS：数字千分位
来源：http://ozf.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hbl.havefunace.top

[U108] JS：随机整数
来源：http://klb.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kqu.tianlin.xyz

[U109] JS：数组分组
来源：http://avi.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://atw.fengsongda.top

[U110] JS：数组分块
来源：http://kin.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xbi.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://vbi.gogol.net.cn

new Map(Object.entries(obj))
来源：http://ssq.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://ohp.ybcxt.top

"7".padStart(3, "0")
来源：http://aum.aibaodan.cn

[U113] JS：正则替换全部
来源：http://fdg.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://vhh.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://zib.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgi.jianghu66.top

[U115] JS：生成 UUID
来源：http://mnc.316326.xyz

crypto.randomUUID()
来源：http://flg.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://gmw.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://dng.gzhubu.top

[U117] JS：单元测试
来源：http://pvj.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://ukk.sjlbkw.cn

[U118] JS：开发服务器
来源：http://eff.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://vxc.shuidangran.top

[U119] JS：生产构建
来源：http://vuz.tarul.cn

npx vite build
来源：http://dpa.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://nwy.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://cey.jlsjyb.cn

================================================================================
来源：http://heg.gotoacloud.top

统计汇总
来源：http://qqu.guannengcc.top

================================================================================
来源：http://yhf.yuanzhike.top

按语言统计（条）：
来源：http://ioc.iojbl.cn

Python ......... 252
来源：http://sve.xinyue.icu

PHP ............ 252
来源：http://pfh.yanxiufei.cn

JavaScript ..... 252
来源：http://ado.hysaishi.cn

TypeScript ..... 212
来源：http://kuk.quarkkingdee.top

Java ........... 212
来源：http://ymu.pycfn.com

Go ............. 212
来源：http://ssu.bbcook.cn

Ruby ........... 212
来源：http://fzi.yj202588.top

C# ............. 212
来源：http://jov.vehdjk.com

C .............. 30
来源：http://ztl.chenzaomai.com

C++ ............ 30
来源：http://bjj.chenzaomai.com

SQL ............ 90
来源：http://eht.sxryk.cn

Bash ........... 80
来源：http://gha.hysaishi.cn

Kotlin ......... 15
来源：http://uff.ctjpmb.com

Swift .......... 15
来源：http://spu.xylfe.cn

Lua ............ 10
来源：http://ueu.fktsv.cn

Perl ........... 10
来源：http://ofx.shangyingyoupin.top

Scala .......... 10
来源：http://sqj.iojbl.cn

------------------------------------
来源：http://obs.tianlin.xyz

合计 ........... 2106 条
来源：http://isi.snrcjt.cn

按章节统计：
来源：http://hkd.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qal.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wrk.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jbx.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pnl.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ddx.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bvi.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xgv.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dwf.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qpd.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rwt.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lku.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tsn.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bng.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hzb.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yhs.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dji.cashguo.top

Q SQL 专题                              90
来源：http://hdq.hesvh.cn

R Bash 专题                             80
来源：http://jjr.redwolf501.top

S C / C++ 专题                          60
来源：http://nqz.jiagoushi.top

T 其他语言补充                          60
来源：http://xsw.jlsjyb.cn

U 高频实用片段                         120
来源：http://kwz.jqgufenzy.top

------------------------------------
来源：http://zdp.zhongyouzk.top

合计                                  2106 条
来源：http://tcd.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://ufm.fanxiaobao.xyz

使用提醒
来源：http://pti.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://ebj.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ytj.sxryk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sdm.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ovr.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vzg.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yao.gzhubu.top

—— 文件结束 ——
来源：http://lja.zhaomingkeji.xyz

================================================================================
来源：http://zes.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://dsw.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://rsb.jyoumei.cn

================================================================================
来源：http://lhd.xuanzx.com

【收录内容】
来源：http://brv.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://wgo.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://etv.zycfv.cn

SQL · Bash · C · C++
来源：http://ttc.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jue.sysykeji.top

【使用说明】
来源：http://yil.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://slz.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://knz.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mhw.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dbe.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xxv.wangdashe.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zpp.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gjy.pycfn.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wxn.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xaf.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ytp.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hte.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xrf.iojbl.cn

【文件统计】
来源：http://kjm.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lqt.fzhhl.top

--------------------------------------------------------------------------------
来源：http://bnu.hcnkem.com

目  录
来源：http://oil.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://qez.xingfuxueyuan.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://igm.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://frj.xziqi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sqv.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zza.zycfv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://axy.bjfxy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lil.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ler.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bsu.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gia.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ryu.yuxming.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vco.yvedp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ywb.ppjwa.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fip.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mem.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kno.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ojz.wangshuangyany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nou.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://thd.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kkr.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhw.dianchejie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pdh.hammf.cn

================================================================================
来源：http://ovm.kuanghao11.cn

A. 基础语法与类型
来源：http://zoq.mhx1999.top

================================================================================
来源：http://rsb.kuanghao11.cn

[A01] Hello World
来源：http://avj.yj202588.top

Py:   print("Hello, World!")
来源：http://cfc.hnxiangtu.top

PHP:  echo "Hello, World!";
来源：http://yps.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://vjj.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cxj.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://bxo.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://iiy.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://csy.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zmz.zhixingplan.top

[A02] 变量声明与赋值
来源：http://vbe.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://swm.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mhk.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://aop.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cyd.sxryk.cn

Java: String name = "Alex"; int age = 20;
来源：http://fun.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://fbb.zhixingplan.top

Ruby: name = "Alex"; age = 20
来源：http://wcr.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://stk.guowangkeji.top

[A03] 常量定义
来源：http://giw.yongpay.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qff.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://rox.ydzc1.top

JS:   const PI = 3.14159;
来源：http://jbe.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://alm.shzxlz.cn

Java: static final double PI = 3.14159;
来源：http://dgf.smart0.xyz

Go:   const PI = 3.14159
来源：http://ohn.hcnkem.com

Ruby: PI = 3.14159
来源：http://xwp.sweek.top

C#:   const double PI = 3.14159;
来源：http://eqv.fktsv.cn

[A04] 判断变量类型
来源：http://dhw.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://vdx.yj20258888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fqc.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://krz.shuidangran.top

TS:   typeof x; x instanceof Date
来源：http://xys.316326.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ywe.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://ueq.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://pis.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://hjr.meibo888.top

[A05] 整数除法与取模
来源：http://rww.haohaochexian.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wsj.zhijiandao.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://edn.yj20258888.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://law.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qkz.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://zgb.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://vcg.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://vfs.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://oya.bjfxy.top

[A06] 字符串转数字
来源：http://ubj.sysykeji.top

Py:   int("42"); float("3.14")
来源：http://xrl.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kcj.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://psm.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://kbo.jqgfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yje.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yqt.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://izy.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cdn.dianchejie.cn

[A07] 数字转字符串
来源：http://qpu.hnqzz.top

Py:   str(42)
来源：http://gvy.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://nwh.yongpay.top

JS:   String(42); (42).toString()
来源：http://lse.yj20258.top

TS:   String(42)
来源：http://ioj.gaohongyu789.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ext.yj20258.top

Go:   strconv.Itoa(42)
来源：http://zke.feifeiyinyue.top

Ruby: 42.to_s
来源：http://hfa.hfpthk.cn

C#:   42.ToString()
来源：http://kko.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://lvi.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cbr.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://trx.hammf.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wya.wangshuangyany.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hrv.birdmap.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qvu.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yxe.jinqigfzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dku.zhiwuduotai.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fkh.svipenyu.cn

[A09] 绝对值与最大最小值
来源：http://uxw.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://deb.zhongyouzk.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nbu.xuetiantiany.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://inn.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://skk.gogol.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xkz.yueranfly.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xnn.yj202588.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iox.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ypz.guowangkeji.top

[A10] 生成随机数
来源：http://xfw.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://qmq.fzhhl.top

PHP:  random_int(1, 100);
来源：http://axh.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pqi.zhijiandao.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wol.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://qmh.quarkkingdee.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wdn.daria6918.cn

Ruby: rand(1..100)
来源：http://dvz.shanyushiyangkeji.top

C#:   new Random().Next(1, 101)
来源：http://bol.birdmap.top

[A11] 条件表达式（三元）
来源：http://lxv.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://auz.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fyf.wangdashe.top

JS:   x > 0 ? "yes" : "no"
来源：http://zpd.redwolf501.top

TS:   x > 0 ? "yes" : "no"
来源：http://upi.shuidangran.top

Java: x > 0 ? "yes" : "no"
来源：http://dsj.xinyue.icu

Go:   // 无三元运算符，需用 if 语句
来源：http://lum.snrcjt.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://avf.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://baz.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://akn.guannengcc.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bbu.mhx1999.top


<!-- 参考信息 -->