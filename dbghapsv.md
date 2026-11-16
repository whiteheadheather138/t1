代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://qtv.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://sjc.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://hra.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://vqj.havefunace.top

[U75] PHP：依赖注入
来源：http://ufv.jiagoushi.top

composer require psr/container
来源：http://hii.epnwcf.com

[U76] PHP：简单路由
来源：http://wpa.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yec.yj20258888.top

[U77] PHP：模板渲染
来源：http://fjm.shzxlz.cn

composer require twig/twig
来源：http://bfx.guannengcc.top

[U78] PHP：单元测试
来源：http://nui.daria6918.cn

composer require --dev phpunit/phpunit
来源：http://vha.chenlongwang.top

[U79] PHP：静态分析
来源：http://eek.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://lrt.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://oop.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oec.hammf.cn

[U81] JS：初始化项目
来源：http://hii.zhijiandao.cn

npm init -y;  npm i express
来源：http://wjz.sxryk.cn

[U82] JS：package.json 脚本
来源：http://kgr.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ggc.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://cuq.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lvg.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://ptf.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://jsg.ydjk.org.cn

[U85] JS：可选链
来源：http://snj.hammf.cn

a?.b?.c
来源：http://sbb.ctjpmb.com

[U86] JS：空值合并
来源：http://htz.hnqzz.top

a ?? b
来源：http://gea.hnqzz.top

[U87] JS：解构默认值
来源：http://xmi.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://fhd.hywenlv.cn

[U88] JS：对象展开合并
来源：http://ggb.svipenyu.cn

{ ...a, ...b }
来源：http://sel.ctjpmb.com

[U89] JS：数组去重
来源：http://lyt.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://dme.cqqwz.cn

[U90] JS：数字数组排序
来源：http://rqo.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://fig.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://lds.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zcq.vqdsnc.cn

[U92] JS：深拷贝
来源：http://tqr.xuetiantiany.cn

structuredClone(obj)
来源：http://khr.jlsjyb.cn

[U93] JS：模板字符串
来源：http://uqi.shuidangran.top

`共 ${n} 条`
来源：http://yfn.aibaodan.cn

[U94] JS：箭头函数
来源：http://vit.jiagoushi.top

const double = x => x * 2;
来源：http://ate.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://fzf.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://dqe.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://asv.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sqb.cqqwz.cn

[U97] JS：并发请求
来源：http://zma.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iwr.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://yzd.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qpb.aizwys.cn

[U99] JS：事件监听
来源：http://sie.daria6918.cn

el.addEventListener("click", e => {})
来源：http://bbk.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://own.xziqi.cn

document.querySelector(".item")
来源：http://ppy.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://gok.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://qxu.jyoumei.cn

[U102] JS：本地存储
来源：http://ucl.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hbf.0kj1m.cn

[U103] JS：定时器
来源：http://uoz.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wbc.yonumen.top

[U104] JS：防抖
来源：http://qax.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://afe.redwolf501.top

[U105] JS：节流
来源：http://vkh.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hbj.kuanghao11.cn

[U106] JS：日期格式化
来源：http://hru.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kiq.sysykeji.top

[U107] JS：数字千分位
来源：http://jot.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvs.wangdashe.top

[U108] JS：随机整数
来源：http://udd.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zsn.fengsongda.top

[U109] JS：数组分组
来源：http://zbl.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://pwc.yuxming.cn

[U110] JS：数组分块
来源：http://yhd.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kbv.aizwys.cn

[U111] JS：对象转 Map
来源：http://xej.xinyue.icu

new Map(Object.entries(obj))
来源：http://zfi.tian-w.cn

[U112] JS：字符串补位
来源：http://lau.gaohongyu789.top

"7".padStart(3, "0")
来源：http://fgb.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://bes.sweek.top

s.replaceAll("a", "b")
来源：http://jyl.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://yde.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://hbu.yongpay.top

[U115] JS：生成 UUID
来源：http://zjh.aizwys.cn

crypto.randomUUID()
来源：http://lud.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://pkk.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://uyc.tanke756.top

[U117] JS：单元测试
来源：http://ypl.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://kwz.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://wvg.hfpthk.cn

npm i -D vite;  npx vite
来源：http://omm.c1oappe.top

[U119] JS：生产构建
来源：http://unt.ydzc1.top

npx vite build
来源：http://img.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://kza.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://jvv.jiagoushi.top

================================================================================
来源：http://lot.hammf.cn

统计汇总
来源：http://wlc.ydjk.org.cn

================================================================================
来源：http://nor.snrcjt.cn

按语言统计（条）：
来源：http://oza.jinyuanbaomall.cn

Python ......... 252
来源：http://pcv.epnwcf.com

PHP ............ 252
来源：http://drj.hfpthk.cn

JavaScript ..... 252
来源：http://cda.9152youxi.cn

TypeScript ..... 212
来源：http://oaw.jinghuilouyu.cn

Java ........... 212
来源：http://nap.ctjpmb.com

Go ............. 212
来源：http://dpj.iojbl.cn

Ruby ........... 212
来源：http://sbx.xuanzx.com

C# ............. 212
来源：http://zto.smart0.xyz

C .............. 30
来源：http://dbf.hysaishi.cn

C++ ............ 30
来源：http://ccp.gzhubu.top

SQL ............ 90
来源：http://muz.yueranfly.top

Bash ........... 80
来源：http://xok.shanyushiyangtech.top

Kotlin ......... 15
来源：http://mvv.hammf.cn

Swift .......... 15
来源：http://crm.c1oappe.top

Lua ............ 10
来源：http://lqh.daria6918.cn

Perl ........... 10
来源：http://gsn.fehbvm.com

Scala .......... 10
来源：http://diq.ppjwa.cn

------------------------------------
来源：http://nuu.xylfe.cn

合计 ........... 2106 条
来源：http://phq.tian-w.cn

按章节统计：
来源：http://duv.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oqi.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://esb.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zvn.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ijk.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lau.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uts.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hdj.jinqigfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vga.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nqg.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xre.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cov.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kcg.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tdk.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uws.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wiv.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gwq.birdmap.top

Q SQL 专题                              90
来源：http://ucl.yongpay.top

R Bash 专题                             80
来源：http://qjp.bbcook.cn

S C / C++ 专题                          60
来源：http://wmx.cheryme.top

T 其他语言补充                          60
来源：http://lma.epnwcf.com

U 高频实用片段                         120
来源：http://koy.xingfuxueyuan.xyz

------------------------------------
来源：http://jtf.cashguo.top

合计                                  2106 条
来源：http://gky.sweek.top

--------------------------------------------------------------------------------
来源：http://mnc.ehwqpu.com

使用提醒
来源：http://rmv.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://yny.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jig.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ipc.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ant.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://drl.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sju.zhoulong.xyz

—— 文件结束 ——
来源：http://jst.sxryk.cn

================================================================================
来源：http://olk.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://sdd.zhixingplan.top

Common Programming Examples Cheat Book
来源：http://mug.feifeiyinyue.top

================================================================================
来源：http://uos.c1oappe.top

【收录内容】
来源：http://rxp.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kpm.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gys.jyoumei.cn

SQL · Bash · C · C++
来源：http://ioh.cashguo.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ata.cqqwz.cn

【使用说明】
来源：http://dxw.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aae.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rbm.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://isw.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aym.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://znf.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pqo.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ptz.snrcjt.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hvq.tian-w.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eoy.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uum.hysaishi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dhh.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ayn.kuanghao11.cn

【文件统计】
来源：http://oee.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jhw.xylfe.cn

--------------------------------------------------------------------------------
来源：http://kzr.bbcook.cn

目  录
来源：http://ezw.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://zky.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://usv.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kkp.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oul.redwolf501.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iop.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aog.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oxu.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fql.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wqh.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dqg.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yqz.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cuc.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jxc.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tqc.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zri.pengpengdd.cyou

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pus.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fju.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gtf.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ypd.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://udr.zhoulong.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwp.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fmo.fengsongda.top

================================================================================
来源：http://bnz.jiagoushi.top

A. 基础语法与类型
来源：http://wgx.cashguo.top

================================================================================
来源：http://hru.yuxming.cn

[A01] Hello World
来源：http://apg.andypj.xyz

Py:   print("Hello, World!")
来源：http://tjg.xuanzx.com

PHP:  echo "Hello, World!";
来源：http://yht.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://okv.aibaodan.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nrv.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://cyh.gotoacloud.top

Go:   fmt.Println("Hello, World!")
来源：http://awx.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://zqc.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ulr.tanke756.top

[A02] 变量声明与赋值
来源：http://ylc.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rmh.aibaodan.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ree.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://cbd.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eej.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://fer.sweek.top

Go:   name := "Alex"; age := 20
来源：http://yeq.tian-w.cn

Ruby: name = "Alex"; age = 20
来源：http://gsd.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://avo.shzxlz.cn

[A03] 常量定义
来源：http://uay.c1oappe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xlj.yj20258.top

PHP:  const PI = 3.14159;
来源：http://qgj.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://reg.kuanghao11.cn

TS:   const PI: number = 3.14159;
来源：http://mhp.meibo888.top

Java: static final double PI = 3.14159;
来源：http://aih.jyoumei.cn

Go:   const PI = 3.14159
来源：http://okq.shuidangran.top

Ruby: PI = 3.14159
来源：http://lpo.xylfe.cn

C#:   const double PI = 3.14159;
来源：http://kph.smart0.xyz

[A04] 判断变量类型
来源：http://fuu.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nqp.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kvl.chenzaomai.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pgq.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://dsl.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bom.jinyuanbaomall.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ncs.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://sfy.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://itn.tarul.cn

[A05] 整数除法与取模
来源：http://uyw.yj202588.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://elu.yonumen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ilo.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ymm.gaohongyu789.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://npd.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://wze.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://evf.gaohongyu789.top

Ruby: 7 / 2; 7 % 2
来源：http://vpe.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://jvl.jianghu66.top

[A06] 字符串转数字
来源：http://jla.shzxlz.cn

Py:   int("42"); float("3.14")
来源：http://fhv.shuidangran.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tte.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gos.nanxuanxn.top

TS:   parseInt("42", 10); Number("42")
来源：http://dvn.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dkh.snrcjt.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://drk.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bjh.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://maa.andypj.xyz

[A07] 数字转字符串
来源：http://loi.fzhhl.top

Py:   str(42)
来源：http://tmk.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://pro.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://fwu.nwbrower.top

TS:   String(42)
来源：http://tad.svipenyu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ksw.gaohongyu789.top

Go:   strconv.Itoa(42)
来源：http://xwo.tian-w.cn

Ruby: 42.to_s
来源：http://men.nanxinkj.top

C#:   42.ToString()
来源：http://jst.snrcjt.cn

[A08] 取整与四舍五入
来源：http://uqc.shanyushiyangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iog.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kyq.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qru.vehdjk.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jbg.shanyushiyangtech.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lvr.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yuj.ehwqpu.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://yis.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bus.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://fjr.0kj1m.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://taz.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qfo.havefunace.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bhc.yueranfly.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ghh.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ebg.epnwcf.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ldz.fktsv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qzf.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lwz.yueranfly.top

[A10] 生成随机数
来源：http://tnk.shangyingyoupin.top

Py:   import random; random.randint(1, 100)
来源：http://iop.zdqjudy.top

PHP:  random_int(1, 100);
来源：http://rbj.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fzn.tian-w.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ycp.xylfe.cn

Java: new Random().nextInt(100) + 1
来源：http://wye.cdnleiting.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://adm.zhengqikj.top

Ruby: rand(1..100)
来源：http://hbx.kuanghao11.cn

C#:   new Random().Next(1, 101)
来源：http://ccg.gotoacloud.top

[A11] 条件表达式（三元）
来源：http://stx.shanyushiyangtech.top

Py:   "yes" if x > 0 else "no"
来源：http://lfm.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oku.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://liq.tian-w.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ulj.nanxinkj.top

Java: x > 0 ? "yes" : "no"
来源：http://mds.tarul.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vdu.yonumen.top


<!-- 参考信息 -->