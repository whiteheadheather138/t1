代发 wailian999

[U69] PHP：PDO 预处理
来源：http://xsm.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lnf.uphjek.com

[U70] PHP：PDO 事务
来源：http://hbl.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://onw.yongpay.top

[U71] PHP：抛出异常
来源：http://fhw.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://iuk.jqgfzy.top

[U72] PHP：写错误日志
来源：http://mim.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://isg.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://iif.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://adg.yj20258888.top

[U74] PHP：读取环境变量
来源：http://vuf.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://oow.dashuyun.cn

[U75] PHP：依赖注入
来源：http://wol.zhoulong.xyz

composer require psr/container
来源：http://nuv.yfazqb.com

[U76] PHP：简单路由
来源：http://fef.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ucs.yuxming.cn

[U77] PHP：模板渲染
来源：http://icn.andypj.xyz

composer require twig/twig
来源：http://jyb.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://zod.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://ahy.fzhhl.top

[U79] PHP：静态分析
来源：http://hff.316326.xyz

composer require --dev phpstan/phpstan
来源：http://ovs.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://aps.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xsr.dashuyun.cn

[U81] JS：初始化项目
来源：http://byf.uphjek.com

npm init -y;  npm i express
来源：http://hxc.epnwcf.com

[U82] JS：package.json 脚本
来源：http://bif.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hup.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://zzz.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qfr.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://avo.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uvw.yongpay.top

[U85] JS：可选链
来源：http://sue.jqgufenzy.top

a?.b?.c
来源：http://ssd.vehdjk.com

[U86] JS：空值合并
来源：http://vpx.yonumen.top

a ?? b
来源：http://zxd.jinqigfzy.top

[U87] JS：解构默认值
来源：http://kcd.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://mqd.zdbjq.cn

[U88] JS：对象展开合并
来源：http://vpj.yvedp.cn

{ ...a, ...b }
来源：http://zzt.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://nmr.epnwcf.com

[...new Set(arr)]
来源：http://edu.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://rit.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://svt.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://qnv.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lre.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://soa.xuanzx.com

structuredClone(obj)
来源：http://bdw.hfpthk.cn

[U93] JS：模板字符串
来源：http://geq.cheryme.top

`共 ${n} 条`
来源：http://ujb.gogol.net.cn

[U94] JS：箭头函数
来源：http://kfv.yvedp.cn

const double = x => x * 2;
来源：http://atz.zdbjq.cn

[U95] JS：Promise 包装
来源：http://zhq.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://yav.xziqi.cn

[U96] JS：async/await 与异常
来源：http://kil.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uge.nwbrower.top

[U97] JS：并发请求
来源：http://zpe.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uej.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://whp.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fsb.ydzc1.top

[U99] JS：事件监听
来源：http://zwo.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://lxn.zhixingplan.top

[U100] JS：DOM 查询
来源：http://ief.316326.xyz

document.querySelector(".item")
来源：http://wuz.sufxvd.cn

[U101] JS：classList 操作
来源：http://yxz.guowangkeji.top

el.classList.toggle("active")
来源：http://tii.hywenlv.cn

[U102] JS：本地存储
来源：http://skg.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tgr.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://tli.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jql.nanxuanxn.top

[U104] JS：防抖
来源：http://vzc.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyz.yj20258.top

[U105] JS：节流
来源：http://ysy.fehbvm.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hqd.sxryk.cn

[U106] JS：日期格式化
来源：http://aqi.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wmp.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://nyt.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vqs.gogol.net.cn

[U108] JS：随机整数
来源：http://gzg.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://syd.havefunace.top

[U109] JS：数组分组
来源：http://jtu.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://pac.sysykeji.top

[U110] JS：数组分块
来源：http://wfv.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hun.fengsongda.top

[U111] JS：对象转 Map
来源：http://ixf.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://pdg.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://frf.tian-w.cn

"7".padStart(3, "0")
来源：http://jkb.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://ipo.pycfn.com

s.replaceAll("a", "b")
来源：http://bdb.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://iwq.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dwl.shzxlz.cn

[U115] JS：生成 UUID
来源：http://pks.shuidangran.top

crypto.randomUUID()
来源：http://gkg.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://eyl.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://flr.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://wbj.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://mxc.andypj.xyz

[U118] JS：开发服务器
来源：http://pbt.jqgfzy.top

npm i -D vite;  npx vite
来源：http://ypf.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://jrp.jinghuilouyu.cn

npx vite build
来源：http://yxi.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://vyu.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://jgg.vehdjk.com

================================================================================
来源：http://ind.c1oappe.top

统计汇总
来源：http://bcv.cucudq.cn

================================================================================
来源：http://pjt.yonumen.top

按语言统计（条）：
来源：http://uyh.fanxiaobao.xyz

Python ......... 252
来源：http://lgf.quarkkingdee.top

PHP ............ 252
来源：http://mgn.cheryme.top

JavaScript ..... 252
来源：http://wsz.yj20258888.top

TypeScript ..... 212
来源：http://rbf.dashuyun.cn

Java ........... 212
来源：http://gll.hysaishi.cn

Go ............. 212
来源：http://epn.hnqzz.top

Ruby ........... 212
来源：http://bvd.zdqjudy.top

C# ............. 212
来源：http://kww.jinyuanbaomall.cn

C .............. 30
来源：http://bbc.xuetiantiany.cn

C++ ............ 30
来源：http://uvx.mhx1999.top

SQL ............ 90
来源：http://dae.cqqwz.cn

Bash ........... 80
来源：http://cap.jianghu66.top

Kotlin ......... 15
来源：http://cwg.ppjwa.cn

Swift .......... 15
来源：http://alj.yuanzhike.top

Lua ............ 10
来源：http://kuq.guowangkeji.top

Perl ........... 10
来源：http://mxt.vehdjk.com

Scala .......... 10
来源：http://suk.hongshengwenyu.top

------------------------------------
来源：http://oqi.xziqi.cn

合计 ........... 2106 条
来源：http://ojc.xylfe.cn

按章节统计：
来源：http://qmn.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tqj.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qgg.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qgk.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://azd.ydjk.org.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://afq.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nth.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dej.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ifo.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://htq.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jmy.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nto.shanyushiyangtech.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vzz.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jcn.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pes.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zxu.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dhw.sufxvd.cn

Q SQL 专题                              90
来源：http://air.zdqjudy.top

R Bash 专题                             80
来源：http://cpx.yongpay.top

S C / C++ 专题                          60
来源：http://ksh.gotoacloud.top

T 其他语言补充                          60
来源：http://fwz.tianlin.xyz

U 高频实用片段                         120
来源：http://icz.dashuyun.cn

------------------------------------
来源：http://sft.tanke756.top

合计                                  2106 条
来源：http://qru.gzhubu.top

--------------------------------------------------------------------------------
来源：http://vab.xuanzx.com

使用提醒
来源：http://kpt.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://gnq.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zcj.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://obs.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ghn.quarkkingdee.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nkg.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ark.gaohongyu789.top

—— 文件结束 ——
来源：http://sxm.zhixingplan.top

================================================================================
来源：http://fja.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://ydp.uphjek.com

Common Programming Examples Cheat Book
来源：http://cqm.hnqzz.top

================================================================================
来源：http://edj.wangshuangyany.cn

【收录内容】
来源：http://zgo.yj20258.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cfk.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bjm.sysykeji.top

SQL · Bash · C · C++
来源：http://gsw.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xky.fzhhl.top

【使用说明】
来源：http://ozf.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hxb.xingfuxueyuan.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bgj.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ppt.aibaodan.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hrv.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wbx.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qfu.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zos.jiagoushi.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vgv.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ulj.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ule.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lod.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vcv.nwbrower.top

【文件统计】
来源：http://rzs.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://afl.hnqzz.top

--------------------------------------------------------------------------------
来源：http://evi.feifeiyinyue.top

目  录
来源：http://ija.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://dse.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://afv.quarkkingdee.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fkd.uphjek.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lbe.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://psi.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jrn.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ose.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rhf.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://twp.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pbv.sweek.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ibq.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ypg.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xkh.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gve.zhengqikj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iki.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qzq.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sig.sweek.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://otd.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://mbj.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xxp.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xyi.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xoa.epnwcf.com

================================================================================
来源：http://tpu.zhijiandao.cn

A. 基础语法与类型
来源：http://mjs.yuxming.cn

================================================================================
来源：http://fqc.gzhubu.top

[A01] Hello World
来源：http://eki.gaohongyu789.top

Py:   print("Hello, World!")
来源：http://jem.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://azq.hammf.cn

JS:   console.log("Hello, World!");
来源：http://xsa.smart0.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://svd.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://lde.wangshuangyany.cn

Go:   fmt.Println("Hello, World!")
来源：http://skx.cashguo.top

Ruby: puts "Hello, World!"
来源：http://kvv.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xgx.smart0.xyz

[A02] 变量声明与赋值
来源：http://euf.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sfu.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vbd.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://wsn.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://axo.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://wzn.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://qrg.sysykeji.top

Ruby: name = "Alex"; age = 20
来源：http://fak.jinghuilouyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zhm.shzxlz.cn

[A03] 常量定义
来源：http://vwe.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cds.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://qcj.shanyushiyangtech.top

JS:   const PI = 3.14159;
来源：http://slm.fktsv.cn

TS:   const PI: number = 3.14159;
来源：http://uvo.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://xwu.jyoumei.cn

Go:   const PI = 3.14159
来源：http://qjh.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://yjm.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://rdg.chenlongwang.top

[A04] 判断变量类型
来源：http://svi.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cae.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yyq.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://brq.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://wok.hywenlv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gns.feifeiyinyue.top

Go:   reflect.TypeOf(x).Name()
来源：http://bhq.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xgm.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://wor.sweek.top

[A05] 整数除法与取模
来源：http://lfd.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zcq.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://erb.jinghuilouyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ebk.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yqf.316326.xyz

Java: 7 / 2; 7 % 2
来源：http://kna.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://ays.mhx1999.top

Ruby: 7 / 2; 7 % 2
来源：http://sfn.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://ljs.gotoacloud.top

[A06] 字符串转数字
来源：http://ujt.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://yto.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fuu.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zkh.ybcxt.top

TS:   parseInt("42", 10); Number("42")
来源：http://soj.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dcm.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ifd.daria6918.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xpc.hywenlv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zap.ybcxt.top

[A07] 数字转字符串
来源：http://nsl.smart0.xyz

Py:   str(42)
来源：http://gzy.jlsjyb.cn

PHP:  (string) 42; strval(42)
来源：http://lvb.tianlin.xyz

JS:   String(42); (42).toString()
来源：http://lzf.zdqjudy.top

TS:   String(42)
来源：http://ynk.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vzt.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://tgl.haohaochexian.top

Ruby: 42.to_s
来源：http://kaz.fanxiaobao.xyz

C#:   42.ToString()
来源：http://ovj.iojbl.cn

[A08] 取整与四舍五入
来源：http://gbe.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kxh.ctjpmb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pkj.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cpe.zhiwuduotai.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://skn.yvedp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://prn.ctjpmb.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dls.316326.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://jnj.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hgd.xylfe.cn

[A09] 绝对值与最大最小值
来源：http://fkt.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zxo.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jiq.yueranfly.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://buh.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zbq.jqgufenzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uaf.uphjek.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rfu.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wnb.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lud.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://mdx.kuanghao11.cn

Py:   import random; random.randint(1, 100)
来源：http://uvq.pycfn.com

PHP:  random_int(1, 100);
来源：http://plt.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bpz.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sms.vqdsnc.cn

Java: new Random().nextInt(100) + 1
来源：http://bte.hcnkem.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://say.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://fci.sufxvd.cn


<!-- 参考信息 -->