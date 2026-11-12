代发 wailian999

[U75] PHP：依赖注入
来源：http://bpb.gogol.net.cn

composer require psr/container
来源：http://fpo.gotoacloud.top

[U76] PHP：简单路由
来源：http://cez.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zuw.aizwys.cn

[U77] PHP：模板渲染
来源：http://npj.fehbvm.com

composer require twig/twig
来源：http://gga.tianlin.xyz

[U78] PHP：单元测试
来源：http://gzh.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://ily.vehdjk.com

[U79] PHP：静态分析
来源：http://ojf.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://oaw.yvedp.cn

[U80] PHP：代码规范修复
来源：http://cwb.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ypv.ctjpmb.com

[U81] JS：初始化项目
来源：http://uuq.yj20258.top

npm init -y;  npm i express
来源：http://pri.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://tbn.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fkg.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://fvv.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://dht.ivvv.top

[U84] JS：CommonJS 写法
来源：http://kux.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://zbg.vehdjk.com

[U85] JS：可选链
来源：http://ixd.ctjpmb.com

a?.b?.c
来源：http://won.hnqzz.top

[U86] JS：空值合并
来源：http://abf.zhiwuduotai.top

a ?? b
来源：http://vmq.feifeiyinyue.top

[U87] JS：解构默认值
来源：http://vcv.tianlin.xyz

const { a = 1, b = 2 } = obj;
来源：http://vlf.ppjwa.cn

[U88] JS：对象展开合并
来源：http://vfs.redwolf501.top

{ ...a, ...b }
来源：http://uol.gaohongyu789.top

[U89] JS：数组去重
来源：http://bed.gaohongyu789.top

[...new Set(arr)]
来源：http://gmm.jinqigufen.top

[U90] JS：数字数组排序
来源：http://nzb.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://tul.316326.xyz

[U91] JS：对象键值遍历
来源：http://fdm.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jrl.jyoumei.cn

[U92] JS：深拷贝
来源：http://hlb.chenlongwang.top

structuredClone(obj)
来源：http://jqn.316326.xyz

[U93] JS：模板字符串
来源：http://sew.yonumen.top

`共 ${n} 条`
来源：http://rmy.bjfxy.top

[U94] JS：箭头函数
来源：http://uoi.snrcjt.cn

const double = x => x * 2;
来源：http://eoe.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://exv.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://jov.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://dnf.zhaomingkeji.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uru.ctjpmb.com

[U97] JS：并发请求
来源：http://sgg.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cbz.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://car.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uqa.shzxlz.cn

[U99] JS：事件监听
来源：http://wlh.hnqzz.top

el.addEventListener("click", e => {})
来源：http://mnb.sxryk.cn

[U100] JS：DOM 查询
来源：http://hen.yuanzhike.top

document.querySelector(".item")
来源：http://zqk.vehdjk.com

[U101] JS：classList 操作
来源：http://aij.xinyue.icu

el.classList.toggle("active")
来源：http://kvw.52xcode.cn

[U102] JS：本地存储
来源：http://wvk.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zvs.yuxming.cn

[U103] JS：定时器
来源：http://cgc.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uns.shzxlz.cn

[U104] JS：防抖
来源：http://atv.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzg.sxryk.cn

[U105] JS：节流
来源：http://hyq.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://erb.snrcjt.cn

[U106] JS：日期格式化
来源：http://cir.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wud.jqgfzy.top

[U107] JS：数字千分位
来源：http://cxy.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ror.hnqzz.top

[U108] JS：随机整数
来源：http://fbp.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pcc.wangshuangyany.cn

[U109] JS：数组分组
来源：http://ebc.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://kwp.jqgufenzy.top

[U110] JS：数组分块
来源：http://ook.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lso.sufxvd.cn

[U111] JS：对象转 Map
来源：http://tat.0kj1m.cn

new Map(Object.entries(obj))
来源：http://myz.yueranfly.top

[U112] JS：字符串补位
来源：http://pxi.zdqjudy.top

"7".padStart(3, "0")
来源：http://rqf.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://xdp.yuxming.cn

s.replaceAll("a", "b")
来源：http://aox.pycfn.com

[U114] JS：JSON 深比较
来源：http://nwi.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://uwp.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://xmd.zdbjq.cn

crypto.randomUUID()
来源：http://hkm.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://ryz.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://pkz.fehbvm.com

[U117] JS：单元测试
来源：http://hpr.havefunace.top

npm i -D vitest;  npx vitest
来源：http://wcm.cdnleiting.top

[U118] JS：开发服务器
来源：http://fow.tanke756.top

npm i -D vite;  npx vite
来源：http://ccz.vqdsnc.cn

[U119] JS：生产构建
来源：http://brr.meibo888.top

npx vite build
来源：http://git.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://hvw.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://cud.yj202588.top

================================================================================
来源：http://vzz.chenlongwang.top

统计汇总
来源：http://zfp.andypj.xyz

================================================================================
来源：http://guv.jinyuanbaomall.cn

按语言统计（条）：
来源：http://mhf.jlsjyb.cn

Python ......... 252
来源：http://gov.hcnkem.com

PHP ............ 252
来源：http://vsx.cheryme.top

JavaScript ..... 252
来源：http://fgf.chenzaomai.com

TypeScript ..... 212
来源：http://xzb.guowangkeji.top

Java ........... 212
来源：http://drx.xuetiantiany.cn

Go ............. 212
来源：http://msr.fanxiaobao.xyz

Ruby ........... 212
来源：http://ubs.gzhubu.top

C# ............. 212
来源：http://qez.0kj1m.cn

C .............. 30
来源：http://ibw.vqdsnc.cn

C++ ............ 30
来源：http://pha.guowangkeji.top

SQL ............ 90
来源：http://itj.zhixingplan.top

Bash ........... 80
来源：http://oep.zdbjq.cn

Kotlin ......... 15
来源：http://mgm.zdqjudy.top

Swift .......... 15
来源：http://ytw.chenjidiqi.icu

Lua ............ 10
来源：http://tjr.yuanzhike.top

Perl ........... 10
来源：http://zqt.yonumen.top

Scala .......... 10
来源：http://ayi.cdnleiting.top

------------------------------------
来源：http://yva.zdbjq.cn

合计 ........... 2106 条
来源：http://xcr.xingfuxueyuan.xyz

按章节统计：
来源：http://xbd.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dzj.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qbi.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vsf.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gzb.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eea.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xpx.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uwh.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xbx.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hzr.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bty.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wcb.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://msq.vehdjk.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://prz.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zgz.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vbl.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fhn.chenlongwang.top

Q SQL 专题                              90
来源：http://opu.zhoulong.xyz

R Bash 专题                             80
来源：http://bjg.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://wgk.bbcook.cn

T 其他语言补充                          60
来源：http://qgj.yangfankeji.com

U 高频实用片段                         120
来源：http://icm.bbcook.cn

------------------------------------
来源：http://chr.jqgufenzy.top

合计                                  2106 条
来源：http://sjb.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://mzr.xuetiantiany.cn

使用提醒
来源：http://tow.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://axz.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tim.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jri.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eao.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zbd.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qvl.daria6918.cn

—— 文件结束 ——
来源：http://keu.kuanghao11.cn

================================================================================
来源：http://ddu.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://onp.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://ecf.cdnleiting.top

================================================================================
来源：http://anx.daria6918.cn

【收录内容】
来源：http://qjg.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vue.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aht.chenlongwang.top

SQL · Bash · C · C++
来源：http://vnk.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rsr.yj202588.top

【使用说明】
来源：http://ukc.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://psl.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fqp.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hwk.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fvv.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ktt.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hvr.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rot.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hfh.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yea.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://peu.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://erx.smart0.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iar.fktsv.cn

【文件统计】
来源：http://bvk.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xkv.smart0.xyz

--------------------------------------------------------------------------------
来源：http://xac.tanke756.top

目  录
来源：http://dkn.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ybi.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vbj.snrcjt.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xij.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lko.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ewv.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fuz.jyoumei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sxd.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xug.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://doq.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://epr.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iao.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://irv.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fqr.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://awt.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aih.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://soo.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qev.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xcm.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://dmc.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vav.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nht.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ydy.epnwcf.com

================================================================================
来源：http://jgg.cheryme.top

A. 基础语法与类型
来源：http://wrk.sxryk.cn

================================================================================
来源：http://qqs.wangshuangyany.cn

[A01] Hello World
来源：http://gio.tianlin.xyz

Py:   print("Hello, World!")
来源：http://qjf.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://hol.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://jxn.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hhd.c1oappe.top

Java: System.out.println("Hello, World!");
来源：http://gpy.haohaochexian.top

Go:   fmt.Println("Hello, World!")
来源：http://mte.zhiwuduotai.top

Ruby: puts "Hello, World!"
来源：http://ebv.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xmp.tianlin.xyz

[A02] 变量声明与赋值
来源：http://hpq.birdmap.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mko.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rol.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://zvv.yangfankeji.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eog.cqqwz.cn

Java: String name = "Alex"; int age = 20;
来源：http://cyz.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://uqh.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://fxm.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://lxe.jinqigfzy.top

[A03] 常量定义
来源：http://qen.52xcode.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://owy.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://zjb.epnwcf.com

JS:   const PI = 3.14159;
来源：http://nnc.zhengqikj.top

TS:   const PI: number = 3.14159;
来源：http://zxv.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://kti.daria6918.cn

Go:   const PI = 3.14159
来源：http://ket.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://tnp.tanke756.top

C#:   const double PI = 3.14159;
来源：http://zgc.xylfe.cn

[A04] 判断变量类型
来源：http://zuq.0kj1m.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uuz.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vnw.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mhc.tianlin.xyz

TS:   typeof x; x instanceof Date
来源：http://qjx.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uls.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qwl.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://kxh.birdmap.top

C#:   x.GetType().Name; x is int
来源：http://nqi.vehdjk.com

[A05] 整数除法与取模
来源：http://mxp.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yoo.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uxn.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bme.yongpay.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qdx.shanyushiyangtech.top

Java: 7 / 2; 7 % 2
来源：http://tod.jyoumei.cn

Go:   7 / 2; 7 % 2
来源：http://nhr.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://hwy.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://qtc.cashguo.top

[A06] 字符串转数字
来源：http://fwy.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://sgt.haohaochexian.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lzy.xuanzx.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hws.guowangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://amf.chenlongwang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mhy.snrcjt.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zmo.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://anq.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qva.ydzc1.top

[A07] 数字转字符串
来源：http://klq.nwbrower.top

Py:   str(42)
来源：http://xec.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://adh.sxryk.cn

JS:   String(42); (42).toString()
来源：http://enn.shuidangran.top

TS:   String(42)
来源：http://sgs.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wpc.jyoumei.cn

Go:   strconv.Itoa(42)
来源：http://coj.hammf.cn

Ruby: 42.to_s
来源：http://nqz.iojbl.cn

C#:   42.ToString()
来源：http://fee.ydzc1.top

[A08] 取整与四舍五入
来源：http://bif.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zww.ctjpmb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pph.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bcv.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yil.yfazqb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zfd.xingfuxueyuan.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jeg.wangdashe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://nzi.jinghuilouyu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qwh.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://han.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rur.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mzc.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://srz.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bgf.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kep.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://las.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eqp.hcnkem.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://swe.nanxuanxn.top

[A10] 生成随机数
来源：http://gma.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://gww.havefunace.top

PHP:  random_int(1, 100);
来源：http://vfx.ehwqpu.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gus.guowangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uxf.shanyushiyangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://yae.yfazqb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tjs.gotoacloud.top

Ruby: rand(1..100)
来源：http://bts.cucudq.cn

C#:   new Random().Next(1, 101)
来源：http://vxj.xuetiantiany.cn

[A11] 条件表达式（三元）
来源：http://zho.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://ecv.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ltr.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://uxh.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://dyq.fktsv.cn

Java: x > 0 ? "yes" : "no"
来源：http://rgm.ydjk.org.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uuj.cucudq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dls.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://thb.wangdashe.top

[A12] 字符串插值 / 格式化
来源：http://qvg.gotoacloud.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iud.xziqi.cn


<!-- 参考信息 -->