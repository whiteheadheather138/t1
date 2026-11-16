代发 wailian999

[U65] PHP：会话
来源：http://hxd.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://itc.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://htw.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jba.havefunace.top

[U67] PHP：处理文件上传
来源：http://rng.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mvc.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://fyi.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aif.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://qfe.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rpi.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://alh.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uds.sxryk.cn

[U71] PHP：抛出异常
来源：http://via.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://tmh.jiagoushi.top

[U72] PHP：写错误日志
来源：http://xuk.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://mys.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://mux.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://etw.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://bjg.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://ije.yj202588.top

[U75] PHP：依赖注入
来源：http://xru.tianlin.xyz

composer require psr/container
来源：http://afy.cashguo.top

[U76] PHP：简单路由
来源：http://sbv.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lal.fktsv.cn

[U77] PHP：模板渲染
来源：http://qqs.yj20258888.top

composer require twig/twig
来源：http://rif.ydzc1.top

[U78] PHP：单元测试
来源：http://pot.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://sye.tianlin.xyz

[U79] PHP：静态分析
来源：http://mox.yj20258.top

composer require --dev phpstan/phpstan
来源：http://cxf.sweek.top

[U80] PHP：代码规范修复
来源：http://ehl.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hwf.zdqjudy.top

[U81] JS：初始化项目
来源：http://igc.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://cje.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://bip.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wxg.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://egf.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://rdr.yonumen.top

[U84] JS：CommonJS 写法
来源：http://efl.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fuj.hongshengwenyu.top

[U85] JS：可选链
来源：http://hjp.jlsjyb.cn

a?.b?.c
来源：http://sxy.wangshuangyany.cn

[U86] JS：空值合并
来源：http://tmk.ehwqpu.com

a ?? b
来源：http://ray.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://dqx.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://zbg.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://bhv.hammf.cn

{ ...a, ...b }
来源：http://mdb.jqgfzy.top

[U89] JS：数组去重
来源：http://prj.zhiwuduotai.top

[...new Set(arr)]
来源：http://gqa.hnqzz.top

[U90] JS：数字数组排序
来源：http://wci.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://vwy.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://qbj.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://odx.jlsjyb.cn

[U92] JS：深拷贝
来源：http://hua.snrcjt.cn

structuredClone(obj)
来源：http://aqy.jinqigfzy.top

[U93] JS：模板字符串
来源：http://bon.yuanzhike.top

`共 ${n} 条`
来源：http://oei.hfpthk.cn

[U94] JS：箭头函数
来源：http://jii.hysaishi.cn

const double = x => x * 2;
来源：http://yeg.yj202588.top

[U95] JS：Promise 包装
来源：http://lbe.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://fvr.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://onb.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://omi.ydzc1.top

[U97] JS：并发请求
来源：http://xdw.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kkt.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://nep.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zse.sxryk.cn

[U99] JS：事件监听
来源：http://zie.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://bxi.c1oappe.top

[U100] JS：DOM 查询
来源：http://cfo.tarul.cn

document.querySelector(".item")
来源：http://cnt.snrcjt.cn

[U101] JS：classList 操作
来源：http://ujj.zdqjudy.top

el.classList.toggle("active")
来源：http://shs.fktsv.cn

[U102] JS：本地存储
来源：http://nbm.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://acg.meibo888.top

[U103] JS：定时器
来源：http://ini.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ics.yuxming.cn

[U104] JS：防抖
来源：http://bie.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odt.xziqi.cn

[U105] JS：节流
来源：http://prs.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ipx.zhixingplan.top

[U106] JS：日期格式化
来源：http://xeq.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zub.havefunace.top

[U107] JS：数字千分位
来源：http://fez.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rtt.yongpay.top

[U108] JS：随机整数
来源：http://qht.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hrt.zhoulong.xyz

[U109] JS：数组分组
来源：http://dss.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://pdi.haohaochexian.top

[U110] JS：数组分块
来源：http://scl.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tpe.cashguo.top

[U111] JS：对象转 Map
来源：http://xdn.ivvv.top

new Map(Object.entries(obj))
来源：http://eim.gogol.net.cn

[U112] JS：字符串补位
来源：http://tya.yj20258.top

"7".padStart(3, "0")
来源：http://rke.yvedp.cn

[U113] JS：正则替换全部
来源：http://tzq.epnwcf.com

s.replaceAll("a", "b")
来源：http://dcl.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://cxj.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://wwc.dashuyun.cn

[U115] JS：生成 UUID
来源：http://xny.quarkkingdee.top

crypto.randomUUID()
来源：http://szm.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://bse.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://epz.hysaishi.cn

[U117] JS：单元测试
来源：http://nzt.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://xhv.pycfn.com

[U118] JS：开发服务器
来源：http://rqc.yj202588.top

npm i -D vite;  npx vite
来源：http://son.cdnleiting.top

[U119] JS：生产构建
来源：http://jgk.guannengcc.top

npx vite build
来源：http://xqd.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://bef.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://ufh.zhaomingkeji.xyz

================================================================================
来源：http://xbm.wangdashe.top

统计汇总
来源：http://adm.feifeiyinyue.top

================================================================================
来源：http://ulm.yj202588.top

按语言统计（条）：
来源：http://azk.c1oappe.top

Python ......... 252
来源：http://kme.zhiwuduotai.top

PHP ............ 252
来源：http://exl.zdqjudy.top

JavaScript ..... 252
来源：http://ign.jiagoushi.top

TypeScript ..... 212
来源：http://cuo.wangdashe.top

Java ........... 212
来源：http://xbi.yuanzhike.top

Go ............. 212
来源：http://rdk.zhoulong.xyz

Ruby ........... 212
来源：http://bmx.hnxiangtu.top

C# ............. 212
来源：http://cjd.fehbvm.com

C .............. 30
来源：http://ywg.zhiwuduotai.top

C++ ............ 30
来源：http://zgx.xziqi.cn

SQL ............ 90
来源：http://jra.jinyuanbaomall.cn

Bash ........... 80
来源：http://bdy.vqdsnc.cn

Kotlin ......... 15
来源：http://sik.nwbrower.top

Swift .......... 15
来源：http://bqq.tian-w.cn

Lua ............ 10
来源：http://aaw.xinyue.icu

Perl ........... 10
来源：http://usm.jlsjyb.cn

Scala .......... 10
来源：http://hxh.xinyue.icu

------------------------------------
来源：http://guc.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://uqc.fzhhl.top

按章节统计：
来源：http://fcd.chenlongwang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ccs.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wxq.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yjg.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bjn.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pje.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yjn.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fls.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pha.jiagoushi.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ajj.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xez.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vvu.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://plw.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pbe.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zyj.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jja.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mho.cqqwz.cn

Q SQL 专题                              90
来源：http://yfb.yj20258.top

R Bash 专题                             80
来源：http://vsw.zhijiandao.cn

S C / C++ 专题                          60
来源：http://ocu.sufxvd.cn

T 其他语言补充                          60
来源：http://ypw.jyoumei.cn

U 高频实用片段                         120
来源：http://mio.yongpay.top

------------------------------------
来源：http://jgy.jqgufenzy.top

合计                                  2106 条
来源：http://xas.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://qbm.zdqjudy.top

使用提醒
来源：http://hja.cucudq.cn

--------------------------------------------------------------------------------
来源：http://flu.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yyp.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kbu.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jsw.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zpc.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://epq.fzhhl.top

—— 文件结束 ——
来源：http://qwq.ywan-chungtsiang.top

================================================================================
来源：http://mae.ywan-chungtsiang.top

程序语言常见例子速查手册（2024 版）
来源：http://gdl.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://nuf.vehdjk.com

================================================================================
来源：http://wug.tanke756.top

【收录内容】
来源：http://wcu.xziqi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cpr.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xzl.svipenyu.cn

SQL · Bash · C · C++
来源：http://rkc.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sfa.sjlbkw.cn

【使用说明】
来源：http://emi.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vyw.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sgz.fanxiaobao.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sru.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rpt.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://haw.vehdjk.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://opf.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wue.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ess.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tkr.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hrc.haohaochexian.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://axb.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dmx.ydzc1.top

【文件统计】
来源：http://vvi.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qhm.bjfxy.top

--------------------------------------------------------------------------------
来源：http://jsn.jinqigfzy.top

目  录
来源：http://cbh.hcnkem.com

--------------------------------------------------------------------------------
来源：http://gqf.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xjt.havefunace.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ypr.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rnw.jqgufenzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jfh.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ery.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://czb.gaohongyu789.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qwi.xinyue.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wqm.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ekr.xuanzx.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jem.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zeo.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fao.havefunace.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lov.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uax.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://knn.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cop.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zdl.smart0.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://hzz.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yrs.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kuv.feifeiyinyue.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mfs.zhijiandao.cn

================================================================================
来源：http://dhd.aibaodan.cn

A. 基础语法与类型
来源：http://vqz.sweek.top

================================================================================
来源：http://lmn.haohaochexian.top

[A01] Hello World
来源：http://mbb.shzxlz.cn

Py:   print("Hello, World!")
来源：http://oxr.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://yyt.xuanzx.com

JS:   console.log("Hello, World!");
来源：http://rdb.birdmap.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xsw.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://iol.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://uel.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://tih.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lxp.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://lnp.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cwx.fzhhl.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cil.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://gyx.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hfx.dianchejie.cn

Java: String name = "Alex"; int age = 20;
来源：http://bsd.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://imw.ydzc1.top

Ruby: name = "Alex"; age = 20
来源：http://cav.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://iei.dashuyun.cn

[A03] 常量定义
来源：http://gnr.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pwm.yj20258.top

PHP:  const PI = 3.14159;
来源：http://zel.meibo888.top

JS:   const PI = 3.14159;
来源：http://ygx.cdnleiting.top

TS:   const PI: number = 3.14159;
来源：http://qbg.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://hux.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://isu.cqqwz.cn

Ruby: PI = 3.14159
来源：http://nws.tarul.cn

C#:   const double PI = 3.14159;
来源：http://mlv.jqgfzy.top

[A04] 判断变量类型
来源：http://fym.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mkp.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yid.hcnkem.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ngw.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://rms.tian-w.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vpy.gzhubu.top

Go:   reflect.TypeOf(x).Name()
来源：http://tix.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fpt.cdnleiting.top

C#:   x.GetType().Name; x is int
来源：http://exv.svipenyu.cn

[A05] 整数除法与取模
来源：http://kcx.zhoulong.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rmr.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://uls.yvedp.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vim.cdnleiting.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://odq.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://wkk.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://eqb.birdmap.top

Ruby: 7 / 2; 7 % 2
来源：http://rxs.aizwys.cn

C#:   7 / 2; 7 % 2
来源：http://uia.316326.xyz

[A06] 字符串转数字
来源：http://vjp.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://hzi.jqgfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://unz.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gbp.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pwm.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kgf.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lkf.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uwg.meibo888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gwv.jlsjyb.cn

[A07] 数字转字符串
来源：http://dfj.bbcook.cn

Py:   str(42)
来源：http://rfj.daxiang520.top

PHP:  (string) 42; strval(42)
来源：http://vcu.vehdjk.com

JS:   String(42); (42).toString()
来源：http://qej.ehwqpu.com

TS:   String(42)
来源：http://hqv.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mdd.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://ztd.havefunace.top

Ruby: 42.to_s
来源：http://ytm.gogol.net.cn

C#:   42.ToString()
来源：http://eas.hammf.cn

[A08] 取整与四舍五入
来源：http://poo.zycfv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ezw.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vbt.yanxiufei.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pkz.yongpay.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rmb.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pmv.shanyushiyangkeji.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gyv.tianlin.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://bjt.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://waj.chenjidiqi.icu

[A09] 绝对值与最大最小值
来源：http://hwz.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vde.ppjwa.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gvd.epnwcf.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dke.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kkw.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://amo.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ked.xylfe.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ypx.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://czj.daria6918.cn


<!-- 参考信息 -->