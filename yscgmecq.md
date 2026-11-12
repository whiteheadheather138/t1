代发 wailian999

[U71] PHP：抛出异常
来源：http://ktq.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://din.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://due.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://qyd.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://oah.tanke756.top

parse_ini_file("config.ini", true)
来源：http://bmz.yfazqb.com

[U74] PHP：读取环境变量
来源：http://ahe.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://muq.yvedp.cn

[U75] PHP：依赖注入
来源：http://ntw.gaohongyu789.top

composer require psr/container
来源：http://knn.hcnkem.com

[U76] PHP：简单路由
来源：http://mfb.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xdj.birdmap.top

[U77] PHP：模板渲染
来源：http://ydu.tarul.cn

composer require twig/twig
来源：http://bmn.zhixingplan.top

[U78] PHP：单元测试
来源：http://fkj.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://wpm.yanxiufei.cn

[U79] PHP：静态分析
来源：http://jkd.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://nho.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://cgy.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jcc.nanxuanxn.top

[U81] JS：初始化项目
来源：http://drg.redwolf501.top

npm init -y;  npm i express
来源：http://lst.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://sun.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ewy.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://ppr.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://kmj.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://ziy.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://lqf.gotoacloud.top

[U85] JS：可选链
来源：http://wyj.zhiwuduotai.top

a?.b?.c
来源：http://htm.tarul.cn

[U86] JS：空值合并
来源：http://sgf.ctjpmb.com

a ?? b
来源：http://bxs.nanxuanxn.top

[U87] JS：解构默认值
来源：http://uxz.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://pfq.fehbvm.com

[U88] JS：对象展开合并
来源：http://iya.uphjek.com

{ ...a, ...b }
来源：http://wpk.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://xqe.jlsjyb.cn

[...new Set(arr)]
来源：http://fhz.hesvh.cn

[U90] JS：数字数组排序
来源：http://mah.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://oub.xylfe.cn

[U91] JS：对象键值遍历
来源：http://ioy.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qxe.hywenlv.cn

[U92] JS：深拷贝
来源：http://pin.xylfe.cn

structuredClone(obj)
来源：http://geb.jyoumei.cn

[U93] JS：模板字符串
来源：http://xwj.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://emb.hesvh.cn

[U94] JS：箭头函数
来源：http://ait.ybcxt.top

const double = x => x * 2;
来源：http://gkc.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://lja.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://btf.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://tvy.zhaomingkeji.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fux.xuetiantiany.cn

[U97] JS：并发请求
来源：http://rrs.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lkg.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://hze.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vkj.daxiang520.top

[U99] JS：事件监听
来源：http://njx.yueranfly.top

el.addEventListener("click", e => {})
来源：http://ikh.daria6918.cn

[U100] JS：DOM 查询
来源：http://ucq.havefunace.top

document.querySelector(".item")
来源：http://rdu.bjfxy.top

[U101] JS：classList 操作
来源：http://juu.cheryme.top

el.classList.toggle("active")
来源：http://qww.nanxuanxn.top

[U102] JS：本地存储
来源：http://ugl.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oav.bbcook.cn

[U103] JS：定时器
来源：http://ipg.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dva.shanyushiyangtech.top

[U104] JS：防抖
来源：http://rhq.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hli.jiagoushi.top

[U105] JS：节流
来源：http://mhb.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wiz.sjlbkw.cn

[U106] JS：日期格式化
来源：http://dop.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ede.mhx1999.top

[U107] JS：数字千分位
来源：http://pzz.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pci.hnqzz.top

[U108] JS：随机整数
来源：http://zhj.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ddt.tian-w.cn

[U109] JS：数组分组
来源：http://nxw.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://jmd.zhixingplan.top

[U110] JS：数组分块
来源：http://oia.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jzp.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://ysa.yfazqb.com

new Map(Object.entries(obj))
来源：http://xcp.uphjek.com

[U112] JS：字符串补位
来源：http://zvp.xylfe.cn

"7".padStart(3, "0")
来源：http://npm.0kj1m.cn

[U113] JS：正则替换全部
来源：http://kon.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://ijx.ybcxt.top

[U114] JS：JSON 深比较
来源：http://ynr.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yjh.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://ube.havefunace.top

crypto.randomUUID()
来源：http://pat.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://bht.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://sre.xinyue.icu

[U117] JS：单元测试
来源：http://hqg.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://vws.birdmap.top

[U118] JS：开发服务器
来源：http://sfj.yangfankeji.com

npm i -D vite;  npx vite
来源：http://yfd.yanxiufei.cn

[U119] JS：生产构建
来源：http://gpi.daxiang520.top

npx vite build
来源：http://ddf.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://vos.yj202588.top

import.meta.env.VITE_API_URL
来源：http://btm.wangshuangyany.cn

================================================================================
来源：http://csj.gaohongyu789.top

统计汇总
来源：http://yuj.zhaomingkeji.xyz

================================================================================
来源：http://uyy.bjfxy.top

按语言统计（条）：
来源：http://qoi.zhengqikj.top

Python ......... 252
来源：http://mws.wangshuangyany.cn

PHP ............ 252
来源：http://kmg.aibaodan.cn

JavaScript ..... 252
来源：http://zra.ctjpmb.com

TypeScript ..... 212
来源：http://xol.xuanzx.com

Java ........... 212
来源：http://mgl.yuanzhike.top

Go ............. 212
来源：http://fpn.9152youxi.cn

Ruby ........... 212
来源：http://frq.cheryme.top

C# ............. 212
来源：http://kbp.fehbvm.com

C .............. 30
来源：http://too.yj202588.top

C++ ............ 30
来源：http://wxc.svipenyu.cn

SQL ............ 90
来源：http://qvj.hongshengwenyu.top

Bash ........... 80
来源：http://fzv.chenjidiqi.icu

Kotlin ......... 15
来源：http://jxw.fanxiaobao.xyz

Swift .......... 15
来源：http://loz.ybcxt.top

Lua ............ 10
来源：http://dsq.xuetiantiany.cn

Perl ........... 10
来源：http://vyk.yuanzhike.top

Scala .......... 10
来源：http://iur.sjlbkw.cn

------------------------------------
来源：http://suf.cashguo.top

合计 ........... 2106 条
来源：http://jts.redwolf501.top

按章节统计：
来源：http://vvr.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mtk.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aig.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xag.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zmk.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dus.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rky.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jox.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rpt.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xaq.ivvv.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rwz.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sru.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gsu.ybcxt.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fgf.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sya.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iai.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wtv.hongshengwenyu.top

Q SQL 专题                              90
来源：http://giq.epnwcf.com

R Bash 专题                             80
来源：http://zdi.tarul.cn

S C / C++ 专题                          60
来源：http://unb.c1oappe.top

T 其他语言补充                          60
来源：http://kzr.vqdsnc.cn

U 高频实用片段                         120
来源：http://brl.jinghuilouyu.cn

------------------------------------
来源：http://ryp.hfpthk.cn

合计                                  2106 条
来源：http://diu.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://bwm.havefunace.top

使用提醒
来源：http://lws.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://bqj.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ewv.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fll.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://elz.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qnr.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nps.yvedp.cn

—— 文件结束 ——
来源：http://dzr.fktsv.cn

================================================================================
来源：http://mjt.meibo888.top

程序语言常见例子速查手册（2024 版）
来源：http://dpd.fengsongda.top

Common Programming Examples Cheat Book
来源：http://cfw.andypj.xyz

================================================================================
来源：http://tlw.birdmap.top

【收录内容】
来源：http://znm.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://jbu.yueranfly.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zyz.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://agv.xuetiantiany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kps.sjlbkw.cn

【使用说明】
来源：http://nxd.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pqy.hammf.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hjh.tanke756.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kvb.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nuz.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://fme.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mlg.zhixingplan.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fyc.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nux.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lax.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fsb.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ycp.nanxinkj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gop.hysaishi.cn

【文件统计】
来源：http://maf.xuetiantiany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fxh.ybcxt.top

--------------------------------------------------------------------------------
来源：http://xda.ivvv.top

目  录
来源：http://haj.hnqzz.top

--------------------------------------------------------------------------------
来源：http://wyc.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nmw.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xqv.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vng.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uqj.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ebg.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ljl.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://och.snrcjt.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://czm.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xhw.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vqc.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ssu.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sob.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sbi.hammf.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://loq.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cbl.ctjpmb.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ogt.tanke756.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ael.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sob.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oam.fzhhl.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvj.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rno.sweek.top

================================================================================
来源：http://xud.fehbvm.com

A. 基础语法与类型
来源：http://wju.ywan-chungtsiang.top

================================================================================
来源：http://wds.cdnleiting.top

[A01] Hello World
来源：http://gdb.uphjek.com

Py:   print("Hello, World!")
来源：http://srk.sysykeji.top

PHP:  echo "Hello, World!";
来源：http://nuf.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://rvn.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cnt.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://hbl.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://hpr.gogol.net.cn

Ruby: puts "Hello, World!"
来源：http://lwm.jinyuanbaomall.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rdo.gzhubu.top

[A02] 变量声明与赋值
来源：http://bpx.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://djk.chenzaomai.com

PHP:  $name = "Alex"; $age = 20;
来源：http://bso.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hik.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qzs.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://ope.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://boq.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://jqm.yangfankeji.com

C#:   string name = "Alex"; int age = 20;
来源：http://acw.aibaodan.cn

[A03] 常量定义
来源：http://vbr.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ibw.hnxiangtu.top

PHP:  const PI = 3.14159;
来源：http://fwc.jqgfzy.top

JS:   const PI = 3.14159;
来源：http://loq.wangdashe.top

TS:   const PI: number = 3.14159;
来源：http://mym.pycfn.com

Java: static final double PI = 3.14159;
来源：http://zai.gzhubu.top

Go:   const PI = 3.14159
来源：http://ocr.zhengqikj.top

Ruby: PI = 3.14159
来源：http://dhk.316326.xyz

C#:   const double PI = 3.14159;
来源：http://yco.jinghuilouyu.cn

[A04] 判断变量类型
来源：http://civ.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://aiy.iojbl.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tfn.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kqu.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://ibz.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rni.yuanzhike.top

Go:   reflect.TypeOf(x).Name()
来源：http://nkc.yonumen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zhn.quarkkingdee.top

C#:   x.GetType().Name; x is int
来源：http://kry.epnwcf.com

[A05] 整数除法与取模
来源：http://mux.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mqj.jinyuanbaomall.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://bmr.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://deq.yuxming.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ulh.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://qjr.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://fbo.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://akd.hcnkem.com

C#:   7 / 2; 7 % 2
来源：http://bpc.hfpthk.cn

[A06] 字符串转数字
来源：http://qle.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://ory.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://umz.pengpengdd.cyou

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zcu.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://ekb.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iua.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gsz.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lrx.zhaomingkeji.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ytc.bbcook.cn

[A07] 数字转字符串
来源：http://tud.jlsjyb.cn

Py:   str(42)
来源：http://wtr.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://epj.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://jsw.gogol.net.cn

TS:   String(42)
来源：http://css.ivvv.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ijm.zhaomingkeji.xyz

Go:   strconv.Itoa(42)
来源：http://hvp.tanke756.top

Ruby: 42.to_s
来源：http://vew.zdbjq.cn

C#:   42.ToString()
来源：http://tnc.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://fxh.chenzaomai.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bey.uphjek.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hdt.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mng.zhongyouzk.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mhk.feifeiyinyue.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ijd.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wxt.gogol.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eez.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bfe.shuidangran.top

[A09] 绝对值与最大最小值
来源：http://eru.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ezs.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mlt.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fpl.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lzo.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yxh.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xbh.hesvh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tdi.yongpay.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gyv.ctjpmb.com

[A10] 生成随机数
来源：http://hhp.hysaishi.cn

Py:   import random; random.randint(1, 100)
来源：http://stb.chenzaomai.com

PHP:  random_int(1, 100);
来源：http://npy.tian-w.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cbv.vqdsnc.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://huw.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://brp.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gzv.nanxinkj.top

Ruby: rand(1..100)
来源：http://xos.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://qzl.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://iab.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://abq.vehdjk.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://cef.hcnkem.com


<!-- 参考信息 -->