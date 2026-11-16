代发 wailian999

[U69] PHP：PDO 预处理
来源：http://stg.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ksh.bbcook.cn

[U70] PHP：PDO 事务
来源：http://eeo.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dma.xylfe.cn

[U71] PHP：抛出异常
来源：http://xto.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://oav.zdbjq.cn

[U72] PHP：写错误日志
来源：http://wil.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://roo.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://ihc.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://wjh.hnqzz.top

[U74] PHP：读取环境变量
来源：http://ayi.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://wif.yonumen.top

[U75] PHP：依赖注入
来源：http://ztc.xingfuxueyuan.xyz

composer require psr/container
来源：http://ktj.andypj.xyz

[U76] PHP：简单路由
来源：http://iga.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nyr.hammf.cn

[U77] PHP：模板渲染
来源：http://cnf.yuanzhike.top

composer require twig/twig
来源：http://eyc.yj20258.top

[U78] PHP：单元测试
来源：http://rvf.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://gvt.hfpthk.cn

[U79] PHP：静态分析
来源：http://sia.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://fwp.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://nwi.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dsj.redwolf501.top

[U81] JS：初始化项目
来源：http://ztx.vehdjk.com

npm init -y;  npm i express
来源：http://lpk.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://pyf.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fto.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://hxf.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pmo.sweek.top

[U84] JS：CommonJS 写法
来源：http://ilr.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hrx.gaohongyu789.top

[U85] JS：可选链
来源：http://zgh.tian-w.cn

a?.b?.c
来源：http://hxj.sjlbkw.cn

[U86] JS：空值合并
来源：http://hgc.gotoacloud.top

a ?? b
来源：http://yah.yuxming.cn

[U87] JS：解构默认值
来源：http://uac.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://fhw.hywenlv.cn

[U88] JS：对象展开合并
来源：http://awq.yvedp.cn

{ ...a, ...b }
来源：http://dlx.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://jsi.shzxlz.cn

[...new Set(arr)]
来源：http://tdf.nanxinkj.top

[U90] JS：数字数组排序
来源：http://dqz.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://qdk.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://lek.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zqy.bbcook.cn

[U92] JS：深拷贝
来源：http://yme.ehwqpu.com

structuredClone(obj)
来源：http://tcu.cucudq.cn

[U93] JS：模板字符串
来源：http://bft.quarkkingdee.top

`共 ${n} 条`
来源：http://jmm.hnxiangtu.top

[U94] JS：箭头函数
来源：http://mxc.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://thw.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://wqm.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://hgh.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://hqm.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hac.svipenyu.cn

[U97] JS：并发请求
来源：http://xyq.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jww.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://xnk.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nfv.andypj.xyz

[U99] JS：事件监听
来源：http://jzf.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://zdm.shzxlz.cn

[U100] JS：DOM 查询
来源：http://zgt.ehwqpu.com

document.querySelector(".item")
来源：http://bmo.pycfn.com

[U101] JS：classList 操作
来源：http://pnx.smart0.xyz

el.classList.toggle("active")
来源：http://mvk.jinqigufen.top

[U102] JS：本地存储
来源：http://unt.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://wdq.pycfn.com

[U103] JS：定时器
来源：http://jbh.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rxg.ppjwa.cn

[U104] JS：防抖
来源：http://iiy.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cix.andypj.xyz

[U105] JS：节流
来源：http://fjw.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gaq.sxryk.cn

[U106] JS：日期格式化
来源：http://feq.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rrd.gogol.net.cn

[U107] JS：数字千分位
来源：http://voc.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fip.gotoacloud.top

[U108] JS：随机整数
来源：http://wcd.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uab.cdnleiting.top

[U109] JS：数组分组
来源：http://zfc.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://bsk.vehdjk.com

[U110] JS：数组分块
来源：http://soq.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aem.yonumen.top

[U111] JS：对象转 Map
来源：http://jui.vehdjk.com

new Map(Object.entries(obj))
来源：http://rpv.tarul.cn

[U112] JS：字符串补位
来源：http://blp.0kj1m.cn

"7".padStart(3, "0")
来源：http://mvj.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://paw.tanke756.top

s.replaceAll("a", "b")
来源：http://ped.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://iib.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qnt.snrcjt.cn

[U115] JS：生成 UUID
来源：http://pqz.yangfankeji.com

crypto.randomUUID()
来源：http://zua.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://iwm.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://sty.ybcxt.top

[U117] JS：单元测试
来源：http://wjz.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://pbw.guannengcc.top

[U118] JS：开发服务器
来源：http://ifm.aibaodan.cn

npm i -D vite;  npx vite
来源：http://bal.shzxlz.cn

[U119] JS：生产构建
来源：http://msr.jinqigufen.top

npx vite build
来源：http://hgb.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://ekz.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://ggp.aizwys.cn

================================================================================
来源：http://wgu.chenzaomai.com

统计汇总
来源：http://klm.hnxiangtu.top

================================================================================
来源：http://inu.zhaomingkeji.xyz

按语言统计（条）：
来源：http://xlb.hcnkem.com

Python ......... 252
来源：http://zlr.quarkkingdee.top

PHP ............ 252
来源：http://dur.ybcxt.top

JavaScript ..... 252
来源：http://bgq.chenlongwang.top

TypeScript ..... 212
来源：http://hbu.nwbrower.top

Java ........... 212
来源：http://hsv.ywan-chungtsiang.top

Go ............. 212
来源：http://jtz.dianchejie.cn

Ruby ........... 212
来源：http://ius.shanyushiyangkeji.top

C# ............. 212
来源：http://xxb.smart0.xyz

C .............. 30
来源：http://glv.chenjidiqi.icu

C++ ............ 30
来源：http://pqr.fehbvm.com

SQL ............ 90
来源：http://rkh.uphjek.com

Bash ........... 80
来源：http://kbr.meibo888.top

Kotlin ......... 15
来源：http://tdm.0kj1m.cn

Swift .......... 15
来源：http://age.jyoumei.cn

Lua ............ 10
来源：http://zyp.fzhhl.top

Perl ........... 10
来源：http://bhn.sufxvd.cn

Scala .......... 10
来源：http://oan.wangshuangyany.cn

------------------------------------
来源：http://ixi.feifeiyinyue.top

合计 ........... 2106 条
来源：http://sgw.sxryk.cn

按章节统计：
来源：http://tyh.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xfb.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yqg.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://utb.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iur.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mrh.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wwd.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://skz.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ynm.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ftc.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xvu.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://idn.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rvi.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qvi.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zvi.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pfy.xziqi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ytn.cdnleiting.top

Q SQL 专题                              90
来源：http://oap.wangdashe.top

R Bash 专题                             80
来源：http://uwa.tian-w.cn

S C / C++ 专题                          60
来源：http://wzm.andypj.xyz

T 其他语言补充                          60
来源：http://oow.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://hju.chenjidiqi.icu

------------------------------------
来源：http://muk.yfazqb.com

合计                                  2106 条
来源：http://jbx.cashguo.top

--------------------------------------------------------------------------------
来源：http://mhw.hongshengwenyu.top

使用提醒
来源：http://ubb.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://sjl.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://omk.iojbl.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xwm.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qux.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://jmb.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jmz.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://tbh.bjfxy.top

================================================================================
来源：http://beq.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://kat.xuanzx.com

Common Programming Examples Cheat Book
来源：http://sdd.yangfankeji.com

================================================================================
来源：http://cva.ppjwa.cn

【收录内容】
来源：http://ytu.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rlo.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dfy.hammf.cn

SQL · Bash · C · C++
来源：http://dut.jinqigfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vjb.zhiwuduotai.top

【使用说明】
来源：http://ind.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qbn.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ota.yuxming.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ssf.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gwd.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://snc.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://evr.cheryme.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ext.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://div.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://epf.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xvl.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jbj.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ytq.hongshengwenyu.top

【文件统计】
来源：http://xzy.vqdsnc.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rfu.yfazqb.com

--------------------------------------------------------------------------------
来源：http://vpo.wangshuangyany.cn

目  录
来源：http://ice.daria6918.cn

--------------------------------------------------------------------------------
来源：http://wwz.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kyo.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bah.jinqigfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pit.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://heg.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wfs.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://utq.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xfr.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fqi.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zjt.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://utj.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vby.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lsw.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ews.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qzw.dashuyun.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ezo.ybcxt.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zdi.xziqi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zfm.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://vsg.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qdr.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xsi.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ucf.shzxlz.cn

================================================================================
来源：http://nmz.hywenlv.cn

A. 基础语法与类型
来源：http://obd.birdmap.top

================================================================================
来源：http://fbl.yvedp.cn

[A01] Hello World
来源：http://cyt.yangfankeji.com

Py:   print("Hello, World!")
来源：http://rtt.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://ivd.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://pyg.zhijiandao.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nnz.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://jqw.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://fth.yj20258.top

Ruby: puts "Hello, World!"
来源：http://crk.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nux.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://uts.jinyuanbaomall.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xgn.yj20258888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zee.pengpengdd.cyou

JS:   let name = "Alex"; const age = 20;
来源：http://zmb.jinqigufen.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bno.yueranfly.top

Java: String name = "Alex"; int age = 20;
来源：http://slo.zycfv.cn

Go:   name := "Alex"; age := 20
来源：http://izm.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://wew.gaohongyu789.top

C#:   string name = "Alex"; int age = 20;
来源：http://wxb.ppjwa.cn

[A03] 常量定义
来源：http://ebk.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wzd.yonumen.top

PHP:  const PI = 3.14159;
来源：http://clu.hammf.cn

JS:   const PI = 3.14159;
来源：http://vbq.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://eku.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://riu.snrcjt.cn

Go:   const PI = 3.14159
来源：http://ond.gaohongyu789.top

Ruby: PI = 3.14159
来源：http://gun.sxryk.cn

C#:   const double PI = 3.14159;
来源：http://wuq.ywan-chungtsiang.top

[A04] 判断变量类型
来源：http://ccs.chenlongwang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dzs.hywenlv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eyd.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pjs.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://etf.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ogq.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qqq.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fff.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://ibs.zdbjq.cn

[A05] 整数除法与取模
来源：http://tmj.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ukx.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uds.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jqe.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nsh.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://tqt.gotoacloud.top

Go:   7 / 2; 7 % 2
来源：http://hqr.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://vqu.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://aej.zdbjq.cn

[A06] 字符串转数字
来源：http://rzo.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://tva.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zql.ydjk.org.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://alw.sweek.top

TS:   parseInt("42", 10); Number("42")
来源：http://avo.tanke756.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jab.havefunace.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://opb.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cvi.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fph.andypj.xyz

[A07] 数字转字符串
来源：http://wda.hnxiangtu.top

Py:   str(42)
来源：http://xxn.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://ivz.xinyue.icu

JS:   String(42); (42).toString()
来源：http://xcn.dianchejie.cn

TS:   String(42)
来源：http://hxi.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://iwl.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://tah.zdbjq.cn

Ruby: 42.to_s
来源：http://pul.hammf.cn

C#:   42.ToString()
来源：http://zyn.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://rty.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://snx.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oyu.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xnt.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ani.mhx1999.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lfw.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ecn.fengsongda.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hnh.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vsr.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://bae.shzxlz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bmj.aibaodan.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mgc.jiagoushi.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rqn.zhiwuduotai.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cwq.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bon.jinyuanbaomall.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eaq.zhijiandao.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://obs.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pul.bbcook.cn

[A10] 生成随机数
来源：http://hkd.gotoacloud.top

Py:   import random; random.randint(1, 100)
来源：http://vvi.sxryk.cn

PHP:  random_int(1, 100);
来源：http://pkz.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yuz.aibaodan.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mlh.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://hlv.ydjk.org.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://abg.xinyue.icu

Ruby: rand(1..100)
来源：http://mij.gzhubu.top


<!-- 参考信息 -->