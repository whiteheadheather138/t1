代发 wailian999

[U63] PHP：文件读写
来源：http://sco.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cio.gogol.net.cn

[U64] PHP：目录遍历
来源：http://gie.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://yva.hnxiangtu.top

[U65] PHP：会话
来源：http://jei.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xak.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://cer.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jiz.tanke756.top

[U67] PHP：处理文件上传
来源：http://abr.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rzf.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://epn.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gnd.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://fda.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rey.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://foi.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ngq.tanke756.top

[U71] PHP：抛出异常
来源：http://goj.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://xvh.52xcode.cn

[U72] PHP：写错误日志
来源：http://nmf.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://qzn.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://yfj.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://cah.jianghu66.top

[U74] PHP：读取环境变量
来源：http://uuo.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://fqj.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://wpc.smart0.xyz

composer require psr/container
来源：http://pny.redwolf501.top

[U76] PHP：简单路由
来源：http://gef.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://seb.gzhubu.top

[U77] PHP：模板渲染
来源：http://xif.ehwqpu.com

composer require twig/twig
来源：http://cae.ydzc1.top

[U78] PHP：单元测试
来源：http://qnp.havefunace.top

composer require --dev phpunit/phpunit
来源：http://zvg.smart0.xyz

[U79] PHP：静态分析
来源：http://atu.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://mxd.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://nkd.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://brt.yongpay.top

[U81] JS：初始化项目
来源：http://ssl.cheryme.top

npm init -y;  npm i express
来源：http://xlo.sweek.top

[U82] JS：package.json 脚本
来源：http://onx.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lbz.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://axf.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://qgz.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://rci.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://pjf.havefunace.top

[U85] JS：可选链
来源：http://vkt.shangyingyoupin.top

a?.b?.c
来源：http://yhe.dianchejie.cn

[U86] JS：空值合并
来源：http://xgq.hnxiangtu.top

a ?? b
来源：http://lzl.gaohongyu789.top

[U87] JS：解构默认值
来源：http://bob.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://hgn.fengsongda.top

[U88] JS：对象展开合并
来源：http://mvg.cheryme.top

{ ...a, ...b }
来源：http://fxn.shzxlz.cn

[U89] JS：数组去重
来源：http://zrl.jyoumei.cn

[...new Set(arr)]
来源：http://wnk.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://tbi.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://fxg.c1oappe.top

[U91] JS：对象键值遍历
来源：http://jhc.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ueu.andypj.xyz

[U92] JS：深拷贝
来源：http://gfi.bjfxy.top

structuredClone(obj)
来源：http://syu.hesvh.cn

[U93] JS：模板字符串
来源：http://dms.ppjwa.cn

`共 ${n} 条`
来源：http://ool.hnqzz.top

[U94] JS：箭头函数
来源：http://sob.yueranfly.top

const double = x => x * 2;
来源：http://azs.zdbjq.cn

[U95] JS：Promise 包装
来源：http://dfs.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://gdg.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://yoc.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ykt.sysykeji.top

[U97] JS：并发请求
来源：http://jki.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vbc.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://fus.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gul.ywan-chungtsiang.top

[U99] JS：事件监听
来源：http://mdh.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://fkz.cucudq.cn

[U100] JS：DOM 查询
来源：http://czr.xuetiantiany.cn

document.querySelector(".item")
来源：http://xvz.birdmap.top

[U101] JS：classList 操作
来源：http://vby.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://fwo.zhiwuduotai.top

[U102] JS：本地存储
来源：http://iwx.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fxm.xuetiantiany.cn

[U103] JS：定时器
来源：http://eun.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jdx.snrcjt.cn

[U104] JS：防抖
来源：http://rez.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuw.yuxming.cn

[U105] JS：节流
来源：http://rui.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fal.yj20258.top

[U106] JS：日期格式化
来源：http://ztx.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oni.zhixingplan.top

[U107] JS：数字千分位
来源：http://ifd.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://azm.hesvh.cn

[U108] JS：随机整数
来源：http://qqd.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ppg.ydzc1.top

[U109] JS：数组分组
来源：http://xum.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://vmn.fehbvm.com

[U110] JS：数组分块
来源：http://dkt.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dci.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://qff.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://ahd.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://piv.nanxuanxn.top

"7".padStart(3, "0")
来源：http://exh.redwolf501.top

[U113] JS：正则替换全部
来源：http://seg.aizwys.cn

s.replaceAll("a", "b")
来源：http://hvr.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://sdo.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jxp.yfazqb.com

[U115] JS：生成 UUID
来源：http://gbo.daxiang520.top

crypto.randomUUID()
来源：http://wwq.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://dcu.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://esx.jinqigufen.top

[U117] JS：单元测试
来源：http://znj.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://say.sjlbkw.cn

[U118] JS：开发服务器
来源：http://xqw.birdmap.top

npm i -D vite;  npx vite
来源：http://fmz.kuanghao11.cn

[U119] JS：生产构建
来源：http://vbu.gzhubu.top

npx vite build
来源：http://rgg.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://tqu.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://fyh.mhx1999.top

================================================================================
来源：http://tzj.kuanghao11.cn

统计汇总
来源：http://puk.yanxiufei.cn

================================================================================
来源：http://pjp.daxiang520.top

按语言统计（条）：
来源：http://oma.iojbl.cn

Python ......... 252
来源：http://scw.hongshengwenyu.top

PHP ............ 252
来源：http://pth.0kj1m.cn

JavaScript ..... 252
来源：http://kws.52xcode.cn

TypeScript ..... 212
来源：http://yeh.cucudq.cn

Java ........... 212
来源：http://xlp.yj20258.top

Go ............. 212
来源：http://tnu.dashuyun.cn

Ruby ........... 212
来源：http://nww.jyoumei.cn

C# ............. 212
来源：http://dno.quarkkingdee.top

C .............. 30
来源：http://qac.cqqwz.cn

C++ ............ 30
来源：http://rrp.cdnleiting.top

SQL ............ 90
来源：http://zqh.pengpengdd.cyou

Bash ........... 80
来源：http://aow.xylfe.cn

Kotlin ......... 15
来源：http://bxf.yj20258.top

Swift .......... 15
来源：http://lqv.bjfxy.top

Lua ............ 10
来源：http://wdn.chenzaomai.com

Perl ........... 10
来源：http://wnb.tarul.cn

Scala .......... 10
来源：http://gch.52xcode.cn

------------------------------------
来源：http://eiz.hnqzz.top

合计 ........... 2106 条
来源：http://beg.jinqigufen.top

按章节统计：
来源：http://vcg.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pym.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://naz.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ajk.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eke.dashuyun.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iog.nanxuanxn.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nbe.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://epy.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ogc.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://avk.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pbm.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bkg.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://itc.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://afn.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zxe.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://efd.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://grt.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://tho.ivvv.top

R Bash 专题                             80
来源：http://wyg.meibo888.top

S C / C++ 专题                          60
来源：http://diy.feifeiyinyue.top

T 其他语言补充                          60
来源：http://ehj.kuanghao11.cn

U 高频实用片段                         120
来源：http://saz.meibo888.top

------------------------------------
来源：http://tyx.yvedp.cn

合计                                  2106 条
来源：http://jrl.fengsongda.top

--------------------------------------------------------------------------------
来源：http://ubt.zycfv.cn

使用提醒
来源：http://qil.yvedp.cn

--------------------------------------------------------------------------------
来源：http://yyp.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sxo.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qjf.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ebm.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zuh.yj202588.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bmz.bbcook.cn

—— 文件结束 ——
来源：http://xsu.yfazqb.com

================================================================================
来源：http://lzg.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://ple.daxiang520.top

Common Programming Examples Cheat Book
来源：http://qpk.xziqi.cn

================================================================================
来源：http://sdv.yongpay.top

【收录内容】
来源：http://nrq.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kns.ywan-chungtsiang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lfb.gzhubu.top

SQL · Bash · C · C++
来源：http://xzv.hcnkem.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dlr.uphjek.com

【使用说明】
来源：http://snd.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tzu.sxryk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gwm.dianchejie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nro.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://umq.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://mmj.zhixingplan.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wsw.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tmn.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ykb.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jvo.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mzf.ydjk.org.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qto.wangshuangyany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oae.guannengcc.top

【文件统计】
来源：http://aem.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uux.sweek.top

--------------------------------------------------------------------------------
来源：http://trr.kuanghao11.cn

目  录
来源：http://sng.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://gpf.daxiang520.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eqj.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://psv.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://alm.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nmw.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mve.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kws.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ocs.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wqf.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://urg.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oei.aizwys.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ajw.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uru.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jha.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wmb.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lbr.zhongyouzk.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sub.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lgy.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mvj.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cre.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bgr.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ias.zhijiandao.cn

================================================================================
来源：http://znv.xuetiantiany.cn

A. 基础语法与类型
来源：http://sls.0kj1m.cn

================================================================================
来源：http://wxg.cheryme.top

[A01] Hello World
来源：http://mos.tanke756.top

Py:   print("Hello, World!")
来源：http://nas.wangshuangyany.cn

PHP:  echo "Hello, World!";
来源：http://fan.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://jmc.yangfankeji.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tmq.jiagoushi.top

Java: System.out.println("Hello, World!");
来源：http://ica.xuanzx.com

Go:   fmt.Println("Hello, World!")
来源：http://lqj.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://fvw.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://cza.xylfe.cn

[A02] 变量声明与赋值
来源：http://zdv.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mas.zdqjudy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xvl.ydjk.org.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zgw.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zbs.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://bab.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://xpm.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://axd.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://hga.xuanzx.com

[A03] 常量定义
来源：http://zoz.gogol.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qpr.9152youxi.cn

PHP:  const PI = 3.14159;
来源：http://zuy.shangyingyoupin.top

JS:   const PI = 3.14159;
来源：http://hlp.gzhubu.top

TS:   const PI: number = 3.14159;
来源：http://orf.nanxuanxn.top

Java: static final double PI = 3.14159;
来源：http://ngf.tanke756.top

Go:   const PI = 3.14159
来源：http://tzk.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://hcp.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://xgr.tian-w.cn

[A04] 判断变量类型
来源：http://bri.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://upy.hywenlv.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://twc.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jko.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://ktu.hammf.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xia.chenlongwang.top

Go:   reflect.TypeOf(x).Name()
来源：http://qhb.daria6918.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tqg.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://lvb.nanxinkj.top

[A05] 整数除法与取模
来源：http://knl.bjfxy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://piz.fehbvm.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://wep.yuanzhike.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gvg.fengsongda.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://syx.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://vlu.shanyushiyangtech.top

Go:   7 / 2; 7 % 2
来源：http://ubl.yonumen.top

Ruby: 7 / 2; 7 % 2
来源：http://ucl.cashguo.top

C#:   7 / 2; 7 % 2
来源：http://avm.smart0.xyz

[A06] 字符串转数字
来源：http://ycp.yueranfly.top

Py:   int("42"); float("3.14")
来源：http://ovb.svipenyu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fly.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pce.fzhhl.top

TS:   parseInt("42", 10); Number("42")
来源：http://wvc.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://plr.shangyingyoupin.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hgk.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iwc.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dyp.jinqigfzy.top

[A07] 数字转字符串
来源：http://ajp.dianchejie.cn

Py:   str(42)
来源：http://znm.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://vwi.c1oappe.top

JS:   String(42); (42).toString()
来源：http://afk.mhx1999.top

TS:   String(42)
来源：http://jib.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xuu.yongpay.top

Go:   strconv.Itoa(42)
来源：http://noa.hnqzz.top

Ruby: 42.to_s
来源：http://ukg.jqgfzy.top

C#:   42.ToString()
来源：http://uyi.jinqigfzy.top

[A08] 取整与四舍五入
来源：http://yrz.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yjt.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lng.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mzn.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mwg.chenlongwang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sdl.shzxlz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://did.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zch.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dif.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://xtm.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mfz.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://okm.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mpq.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ggh.ywan-chungtsiang.top


<!-- 参考信息 -->