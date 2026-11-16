代发 wailian999

[U63] PHP：文件读写
来源：http://dur.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bpu.c1oappe.top

[U64] PHP：目录遍历
来源：http://joz.dianchejie.cn

glob("dir/*.php");  scandir("dir");
来源：http://iyd.hfpthk.cn

[U65] PHP：会话
来源：http://sgb.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rqa.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://myt.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://szf.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://bhv.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iab.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://wri.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://stc.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://haw.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yrj.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://fxh.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lgi.havefunace.top

[U71] PHP：抛出异常
来源：http://jeb.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://wuv.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://thh.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://omj.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://sky.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://dbc.jinghuilouyu.cn

[U74] PHP：读取环境变量
来源：http://yel.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://ibd.yfazqb.com

[U75] PHP：依赖注入
来源：http://uxs.sxryk.cn

composer require psr/container
来源：http://lns.yfazqb.com

[U76] PHP：简单路由
来源：http://lqb.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lyy.hcnkem.com

[U77] PHP：模板渲染
来源：http://jbt.gogol.net.cn

composer require twig/twig
来源：http://upz.uphjek.com

[U78] PHP：单元测试
来源：http://xxy.birdmap.top

composer require --dev phpunit/phpunit
来源：http://ezq.ybcxt.top

[U79] PHP：静态分析
来源：http://nci.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://cjx.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://onv.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tcc.tianlin.xyz

[U81] JS：初始化项目
来源：http://rtc.hfpthk.cn

npm init -y;  npm i express
来源：http://pvw.yueranfly.top

[U82] JS：package.json 脚本
来源：http://tag.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nmd.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://iqd.shangyingyoupin.top

export const a = 1;  import { a } from "./m.js";
来源：http://fat.ydzc1.top

[U84] JS：CommonJS 写法
来源：http://yzy.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://kgg.quarkkingdee.top

[U85] JS：可选链
来源：http://gnu.daxiang520.top

a?.b?.c
来源：http://prl.meibo888.top

[U86] JS：空值合并
来源：http://qui.zhoulong.xyz

a ?? b
来源：http://ujf.ctjpmb.com

[U87] JS：解构默认值
来源：http://iya.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://sur.hesvh.cn

[U88] JS：对象展开合并
来源：http://ffp.zhijiandao.cn

{ ...a, ...b }
来源：http://tdd.yuxming.cn

[U89] JS：数组去重
来源：http://dje.redwolf501.top

[...new Set(arr)]
来源：http://xri.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://mxs.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://vdu.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://joy.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gvi.zdbjq.cn

[U92] JS：深拷贝
来源：http://hzu.ydjk.org.cn

structuredClone(obj)
来源：http://kjg.nanxinkj.top

[U93] JS：模板字符串
来源：http://epv.zhixingplan.top

`共 ${n} 条`
来源：http://hyi.yueranfly.top

[U94] JS：箭头函数
来源：http://yje.tanke756.top

const double = x => x * 2;
来源：http://lhd.zhixingplan.top

[U95] JS：Promise 包装
来源：http://dwn.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://oxj.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://bop.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vyp.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://pcw.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zgd.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://nsn.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://igm.gzhubu.top

[U99] JS：事件监听
来源：http://xqe.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://bmk.chenlongwang.top

[U100] JS：DOM 查询
来源：http://eto.nwbrower.top

document.querySelector(".item")
来源：http://prk.xinyue.icu

[U101] JS：classList 操作
来源：http://juj.52xcode.cn

el.classList.toggle("active")
来源：http://pfh.gaohongyu789.top

[U102] JS：本地存储
来源：http://ira.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://opo.ehwqpu.com

[U103] JS：定时器
来源：http://vmp.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jer.jqgfzy.top

[U104] JS：防抖
来源：http://uwh.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tfi.xuetiantiany.cn

[U105] JS：节流
来源：http://yii.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://scj.kuanghao11.cn

[U106] JS：日期格式化
来源：http://ahf.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fpw.shuidangran.top

[U107] JS：数字千分位
来源：http://fif.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uwv.jinqigufen.top

[U108] JS：随机整数
来源：http://rmn.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ajk.xinyue.icu

[U109] JS：数组分组
来源：http://vvi.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://pra.sjlbkw.cn

[U110] JS：数组分块
来源：http://rsv.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rey.xuetiantiany.cn

[U111] JS：对象转 Map
来源：http://oxl.jianghu66.top

new Map(Object.entries(obj))
来源：http://pki.nwbrower.top

[U112] JS：字符串补位
来源：http://qep.dashuyun.cn

"7".padStart(3, "0")
来源：http://nez.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://enn.dashuyun.cn

s.replaceAll("a", "b")
来源：http://agk.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://ofz.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://blg.jyoumei.cn

[U115] JS：生成 UUID
来源：http://nhh.gotoacloud.top

crypto.randomUUID()
来源：http://vbq.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://utv.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://poo.tanke756.top

[U117] JS：单元测试
来源：http://dvx.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://duc.xylfe.cn

[U118] JS：开发服务器
来源：http://wne.chenlongwang.top

npm i -D vite;  npx vite
来源：http://buj.gzhubu.top

[U119] JS：生产构建
来源：http://gqw.hywenlv.cn

npx vite build
来源：http://nes.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://xry.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://pcz.jyoumei.cn

================================================================================
来源：http://keq.xinyue.icu

统计汇总
来源：http://oaf.jqgufenzy.top

================================================================================
来源：http://oqz.birdmap.top

按语言统计（条）：
来源：http://gah.xziqi.cn

Python ......... 252
来源：http://dud.bbcook.cn

PHP ............ 252
来源：http://gpa.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://yor.gotoacloud.top

TypeScript ..... 212
来源：http://von.aizwys.cn

Java ........... 212
来源：http://lwv.aizwys.cn

Go ............. 212
来源：http://xgy.yonumen.top

Ruby ........... 212
来源：http://kfs.yj202588.top

C# ............. 212
来源：http://hoa.zhixingplan.top

C .............. 30
来源：http://xrc.yuanzhike.top

C++ ............ 30
来源：http://mqg.aibaodan.cn

SQL ............ 90
来源：http://nbm.pengpengdd.cyou

Bash ........... 80
来源：http://xby.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://qkv.zdbjq.cn

Swift .......... 15
来源：http://asa.hammf.cn

Lua ............ 10
来源：http://jbf.fktsv.cn

Perl ........... 10
来源：http://tjv.yj20258.top

Scala .......... 10
来源：http://dfp.zhengqikj.top

------------------------------------
来源：http://avo.feifeiyinyue.top

合计 ........... 2106 条
来源：http://nnl.gotoacloud.top

按章节统计：
来源：http://ajb.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://enq.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eib.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dji.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tmy.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://swd.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wpw.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://syw.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zib.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rzz.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://set.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wyy.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://whk.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://igv.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pma.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bbg.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dgx.chenlongwang.top

Q SQL 专题                              90
来源：http://iir.fzhhl.top

R Bash 专题                             80
来源：http://vdz.pycfn.com

S C / C++ 专题                          60
来源：http://las.cdnleiting.top

T 其他语言补充                          60
来源：http://kxo.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://hrq.pengpengdd.cyou

------------------------------------
来源：http://nfg.xinyue.icu

合计                                  2106 条
来源：http://iqa.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://cze.ydjk.org.cn

使用提醒
来源：http://cne.gzhubu.top

--------------------------------------------------------------------------------
来源：http://xqo.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://upo.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lzi.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qoj.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zfy.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cfu.ctjpmb.com

—— 文件结束 ——
来源：http://zxv.yj202588.top

================================================================================
来源：http://qdi.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://ews.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://osf.redwolf501.top

================================================================================
来源：http://hls.daria6918.cn

【收录内容】
来源：http://nha.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ocz.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://efy.jqgufenzy.top

SQL · Bash · C · C++
来源：http://biv.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cbe.daxiang520.top

【使用说明】
来源：http://lrt.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://inq.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://njb.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yvk.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wlr.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vwe.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lhh.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://upo.nanxinkj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ywa.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ibu.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hjl.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ugq.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lfe.hywenlv.cn

【文件统计】
来源：http://agw.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://utv.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://eaj.xuetiantiany.cn

目  录
来源：http://mcp.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://btv.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ypa.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tqe.nanxinkj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qde.bjfxy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oiq.xinyue.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ypr.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qql.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uli.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://org.daria6918.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xtu.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eiu.jqgufenzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pov.smart0.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ljo.gogol.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bma.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zsi.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ihb.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ngq.tian-w.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nxw.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://icp.zhixingplan.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pyu.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gen.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jmq.shzxlz.cn

================================================================================
来源：http://edz.yongpay.top

A. 基础语法与类型
来源：http://yid.dianchejie.cn

================================================================================
来源：http://lya.hammf.cn

[A01] Hello World
来源：http://hhe.yonumen.top

Py:   print("Hello, World!")
来源：http://ddk.quarkkingdee.top

PHP:  echo "Hello, World!";
来源：http://yvf.meibo888.top

JS:   console.log("Hello, World!");
来源：http://mik.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ycm.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://wnu.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://rtj.shuidangran.top

Ruby: puts "Hello, World!"
来源：http://oem.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tyf.tianlin.xyz

[A02] 变量声明与赋值
来源：http://hbn.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://syr.bbcook.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hls.zhengqikj.top

JS:   let name = "Alex"; const age = 20;
来源：http://pty.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lsn.sxryk.cn

Java: String name = "Alex"; int age = 20;
来源：http://ymc.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://lal.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://mfi.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zgt.zhixingplan.top

[A03] 常量定义
来源：http://gdl.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tbo.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://mbq.cdnleiting.top

JS:   const PI = 3.14159;
来源：http://lqg.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://tag.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://gjo.yangfankeji.com

Go:   const PI = 3.14159
来源：http://rji.hnqzz.top

Ruby: PI = 3.14159
来源：http://dgn.c1oappe.top

C#:   const double PI = 3.14159;
来源：http://ueg.zhoulong.xyz

[A04] 判断变量类型
来源：http://tqk.jinqigfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bvk.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iix.sysykeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jhc.hcnkem.com

TS:   typeof x; x instanceof Date
来源：http://nke.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ntv.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kuz.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://olp.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://zub.zhoulong.xyz

[A05] 整数除法与取模
来源：http://wnx.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qto.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://bzp.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uws.fzhhl.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yzu.zhoulong.xyz

Java: 7 / 2; 7 % 2
来源：http://xxc.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://iyg.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://nly.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://wbj.wangshuangyany.cn

[A06] 字符串转数字
来源：http://ncu.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://oaz.hongshengwenyu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xrd.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kns.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://vow.bbcook.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kwq.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://syn.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nry.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eur.xuanzx.com

[A07] 数字转字符串
来源：http://cyq.hammf.cn

Py:   str(42)
来源：http://vjo.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://lkn.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://ymn.ppjwa.cn

TS:   String(42)
来源：http://szw.shanyushiyangkeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://avm.tarul.cn

Go:   strconv.Itoa(42)
来源：http://bil.wangshuangyany.cn

Ruby: 42.to_s
来源：http://ykd.zhengqikj.top

C#:   42.ToString()
来源：http://lhl.nanxinkj.top

[A08] 取整与四舍五入
来源：http://fbe.fzhhl.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uvl.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uei.hcnkem.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mmc.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lxk.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mbi.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zmp.yfazqb.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://eqo.zhijiandao.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jup.hcnkem.com

[A09] 绝对值与最大最小值
来源：http://qxc.cdnleiting.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vtq.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qvv.hnqzz.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lyi.yongpay.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lxt.hesvh.cn


<!-- 参考信息 -->