代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://ecg.tarul.cn

parse_ini_file("config.ini", true)
来源：http://ihm.hcnkem.com

[U74] PHP：读取环境变量
来源：http://cyf.cashguo.top

getenv("APP_ENV") ?: "production"
来源：http://wxh.meibo888.top

[U75] PHP：依赖注入
来源：http://owv.yueranfly.top

composer require psr/container
来源：http://omi.tarul.cn

[U76] PHP：简单路由
来源：http://pcj.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://svz.fzhhl.top

[U77] PHP：模板渲染
来源：http://uke.hfpthk.cn

composer require twig/twig
来源：http://klv.xuanzx.com

[U78] PHP：单元测试
来源：http://zpt.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://cwp.bjfxy.top

[U79] PHP：静态分析
来源：http://hof.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://pka.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://hso.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ljq.chenlongwang.top

[U81] JS：初始化项目
来源：http://bpr.cashguo.top

npm init -y;  npm i express
来源：http://tek.daria6918.cn

[U82] JS：package.json 脚本
来源：http://tmh.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vwl.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://xxp.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://huc.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://uma.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://bjt.yuxming.cn

[U85] JS：可选链
来源：http://lwy.yvedp.cn

a?.b?.c
来源：http://ppi.tarul.cn

[U86] JS：空值合并
来源：http://mqr.jqgfzy.top

a ?? b
来源：http://kbe.jianghu66.top

[U87] JS：解构默认值
来源：http://rgs.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://dnq.yongpay.top

[U88] JS：对象展开合并
来源：http://cyy.bjfxy.top

{ ...a, ...b }
来源：http://cpx.sufxvd.cn

[U89] JS：数组去重
来源：http://lfj.mhx1999.top

[...new Set(arr)]
来源：http://waj.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://zya.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://usj.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://jcp.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vfu.havefunace.top

[U92] JS：深拷贝
来源：http://ssb.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://svo.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://wqq.yueranfly.top

`共 ${n} 条`
来源：http://cea.tanke756.top

[U94] JS：箭头函数
来源：http://kmj.zycfv.cn

const double = x => x * 2;
来源：http://crc.hywenlv.cn

[U95] JS：Promise 包装
来源：http://hka.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://hic.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://upb.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ygy.pycfn.com

[U97] JS：并发请求
来源：http://jvk.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bvo.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://hao.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eki.c1oappe.top

[U99] JS：事件监听
来源：http://ssl.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://rbq.redwolf501.top

[U100] JS：DOM 查询
来源：http://koi.shanyushiyangtech.top

document.querySelector(".item")
来源：http://wle.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://rev.ctjpmb.com

el.classList.toggle("active")
来源：http://gkb.xylfe.cn

[U102] JS：本地存储
来源：http://her.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://exb.daxiang520.top

[U103] JS：定时器
来源：http://rch.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uut.bjfxy.top

[U104] JS：防抖
来源：http://rjw.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hjh.ydzc1.top

[U105] JS：节流
来源：http://mnc.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hmu.jqgfzy.top

[U106] JS：日期格式化
来源：http://ysj.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qos.cdnleiting.top

[U107] JS：数字千分位
来源：http://puu.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pgb.pengpengdd.cyou

[U108] JS：随机整数
来源：http://okf.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fzf.wangdashe.top

[U109] JS：数组分组
来源：http://yod.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://gcx.shangyingyoupin.top

[U110] JS：数组分块
来源：http://jrs.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wij.mhx1999.top

[U111] JS：对象转 Map
来源：http://eci.ehwqpu.com

new Map(Object.entries(obj))
来源：http://bjl.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://bpb.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://jmx.52xcode.cn

[U113] JS：正则替换全部
来源：http://kgx.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://rvv.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://ojw.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://amc.xuanzx.com

[U115] JS：生成 UUID
来源：http://vwo.fktsv.cn

crypto.randomUUID()
来源：http://wim.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://upw.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://mon.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://jna.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://plq.zdqjudy.top

[U118] JS：开发服务器
来源：http://hbu.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://jro.yueranfly.top

[U119] JS：生产构建
来源：http://vdf.zdbjq.cn

npx vite build
来源：http://xlq.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://cgo.pycfn.com

import.meta.env.VITE_API_URL
来源：http://shs.quarkkingdee.top

================================================================================
来源：http://szl.aizwys.cn

统计汇总
来源：http://cyj.dianchejie.cn

================================================================================
来源：http://dwz.wangshuangyany.cn

按语言统计（条）：
来源：http://bxx.hongshengwenyu.top

Python ......... 252
来源：http://zch.yvedp.cn

PHP ............ 252
来源：http://wwc.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://rdo.yj202588.top

TypeScript ..... 212
来源：http://ppg.kuanghao11.cn

Java ........... 212
来源：http://ogq.sweek.top

Go ............. 212
来源：http://hdr.chenjidiqi.icu

Ruby ........... 212
来源：http://nnb.bjfxy.top

C# ............. 212
来源：http://mra.shzxlz.cn

C .............. 30
来源：http://xzm.shuidangran.top

C++ ............ 30
来源：http://gkl.aibaodan.cn

SQL ............ 90
来源：http://xhh.yj202588.top

Bash ........... 80
来源：http://ewd.zdbjq.cn

Kotlin ......... 15
来源：http://lib.jlsjyb.cn

Swift .......... 15
来源：http://ewh.gotoacloud.top

Lua ............ 10
来源：http://log.zhixingplan.top

Perl ........... 10
来源：http://jpp.ehwqpu.com

Scala .......... 10
来源：http://wfv.fktsv.cn

------------------------------------
来源：http://rrp.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://lrp.fktsv.cn

按章节统计：
来源：http://mkn.chenlongwang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ezk.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://anl.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wil.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fje.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rwb.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bvb.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jxg.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qcm.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ngp.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://urr.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hla.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mjq.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ptq.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qft.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wlw.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vni.52xcode.cn

Q SQL 专题                              90
来源：http://ues.jinqigfzy.top

R Bash 专题                             80
来源：http://hxm.daria6918.cn

S C / C++ 专题                          60
来源：http://ztn.xuetiantiany.cn

T 其他语言补充                          60
来源：http://tpd.cheryme.top

U 高频实用片段                         120
来源：http://lcg.sysykeji.top

------------------------------------
来源：http://nus.xylfe.cn

合计                                  2106 条
来源：http://ohz.tanke756.top

--------------------------------------------------------------------------------
来源：http://tzd.shuidangran.top

使用提醒
来源：http://uaf.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://pat.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aco.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://adg.9152youxi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wbo.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bpw.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://crm.shuidangran.top

—— 文件结束 ——
来源：http://esc.cheryme.top

================================================================================
来源：http://pky.bjfxy.top

程序语言常见例子速查手册（2024 版）
来源：http://ciy.redwolf501.top

Common Programming Examples Cheat Book
来源：http://vvm.fktsv.cn

================================================================================
来源：http://fhq.tanke756.top

【收录内容】
来源：http://owk.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oen.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://irc.jinqigufen.top

SQL · Bash · C · C++
来源：http://ogq.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rjb.ydzc1.top

【使用说明】
来源：http://ebc.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://apt.xuanzx.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wwt.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lhk.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lwl.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lcy.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kum.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ivt.daria6918.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ccr.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mpl.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://atk.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pxk.tianlin.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rnh.ppjwa.cn

【文件统计】
来源：http://jmz.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qoo.fengsongda.top

--------------------------------------------------------------------------------
来源：http://jrc.xinyue.icu

目  录
来源：http://okz.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://mpg.gogol.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qai.ppjwa.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://epl.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gwx.wangdashe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://frc.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kvo.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bkb.yfazqb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://quv.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aoq.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pma.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://psx.chenzaomai.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wgb.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rjd.jqgufenzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kcn.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nnn.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jso.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://szx.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cqw.smart0.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://yma.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dij.tian-w.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bci.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vhl.yonumen.top

================================================================================
来源：http://bod.fzhhl.top

A. 基础语法与类型
来源：http://qjz.shanyushiyangkeji.top

================================================================================
来源：http://cbd.svipenyu.cn

[A01] Hello World
来源：http://jmz.snrcjt.cn

Py:   print("Hello, World!")
来源：http://yuy.mhx1999.top

PHP:  echo "Hello, World!";
来源：http://ses.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://kgs.hnqzz.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cvj.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://ecc.hongshengwenyu.top

Go:   fmt.Println("Hello, World!")
来源：http://ufr.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://qqn.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://omk.ydzc1.top

[A02] 变量声明与赋值
来源：http://lhm.yueranfly.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ymu.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yek.cqqwz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://djj.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://exe.ydzc1.top

Java: String name = "Alex"; int age = 20;
来源：http://fdz.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://vta.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://qte.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lwi.kuanghao11.cn

[A03] 常量定义
来源：http://frc.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nkb.redwolf501.top

PHP:  const PI = 3.14159;
来源：http://fqg.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://fmu.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://uyj.sxryk.cn

Java: static final double PI = 3.14159;
来源：http://exk.hesvh.cn

Go:   const PI = 3.14159
来源：http://exn.9152youxi.cn

Ruby: PI = 3.14159
来源：http://app.yuxming.cn

C#:   const double PI = 3.14159;
来源：http://hur.cheryme.top

[A04] 判断变量类型
来源：http://bsu.yj20258.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://gnu.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://shj.yuxming.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vtv.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://vke.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mzb.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dxa.jinyuanbaomall.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pcr.sufxvd.cn

C#:   x.GetType().Name; x is int
来源：http://bpt.c1oappe.top

[A05] 整数除法与取模
来源：http://mtg.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://auj.chenzaomai.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ajd.smart0.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tih.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ojm.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://wgd.uphjek.com

Go:   7 / 2; 7 % 2
来源：http://bzw.zhengqikj.top

Ruby: 7 / 2; 7 % 2
来源：http://hqo.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://nja.shanyushiyangtech.top

[A06] 字符串转数字
来源：http://qkc.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://haj.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eyn.ybcxt.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wed.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://qdf.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wmh.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fis.xinyue.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://lej.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wbc.yj202588.top

[A07] 数字转字符串
来源：http://nnb.chenlongwang.top

Py:   str(42)
来源：http://krn.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://vyy.jianghu66.top

JS:   String(42); (42).toString()
来源：http://ryy.jlsjyb.cn

TS:   String(42)
来源：http://vtc.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://grv.cheryme.top

Go:   strconv.Itoa(42)
来源：http://fan.gogol.net.cn

Ruby: 42.to_s
来源：http://yzq.hcnkem.com

C#:   42.ToString()
来源：http://nip.hnqzz.top

[A08] 取整与四舍五入
来源：http://lkm.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yrk.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mus.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://toh.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zgd.bbcook.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mpr.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jsh.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yww.yanxiufei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pdd.jinyuanbaomall.cn

[A09] 绝对值与最大最小值
来源：http://lwb.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ttb.wangdashe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jmc.xylfe.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mqz.zdbjq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://acr.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yrb.yonumen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://unx.nanxinkj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://syc.yuxming.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sey.jinqigfzy.top

[A10] 生成随机数
来源：http://mvf.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://qjr.dashuyun.cn

PHP:  random_int(1, 100);
来源：http://nht.yj20258.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://glz.pycfn.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mxe.haohaochexian.top

Java: new Random().nextInt(100) + 1
来源：http://rvu.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aop.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://rei.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://vjh.cheryme.top

[A11] 条件表达式（三元）
来源：http://nwf.hfpthk.cn

Py:   "yes" if x > 0 else "no"
来源：http://fny.sufxvd.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://brg.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aue.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dbd.vehdjk.com

Java: x > 0 ? "yes" : "no"
来源：http://who.nanxuanxn.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ofq.yongpay.top


<!-- 参考信息 -->