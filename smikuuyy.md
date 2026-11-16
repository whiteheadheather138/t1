代发 wailian999

[U69] PHP：PDO 预处理
来源：http://slg.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mvc.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://zqx.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pxx.jyoumei.cn

[U71] PHP：抛出异常
来源：http://thg.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://qsa.zhengqikj.top

[U72] PHP：写错误日志
来源：http://lqt.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://sun.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://uwx.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://plj.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://fsz.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://rwg.yonumen.top

[U75] PHP：依赖注入
来源：http://rto.ivvv.top

composer require psr/container
来源：http://gzd.yongpay.top

[U76] PHP：简单路由
来源：http://iwi.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://niw.hywenlv.cn

[U77] PHP：模板渲染
来源：http://muw.yueranfly.top

composer require twig/twig
来源：http://bba.tarul.cn

[U78] PHP：单元测试
来源：http://ayy.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://xyf.guannengcc.top

[U79] PHP：静态分析
来源：http://lvk.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://hkm.bbcook.cn

[U80] PHP：代码规范修复
来源：http://xlj.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wyq.hesvh.cn

[U81] JS：初始化项目
来源：http://hwj.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://tai.fzhhl.top

[U82] JS：package.json 脚本
来源：http://cpp.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://trt.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://fmj.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://alk.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://aho.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://lpo.yj202588.top

[U85] JS：可选链
来源：http://hyd.zhijiandao.cn

a?.b?.c
来源：http://jrk.svipenyu.cn

[U86] JS：空值合并
来源：http://krb.daria6918.cn

a ?? b
来源：http://pxf.yanxiufei.cn

[U87] JS：解构默认值
来源：http://mis.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://jqx.cashguo.top

[U88] JS：对象展开合并
来源：http://fii.zhongyouzk.top

{ ...a, ...b }
来源：http://wfu.hesvh.cn

[U89] JS：数组去重
来源：http://mis.zhongyouzk.top

[...new Set(arr)]
来源：http://jcu.svipenyu.cn

[U90] JS：数字数组排序
来源：http://xfy.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://bgk.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://ljd.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vvs.hysaishi.cn

[U92] JS：深拷贝
来源：http://auh.jinghuilouyu.cn

structuredClone(obj)
来源：http://nvq.jqgfzy.top

[U93] JS：模板字符串
来源：http://rvc.ydjk.org.cn

`共 ${n} 条`
来源：http://jmr.birdmap.top

[U94] JS：箭头函数
来源：http://wzf.zdqjudy.top

const double = x => x * 2;
来源：http://esy.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://gnc.jinghuilouyu.cn

new Promise((resolve, reject) => {})
来源：http://jlg.tian-w.cn

[U96] JS：async/await 与异常
来源：http://dge.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uzs.zycfv.cn

[U97] JS：并发请求
来源：http://nfa.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eig.hnxiangtu.top

[U98] JS：fetch 带 JSON
来源：http://qja.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://toa.fktsv.cn

[U99] JS：事件监听
来源：http://bay.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://jnb.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://via.gotoacloud.top

document.querySelector(".item")
来源：http://muv.yuxming.cn

[U101] JS：classList 操作
来源：http://wdk.chenzaomai.com

el.classList.toggle("active")
来源：http://kaj.zhoulong.xyz

[U102] JS：本地存储
来源：http://pdg.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qmm.cashguo.top

[U103] JS：定时器
来源：http://xwm.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yyc.aizwys.cn

[U104] JS：防抖
来源：http://jgt.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuu.cdnleiting.top

[U105] JS：节流
来源：http://qdb.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trn.nanxinkj.top

[U106] JS：日期格式化
来源：http://wha.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://muo.epnwcf.com

[U107] JS：数字千分位
来源：http://ycu.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qeq.wangshuangyany.cn

[U108] JS：随机整数
来源：http://sdk.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vni.ivvv.top

[U109] JS：数组分组
来源：http://iqb.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://scm.aibaodan.cn

[U110] JS：数组分块
来源：http://dpf.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qze.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://zqr.aibaodan.cn

new Map(Object.entries(obj))
来源：http://clk.svipenyu.cn

[U112] JS：字符串补位
来源：http://tpm.epnwcf.com

"7".padStart(3, "0")
来源：http://ymx.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://yxj.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://bah.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://cjm.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pva.nanxinkj.top

[U115] JS：生成 UUID
来源：http://gdg.yuanzhike.top

crypto.randomUUID()
来源：http://wsa.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://bly.tanke756.top

/** @param {string} name */ function f(name) {}
来源：http://upe.tarul.cn

[U117] JS：单元测试
来源：http://qbj.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://uyl.fengsongda.top

[U118] JS：开发服务器
来源：http://zkp.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://gwe.zhiwuduotai.top

[U119] JS：生产构建
来源：http://luf.vqdsnc.cn

npx vite build
来源：http://gou.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://ove.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://oru.yonumen.top

================================================================================
来源：http://uef.nanxinkj.top

统计汇总
来源：http://clj.gaohongyu789.top

================================================================================
来源：http://aax.fzhhl.top

按语言统计（条）：
来源：http://yyw.shuidangran.top

Python ......... 252
来源：http://otx.hammf.cn

PHP ............ 252
来源：http://ctw.dianchejie.cn

JavaScript ..... 252
来源：http://jza.cdnleiting.top

TypeScript ..... 212
来源：http://ekq.yj20258888.top

Java ........... 212
来源：http://kga.chenzaomai.com

Go ............. 212
来源：http://agw.xylfe.cn

Ruby ........... 212
来源：http://hfg.yfazqb.com

C# ............. 212
来源：http://fpr.guannengcc.top

C .............. 30
来源：http://cgo.xuanzx.com

C++ ............ 30
来源：http://psa.daxiang520.top

SQL ............ 90
来源：http://ljg.jinyuanbaomall.cn

Bash ........... 80
来源：http://ifo.jiagoushi.top

Kotlin ......... 15
来源：http://log.cashguo.top

Swift .......... 15
来源：http://jjb.quarkkingdee.top

Lua ............ 10
来源：http://zwu.jqgfzy.top

Perl ........... 10
来源：http://xkb.ivvv.top

Scala .......... 10
来源：http://ivb.zhongyouzk.top

------------------------------------
来源：http://yjb.feifeiyinyue.top

合计 ........... 2106 条
来源：http://mnj.sjlbkw.cn

按章节统计：
来源：http://mgp.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dhm.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rwi.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ylq.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fzf.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wda.yvedp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://owu.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://auq.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iml.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zcv.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hyq.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jge.smart0.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ydr.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yfh.vehdjk.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tvv.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://auj.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xlm.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://uhb.jiagoushi.top

R Bash 专题                             80
来源：http://mpe.tianlin.xyz

S C / C++ 专题                          60
来源：http://cvq.shanyushiyangkeji.top

T 其他语言补充                          60
来源：http://nxj.yanxiufei.cn

U 高频实用片段                         120
来源：http://zyx.jqgfzy.top

------------------------------------
来源：http://ysd.zhijiandao.cn

合计                                  2106 条
来源：http://qno.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://iot.c1oappe.top

使用提醒
来源：http://qrc.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://uxw.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wra.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ejj.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://znz.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ysr.zhongyouzk.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ief.zycfv.cn

—— 文件结束 ——
来源：http://rid.gogol.net.cn

================================================================================
来源：http://mil.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://vwk.sxryk.cn

Common Programming Examples Cheat Book
来源：http://lrm.chenjidiqi.icu

================================================================================
来源：http://uzh.xziqi.cn

【收录内容】
来源：http://hps.daria6918.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gcj.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fei.zycfv.cn

SQL · Bash · C · C++
来源：http://qfy.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://naf.sufxvd.cn

【使用说明】
来源：http://sjb.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ggg.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ndn.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qct.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vlv.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://awt.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wyw.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vne.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://apq.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ibi.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oqk.gotoacloud.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://avl.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://liy.gzhubu.top

【文件统计】
来源：http://psb.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hpm.hammf.cn

--------------------------------------------------------------------------------
来源：http://kwh.yongpay.top

目  录
来源：http://dgs.xziqi.cn

--------------------------------------------------------------------------------
来源：http://umu.fehbvm.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vie.ywan-chungtsiang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zcq.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dha.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cus.jlsjyb.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jjf.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vkv.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://edu.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pli.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ltu.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mrh.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ksw.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hbc.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://whz.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fyu.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://snb.hysaishi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cpr.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mfj.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hna.zhongyouzk.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xqu.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vbp.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gci.xylfe.cn

================================================================================
来源：http://wgi.gaohongyu789.top

A. 基础语法与类型
来源：http://inq.yuanzhike.top

================================================================================
来源：http://lix.xinyue.icu

[A01] Hello World
来源：http://fda.birdmap.top

Py:   print("Hello, World!")
来源：http://mqe.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://zvu.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://rfd.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eew.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://tma.iojbl.cn

Go:   fmt.Println("Hello, World!")
来源：http://end.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://fcg.zdqjudy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ges.smart0.xyz

[A02] 变量声明与赋值
来源：http://idq.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eri.yanxiufei.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ppw.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://txa.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vef.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://pra.cdnleiting.top

Go:   name := "Alex"; age := 20
来源：http://avp.c1oappe.top

Ruby: name = "Alex"; age = 20
来源：http://mjj.hcnkem.com

C#:   string name = "Alex"; int age = 20;
来源：http://iep.gotoacloud.top

[A03] 常量定义
来源：http://qrk.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aho.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://ayr.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://exu.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://bzq.jqgufenzy.top

Java: static final double PI = 3.14159;
来源：http://npp.tian-w.cn

Go:   const PI = 3.14159
来源：http://huv.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://dyy.chenzaomai.com

C#:   const double PI = 3.14159;
来源：http://yfw.yongpay.top

[A04] 判断变量类型
来源：http://vwr.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://lrf.yj202588.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ohv.xuetiantiany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://twi.wangdashe.top

TS:   typeof x; x instanceof Date
来源：http://dea.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blb.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://npl.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jpc.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://bmq.chenzaomai.com

[A05] 整数除法与取模
来源：http://jxr.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ocl.chenjidiqi.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://rrh.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wks.fehbvm.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vat.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://goj.zhengqikj.top

Go:   7 / 2; 7 % 2
来源：http://jfh.xuanzx.com

Ruby: 7 / 2; 7 % 2
来源：http://ejp.jinghuilouyu.cn

C#:   7 / 2; 7 % 2
来源：http://lgg.daria6918.cn

[A06] 字符串转数字
来源：http://too.snrcjt.cn

Py:   int("42"); float("3.14")
来源：http://rna.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://air.zdbjq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qpo.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://bdy.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kuf.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bzt.ywan-chungtsiang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ukj.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vmf.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://aen.zhixingplan.top

Py:   str(42)
来源：http://qqn.hysaishi.cn

PHP:  (string) 42; strval(42)
来源：http://sgb.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://qmg.zycfv.cn

TS:   String(42)
来源：http://dqw.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://tcj.yj202588.top

Go:   strconv.Itoa(42)
来源：http://wqe.jinqigfzy.top

Ruby: 42.to_s
来源：http://sjl.jinqigfzy.top

C#:   42.ToString()
来源：http://cvy.dashuyun.cn

[A08] 取整与四舍五入
来源：http://zyk.jinqigfzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uys.wangshuangyany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lmy.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://opg.tian-w.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cwn.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ljw.jiagoushi.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gkq.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://fat.yj20258.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dcu.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://atp.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ogz.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ism.nanxuanxn.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nym.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xbp.cqqwz.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rfo.jqgfzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sxj.chenlongwang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://poy.aizwys.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jky.cashguo.top

[A10] 生成随机数
来源：http://jdb.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://kqn.zhoulong.xyz

PHP:  random_int(1, 100);
来源：http://zxc.dianchejie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kvf.tarul.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lbg.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://xqe.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://twp.hnqzz.top

Ruby: rand(1..100)
来源：http://sgh.meibo888.top


<!-- 参考信息 -->