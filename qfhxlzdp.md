代发 wailian999

[U67] PHP：处理文件上传
来源：http://thu.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gbl.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://tyd.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wsg.havefunace.top

[U69] PHP：PDO 预处理
来源：http://fcd.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://azp.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://dfr.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ddg.epnwcf.com

[U71] PHP：抛出异常
来源：http://tav.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://mwf.hywenlv.cn

[U72] PHP：写错误日志
来源：http://knz.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://nuk.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://phk.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://qpx.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://fhu.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://yuv.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://rcl.daxiang520.top

composer require psr/container
来源：http://mnr.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://yhz.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zyn.ybcxt.top

[U77] PHP：模板渲染
来源：http://veu.aizwys.cn

composer require twig/twig
来源：http://wod.yj202588.top

[U78] PHP：单元测试
来源：http://mtj.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://lab.52xcode.cn

[U79] PHP：静态分析
来源：http://mhl.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://ypk.sweek.top

[U80] PHP：代码规范修复
来源：http://tal.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wyl.zhengqikj.top

[U81] JS：初始化项目
来源：http://gie.zdqjudy.top

npm init -y;  npm i express
来源：http://uvj.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://urt.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://akl.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://dqr.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://hxf.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://zmi.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://ojz.0kj1m.cn

[U85] JS：可选链
来源：http://hwh.birdmap.top

a?.b?.c
来源：http://mwq.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://teg.tianlin.xyz

a ?? b
来源：http://buw.fengsongda.top

[U87] JS：解构默认值
来源：http://gav.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://xbu.yj202588.top

[U88] JS：对象展开合并
来源：http://qme.chenlongwang.top

{ ...a, ...b }
来源：http://vqi.ppjwa.cn

[U89] JS：数组去重
来源：http://jbk.yonumen.top

[...new Set(arr)]
来源：http://pnt.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://pmb.uphjek.com

[...arr].sort((a, b) => a - b)
来源：http://zgo.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://xzi.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lua.epnwcf.com

[U92] JS：深拷贝
来源：http://vne.cucudq.cn

structuredClone(obj)
来源：http://tus.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://uhu.xuetiantiany.cn

`共 ${n} 条`
来源：http://sro.kuanghao11.cn

[U94] JS：箭头函数
来源：http://lpo.9152youxi.cn

const double = x => x * 2;
来源：http://bge.gotoacloud.top

[U95] JS：Promise 包装
来源：http://ifd.uphjek.com

new Promise((resolve, reject) => {})
来源：http://pwc.yueranfly.top

[U96] JS：async/await 与异常
来源：http://gcg.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ouu.hfpthk.cn

[U97] JS：并发请求
来源：http://mdv.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sbe.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://dcp.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mqt.mhx1999.top

[U99] JS：事件监听
来源：http://hij.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://tgo.hfpthk.cn

[U100] JS：DOM 查询
来源：http://jre.xylfe.cn

document.querySelector(".item")
来源：http://pon.nwbrower.top

[U101] JS：classList 操作
来源：http://fmt.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://glr.wangdashe.top

[U102] JS：本地存储
来源：http://nea.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cjv.aibaodan.cn

[U103] JS：定时器
来源：http://wld.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uml.daxiang520.top

[U104] JS：防抖
来源：http://ptd.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ids.ivvv.top

[U105] JS：节流
来源：http://igq.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jug.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://xks.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ime.hnqzz.top

[U107] JS：数字千分位
来源：http://kny.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uxg.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://mzo.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pig.smart0.xyz

[U109] JS：数组分组
来源：http://zuk.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://oke.yuxming.cn

[U110] JS：数组分块
来源：http://qit.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ysy.svipenyu.cn

[U111] JS：对象转 Map
来源：http://ojw.birdmap.top

new Map(Object.entries(obj))
来源：http://bke.cashguo.top

[U112] JS：字符串补位
来源：http://xnh.yj20258888.top

"7".padStart(3, "0")
来源：http://fck.jianghu66.top

[U113] JS：正则替换全部
来源：http://led.tarul.cn

s.replaceAll("a", "b")
来源：http://scg.hesvh.cn

[U114] JS：JSON 深比较
来源：http://vfs.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cva.nwbrower.top

[U115] JS：生成 UUID
来源：http://gkf.zdbjq.cn

crypto.randomUUID()
来源：http://vad.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://hcg.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://bwf.c1oappe.top

[U117] JS：单元测试
来源：http://glk.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://jmp.9152youxi.cn

[U118] JS：开发服务器
来源：http://cpr.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://whk.hysaishi.cn

[U119] JS：生产构建
来源：http://gfb.bbcook.cn

npx vite build
来源：http://puh.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://nfq.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://rhr.zycfv.cn

================================================================================
来源：http://iug.ivvv.top

统计汇总
来源：http://lpy.yangfankeji.com

================================================================================
来源：http://zfb.zdbjq.cn

按语言统计（条）：
来源：http://npa.aibaodan.cn

Python ......... 252
来源：http://kqk.ehwqpu.com

PHP ............ 252
来源：http://vnn.jlsjyb.cn

JavaScript ..... 252
来源：http://xxv.gotoacloud.top

TypeScript ..... 212
来源：http://gja.dashuyun.cn

Java ........... 212
来源：http://lkc.tian-w.cn

Go ............. 212
来源：http://fvb.ctjpmb.com

Ruby ........... 212
来源：http://uip.gotoacloud.top

C# ............. 212
来源：http://uip.hammf.cn

C .............. 30
来源：http://pqp.ppjwa.cn

C++ ............ 30
来源：http://xcl.cashguo.top

SQL ............ 90
来源：http://zfv.wangshuangyany.cn

Bash ........... 80
来源：http://wtx.fzhhl.top

Kotlin ......... 15
来源：http://gtd.zdbjq.cn

Swift .......... 15
来源：http://hhk.jyoumei.cn

Lua ............ 10
来源：http://nbx.zhijiandao.cn

Perl ........... 10
来源：http://fep.yueranfly.top

Scala .......... 10
来源：http://lgf.yangfankeji.com

------------------------------------
来源：http://fkp.daxiang520.top

合计 ........... 2106 条
来源：http://dyd.haohaochexian.top

按章节统计：
来源：http://dav.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://asp.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bos.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bkd.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wsn.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ahm.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yub.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fxn.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://agi.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kqg.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eut.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sxw.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wwr.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dng.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dnp.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pee.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sfe.tarul.cn

Q SQL 专题                              90
来源：http://sbs.jqgfzy.top

R Bash 专题                             80
来源：http://qex.vehdjk.com

S C / C++ 专题                          60
来源：http://zca.xinyue.icu

T 其他语言补充                          60
来源：http://hni.jlsjyb.cn

U 高频实用片段                         120
来源：http://rqu.chenlongwang.top

------------------------------------
来源：http://tvw.0kj1m.cn

合计                                  2106 条
来源：http://ett.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://bxg.aibaodan.cn

使用提醒
来源：http://bgt.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://xom.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ski.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lxh.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://snd.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://jjq.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ydu.cheryme.top

—— 文件结束 ——
来源：http://dnf.zdqjudy.top

================================================================================
来源：http://bxc.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://fku.zdbjq.cn

Common Programming Examples Cheat Book
来源：http://hrw.redwolf501.top

================================================================================
来源：http://cnx.hesvh.cn

【收录内容】
来源：http://cbw.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fgx.chenlongwang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nvh.guannengcc.top

SQL · Bash · C · C++
来源：http://wed.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://omu.jiagoushi.top

【使用说明】
来源：http://owo.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lkb.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cbw.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kli.epnwcf.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dye.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://eki.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pcx.cheryme.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ero.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jed.tianlin.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nqk.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nht.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://byx.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qun.cheryme.top

【文件统计】
来源：http://oas.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rwg.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://chn.xylfe.cn

目  录
来源：http://tdm.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://psa.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vlm.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dcz.smart0.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lvy.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bkn.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tep.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lzo.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vxg.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ykq.hnqzz.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pmw.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ptp.nanxuanxn.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wer.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pkq.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iwj.hongshengwenyu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gti.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://snk.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vfr.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jyo.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://aqp.shuidangran.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://upf.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cmz.wangdashe.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wmk.sysykeji.top

================================================================================
来源：http://nzi.zycfv.cn

A. 基础语法与类型
来源：http://wsb.feifeiyinyue.top

================================================================================
来源：http://adx.gaohongyu789.top

[A01] Hello World
来源：http://fdc.cdnleiting.top

Py:   print("Hello, World!")
来源：http://zcx.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://qjt.vqdsnc.cn

JS:   console.log("Hello, World!");
来源：http://qfb.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pwc.316326.xyz

Java: System.out.println("Hello, World!");
来源：http://esw.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://ubt.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://jym.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wtd.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://grf.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fdh.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zkg.yvedp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://asp.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ndv.mhx1999.top

Java: String name = "Alex"; int age = 20;
来源：http://fwg.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://rkv.zycfv.cn

Ruby: name = "Alex"; age = 20
来源：http://iii.xinyue.icu

C#:   string name = "Alex"; int age = 20;
来源：http://igf.zhijiandao.cn

[A03] 常量定义
来源：http://hmb.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xeb.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://zet.epnwcf.com

JS:   const PI = 3.14159;
来源：http://gfk.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://lqb.hongshengwenyu.top

Java: static final double PI = 3.14159;
来源：http://cnw.jinqigufen.top

Go:   const PI = 3.14159
来源：http://ycr.yuanzhike.top

Ruby: PI = 3.14159
来源：http://bgh.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://ctv.yuanzhike.top

[A04] 判断变量类型
来源：http://ftn.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bwj.nanxuanxn.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hwg.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ajc.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://rgo.chenlongwang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gvs.jqgufenzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://rnw.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bcz.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://nnz.ydzc1.top

[A05] 整数除法与取模
来源：http://vjp.fanxiaobao.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ice.shangyingyoupin.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bwl.cucudq.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dfk.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qub.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://vat.bjfxy.top

Go:   7 / 2; 7 % 2
来源：http://zda.ydzc1.top

Ruby: 7 / 2; 7 % 2
来源：http://euf.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://fjo.redwolf501.top

[A06] 字符串转数字
来源：http://muf.quarkkingdee.top

Py:   int("42"); float("3.14")
来源：http://vvt.dashuyun.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xfe.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nbe.zhijiandao.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jyu.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zui.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gki.yuanzhike.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hxg.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mdl.birdmap.top

[A07] 数字转字符串
来源：http://jwe.yuanzhike.top

Py:   str(42)
来源：http://sus.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://uxn.jinghuilouyu.cn

JS:   String(42); (42).toString()
来源：http://bqz.smart0.xyz

TS:   String(42)
来源：http://ome.yangfankeji.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://clo.yueranfly.top

Go:   strconv.Itoa(42)
来源：http://lvj.kuanghao11.cn

Ruby: 42.to_s
来源：http://egi.sxryk.cn

C#:   42.ToString()
来源：http://xuv.yangfankeji.com

[A08] 取整与四舍五入
来源：http://mlb.ctjpmb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fxz.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kti.zdqjudy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lfk.jianghu66.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gqo.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zhf.ppjwa.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vfu.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xnd.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jed.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://vtj.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yie.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bgc.gogol.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cec.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://phn.hfpthk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ksn.bjfxy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ogx.zhaomingkeji.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qwx.ybcxt.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tpd.wangshuangyany.cn

[A10] 生成随机数
来源：http://jyt.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://igo.chenzaomai.com

PHP:  random_int(1, 100);
来源：http://xxt.316326.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://eqs.cdnleiting.top


<!-- 参考信息 -->