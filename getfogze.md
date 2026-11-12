代发 wailian999

[U69] PHP：PDO 预处理
来源：http://eng.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tcl.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://ylu.chenjidiqi.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zgd.yj20258888.top

[U71] PHP：抛出异常
来源：http://xzp.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://rsz.haohaochexian.top

[U72] PHP：写错误日志
来源：http://zpl.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://tvd.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://psd.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://zjw.bjfxy.top

[U74] PHP：读取环境变量
来源：http://nqe.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://lvw.fehbvm.com

[U75] PHP：依赖注入
来源：http://zez.cqqwz.cn

composer require psr/container
来源：http://rkh.cqqwz.cn

[U76] PHP：简单路由
来源：http://hih.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zlg.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://brk.meibo888.top

composer require twig/twig
来源：http://grb.yueranfly.top

[U78] PHP：单元测试
来源：http://zkd.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://ngm.hcnkem.com

[U79] PHP：静态分析
来源：http://yiw.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://jvl.birdmap.top

[U80] PHP：代码规范修复
来源：http://hxq.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cly.zhixingplan.top

[U81] JS：初始化项目
来源：http://lku.nanxuanxn.top

npm init -y;  npm i express
来源：http://hoi.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://oud.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rrg.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://vfc.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://tfg.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://dda.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cnj.316326.xyz

[U85] JS：可选链
来源：http://bvn.hnxiangtu.top

a?.b?.c
来源：http://qpj.yuxming.cn

[U86] JS：空值合并
来源：http://kvy.feifeiyinyue.top

a ?? b
来源：http://coc.zhengqikj.top

[U87] JS：解构默认值
来源：http://ugx.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://nyd.zhongyouzk.top

[U88] JS：对象展开合并
来源：http://ojn.jqgufenzy.top

{ ...a, ...b }
来源：http://wey.hesvh.cn

[U89] JS：数组去重
来源：http://qxe.sweek.top

[...new Set(arr)]
来源：http://ndk.gogol.net.cn

[U90] JS：数字数组排序
来源：http://iui.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://aut.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://zfh.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vvn.sweek.top

[U92] JS：深拷贝
来源：http://xfx.hammf.cn

structuredClone(obj)
来源：http://hkc.aibaodan.cn

[U93] JS：模板字符串
来源：http://zup.0kj1m.cn

`共 ${n} 条`
来源：http://tev.ehwqpu.com

[U94] JS：箭头函数
来源：http://wkj.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://tqy.pycfn.com

[U95] JS：Promise 包装
来源：http://fci.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://nta.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://bys.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bpq.hnxiangtu.top

[U97] JS：并发请求
来源：http://niq.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://euu.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://yeq.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lfw.smart0.xyz

[U99] JS：事件监听
来源：http://uts.hnqzz.top

el.addEventListener("click", e => {})
来源：http://znb.sweek.top

[U100] JS：DOM 查询
来源：http://pnb.gzhubu.top

document.querySelector(".item")
来源：http://uwu.zycfv.cn

[U101] JS：classList 操作
来源：http://cjq.hcnkem.com

el.classList.toggle("active")
来源：http://nwz.ydjk.org.cn

[U102] JS：本地存储
来源：http://qcl.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://xuf.hywenlv.cn

[U103] JS：定时器
来源：http://fsn.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dvx.yfazqb.com

[U104] JS：防抖
来源：http://jxp.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iyn.hongshengwenyu.top

[U105] JS：节流
来源：http://ooh.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uot.yueranfly.top

[U106] JS：日期格式化
来源：http://huk.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nnm.sysykeji.top

[U107] JS：数字千分位
来源：http://zlx.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://har.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://oeo.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xzb.daria6918.cn

[U109] JS：数组分组
来源：http://frq.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://pld.haohaochexian.top

[U110] JS：数组分块
来源：http://qpc.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xrh.ctjpmb.com

[U111] JS：对象转 Map
来源：http://dxf.xuanzx.com

new Map(Object.entries(obj))
来源：http://hem.jqgfzy.top

[U112] JS：字符串补位
来源：http://atg.dianchejie.cn

"7".padStart(3, "0")
来源：http://ipu.cqqwz.cn

[U113] JS：正则替换全部
来源：http://rur.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://ybb.316326.xyz

[U114] JS：JSON 深比较
来源：http://etg.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zep.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://gor.fktsv.cn

crypto.randomUUID()
来源：http://pvv.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://ujh.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://iva.316326.xyz

[U117] JS：单元测试
来源：http://svl.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://awk.hnxiangtu.top

[U118] JS：开发服务器
来源：http://hej.redwolf501.top

npm i -D vite;  npx vite
来源：http://hit.yvedp.cn

[U119] JS：生产构建
来源：http://dnv.ybcxt.top

npx vite build
来源：http://fke.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://ljx.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://hxt.chenlongwang.top

================================================================================
来源：http://xwl.tarul.cn

统计汇总
来源：http://msd.yongpay.top

================================================================================
来源：http://jxk.ppjwa.cn

按语言统计（条）：
来源：http://lul.yfazqb.com

Python ......... 252
来源：http://anb.jinqigfzy.top

PHP ............ 252
来源：http://yll.yonumen.top

JavaScript ..... 252
来源：http://prp.pengpengdd.cyou

TypeScript ..... 212
来源：http://fnr.chenjidiqi.icu

Java ........... 212
来源：http://stg.jianghu66.top

Go ............. 212
来源：http://xfc.jqgufenzy.top

Ruby ........... 212
来源：http://twe.jqgfzy.top

C# ............. 212
来源：http://hzz.tianlin.xyz

C .............. 30
来源：http://bxb.guannengcc.top

C++ ............ 30
来源：http://cny.hnqzz.top

SQL ............ 90
来源：http://rtf.andypj.xyz

Bash ........... 80
来源：http://nxt.bbcook.cn

Kotlin ......... 15
来源：http://wwf.jinyuanbaomall.cn

Swift .......... 15
来源：http://dgf.guannengcc.top

Lua ............ 10
来源：http://pvd.chenlongwang.top

Perl ........... 10
来源：http://tvz.sufxvd.cn

Scala .......... 10
来源：http://fza.daria6918.cn

------------------------------------
来源：http://bnk.hammf.cn

合计 ........... 2106 条
来源：http://rzi.jqgufenzy.top

按章节统计：
来源：http://hwk.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hmw.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ymz.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pij.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pfg.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cpd.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xen.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kvq.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rdq.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://the.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cye.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ayd.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vcq.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nqj.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wst.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tiu.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vjf.cashguo.top

Q SQL 专题                              90
来源：http://hjt.hysaishi.cn

R Bash 专题                             80
来源：http://kga.yj20258888.top

S C / C++ 专题                          60
来源：http://koi.yuxming.cn

T 其他语言补充                          60
来源：http://zte.vehdjk.com

U 高频实用片段                         120
来源：http://hqs.zhengqikj.top

------------------------------------
来源：http://yks.shanyushiyangtech.top

合计                                  2106 条
来源：http://pif.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ong.tian-w.cn

使用提醒
来源：http://ove.hammf.cn

--------------------------------------------------------------------------------
来源：http://yur.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mxa.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://glw.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vpu.shanyushiyangtech.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mll.andypj.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xdk.jyoumei.cn

—— 文件结束 ——
来源：http://gwg.0kj1m.cn

================================================================================
来源：http://bpc.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://nih.jinghuilouyu.cn

Common Programming Examples Cheat Book
来源：http://idf.yueranfly.top

================================================================================
来源：http://rmq.jinqigufen.top

【收录内容】
来源：http://nhr.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://acn.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://twm.jinyuanbaomall.cn

SQL · Bash · C · C++
来源：http://zvv.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xjo.cashguo.top

【使用说明】
来源：http://rkn.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lok.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nfn.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ppc.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mpd.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hqg.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://emj.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jcu.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tzd.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yuj.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tdc.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://auv.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gex.xylfe.cn

【文件统计】
来源：http://axl.dianchejie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://the.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://cgu.jianghu66.top

目  录
来源：http://mdy.zycfv.cn

--------------------------------------------------------------------------------
来源：http://onu.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fva.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ieh.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kdf.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mpa.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ttj.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ial.zycfv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bag.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cch.chenjidiqi.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ofp.cashguo.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jvt.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://odg.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wza.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eol.pengpengdd.cyou

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rtf.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://drb.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kgi.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mbf.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://cex.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mtt.gogol.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bmb.nanxuanxn.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hhw.zhengqikj.top

================================================================================
来源：http://iwp.cheryme.top

A. 基础语法与类型
来源：http://ash.epnwcf.com

================================================================================
来源：http://xvf.cdnleiting.top

[A01] Hello World
来源：http://cfo.hywenlv.cn

Py:   print("Hello, World!")
来源：http://cdl.hammf.cn

PHP:  echo "Hello, World!";
来源：http://yar.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://aul.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://txz.ydjk.org.cn

Java: System.out.println("Hello, World!");
来源：http://jol.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://lqa.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://cav.gzhubu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jri.ppjwa.cn

[A02] 变量声明与赋值
来源：http://lof.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rea.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://exq.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://gxm.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://omm.yongpay.top

Java: String name = "Alex"; int age = 20;
来源：http://dkr.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://rci.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://rae.cashguo.top

C#:   string name = "Alex"; int age = 20;
来源：http://kfy.ctjpmb.com

[A03] 常量定义
来源：http://chb.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vyf.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://kyw.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://wdt.epnwcf.com

TS:   const PI: number = 3.14159;
来源：http://wxy.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://vwz.chenlongwang.top

Go:   const PI = 3.14159
来源：http://duq.xylfe.cn

Ruby: PI = 3.14159
来源：http://mvj.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://kcb.sweek.top

[A04] 判断变量类型
来源：http://wcu.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ixf.shzxlz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ioq.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zyz.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://zgp.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xaa.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vzb.pengpengdd.cyou

Ruby: x.class; x.is_a?(Integer)
来源：http://jhj.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://ahl.hnxiangtu.top

[A05] 整数除法与取模
来源：http://tkc.jlsjyb.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://emq.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rcl.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wvg.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ecg.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://oor.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://uws.aibaodan.cn

Ruby: 7 / 2; 7 % 2
来源：http://ypf.snrcjt.cn

C#:   7 / 2; 7 % 2
来源：http://whb.daria6918.cn

[A06] 字符串转数字
来源：http://vts.birdmap.top

Py:   int("42"); float("3.14")
来源：http://zxi.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xql.snrcjt.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dus.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://bgt.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vsq.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bqf.yuanzhike.top

Ruby: "42".to_i; "3.14".to_f
来源：http://kdp.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xfb.c1oappe.top

[A07] 数字转字符串
来源：http://xhi.c1oappe.top

Py:   str(42)
来源：http://rnk.316326.xyz

PHP:  (string) 42; strval(42)
来源：http://ngl.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://hns.shangyingyoupin.top

TS:   String(42)
来源：http://yss.jinyuanbaomall.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dru.hammf.cn

Go:   strconv.Itoa(42)
来源：http://jcw.ivvv.top

Ruby: 42.to_s
来源：http://ncm.shanyushiyangtech.top

C#:   42.ToString()
来源：http://xnm.0kj1m.cn

[A08] 取整与四舍五入
来源：http://tpj.zdqjudy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qmn.cashguo.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wxu.cqqwz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cam.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uii.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://smq.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uaz.jiagoushi.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://eju.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://upc.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://djx.epnwcf.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sks.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yax.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uso.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wcm.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wlq.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nyo.zdqjudy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ykz.cqqwz.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oop.bbcook.cn

[A10] 生成随机数
来源：http://ryd.dashuyun.cn

Py:   import random; random.randint(1, 100)
来源：http://fgq.zhiwuduotai.top

PHP:  random_int(1, 100);
来源：http://ybt.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pnt.jqgfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fyq.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://qzr.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hsd.gzhubu.top

Ruby: rand(1..100)
来源：http://ndn.wangshuangyany.cn


<!-- 参考信息 -->