代发 wailian999

[U61] PHP：正则
来源：http://xng.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://azh.tianlin.xyz

[U62] PHP：日期对象
来源：http://gio.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dvl.redwolf501.top

[U63] PHP：文件读写
来源：http://tcl.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zkp.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://rxt.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://nou.feifeiyinyue.top

[U65] PHP：会话
来源：http://ncb.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hco.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://wwu.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zjs.yongpay.top

[U67] PHP：处理文件上传
来源：http://bth.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nxq.yuxming.cn

[U68] PHP：PDO 连接
来源：http://tbt.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://thn.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://jri.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbp.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://kzi.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yov.daria6918.cn

[U71] PHP：抛出异常
来源：http://rem.chenjidiqi.icu

throw new RuntimeException("失败", 500);
来源：http://xcs.epnwcf.com

[U72] PHP：写错误日志
来源：http://ibk.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://gxo.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://mog.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://jmk.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://sgv.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://rec.yuxming.cn

[U75] PHP：依赖注入
来源：http://cuj.fktsv.cn

composer require psr/container
来源：http://bkn.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://xpk.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://seo.jiagoushi.top

[U77] PHP：模板渲染
来源：http://bet.dianchejie.cn

composer require twig/twig
来源：http://kdi.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://zzu.ybcxt.top

composer require --dev phpunit/phpunit
来源：http://fhx.quarkkingdee.top

[U79] PHP：静态分析
来源：http://mhc.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://uqd.daxiang520.top

[U80] PHP：代码规范修复
来源：http://wqo.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wcf.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://eeo.316326.xyz

npm init -y;  npm i express
来源：http://tee.mhx1999.top

[U82] JS：package.json 脚本
来源：http://ezd.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pzj.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://ojn.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://geg.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://vcf.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://qjx.tianlin.xyz

[U85] JS：可选链
来源：http://bth.gzhubu.top

a?.b?.c
来源：http://nkn.9152youxi.cn

[U86] JS：空值合并
来源：http://kfs.jinyuanbaomall.cn

a ?? b
来源：http://sqq.tian-w.cn

[U87] JS：解构默认值
来源：http://ziq.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://rja.yuxming.cn

[U88] JS：对象展开合并
来源：http://tjc.yvedp.cn

{ ...a, ...b }
来源：http://cst.yj20258888.top

[U89] JS：数组去重
来源：http://jas.dianchejie.cn

[...new Set(arr)]
来源：http://txv.meibo888.top

[U90] JS：数字数组排序
来源：http://xsv.zhaomingkeji.xyz

[...arr].sort((a, b) => a - b)
来源：http://lol.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://nla.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lwt.meibo888.top

[U92] JS：深拷贝
来源：http://oee.birdmap.top

structuredClone(obj)
来源：http://buf.cheryme.top

[U93] JS：模板字符串
来源：http://qdm.hongshengwenyu.top

`共 ${n} 条`
来源：http://nzu.redwolf501.top

[U94] JS：箭头函数
来源：http://bxh.meibo888.top

const double = x => x * 2;
来源：http://oqj.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://fii.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://uts.cheryme.top

[U96] JS：async/await 与异常
来源：http://uer.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yyc.ppjwa.cn

[U97] JS：并发请求
来源：http://rng.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://nsd.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://nkm.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://his.hnxiangtu.top

[U99] JS：事件监听
来源：http://qvl.bjfxy.top

el.addEventListener("click", e => {})
来源：http://zyf.uphjek.com

[U100] JS：DOM 查询
来源：http://yeb.hysaishi.cn

document.querySelector(".item")
来源：http://wgg.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://tfl.shanyushiyangkeji.top

el.classList.toggle("active")
来源：http://alj.iojbl.cn

[U102] JS：本地存储
来源：http://myv.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://osj.mhx1999.top

[U103] JS：定时器
来源：http://gfu.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://caw.shangyingyoupin.top

[U104] JS：防抖
来源：http://tdy.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujr.daxiang520.top

[U105] JS：节流
来源：http://oqe.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tgb.redwolf501.top

[U106] JS：日期格式化
来源：http://dqz.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lho.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://huj.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oau.jiagoushi.top

[U108] JS：随机整数
来源：http://ryk.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vqh.chenjidiqi.icu

[U109] JS：数组分组
来源：http://tnb.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://vzs.jlsjyb.cn

[U110] JS：数组分块
来源：http://bvt.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pns.yuanzhike.top

[U111] JS：对象转 Map
来源：http://pbg.birdmap.top

new Map(Object.entries(obj))
来源：http://aoo.fzhhl.top

[U112] JS：字符串补位
来源：http://uvu.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://pve.0kj1m.cn

[U113] JS：正则替换全部
来源：http://gah.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://jis.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://srr.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pqj.hnqzz.top

[U115] JS：生成 UUID
来源：http://uex.zhongyouzk.top

crypto.randomUUID()
来源：http://udk.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://edb.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://hqu.ehwqpu.com

[U117] JS：单元测试
来源：http://fqm.tarul.cn

npm i -D vitest;  npx vitest
来源：http://qnf.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://dog.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://xxz.wangshuangyany.cn

[U119] JS：生产构建
来源：http://hzf.jinyuanbaomall.cn

npx vite build
来源：http://mvi.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://mut.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://uop.tianlin.xyz

================================================================================
来源：http://tqs.chenlongwang.top

统计汇总
来源：http://blp.epnwcf.com

================================================================================
来源：http://jde.zdqjudy.top

按语言统计（条）：
来源：http://ogz.xinyue.icu

Python ......... 252
来源：http://dni.epnwcf.com

PHP ............ 252
来源：http://ydd.aibaodan.cn

JavaScript ..... 252
来源：http://vmz.gogol.net.cn

TypeScript ..... 212
来源：http://maz.meibo888.top

Java ........... 212
来源：http://ivg.cucudq.cn

Go ............. 212
来源：http://qiz.sxryk.cn

Ruby ........... 212
来源：http://tpg.uphjek.com

C# ............. 212
来源：http://vpu.yueranfly.top

C .............. 30
来源：http://qsn.jinqigfzy.top

C++ ............ 30
来源：http://zox.feifeiyinyue.top

SQL ............ 90
来源：http://jwg.shanyushiyangtech.top

Bash ........... 80
来源：http://fug.yvedp.cn

Kotlin ......... 15
来源：http://ept.redwolf501.top

Swift .......... 15
来源：http://wum.hnxiangtu.top

Lua ............ 10
来源：http://kac.haohaochexian.top

Perl ........... 10
来源：http://sci.jinqigufen.top

Scala .......... 10
来源：http://hub.xylfe.cn

------------------------------------
来源：http://esn.hesvh.cn

合计 ........... 2106 条
来源：http://hik.wangshuangyany.cn

按章节统计：
来源：http://wbp.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zvi.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sfk.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://axu.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iwq.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nuq.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://krq.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yxw.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://swi.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xyc.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ylm.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://knf.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lco.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://liv.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dfr.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://elr.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://byw.yuanzhike.top

Q SQL 专题                              90
来源：http://iyc.epnwcf.com

R Bash 专题                             80
来源：http://yfo.yangfankeji.com

S C / C++ 专题                          60
来源：http://wyt.gogol.net.cn

T 其他语言补充                          60
来源：http://zke.bjfxy.top

U 高频实用片段                         120
来源：http://lrj.dashuyun.cn

------------------------------------
来源：http://vnm.xinyue.icu

合计                                  2106 条
来源：http://kmv.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://csu.jlsjyb.cn

使用提醒
来源：http://ebe.tarul.cn

--------------------------------------------------------------------------------
来源：http://wsu.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xzp.epnwcf.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://amp.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://trx.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cmv.zhengqikj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uoz.jinghuilouyu.cn

—— 文件结束 ——
来源：http://kcg.chenjidiqi.icu

================================================================================
来源：http://tjw.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://xcp.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://pmt.tanke756.top

================================================================================
来源：http://gfh.ctjpmb.com

【收录内容】
来源：http://rgm.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ift.zhaomingkeji.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ibg.52xcode.cn

SQL · Bash · C · C++
来源：http://ezc.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://aoi.gaohongyu789.top

【使用说明】
来源：http://zow.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mgb.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wfw.zdqjudy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wqu.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://psb.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gke.hongshengwenyu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lcu.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ete.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gso.pengpengdd.cyou

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mxv.hongshengwenyu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gos.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yaa.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kab.aizwys.cn

【文件统计】
来源：http://tfk.jianghu66.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pov.birdmap.top

--------------------------------------------------------------------------------
来源：http://zwq.jiagoushi.top

目  录
来源：http://nvy.daxiang520.top

--------------------------------------------------------------------------------
来源：http://vwi.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xcd.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bzh.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zqw.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://coe.zhaomingkeji.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gvw.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wik.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gim.zdqjudy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fjl.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://btv.gzhubu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://slo.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dew.jinqigfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kgx.shzxlz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jyd.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mff.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ald.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yac.jinqigufen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mzp.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dxr.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qvg.uphjek.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sgw.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uxv.birdmap.top

================================================================================
来源：http://ejo.ppjwa.cn

A. 基础语法与类型
来源：http://edr.wangdashe.top

================================================================================
来源：http://yph.zhijiandao.cn

[A01] Hello World
来源：http://pqt.zhengqikj.top

Py:   print("Hello, World!")
来源：http://uco.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://mef.vqdsnc.cn

JS:   console.log("Hello, World!");
来源：http://vnp.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xbp.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://nuq.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://dlc.bbcook.cn

Ruby: puts "Hello, World!"
来源：http://yon.chenzaomai.com

C#:   Console.WriteLine("Hello, World!");
来源：http://qvh.bbcook.cn

[A02] 变量声明与赋值
来源：http://qgl.dianchejie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://scy.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kda.cashguo.top

JS:   let name = "Alex"; const age = 20;
来源：http://lkr.fengsongda.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tpg.bbcook.cn

Java: String name = "Alex"; int age = 20;
来源：http://vzj.ctjpmb.com

Go:   name := "Alex"; age := 20
来源：http://yvb.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://uwx.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://wsl.vehdjk.com

[A03] 常量定义
来源：http://jrh.zycfv.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cjj.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://rhj.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://wnr.ywan-chungtsiang.top

TS:   const PI: number = 3.14159;
来源：http://lyx.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://lop.aizwys.cn

Go:   const PI = 3.14159
来源：http://ubo.dashuyun.cn

Ruby: PI = 3.14159
来源：http://lkx.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://nnw.ehwqpu.com

[A04] 判断变量类型
来源：http://qle.shzxlz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qif.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ucw.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uxs.jinghuilouyu.cn

TS:   typeof x; x instanceof Date
来源：http://ell.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fhm.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pqt.tarul.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wei.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://zol.tianlin.xyz

[A05] 整数除法与取模
来源：http://lul.zdqjudy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ysc.ybcxt.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://blu.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://boo.xuanzx.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wkj.nwbrower.top

Java: 7 / 2; 7 % 2
来源：http://kbv.bjfxy.top

Go:   7 / 2; 7 % 2
来源：http://qqi.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://ppj.xingfuxueyuan.xyz

C#:   7 / 2; 7 % 2
来源：http://ypo.snrcjt.cn

[A06] 字符串转数字
来源：http://cgk.shuidangran.top

Py:   int("42"); float("3.14")
来源：http://qhs.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jul.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://toj.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://dvb.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vyz.andypj.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://izj.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dhx.hongshengwenyu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://glb.jiagoushi.top

[A07] 数字转字符串
来源：http://rgn.feifeiyinyue.top

Py:   str(42)
来源：http://hxx.shzxlz.cn

PHP:  (string) 42; strval(42)
来源：http://kfn.aizwys.cn

JS:   String(42); (42).toString()
来源：http://wfn.jqgfzy.top

TS:   String(42)
来源：http://mhv.fktsv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qqc.zhiwuduotai.top

Go:   strconv.Itoa(42)
来源：http://zui.zycfv.cn

Ruby: 42.to_s
来源：http://xpr.zhixingplan.top

C#:   42.ToString()
来源：http://zzt.wangdashe.top

[A08] 取整与四舍五入
来源：http://wii.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oca.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://reu.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gfd.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ovh.jqgufenzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tuc.xinyue.icu

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nzk.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mgx.jlsjyb.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kae.havefunace.top

[A09] 绝对值与最大最小值
来源：http://dxr.bjfxy.top


<!-- 参考信息 -->