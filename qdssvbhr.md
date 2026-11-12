代发 wailian999

[U77] PHP：模板渲染
来源：http://wtu.jlsjyb.cn

composer require twig/twig
来源：http://avh.ivvv.top

[U78] PHP：单元测试
来源：http://qwo.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://qmh.fzhhl.top

[U79] PHP：静态分析
来源：http://cwz.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://bgg.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://epe.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vvs.guannengcc.top

[U81] JS：初始化项目
来源：http://amz.nanxuanxn.top

npm init -y;  npm i express
来源：http://vbo.jianghu66.top

[U82] JS：package.json 脚本
来源：http://vld.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lfr.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://swx.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ile.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://pse.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://dvo.xuetiantiany.cn

[U85] JS：可选链
来源：http://gxj.meibo888.top

a?.b?.c
来源：http://lxe.ivvv.top

[U86] JS：空值合并
来源：http://ani.ydzc1.top

a ?? b
来源：http://luz.tian-w.cn

[U87] JS：解构默认值
来源：http://ejg.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://cah.xylfe.cn

[U88] JS：对象展开合并
来源：http://mpa.aizwys.cn

{ ...a, ...b }
来源：http://ord.pycfn.com

[U89] JS：数组去重
来源：http://jxx.zdqjudy.top

[...new Set(arr)]
来源：http://jyz.hnqzz.top

[U90] JS：数字数组排序
来源：http://llu.gotoacloud.top

[...arr].sort((a, b) => a - b)
来源：http://rag.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://uxb.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fhp.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://emo.pycfn.com

structuredClone(obj)
来源：http://ubs.zycfv.cn

[U93] JS：模板字符串
来源：http://rkt.wangshuangyany.cn

`共 ${n} 条`
来源：http://lae.zhengqikj.top

[U94] JS：箭头函数
来源：http://eif.ppjwa.cn

const double = x => x * 2;
来源：http://lcb.hammf.cn

[U95] JS：Promise 包装
来源：http://yde.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://tyt.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://sku.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://loy.iojbl.cn

[U97] JS：并发请求
来源：http://iyr.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zsp.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://kih.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rby.yonumen.top

[U99] JS：事件监听
来源：http://den.epnwcf.com

el.addEventListener("click", e => {})
来源：http://hrt.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://klm.sweek.top

document.querySelector(".item")
来源：http://cpd.jinqigufen.top

[U101] JS：classList 操作
来源：http://cvm.svipenyu.cn

el.classList.toggle("active")
来源：http://hjf.xuetiantiany.cn

[U102] JS：本地存储
来源：http://zoq.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mmt.feifeiyinyue.top

[U103] JS：定时器
来源：http://wix.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ihw.aizwys.cn

[U104] JS：防抖
来源：http://exh.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://htw.tanke756.top

[U105] JS：节流
来源：http://dqs.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wyf.chenzaomai.com

[U106] JS：日期格式化
来源：http://ppt.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jna.zycfv.cn

[U107] JS：数字千分位
来源：http://pzq.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sup.fktsv.cn

[U108] JS：随机整数
来源：http://atx.xuetiantiany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zfd.yfazqb.com

[U109] JS：数组分组
来源：http://uxc.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://cux.hammf.cn

[U110] JS：数组分块
来源：http://yhd.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ykv.aibaodan.cn

[U111] JS：对象转 Map
来源：http://gsj.gogol.net.cn

new Map(Object.entries(obj))
来源：http://nns.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://oiv.ppjwa.cn

"7".padStart(3, "0")
来源：http://pag.svipenyu.cn

[U113] JS：正则替换全部
来源：http://uii.yj20258888.top

s.replaceAll("a", "b")
来源：http://tyg.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://dne.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jzz.0kj1m.cn

[U115] JS：生成 UUID
来源：http://xnp.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://gcr.jqgufenzy.top

[U116] JS：类型检查（JSDoc）
来源：http://ywc.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://ypd.pycfn.com

[U117] JS：单元测试
来源：http://tfc.pycfn.com

npm i -D vitest;  npx vitest
来源：http://vnl.jqgfzy.top

[U118] JS：开发服务器
来源：http://bjp.iojbl.cn

npm i -D vite;  npx vite
来源：http://gju.birdmap.top

[U119] JS：生产构建
来源：http://rcw.iojbl.cn

npx vite build
来源：http://lkv.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://ncq.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://qed.yj202588.top

================================================================================
来源：http://dxm.xuanzx.com

统计汇总
来源：http://hst.zycfv.cn

================================================================================
来源：http://vwr.chenzaomai.com

按语言统计（条）：
来源：http://vvo.chenjidiqi.icu

Python ......... 252
来源：http://ekw.zhiwuduotai.top

PHP ............ 252
来源：http://bbv.chenzaomai.com

JavaScript ..... 252
来源：http://zja.haohaochexian.top

TypeScript ..... 212
来源：http://ajg.redwolf501.top

Java ........... 212
来源：http://qbw.hysaishi.cn

Go ............. 212
来源：http://xlq.xuanzx.com

Ruby ........... 212
来源：http://ztw.ctjpmb.com

C# ............. 212
来源：http://egj.chenlongwang.top

C .............. 30
来源：http://kvi.fanxiaobao.xyz

C++ ............ 30
来源：http://mlz.yonumen.top

SQL ............ 90
来源：http://def.yueranfly.top

Bash ........... 80
来源：http://nlx.yanxiufei.cn

Kotlin ......... 15
来源：http://ecy.yj202588.top

Swift .......... 15
来源：http://mur.nwbrower.top

Lua ............ 10
来源：http://wnl.vehdjk.com

Perl ........... 10
来源：http://dhp.iojbl.cn

Scala .......... 10
来源：http://egd.shanyushiyangkeji.top

------------------------------------
来源：http://pue.jiagoushi.top

合计 ........... 2106 条
来源：http://wsu.guowangkeji.top

按章节统计：
来源：http://fum.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eoa.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qkw.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gaf.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hjz.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uod.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ihj.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://afl.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oze.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xci.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ckn.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fle.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zwr.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ccc.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zbh.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xwm.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://buw.ybcxt.top

Q SQL 专题                              90
来源：http://dea.chenzaomai.com

R Bash 专题                             80
来源：http://ven.hnxiangtu.top

S C / C++ 专题                          60
来源：http://pep.chenzaomai.com

T 其他语言补充                          60
来源：http://icv.jinqigfzy.top

U 高频实用片段                         120
来源：http://xci.cucudq.cn

------------------------------------
来源：http://rak.shuidangran.top

合计                                  2106 条
来源：http://lfi.zycfv.cn

--------------------------------------------------------------------------------
来源：http://wii.nwbrower.top

使用提醒
来源：http://fix.tarul.cn

--------------------------------------------------------------------------------
来源：http://gle.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzu.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wka.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pzs.daxiang520.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mvb.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uga.bjfxy.top

—— 文件结束 ——
来源：http://rkv.fanxiaobao.xyz

================================================================================
来源：http://ynz.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://dkb.epnwcf.com

Common Programming Examples Cheat Book
来源：http://spq.zhaomingkeji.xyz

================================================================================
来源：http://jxu.xziqi.cn

【收录内容】
来源：http://hpl.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wog.hcnkem.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gmt.tianlin.xyz

SQL · Bash · C · C++
来源：http://cai.fanxiaobao.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://huc.zhixingplan.top

【使用说明】
来源：http://zhl.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cdm.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rhh.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zaz.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://scd.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xrq.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ehy.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ewz.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://unh.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wjs.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ilj.yongpay.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qwo.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bxq.birdmap.top

【文件统计】
来源：http://sip.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ifq.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://ygf.xziqi.cn

目  录
来源：http://ccv.iojbl.cn

--------------------------------------------------------------------------------
来源：http://kms.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://slf.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gpy.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hld.chenlongwang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ktj.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rli.ydzc1.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rwu.jqgufenzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mus.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hid.yj20258.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cwf.shanyushiyangtech.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://htj.ydjk.org.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://znj.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ylk.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nmy.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xwj.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zfx.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hyn.ctjpmb.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cow.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://oso.yj202588.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zmj.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rir.hywenlv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wxf.fktsv.cn

================================================================================
来源：http://nmv.hfpthk.cn

A. 基础语法与类型
来源：http://fal.cashguo.top

================================================================================
来源：http://pln.hywenlv.cn

[A01] Hello World
来源：http://gko.jianghu66.top

Py:   print("Hello, World!")
来源：http://oxh.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://bci.yanxiufei.cn

JS:   console.log("Hello, World!");
来源：http://npt.cashguo.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lrx.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://fqe.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://rxs.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://evd.nwbrower.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bik.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://fcp.mhx1999.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://usj.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mhs.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://uio.zdbjq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wgd.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://svs.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://eak.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://qjj.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://ptp.kuanghao11.cn

[A03] 常量定义
来源：http://akf.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xpc.tanke756.top

PHP:  const PI = 3.14159;
来源：http://nva.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://smu.52xcode.cn

TS:   const PI: number = 3.14159;
来源：http://zrc.9152youxi.cn

Java: static final double PI = 3.14159;
来源：http://ptl.tarul.cn

Go:   const PI = 3.14159
来源：http://uje.zdqjudy.top

Ruby: PI = 3.14159
来源：http://mmx.svipenyu.cn

C#:   const double PI = 3.14159;
来源：http://cvu.yuxming.cn

[A04] 判断变量类型
来源：http://zii.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nei.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dvp.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://klj.aibaodan.cn

TS:   typeof x; x instanceof Date
来源：http://pxq.shangyingyoupin.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gke.hesvh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rox.cqqwz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tae.xuetiantiany.cn

C#:   x.GetType().Name; x is int
来源：http://pvg.shangyingyoupin.top

[A05] 整数除法与取模
来源：http://xxk.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hta.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iad.jlsjyb.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nzf.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yuw.xuanzx.com

Java: 7 / 2; 7 % 2
来源：http://mpv.jqgufenzy.top

Go:   7 / 2; 7 % 2
来源：http://eux.jinqigfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://nfw.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://sgc.gogol.net.cn

[A06] 字符串转数字
来源：http://njz.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://lik.zhixingplan.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fgn.9152youxi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wqs.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://dnf.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qec.ehwqpu.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cob.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://djc.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oaq.gaohongyu789.top

[A07] 数字转字符串
来源：http://qjq.shzxlz.cn

Py:   str(42)
来源：http://bvt.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://lck.fktsv.cn

JS:   String(42); (42).toString()
来源：http://mjo.ywan-chungtsiang.top

TS:   String(42)
来源：http://qld.hysaishi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zgt.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://pcg.shzxlz.cn

Ruby: 42.to_s
来源：http://yez.sweek.top

C#:   42.ToString()
来源：http://djx.cqqwz.cn

[A08] 取整与四舍五入
来源：http://wiu.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bpb.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://exy.dashuyun.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://dlf.9152youxi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://era.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pee.zhongyouzk.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qeq.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fxw.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ypu.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://ylq.jqgfzy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lee.chenzaomai.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://smr.cdnleiting.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pjj.zhijiandao.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lvs.jqgfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ceq.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jwu.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gdd.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dxd.sweek.top

[A10] 生成随机数
来源：http://bwy.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://fnx.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://cmd.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jms.haohaochexian.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lxt.pengpengdd.cyou

Java: new Random().nextInt(100) + 1
来源：http://xzk.ywan-chungtsiang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://msn.sxryk.cn

Ruby: rand(1..100)
来源：http://rua.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://ejm.yj202588.top

[A11] 条件表达式（三元）
来源：http://xje.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://bzu.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mou.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://mxn.aibaodan.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vfx.jiagoushi.top

Java: x > 0 ? "yes" : "no"
来源：http://wli.cashguo.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rat.epnwcf.com

Ruby: x > 0 ? "yes" : "no"
来源：http://feb.zhixingplan.top

C#:   x > 0 ? "yes" : "no"
来源：http://len.xziqi.cn

[A12] 字符串插值 / 格式化
来源：http://gxf.xinyue.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vvt.hnxiangtu.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wlj.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://fnl.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://cee.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://klh.sufxvd.cn


<!-- 参考信息 -->