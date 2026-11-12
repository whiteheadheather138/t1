代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://sgj.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://mnh.yj202588.top

[U74] PHP：读取环境变量
来源：http://goe.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://xjn.bbcook.cn

[U75] PHP：依赖注入
来源：http://fyi.tianlin.xyz

composer require psr/container
来源：http://ogx.zycfv.cn

[U76] PHP：简单路由
来源：http://opq.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ggz.jiagoushi.top

[U77] PHP：模板渲染
来源：http://oqd.jinghuilouyu.cn

composer require twig/twig
来源：http://lix.cheryme.top

[U78] PHP：单元测试
来源：http://agp.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://ckq.tianlin.xyz

[U79] PHP：静态分析
来源：http://pkp.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://nyq.redwolf501.top

[U80] PHP：代码规范修复
来源：http://xkr.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pme.ydjk.org.cn

[U81] JS：初始化项目
来源：http://yiv.feifeiyinyue.top

npm init -y;  npm i express
来源：http://vje.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://kqf.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jcu.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://mgg.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://sez.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://ami.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://scs.guowangkeji.top

[U85] JS：可选链
来源：http://ujp.tian-w.cn

a?.b?.c
来源：http://fvg.ppjwa.cn

[U86] JS：空值合并
来源：http://yua.hammf.cn

a ?? b
来源：http://kvy.guowangkeji.top

[U87] JS：解构默认值
来源：http://jfx.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://unb.sweek.top

[U88] JS：对象展开合并
来源：http://mkn.yangfankeji.com

{ ...a, ...b }
来源：http://ahn.yongpay.top

[U89] JS：数组去重
来源：http://hdy.feifeiyinyue.top

[...new Set(arr)]
来源：http://jsx.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://rga.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://ubq.cheryme.top

[U91] JS：对象键值遍历
来源：http://ttj.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cok.jianghu66.top

[U92] JS：深拷贝
来源：http://djy.zhixingplan.top

structuredClone(obj)
来源：http://mca.daria6918.cn

[U93] JS：模板字符串
来源：http://klh.cheryme.top

`共 ${n} 条`
来源：http://tcs.uphjek.com

[U94] JS：箭头函数
来源：http://vry.hesvh.cn

const double = x => x * 2;
来源：http://cjk.ppjwa.cn

[U95] JS：Promise 包装
来源：http://jal.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://hkl.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://xzd.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hza.tian-w.cn

[U97] JS：并发请求
来源：http://guu.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qxw.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://zol.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yoj.52xcode.cn

[U99] JS：事件监听
来源：http://mso.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://xao.yfazqb.com

[U100] JS：DOM 查询
来源：http://lad.tian-w.cn

document.querySelector(".item")
来源：http://lxx.jinqigufen.top

[U101] JS：classList 操作
来源：http://heq.cdnleiting.top

el.classList.toggle("active")
来源：http://std.ppjwa.cn

[U102] JS：本地存储
来源：http://giu.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zlr.ehwqpu.com

[U103] JS：定时器
来源：http://yzh.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://byb.quarkkingdee.top

[U104] JS：防抖
来源：http://jqz.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yfz.xinyue.icu

[U105] JS：节流
来源：http://yzt.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gzl.sjlbkw.cn

[U106] JS：日期格式化
来源：http://vvt.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lgv.vqdsnc.cn

[U107] JS：数字千分位
来源：http://vwi.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tbq.vqdsnc.cn

[U108] JS：随机整数
来源：http://gnd.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yau.pycfn.com

[U109] JS：数组分组
来源：http://uda.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://tiq.ctjpmb.com

[U110] JS：数组分块
来源：http://tcf.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jtc.hammf.cn

[U111] JS：对象转 Map
来源：http://lwm.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://tjo.bbcook.cn

[U112] JS：字符串补位
来源：http://nob.daria6918.cn

"7".padStart(3, "0")
来源：http://lkk.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://gcc.zycfv.cn

s.replaceAll("a", "b")
来源：http://poe.xziqi.cn

[U114] JS：JSON 深比较
来源：http://jgn.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xty.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://edt.uphjek.com

crypto.randomUUID()
来源：http://mov.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://srr.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://yct.jqgfzy.top

[U117] JS：单元测试
来源：http://xii.yj20258.top

npm i -D vitest;  npx vitest
来源：http://tqa.daxiang520.top

[U118] JS：开发服务器
来源：http://vex.cdnleiting.top

npm i -D vite;  npx vite
来源：http://mdu.sysykeji.top

[U119] JS：生产构建
来源：http://dpt.xylfe.cn

npx vite build
来源：http://wyj.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://hld.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://afp.jinghuilouyu.cn

================================================================================
来源：http://fwy.hongshengwenyu.top

统计汇总
来源：http://pea.tanke756.top

================================================================================
来源：http://dut.52xcode.cn

按语言统计（条）：
来源：http://lvv.cucudq.cn

Python ......... 252
来源：http://aiq.xylfe.cn

PHP ............ 252
来源：http://epi.hesvh.cn

JavaScript ..... 252
来源：http://tdc.redwolf501.top

TypeScript ..... 212
来源：http://zop.iojbl.cn

Java ........... 212
来源：http://pzz.xuetiantiany.cn

Go ............. 212
来源：http://zjz.52xcode.cn

Ruby ........... 212
来源：http://zxj.52xcode.cn

C# ............. 212
来源：http://njd.cheryme.top

C .............. 30
来源：http://auu.hnxiangtu.top

C++ ............ 30
来源：http://hal.yuanzhike.top

SQL ............ 90
来源：http://kmb.redwolf501.top

Bash ........... 80
来源：http://cgv.yueranfly.top

Kotlin ......... 15
来源：http://vrp.ehwqpu.com

Swift .......... 15
来源：http://wpc.ehwqpu.com

Lua ............ 10
来源：http://ndd.hesvh.cn

Perl ........... 10
来源：http://chc.yj20258888.top

Scala .......... 10
来源：http://gsf.zhixingplan.top

------------------------------------
来源：http://wqz.quarkkingdee.top

合计 ........... 2106 条
来源：http://pkr.fktsv.cn

按章节统计：
来源：http://fhc.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dmc.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aax.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wcg.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eaz.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ozr.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cwf.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mwj.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ijc.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jmp.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vzv.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://acm.shangyingyoupin.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yoy.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pjr.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nsv.redwolf501.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qkj.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nmf.9152youxi.cn

Q SQL 专题                              90
来源：http://vsh.ctjpmb.com

R Bash 专题                             80
来源：http://epc.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://eax.yj20258.top

T 其他语言补充                          60
来源：http://xji.dashuyun.cn

U 高频实用片段                         120
来源：http://kdd.316326.xyz

------------------------------------
来源：http://rva.zhixingplan.top

合计                                  2106 条
来源：http://rsv.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://ucz.tanke756.top

使用提醒
来源：http://xsb.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://tau.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gfd.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sks.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zvs.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://xrq.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qnc.xylfe.cn

—— 文件结束 ——
来源：http://dvi.shangyingyoupin.top

================================================================================
来源：http://kdr.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://cki.ivvv.top

Common Programming Examples Cheat Book
来源：http://wgt.birdmap.top

================================================================================
来源：http://xrn.yj20258.top

【收录内容】
来源：http://rew.hesvh.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gdg.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://elp.xziqi.cn

SQL · Bash · C · C++
来源：http://qiw.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oty.andypj.xyz

【使用说明】
来源：http://oxn.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rrd.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ued.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://efl.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pgv.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nod.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bnb.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nmp.cheryme.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zpq.zhengqikj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jjz.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hvl.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hdp.sweek.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bsa.fanxiaobao.xyz

【文件统计】
来源：http://bts.hywenlv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vhj.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://fyd.xziqi.cn

目  录
来源：http://kem.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://rwd.fanxiaobao.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cxq.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qkh.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://erg.hysaishi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://flb.gaohongyu789.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cmu.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pxx.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lhl.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gpf.sufxvd.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oye.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://orv.yj202588.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jsr.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jaa.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qqe.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ptd.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://irm.smart0.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://apo.zhijiandao.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ayk.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ndn.zhijiandao.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sao.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sja.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xkp.yvedp.cn

================================================================================
来源：http://xew.daria6918.cn

A. 基础语法与类型
来源：http://vxz.birdmap.top

================================================================================
来源：http://jqo.zhijiandao.cn

[A01] Hello World
来源：http://glf.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://lxs.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://cqy.xinyue.icu

JS:   console.log("Hello, World!");
来源：http://rwd.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://boa.hnxiangtu.top

Java: System.out.println("Hello, World!");
来源：http://bxj.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://sfj.wangshuangyany.cn

Ruby: puts "Hello, World!"
来源：http://yos.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mnc.jqgufenzy.top

[A02] 变量声明与赋值
来源：http://ree.yonumen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yvk.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fir.shuidangran.top

JS:   let name = "Alex"; const age = 20;
来源：http://mhe.sjlbkw.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jxx.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://gzj.sysykeji.top

Go:   name := "Alex"; age := 20
来源：http://zna.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://hho.hnxiangtu.top

C#:   string name = "Alex"; int age = 20;
来源：http://gye.jinyuanbaomall.cn

[A03] 常量定义
来源：http://boj.zhongyouzk.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sfa.ivvv.top

PHP:  const PI = 3.14159;
来源：http://tzu.ppjwa.cn

JS:   const PI = 3.14159;
来源：http://zfa.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://eqa.jiagoushi.top

Java: static final double PI = 3.14159;
来源：http://fng.uphjek.com

Go:   const PI = 3.14159
来源：http://hpr.uphjek.com

Ruby: PI = 3.14159
来源：http://npn.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://cwd.cashguo.top

[A04] 判断变量类型
来源：http://pyi.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uec.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sip.ivvv.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kzk.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://zdj.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://szf.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://ust.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ngl.ppjwa.cn

C#:   x.GetType().Name; x is int
来源：http://ypy.yueranfly.top

[A05] 整数除法与取模
来源：http://agp.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xhw.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://waa.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sls.9152youxi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://etx.hysaishi.cn

Java: 7 / 2; 7 % 2
来源：http://qae.ehwqpu.com

Go:   7 / 2; 7 % 2
来源：http://huh.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://vjr.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://sjw.guowangkeji.top

[A06] 字符串转数字
来源：http://vsu.uphjek.com

Py:   int("42"); float("3.14")
来源：http://zzd.52xcode.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tze.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zug.xziqi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vzj.zhengqikj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://txh.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rbg.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nrm.yvedp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xvv.shuidangran.top

[A07] 数字转字符串
来源：http://alz.havefunace.top

Py:   str(42)
来源：http://dpx.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://yhu.ydzc1.top

JS:   String(42); (42).toString()
来源：http://gku.fehbvm.com

TS:   String(42)
来源：http://psj.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://axh.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://awi.ctjpmb.com

Ruby: 42.to_s
来源：http://hjf.guowangkeji.top

C#:   42.ToString()
来源：http://wef.ivvv.top

[A08] 取整与四舍五入
来源：http://mnn.zhixingplan.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://npy.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rhk.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lkk.bjfxy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ows.bbcook.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://djy.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bgr.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wtw.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://txs.vehdjk.com

[A09] 绝对值与最大最小值
来源：http://omy.yj202588.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ntn.dashuyun.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cuq.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rkz.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ibp.iojbl.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fqd.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qht.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jbb.snrcjt.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ftm.zdbjq.cn

[A10] 生成随机数
来源：http://kcj.snrcjt.cn

Py:   import random; random.randint(1, 100)
来源：http://mtp.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://pdo.nanxuanxn.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bam.yongpay.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bie.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://hkw.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qtf.nwbrower.top

Ruby: rand(1..100)
来源：http://rjb.chenjidiqi.icu

C#:   new Random().Next(1, 101)
来源：http://pbj.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://fyl.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://wbk.andypj.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://fja.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://qdd.aizwys.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fcc.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://vpf.yj20258888.top

Go:   // 无三元运算符，需用 if 语句
来源：http://riv.tianlin.xyz


<!-- 参考信息 -->