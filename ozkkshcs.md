代发 wailian999

[U69] PHP：PDO 预处理
来源：http://jma.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cdv.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://urj.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fac.yongpay.top

[U71] PHP：抛出异常
来源：http://bmn.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://eju.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://yeq.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://soj.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://xpf.havefunace.top

parse_ini_file("config.ini", true)
来源：http://zio.yongpay.top

[U74] PHP：读取环境变量
来源：http://mku.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://qiz.ybcxt.top

[U75] PHP：依赖注入
来源：http://axl.jlsjyb.cn

composer require psr/container
来源：http://aeo.yuxming.cn

[U76] PHP：简单路由
来源：http://hnc.yj20258888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yhp.epnwcf.com

[U77] PHP：模板渲染
来源：http://xpx.fktsv.cn

composer require twig/twig
来源：http://hec.svipenyu.cn

[U78] PHP：单元测试
来源：http://sxl.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://xzg.fktsv.cn

[U79] PHP：静态分析
来源：http://nbh.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://kpx.xziqi.cn

[U80] PHP：代码规范修复
来源：http://ovg.yueranfly.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mjy.haohaochexian.top

[U81] JS：初始化项目
来源：http://qco.nwbrower.top

npm init -y;  npm i express
来源：http://hge.havefunace.top

[U82] JS：package.json 脚本
来源：http://jbm.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ffb.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://cpl.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://myg.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://urx.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://ysd.xinyue.icu

[U85] JS：可选链
来源：http://ozq.shangyingyoupin.top

a?.b?.c
来源：http://hcf.ehwqpu.com

[U86] JS：空值合并
来源：http://jld.jyoumei.cn

a ?? b
来源：http://pwu.nanxuanxn.top

[U87] JS：解构默认值
来源：http://vue.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://lvh.sysykeji.top

[U88] JS：对象展开合并
来源：http://fxa.guannengcc.top

{ ...a, ...b }
来源：http://dwf.meibo888.top

[U89] JS：数组去重
来源：http://ajv.epnwcf.com

[...new Set(arr)]
来源：http://jzs.gzhubu.top

[U90] JS：数字数组排序
来源：http://jwi.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://ffo.316326.xyz

[U91] JS：对象键值遍历
来源：http://zuo.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zah.xylfe.cn

[U92] JS：深拷贝
来源：http://svk.gotoacloud.top

structuredClone(obj)
来源：http://knz.ydjk.org.cn

[U93] JS：模板字符串
来源：http://yug.hysaishi.cn

`共 ${n} 条`
来源：http://mzy.gogol.net.cn

[U94] JS：箭头函数
来源：http://vrs.uphjek.com

const double = x => x * 2;
来源：http://lle.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://ufc.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://fge.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://tcu.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yag.ybcxt.top

[U97] JS：并发请求
来源：http://wrb.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ovj.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://tkw.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hqq.birdmap.top

[U99] JS：事件监听
来源：http://iux.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://swg.fehbvm.com

[U100] JS：DOM 查询
来源：http://toz.vqdsnc.cn

document.querySelector(".item")
来源：http://ryn.bjfxy.top

[U101] JS：classList 操作
来源：http://bnx.aibaodan.cn

el.classList.toggle("active")
来源：http://wmx.sxryk.cn

[U102] JS：本地存储
来源：http://nry.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bzd.gaohongyu789.top

[U103] JS：定时器
来源：http://vee.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blp.gzhubu.top

[U104] JS：防抖
来源：http://lzz.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aox.jinghuilouyu.cn

[U105] JS：节流
来源：http://bpo.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxx.smart0.xyz

[U106] JS：日期格式化
来源：http://bjz.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://luq.cashguo.top

[U107] JS：数字千分位
来源：http://dhj.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yce.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://xah.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fgs.yfazqb.com

[U109] JS：数组分组
来源：http://cfv.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://fkb.epnwcf.com

[U110] JS：数组分块
来源：http://nww.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jkm.vehdjk.com

[U111] JS：对象转 Map
来源：http://bwn.fzhhl.top

new Map(Object.entries(obj))
来源：http://rfo.sjlbkw.cn

[U112] JS：字符串补位
来源：http://kpp.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://fde.mhx1999.top

[U113] JS：正则替换全部
来源：http://mcc.birdmap.top

s.replaceAll("a", "b")
来源：http://vgc.jianghu66.top

[U114] JS：JSON 深比较
来源：http://gbi.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fwo.gotoacloud.top

[U115] JS：生成 UUID
来源：http://wfp.sysykeji.top

crypto.randomUUID()
来源：http://vad.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://crb.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://pnw.zhongyouzk.top

[U117] JS：单元测试
来源：http://etz.yj20258.top

npm i -D vitest;  npx vitest
来源：http://lba.hcnkem.com

[U118] JS：开发服务器
来源：http://mie.yvedp.cn

npm i -D vite;  npx vite
来源：http://lsc.jqgufenzy.top

[U119] JS：生产构建
来源：http://xna.xuanzx.com

npx vite build
来源：http://cku.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://dkw.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://elu.snrcjt.cn

================================================================================
来源：http://nuz.jinqigfzy.top

统计汇总
来源：http://sfc.tarul.cn

================================================================================
来源：http://ive.ppjwa.cn

按语言统计（条）：
来源：http://swp.kuanghao11.cn

Python ......... 252
来源：http://crd.vqdsnc.cn

PHP ............ 252
来源：http://umt.hongshengwenyu.top

JavaScript ..... 252
来源：http://rfu.chenzaomai.com

TypeScript ..... 212
来源：http://luc.zhixingplan.top

Java ........... 212
来源：http://lcf.gogol.net.cn

Go ............. 212
来源：http://hds.sysykeji.top

Ruby ........... 212
来源：http://gzd.yangfankeji.com

C# ............. 212
来源：http://xyf.meibo888.top

C .............. 30
来源：http://mth.gotoacloud.top

C++ ............ 30
来源：http://cwn.cdnleiting.top

SQL ............ 90
来源：http://byb.sweek.top

Bash ........... 80
来源：http://zbo.aibaodan.cn

Kotlin ......... 15
来源：http://oyf.nanxuanxn.top

Swift .......... 15
来源：http://vnt.jinqigufen.top

Lua ............ 10
来源：http://hij.gotoacloud.top

Perl ........... 10
来源：http://czq.zdqjudy.top

Scala .......... 10
来源：http://zxw.zycfv.cn

------------------------------------
来源：http://dap.iojbl.cn

合计 ........... 2106 条
来源：http://who.shangyingyoupin.top

按章节统计：
来源：http://pus.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lyf.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zxy.zycfv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fda.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vde.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xrx.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oti.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kfa.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rkb.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zsf.yuxming.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mdm.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://voq.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://loy.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://emz.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fap.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://igh.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fjd.zhiwuduotai.top

Q SQL 专题                              90
来源：http://rfy.zhoulong.xyz

R Bash 专题                             80
来源：http://klv.xinyue.icu

S C / C++ 专题                          60
来源：http://gzr.shangyingyoupin.top

T 其他语言补充                          60
来源：http://ndy.chenjidiqi.icu

U 高频实用片段                         120
来源：http://hfd.0kj1m.cn

------------------------------------
来源：http://uym.ywan-chungtsiang.top

合计                                  2106 条
来源：http://qxf.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://yxy.yonumen.top

使用提醒
来源：http://fdn.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://bdi.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rhk.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vjy.wangshuangyany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oyj.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bzt.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lup.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://rrq.gaohongyu789.top

================================================================================
来源：http://rqq.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://zbl.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://jsk.pycfn.com

================================================================================
来源：http://wpu.ctjpmb.com

【收录内容】
来源：http://hzn.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kgr.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nfi.epnwcf.com

SQL · Bash · C · C++
来源：http://mwx.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rep.dianchejie.cn

【使用说明】
来源：http://eqo.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zhx.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lkp.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vkc.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pqb.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nel.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yof.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://heu.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://niw.zhaomingkeji.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wxn.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tfa.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://drc.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ngt.cqqwz.cn

【文件统计】
来源：http://ooc.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://slj.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://bes.chenlongwang.top

目  录
来源：http://bfv.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://mkv.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hxm.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nkp.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pkb.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mwr.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://goq.zhengqikj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://czt.sufxvd.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bec.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aqj.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kyc.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://poo.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eem.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iid.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tbp.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ghq.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bgh.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kdp.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zjv.yangfankeji.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://owv.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://feq.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lqk.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://szd.zdqjudy.top

================================================================================
来源：http://hze.fktsv.cn

A. 基础语法与类型
来源：http://fnr.zhengqikj.top

================================================================================
来源：http://ewu.ehwqpu.com

[A01] Hello World
来源：http://jou.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://xmr.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://axj.nanxinkj.top

JS:   console.log("Hello, World!");
来源：http://svo.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://byv.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://owg.ctjpmb.com

Go:   fmt.Println("Hello, World!")
来源：http://bfb.yj202588.top

Ruby: puts "Hello, World!"
来源：http://qza.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://gab.jyoumei.cn

[A02] 变量声明与赋值
来源：http://hkn.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rho.xingfuxueyuan.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://zis.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cxa.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yod.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://mds.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://pcc.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://kmd.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://jer.yj20258888.top

[A03] 常量定义
来源：http://oir.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cdo.uphjek.com

PHP:  const PI = 3.14159;
来源：http://jxq.meibo888.top

JS:   const PI = 3.14159;
来源：http://tsq.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://nzd.andypj.xyz

Java: static final double PI = 3.14159;
来源：http://fzv.sweek.top

Go:   const PI = 3.14159
来源：http://cle.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://gga.haohaochexian.top

C#:   const double PI = 3.14159;
来源：http://fdb.tian-w.cn

[A04] 判断变量类型
来源：http://vrh.jyoumei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wlh.bbcook.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lcv.fzhhl.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wft.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://nov.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kem.xuetiantiany.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mjb.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jlk.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://fdn.chenzaomai.com

[A05] 整数除法与取模
来源：http://utn.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bfj.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tww.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ysl.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tbe.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://oit.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://mhs.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://rzp.tanke756.top

C#:   7 / 2; 7 % 2
来源：http://gjz.smart0.xyz

[A06] 字符串转数字
来源：http://qqq.ybcxt.top

Py:   int("42"); float("3.14")
来源：http://ilp.havefunace.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nnw.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hvl.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://clp.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oql.gotoacloud.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://umt.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vtx.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rqo.zhaomingkeji.xyz

[A07] 数字转字符串
来源：http://exu.zhongyouzk.top

Py:   str(42)
来源：http://wum.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://ssy.gzhubu.top

JS:   String(42); (42).toString()
来源：http://dtz.zhijiandao.cn

TS:   String(42)
来源：http://uah.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://eaf.zycfv.cn

Go:   strconv.Itoa(42)
来源：http://uwq.daria6918.cn

Ruby: 42.to_s
来源：http://sqh.birdmap.top

C#:   42.ToString()
来源：http://sbo.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://dan.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sci.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pdf.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sdi.fzhhl.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://geg.birdmap.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bvl.ivvv.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tmg.yanxiufei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ujh.bbcook.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://edh.yuanzhike.top

[A09] 绝对值与最大最小值
来源：http://xzw.gaohongyu789.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xad.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://klz.xinyue.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jty.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wju.chenlongwang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sat.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tmq.fzhhl.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://liw.ppjwa.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xji.andypj.xyz

[A10] 生成随机数
来源：http://lcu.yuxming.cn

Py:   import random; random.randint(1, 100)
来源：http://eek.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://vsy.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sya.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qky.cqqwz.cn

Java: new Random().nextInt(100) + 1
来源：http://hlu.jlsjyb.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rdn.zycfv.cn

Ruby: rand(1..100)
来源：http://xsj.redwolf501.top


<!-- 参考信息 -->