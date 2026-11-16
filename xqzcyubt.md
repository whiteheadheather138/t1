代发 wailian999

[U63] PHP：文件读写
来源：http://uzf.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xyi.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://lpt.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://opu.shuidangran.top

[U65] PHP：会话
来源：http://cud.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://opv.sjlbkw.cn

[U66] PHP：设置 Cookie
来源：http://fga.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eba.daxiang520.top

[U67] PHP：处理文件上传
来源：http://xul.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pow.fengsongda.top

[U68] PHP：PDO 连接
来源：http://haf.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mky.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://asw.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bbc.iojbl.cn

[U70] PHP：PDO 事务
来源：http://aev.vqdsnc.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ppu.daria6918.cn

[U71] PHP：抛出异常
来源：http://gnm.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://grl.sweek.top

[U72] PHP：写错误日志
来源：http://zqv.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://prl.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://cgy.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://aep.jianghu66.top

[U74] PHP：读取环境变量
来源：http://doi.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://tgp.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://tsw.hysaishi.cn

composer require psr/container
来源：http://ndw.jinqigufen.top

[U76] PHP：简单路由
来源：http://ehs.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iuz.cheryme.top

[U77] PHP：模板渲染
来源：http://hll.ydjk.org.cn

composer require twig/twig
来源：http://jwd.sxryk.cn

[U78] PHP：单元测试
来源：http://hml.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://fny.ivvv.top

[U79] PHP：静态分析
来源：http://nkz.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://fdr.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://odv.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fes.svipenyu.cn

[U81] JS：初始化项目
来源：http://ljx.chenjidiqi.icu

npm init -y;  npm i express
来源：http://rmy.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://did.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qrk.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://rlj.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://nsp.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://wsc.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://cms.vqdsnc.cn

[U85] JS：可选链
来源：http://gnu.gaohongyu789.top

a?.b?.c
来源：http://tdy.yj20258.top

[U86] JS：空值合并
来源：http://nlo.fktsv.cn

a ?? b
来源：http://gcy.birdmap.top

[U87] JS：解构默认值
来源：http://bas.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://iol.zhixingplan.top

[U88] JS：对象展开合并
来源：http://nzq.yj202588.top

{ ...a, ...b }
来源：http://sox.pengpengdd.cyou

[U89] JS：数组去重
来源：http://vql.daria6918.cn

[...new Set(arr)]
来源：http://zvf.shuidangran.top

[U90] JS：数字数组排序
来源：http://wxl.gotoacloud.top

[...arr].sort((a, b) => a - b)
来源：http://wtk.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://uth.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rmg.jqgufenzy.top

[U92] JS：深拷贝
来源：http://lga.jinyuanbaomall.cn

structuredClone(obj)
来源：http://ldb.yongpay.top

[U93] JS：模板字符串
来源：http://fbh.zhoulong.xyz

`共 ${n} 条`
来源：http://kit.gzhubu.top

[U94] JS：箭头函数
来源：http://pti.tanke756.top

const double = x => x * 2;
来源：http://mij.ivvv.top

[U95] JS：Promise 包装
来源：http://rnm.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://ojz.hammf.cn

[U96] JS：async/await 与异常
来源：http://cld.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://llo.gaohongyu789.top

[U97] JS：并发请求
来源：http://ztt.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kkz.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://drh.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://olk.pengpengdd.cyou

[U99] JS：事件监听
来源：http://luo.yj20258.top

el.addEventListener("click", e => {})
来源：http://nhe.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://fwn.sxryk.cn

document.querySelector(".item")
来源：http://pfl.jyoumei.cn

[U101] JS：classList 操作
来源：http://woq.feifeiyinyue.top

el.classList.toggle("active")
来源：http://rkv.jqgufenzy.top

[U102] JS：本地存储
来源：http://juk.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oru.0kj1m.cn

[U103] JS：定时器
来源：http://mdu.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yyr.zdqjudy.top

[U104] JS：防抖
来源：http://syf.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wry.zycfv.cn

[U105] JS：节流
来源：http://jyi.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://urd.hywenlv.cn

[U106] JS：日期格式化
来源：http://rhi.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://clo.birdmap.top

[U107] JS：数字千分位
来源：http://qgv.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cii.hongshengwenyu.top

[U108] JS：随机整数
来源：http://epu.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xyf.hfpthk.cn

[U109] JS：数组分组
来源：http://gux.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://rfw.jyoumei.cn

[U110] JS：数组分块
来源：http://hoq.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://muy.aibaodan.cn

[U111] JS：对象转 Map
来源：http://ezd.cashguo.top

new Map(Object.entries(obj))
来源：http://ghl.fktsv.cn

[U112] JS：字符串补位
来源：http://sgq.cucudq.cn

"7".padStart(3, "0")
来源：http://qsp.haohaochexian.top

[U113] JS：正则替换全部
来源：http://yoh.yvedp.cn

s.replaceAll("a", "b")
来源：http://bqs.zycfv.cn

[U114] JS：JSON 深比较
来源：http://amw.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wdh.jyoumei.cn

[U115] JS：生成 UUID
来源：http://vdy.yj20258888.top

crypto.randomUUID()
来源：http://wpj.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://lbe.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://niq.cashguo.top

[U117] JS：单元测试
来源：http://ayq.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://yyc.bjfxy.top

[U118] JS：开发服务器
来源：http://hbu.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://ndg.xylfe.cn

[U119] JS：生产构建
来源：http://rqq.aizwys.cn

npx vite build
来源：http://ftm.chenlongwang.top

[U120] JS：读取环境变量（Vite）
来源：http://inj.hammf.cn

import.meta.env.VITE_API_URL
来源：http://xrv.gzhubu.top

================================================================================
来源：http://pbp.hongshengwenyu.top

统计汇总
来源：http://sao.cashguo.top

================================================================================
来源：http://dja.yangfankeji.com

按语言统计（条）：
来源：http://lnb.dianchejie.cn

Python ......... 252
来源：http://zgz.ivvv.top

PHP ............ 252
来源：http://vvq.fzhhl.top

JavaScript ..... 252
来源：http://tpy.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://auj.ivvv.top

Java ........... 212
来源：http://xpp.svipenyu.cn

Go ............. 212
来源：http://uji.yj202588.top

Ruby ........... 212
来源：http://jxm.jinqigufen.top

C# ............. 212
来源：http://tjf.ivvv.top

C .............. 30
来源：http://kqi.andypj.xyz

C++ ............ 30
来源：http://xfa.gogol.net.cn

SQL ............ 90
来源：http://lsv.shanyushiyangtech.top

Bash ........... 80
来源：http://evr.gogol.net.cn

Kotlin ......... 15
来源：http://gbq.sysykeji.top

Swift .......... 15
来源：http://nzq.jinqigufen.top

Lua ............ 10
来源：http://bgj.zhengqikj.top

Perl ........... 10
来源：http://vtz.hfpthk.cn

Scala .......... 10
来源：http://tsc.dianchejie.cn

------------------------------------
来源：http://qzv.cheryme.top

合计 ........... 2106 条
来源：http://dmf.yongpay.top

按章节统计：
来源：http://pxu.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gty.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jfl.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tia.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://epr.zhoulong.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ubg.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mmj.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pmd.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nty.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://txc.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ipu.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xqx.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wuv.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://btd.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bpz.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hlt.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tiz.sweek.top

Q SQL 专题                              90
来源：http://xdg.vehdjk.com

R Bash 专题                             80
来源：http://xih.daxiang520.top

S C / C++ 专题                          60
来源：http://uua.chenzaomai.com

T 其他语言补充                          60
来源：http://bqe.yongpay.top

U 高频实用片段                         120
来源：http://adm.hfpthk.cn

------------------------------------
来源：http://euz.uphjek.com

合计                                  2106 条
来源：http://jnp.nwbrower.top

--------------------------------------------------------------------------------
来源：http://iuy.cqqwz.cn

使用提醒
来源：http://dha.jianghu66.top

--------------------------------------------------------------------------------
来源：http://gin.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wpu.xuetiantiany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zuj.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zmx.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://osb.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gcs.vqdsnc.cn

—— 文件结束 ——
来源：http://rtq.yuxming.cn

================================================================================
来源：http://jdl.yj20258.top

程序语言常见例子速查手册（2024 版）
来源：http://exh.yfazqb.com

Common Programming Examples Cheat Book
来源：http://mmd.yuxming.cn

================================================================================
来源：http://lln.tarul.cn

【收录内容】
来源：http://umj.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jrc.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ykl.9152youxi.cn

SQL · Bash · C · C++
来源：http://dsx.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lzw.zdbjq.cn

【使用说明】
来源：http://srt.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bzc.pycfn.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://upi.cucudq.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kke.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zgj.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fbs.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://spo.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jpz.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kai.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mdw.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qhx.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ehn.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tqp.jinqigufen.top

【文件统计】
来源：http://yqu.ehwqpu.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jck.yfazqb.com

--------------------------------------------------------------------------------
来源：http://jxe.yvedp.cn

目  录
来源：http://aaq.hesvh.cn

--------------------------------------------------------------------------------
来源：http://jtk.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ymh.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://olj.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zkr.yuanzhike.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://prm.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xwe.0kj1m.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xac.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vkm.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fif.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mvb.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iew.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zhq.jqgufenzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://otb.yuxming.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qxf.wangshuangyany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zeb.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://glu.xziqi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wvr.fzhhl.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://oyo.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tqb.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dpg.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xue.yongpay.top

================================================================================
来源：http://yzf.chenzaomai.com

A. 基础语法与类型
来源：http://jks.meibo888.top

================================================================================
来源：http://ezm.chenlongwang.top

[A01] Hello World
来源：http://sjz.shuidangran.top

Py:   print("Hello, World!")
来源：http://fst.ivvv.top

PHP:  echo "Hello, World!";
来源：http://xrz.nwbrower.top

JS:   console.log("Hello, World!");
来源：http://nxi.jlsjyb.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zyh.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://zng.yj202588.top

Go:   fmt.Println("Hello, World!")
来源：http://bfr.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://ctu.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://adb.guowangkeji.top

[A02] 变量声明与赋值
来源：http://tci.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://btu.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hzj.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://end.ctjpmb.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sph.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://ilt.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://ngm.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://xur.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://yzd.vqdsnc.cn

[A03] 常量定义
来源：http://ntq.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tju.yonumen.top

PHP:  const PI = 3.14159;
来源：http://etr.sweek.top

JS:   const PI = 3.14159;
来源：http://opc.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://bvs.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://txy.shzxlz.cn

Go:   const PI = 3.14159
来源：http://ytb.shuidangran.top

Ruby: PI = 3.14159
来源：http://riz.zhijiandao.cn

C#:   const double PI = 3.14159;
来源：http://rmc.redwolf501.top

[A04] 判断变量类型
来源：http://nlw.mhx1999.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://swb.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yjg.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gvu.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://mpp.c1oappe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cif.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rxo.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ljp.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://ody.zhijiandao.cn

[A05] 整数除法与取模
来源：http://mmt.epnwcf.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pre.zhaomingkeji.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://jzv.yj20258.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sob.52xcode.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vjx.dashuyun.cn

Java: 7 / 2; 7 % 2
来源：http://qgo.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://ubc.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://vlj.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://orw.hfpthk.cn

[A06] 字符串转数字
来源：http://gpq.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://zaz.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hkf.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tgt.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://aha.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hny.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://arn.zdqjudy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qmj.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pko.hnqzz.top

[A07] 数字转字符串
来源：http://cli.guannengcc.top

Py:   str(42)
来源：http://uag.ydjk.org.cn

PHP:  (string) 42; strval(42)
来源：http://zev.fehbvm.com

JS:   String(42); (42).toString()
来源：http://gin.jyoumei.cn

TS:   String(42)
来源：http://eal.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://pqr.daria6918.cn

Go:   strconv.Itoa(42)
来源：http://zxr.wangdashe.top

Ruby: 42.to_s
来源：http://hky.redwolf501.top

C#:   42.ToString()
来源：http://jge.316326.xyz

[A08] 取整与四舍五入
来源：http://zxv.shanyushiyangtech.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iod.yj20258888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uis.hfpthk.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ymi.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qfs.nanxinkj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gnd.dashuyun.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xku.xylfe.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rvo.wangshuangyany.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wom.zhixingplan.top

[A09] 绝对值与最大最小值
来源：http://jhu.hysaishi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jwy.vehdjk.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xnm.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ttp.yongpay.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wqv.bjfxy.top


<!-- 参考信息 -->