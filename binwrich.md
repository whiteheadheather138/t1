代发 wailian999

[U65] PHP：会话
来源：http://fwf.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hwr.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://nfa.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zqi.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://woz.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dac.xziqi.cn

[U68] PHP：PDO 连接
来源：http://lij.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hju.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://kel.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dzk.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://hgk.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vvq.hnqzz.top

[U71] PHP：抛出异常
来源：http://cxf.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://czu.fktsv.cn

[U72] PHP：写错误日志
来源：http://emf.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://ite.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://lpz.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://mkd.pycfn.com

[U74] PHP：读取环境变量
来源：http://xas.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://ohh.wangdashe.top

[U75] PHP：依赖注入
来源：http://wfa.fzhhl.top

composer require psr/container
来源：http://fwf.gogol.net.cn

[U76] PHP：简单路由
来源：http://prr.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jpp.cdnleiting.top

[U77] PHP：模板渲染
来源：http://tqx.zdbjq.cn

composer require twig/twig
来源：http://twc.zycfv.cn

[U78] PHP：单元测试
来源：http://kxr.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://pxx.sjlbkw.cn

[U79] PHP：静态分析
来源：http://dyv.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://rbe.xuanzx.com

[U80] PHP：代码规范修复
来源：http://uwf.zhijiandao.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lly.bjfxy.top

[U81] JS：初始化项目
来源：http://tjt.nanxinkj.top

npm init -y;  npm i express
来源：http://flc.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://wrg.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wto.ydjk.org.cn

[U83] JS：ES Module 导入导出
来源：http://kkv.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://fqk.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://ayz.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://jre.gaohongyu789.top

[U85] JS：可选链
来源：http://gdt.ppjwa.cn

a?.b?.c
来源：http://fgx.yueranfly.top

[U86] JS：空值合并
来源：http://skq.zhijiandao.cn

a ?? b
来源：http://fte.hfpthk.cn

[U87] JS：解构默认值
来源：http://phy.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://urb.svipenyu.cn

[U88] JS：对象展开合并
来源：http://bvc.redwolf501.top

{ ...a, ...b }
来源：http://pdq.sufxvd.cn

[U89] JS：数组去重
来源：http://smi.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://qlt.zdqjudy.top

[U90] JS：数字数组排序
来源：http://erq.chenjidiqi.icu

[...arr].sort((a, b) => a - b)
来源：http://ipd.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://wbm.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yiq.cqqwz.cn

[U92] JS：深拷贝
来源：http://kca.jinqigufen.top

structuredClone(obj)
来源：http://hgb.hysaishi.cn

[U93] JS：模板字符串
来源：http://lfv.316326.xyz

`共 ${n} 条`
来源：http://ntl.nanxuanxn.top

[U94] JS：箭头函数
来源：http://olx.jinqigfzy.top

const double = x => x * 2;
来源：http://opl.yj20258.top

[U95] JS：Promise 包装
来源：http://xck.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://ryk.yueranfly.top

[U96] JS：async/await 与异常
来源：http://fgs.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lvg.haohaochexian.top

[U97] JS：并发请求
来源：http://hbl.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lcj.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://bas.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gxs.yueranfly.top

[U99] JS：事件监听
来源：http://khd.52xcode.cn

el.addEventListener("click", e => {})
来源：http://sxa.yj20258888.top

[U100] JS：DOM 查询
来源：http://pps.gzhubu.top

document.querySelector(".item")
来源：http://dpk.ydzc1.top

[U101] JS：classList 操作
来源：http://fup.nanxuanxn.top

el.classList.toggle("active")
来源：http://pic.tarul.cn

[U102] JS：本地存储
来源：http://dgu.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nuf.cqqwz.cn

[U103] JS：定时器
来源：http://rja.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wzc.kuanghao11.cn

[U104] JS：防抖
来源：http://tkh.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cce.uphjek.com

[U105] JS：节流
来源：http://utz.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bec.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://yfx.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xjg.jlsjyb.cn

[U107] JS：数字千分位
来源：http://ylx.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rff.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://azn.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cuo.yongpay.top

[U109] JS：数组分组
来源：http://tfq.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://ewa.tianlin.xyz

[U110] JS：数组分块
来源：http://bhn.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nhf.redwolf501.top

[U111] JS：对象转 Map
来源：http://xut.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://pfl.zhongyouzk.top

[U112] JS：字符串补位
来源：http://nih.fehbvm.com

"7".padStart(3, "0")
来源：http://ewb.havefunace.top

[U113] JS：正则替换全部
来源：http://bga.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://rnx.yuxming.cn

[U114] JS：JSON 深比较
来源：http://cgd.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://svz.daxiang520.top

[U115] JS：生成 UUID
来源：http://ggg.guannengcc.top

crypto.randomUUID()
来源：http://doh.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://yng.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://buc.jianghu66.top

[U117] JS：单元测试
来源：http://rcx.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://dsm.svipenyu.cn

[U118] JS：开发服务器
来源：http://lww.hfpthk.cn

npm i -D vite;  npx vite
来源：http://ueb.yj202588.top

[U119] JS：生产构建
来源：http://lfn.dashuyun.cn

npx vite build
来源：http://jfz.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://tdb.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://rcx.pycfn.com

================================================================================
来源：http://hjl.zhixingplan.top

统计汇总
来源：http://xyp.fanxiaobao.xyz

================================================================================
来源：http://fvf.tanke756.top

按语言统计（条）：
来源：http://cna.shangyingyoupin.top

Python ......... 252
来源：http://klz.sufxvd.cn

PHP ............ 252
来源：http://zqc.svipenyu.cn

JavaScript ..... 252
来源：http://dgv.bbcook.cn

TypeScript ..... 212
来源：http://xad.sweek.top

Java ........... 212
来源：http://ius.jyoumei.cn

Go ............. 212
来源：http://cji.cdnleiting.top

Ruby ........... 212
来源：http://gwv.yonumen.top

C# ............. 212
来源：http://eoz.ctjpmb.com

C .............. 30
来源：http://kpb.hongshengwenyu.top

C++ ............ 30
来源：http://ple.ywan-chungtsiang.top

SQL ............ 90
来源：http://kec.cqqwz.cn

Bash ........... 80
来源：http://lmf.andypj.xyz

Kotlin ......... 15
来源：http://uui.hnxiangtu.top

Swift .......... 15
来源：http://tby.jinqigufen.top

Lua ............ 10
来源：http://jwu.epnwcf.com

Perl ........... 10
来源：http://azu.hysaishi.cn

Scala .......... 10
来源：http://cpl.jqgfzy.top

------------------------------------
来源：http://cqz.jqgufenzy.top

合计 ........... 2106 条
来源：http://ttd.nwbrower.top

按章节统计：
来源：http://odb.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zpq.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gve.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://adm.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bwg.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uhb.feifeiyinyue.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ddp.cashguo.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rar.daria6918.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://twt.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mvh.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xnv.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://brf.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lzg.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xdx.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cwb.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bql.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hws.tanke756.top

Q SQL 专题                              90
来源：http://kmx.zhixingplan.top

R Bash 专题                             80
来源：http://wba.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://gcb.jiagoushi.top

T 其他语言补充                          60
来源：http://mes.havefunace.top

U 高频实用片段                         120
来源：http://wzl.cucudq.cn

------------------------------------
来源：http://iib.ydzc1.top

合计                                  2106 条
来源：http://oda.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://got.ctjpmb.com

使用提醒
来源：http://vyb.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://abt.daria6918.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dyh.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sxa.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gpu.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lpo.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hbl.hnxiangtu.top

—— 文件结束 ——
来源：http://doo.smart0.xyz

================================================================================
来源：http://dcc.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://aki.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://sgj.andypj.xyz

================================================================================
来源：http://ofd.jinyuanbaomall.cn

【收录内容】
来源：http://mlw.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://rca.pengpengdd.cyou

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fsx.svipenyu.cn

SQL · Bash · C · C++
来源：http://hjt.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ocs.tanke756.top

【使用说明】
来源：http://wud.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cmq.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://txd.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wwa.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qho.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zfr.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wdm.nanxuanxn.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jni.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ubw.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://thq.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lbp.tarul.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mvm.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qgo.yuxming.cn

【文件统计】
来源：http://kah.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hmo.shuidangran.top

--------------------------------------------------------------------------------
来源：http://ddo.gzhubu.top

目  录
来源：http://sfd.aizwys.cn

--------------------------------------------------------------------------------
来源：http://ndv.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cvq.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xjm.gotoacloud.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dyp.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vkq.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://brq.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://imn.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yvu.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ibn.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sbq.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kgk.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dmc.guowangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://msn.ehwqpu.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://flv.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vyt.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bxa.jqgufenzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jzs.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jvw.hcnkem.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://cme.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bzg.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zka.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zcs.uphjek.com

================================================================================
来源：http://klx.daria6918.cn

A. 基础语法与类型
来源：http://sir.jinghuilouyu.cn

================================================================================
来源：http://ewj.sweek.top

[A01] Hello World
来源：http://bxp.zycfv.cn

Py:   print("Hello, World!")
来源：http://vfz.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://wim.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://npl.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hxl.jqgufenzy.top

Java: System.out.println("Hello, World!");
来源：http://vga.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://cwu.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://ghw.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://pmj.hysaishi.cn

[A02] 变量声明与赋值
来源：http://gjp.xziqi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gck.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dki.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://wll.52xcode.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://naw.tanke756.top

Java: String name = "Alex"; int age = 20;
来源：http://kjz.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://pcd.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://chs.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://vbj.shangyingyoupin.top

[A03] 常量定义
来源：http://kfb.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sej.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://ovj.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://bbz.yanxiufei.cn

TS:   const PI: number = 3.14159;
来源：http://tcs.feifeiyinyue.top

Java: static final double PI = 3.14159;
来源：http://sru.mhx1999.top

Go:   const PI = 3.14159
来源：http://lpi.dashuyun.cn

Ruby: PI = 3.14159
来源：http://axz.yj202588.top

C#:   const double PI = 3.14159;
来源：http://byt.tanke756.top

[A04] 判断变量类型
来源：http://ght.zdqjudy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wte.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cen.hongshengwenyu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://woc.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://vbs.uphjek.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wxv.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://oua.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bzc.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://qwk.zdbjq.cn

[A05] 整数除法与取模
来源：http://gyk.jinqigfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zux.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rpx.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hjg.hnqzz.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://try.316326.xyz

Java: 7 / 2; 7 % 2
来源：http://wzt.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://ndh.cucudq.cn

Ruby: 7 / 2; 7 % 2
来源：http://fuk.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://emw.daria6918.cn

[A06] 字符串转数字
来源：http://jts.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://gzi.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://coc.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ilo.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ole.zycfv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tyj.cucudq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hhg.zhengqikj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gzm.guowangkeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sul.svipenyu.cn

[A07] 数字转字符串
来源：http://kjr.hammf.cn

Py:   str(42)
来源：http://src.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://xdi.jianghu66.top

JS:   String(42); (42).toString()
来源：http://adb.haohaochexian.top

TS:   String(42)
来源：http://vvl.redwolf501.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tyt.ywan-chungtsiang.top

Go:   strconv.Itoa(42)
来源：http://keb.zhengqikj.top

Ruby: 42.to_s
来源：http://uls.zhixingplan.top

C#:   42.ToString()
来源：http://uhj.hcnkem.com

[A08] 取整与四舍五入
来源：http://jqv.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cov.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rxv.hysaishi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://abs.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zku.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xlx.fengsongda.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kds.zhiwuduotai.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dqk.hesvh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ltm.yj20258.top

[A09] 绝对值与最大最小值
来源：http://uaf.zhijiandao.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rsm.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tst.hcnkem.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ahi.nanxuanxn.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ena.nwbrower.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gek.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://okl.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://duw.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vlj.jinqigfzy.top


<!-- 参考信息 -->