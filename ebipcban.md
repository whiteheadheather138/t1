代发 wailian999

[U69] PHP：PDO 预处理
来源：http://suj.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zed.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://gua.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://idg.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://xwk.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://yoq.0kj1m.cn

[U72] PHP：写错误日志
来源：http://heh.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://fkp.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://cma.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://qft.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://bjm.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://vdg.yvedp.cn

[U75] PHP：依赖注入
来源：http://upq.ydjk.org.cn

composer require psr/container
来源：http://cau.hnqzz.top

[U76] PHP：简单路由
来源：http://ect.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yvr.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://oja.xingfuxueyuan.xyz

composer require twig/twig
来源：http://rpm.hnxiangtu.top

[U78] PHP：单元测试
来源：http://lhv.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://agu.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://ize.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://nwf.zycfv.cn

[U80] PHP：代码规范修复
来源：http://nqp.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uwz.yuanzhike.top

[U81] JS：初始化项目
来源：http://gxh.cucudq.cn

npm init -y;  npm i express
来源：http://wvi.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://wzh.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xxr.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://mjn.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hfi.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://gyl.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://oup.yueranfly.top

[U85] JS：可选链
来源：http://nol.xylfe.cn

a?.b?.c
来源：http://mkg.zycfv.cn

[U86] JS：空值合并
来源：http://hyw.cdnleiting.top

a ?? b
来源：http://hkq.ydjk.org.cn

[U87] JS：解构默认值
来源：http://nad.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://ocl.9152youxi.cn

[U88] JS：对象展开合并
来源：http://osy.shuidangran.top

{ ...a, ...b }
来源：http://ume.hfpthk.cn

[U89] JS：数组去重
来源：http://gde.svipenyu.cn

[...new Set(arr)]
来源：http://sgo.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://uez.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://kiq.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://syo.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rqj.jqgufenzy.top

[U92] JS：深拷贝
来源：http://acg.dashuyun.cn

structuredClone(obj)
来源：http://klf.bbcook.cn

[U93] JS：模板字符串
来源：http://ojh.chenzaomai.com

`共 ${n} 条`
来源：http://qva.yuxming.cn

[U94] JS：箭头函数
来源：http://hfe.havefunace.top

const double = x => x * 2;
来源：http://kni.mhx1999.top

[U95] JS：Promise 包装
来源：http://ktq.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://myd.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://rfx.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qin.zdbjq.cn

[U97] JS：并发请求
来源：http://ijx.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://inw.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://svv.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bnk.daria6918.cn

[U99] JS：事件监听
来源：http://iid.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://tio.yfazqb.com

[U100] JS：DOM 查询
来源：http://gmc.dashuyun.cn

document.querySelector(".item")
来源：http://tmy.uphjek.com

[U101] JS：classList 操作
来源：http://acr.shangyingyoupin.top

el.classList.toggle("active")
来源：http://iob.yj20258888.top

[U102] JS：本地存储
来源：http://hcv.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tep.ydzc1.top

[U103] JS：定时器
来源：http://hjb.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://axg.cqqwz.cn

[U104] JS：防抖
来源：http://irc.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywp.sjlbkw.cn

[U105] JS：节流
来源：http://mqt.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://twn.andypj.xyz

[U106] JS：日期格式化
来源：http://vsp.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ujm.daria6918.cn

[U107] JS：数字千分位
来源：http://kpf.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sqe.ivvv.top

[U108] JS：随机整数
来源：http://fqd.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://euk.nanxuanxn.top

[U109] JS：数组分组
来源：http://xgc.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://fgt.chenjidiqi.icu

[U110] JS：数组分块
来源：http://dra.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dck.0kj1m.cn

[U111] JS：对象转 Map
来源：http://qzc.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://usi.zhoulong.xyz

[U112] JS：字符串补位
来源：http://nsz.guannengcc.top

"7".padStart(3, "0")
来源：http://cod.haohaochexian.top

[U113] JS：正则替换全部
来源：http://aql.xinyue.icu

s.replaceAll("a", "b")
来源：http://wja.wangdashe.top

[U114] JS：JSON 深比较
来源：http://lku.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xks.sweek.top

[U115] JS：生成 UUID
来源：http://ibc.zycfv.cn

crypto.randomUUID()
来源：http://blm.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://lxn.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://osb.zhoulong.xyz

[U117] JS：单元测试
来源：http://gmi.tanke756.top

npm i -D vitest;  npx vitest
来源：http://cwu.aibaodan.cn

[U118] JS：开发服务器
来源：http://boe.wangdashe.top

npm i -D vite;  npx vite
来源：http://fyj.tarul.cn

[U119] JS：生产构建
来源：http://epw.xziqi.cn

npx vite build
来源：http://vmf.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://tse.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://zso.fktsv.cn

================================================================================
来源：http://nwk.gogol.net.cn

统计汇总
来源：http://qzf.hfpthk.cn

================================================================================
来源：http://qqr.jiagoushi.top

按语言统计（条）：
来源：http://kee.sysykeji.top

Python ......... 252
来源：http://tkc.aibaodan.cn

PHP ............ 252
来源：http://ifj.feifeiyinyue.top

JavaScript ..... 252
来源：http://qek.vqdsnc.cn

TypeScript ..... 212
来源：http://pgw.xuanzx.com

Java ........... 212
来源：http://jbw.yangfankeji.com

Go ............. 212
来源：http://vsk.bbcook.cn

Ruby ........... 212
来源：http://rin.sysykeji.top

C# ............. 212
来源：http://qml.hesvh.cn

C .............. 30
来源：http://txx.redwolf501.top

C++ ............ 30
来源：http://amk.cashguo.top

SQL ............ 90
来源：http://ffe.wangdashe.top

Bash ........... 80
来源：http://kea.guowangkeji.top

Kotlin ......... 15
来源：http://ozt.cheryme.top

Swift .......... 15
来源：http://ncm.vqdsnc.cn

Lua ............ 10
来源：http://hwu.zhengqikj.top

Perl ........... 10
来源：http://zuo.tian-w.cn

Scala .......... 10
来源：http://diz.yvedp.cn

------------------------------------
来源：http://ylv.c1oappe.top

合计 ........... 2106 条
来源：http://efi.gotoacloud.top

按章节统计：
来源：http://mea.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tmp.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vmk.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yum.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ssr.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://exe.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wxd.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qdk.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dde.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wzv.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bca.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qva.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://akq.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wgh.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://shx.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ndc.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://itv.wangdashe.top

Q SQL 专题                              90
来源：http://drl.ivvv.top

R Bash 专题                             80
来源：http://vrh.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://fcj.zdbjq.cn

T 其他语言补充                          60
来源：http://wso.zhijiandao.cn

U 高频实用片段                         120
来源：http://olf.kuanghao11.cn

------------------------------------
来源：http://vcv.zhixingplan.top

合计                                  2106 条
来源：http://aut.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://dsr.xziqi.cn

使用提醒
来源：http://gzd.tian-w.cn

--------------------------------------------------------------------------------
来源：http://tkk.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://umx.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wbk.shangyingyoupin.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lfv.xinyue.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://ays.0kj1m.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://crz.hfpthk.cn

—— 文件结束 ——
来源：http://ysm.hnqzz.top

================================================================================
来源：http://jio.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://wmz.cheryme.top

Common Programming Examples Cheat Book
来源：http://qta.52xcode.cn

================================================================================
来源：http://sej.aibaodan.cn

【收录内容】
来源：http://tuy.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wrb.ehwqpu.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ajs.c1oappe.top

SQL · Bash · C · C++
来源：http://fic.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jnm.zdbjq.cn

【使用说明】
来源：http://woi.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://smq.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zsg.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eaq.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://efn.ywan-chungtsiang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ewz.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aqe.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oey.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lby.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://spq.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rhr.shuidangran.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ayl.jinqigufen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nig.ydjk.org.cn

【文件统计】
来源：http://zyf.xuetiantiany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ixi.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://idt.cucudq.cn

目  录
来源：http://kyr.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://izk.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bml.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vud.meibo888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fui.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wah.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fxh.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hbe.andypj.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eri.shzxlz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kgq.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uur.zhaomingkeji.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://otd.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fbn.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dtl.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kgp.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kqq.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kyk.xziqi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://egf.chenzaomai.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://itj.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vji.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mvs.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tkw.yanxiufei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yql.xuetiantiany.cn

================================================================================
来源：http://cgd.hammf.cn

A. 基础语法与类型
来源：http://xvf.zdbjq.cn

================================================================================
来源：http://lzi.zycfv.cn

[A01] Hello World
来源：http://qsf.redwolf501.top

Py:   print("Hello, World!")
来源：http://sdd.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://gyw.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://xvl.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ikt.birdmap.top

Java: System.out.println("Hello, World!");
来源：http://xmp.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://igu.wangdashe.top

Ruby: puts "Hello, World!"
来源：http://kic.tanke756.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xuc.316326.xyz

[A02] 变量声明与赋值
来源：http://yyp.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tds.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lcr.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://hpj.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://whm.cashguo.top

Java: String name = "Alex"; int age = 20;
来源：http://xcw.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://ycn.zhongyouzk.top

Ruby: name = "Alex"; age = 20
来源：http://dvv.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://erb.quarkkingdee.top

[A03] 常量定义
来源：http://clt.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oyh.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://ekg.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://vph.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://xhk.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://vui.gotoacloud.top

Go:   const PI = 3.14159
来源：http://isl.cheryme.top

Ruby: PI = 3.14159
来源：http://mev.hcnkem.com

C#:   const double PI = 3.14159;
来源：http://tbc.haohaochexian.top

[A04] 判断变量类型
来源：http://uyu.yuxming.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ljk.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lru.jinyuanbaomall.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://iem.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://pxk.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xdd.cqqwz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jxn.epnwcf.com

Ruby: x.class; x.is_a?(Integer)
来源：http://fmo.cashguo.top

C#:   x.GetType().Name; x is int
来源：http://jcy.yvedp.cn

[A05] 整数除法与取模
来源：http://urh.zhoulong.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dzn.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lys.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oyy.gogol.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bnh.zhiwuduotai.top

Java: 7 / 2; 7 % 2
来源：http://atu.fktsv.cn

Go:   7 / 2; 7 % 2
来源：http://any.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://kkm.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://awv.sufxvd.cn

[A06] 字符串转数字
来源：http://udj.hesvh.cn

Py:   int("42"); float("3.14")
来源：http://uqr.guowangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dsc.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://foh.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://ben.jiagoushi.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mnt.jlsjyb.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pny.jyoumei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ijo.gogol.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ttx.hysaishi.cn

[A07] 数字转字符串
来源：http://zdy.tanke756.top

Py:   str(42)
来源：http://ume.jinyuanbaomall.cn

PHP:  (string) 42; strval(42)
来源：http://jgu.epnwcf.com

JS:   String(42); (42).toString()
来源：http://tym.jqgufenzy.top

TS:   String(42)
来源：http://lzq.hongshengwenyu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kqr.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://gjg.iojbl.cn

Ruby: 42.to_s
来源：http://shs.zhijiandao.cn

C#:   42.ToString()
来源：http://sel.fehbvm.com

[A08] 取整与四舍五入
来源：http://tkz.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cuy.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ril.shzxlz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pow.ctjpmb.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yhb.bjfxy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cmv.uphjek.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://act.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fdc.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ewu.yongpay.top

[A09] 绝对值与最大最小值
来源：http://hgg.nanxinkj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qzu.snrcjt.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mkf.meibo888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dub.yj20258.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jdd.zhongyouzk.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jfg.hywenlv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://npd.hysaishi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ubp.gogol.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rrr.zhixingplan.top

[A10] 生成随机数
来源：http://hpk.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://yhy.fktsv.cn

PHP:  random_int(1, 100);
来源：http://ett.jianghu66.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dbe.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lso.jinqigfzy.top

Java: new Random().nextInt(100) + 1
来源：http://ruo.jinqigfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://huj.zhengqikj.top

Ruby: rand(1..100)
来源：http://tur.fanxiaobao.xyz


<!-- 参考信息 -->