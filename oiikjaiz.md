代发 wailian999

[U63] PHP：文件读写
来源：http://hsj.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kqa.yueranfly.top

[U64] PHP：目录遍历
来源：http://thr.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://wqe.tanke756.top

[U65] PHP：会话
来源：http://sxw.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rjl.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://ffz.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ylj.havefunace.top

[U67] PHP：处理文件上传
来源：http://qek.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yfc.316326.xyz

[U68] PHP：PDO 连接
来源：http://lll.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ich.cashguo.top

[U69] PHP：PDO 预处理
来源：http://cft.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://npq.yongpay.top

[U70] PHP：PDO 事务
来源：http://tim.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://agk.c1oappe.top

[U71] PHP：抛出异常
来源：http://jwr.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://nfr.gotoacloud.top

[U72] PHP：写错误日志
来源：http://igm.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://umi.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://gky.pycfn.com

parse_ini_file("config.ini", true)
来源：http://rdv.iojbl.cn

[U74] PHP：读取环境变量
来源：http://gpm.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://zkl.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://xxz.yuanzhike.top

composer require psr/container
来源：http://hrv.jinqigfzy.top

[U76] PHP：简单路由
来源：http://sqv.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ygt.uphjek.com

[U77] PHP：模板渲染
来源：http://fmp.mhx1999.top

composer require twig/twig
来源：http://snv.ydzc1.top

[U78] PHP：单元测试
来源：http://kmn.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://mam.svipenyu.cn

[U79] PHP：静态分析
来源：http://rio.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://gag.fzhhl.top

[U80] PHP：代码规范修复
来源：http://jqg.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wgu.daxiang520.top

[U81] JS：初始化项目
来源：http://lzq.52xcode.cn

npm init -y;  npm i express
来源：http://czn.xuanzx.com

[U82] JS：package.json 脚本
来源：http://avg.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hav.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://ald.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://uqj.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://gkm.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eur.jianghu66.top

[U85] JS：可选链
来源：http://etk.andypj.xyz

a?.b?.c
来源：http://orq.yanxiufei.cn

[U86] JS：空值合并
来源：http://pwy.shangyingyoupin.top

a ?? b
来源：http://zam.yongpay.top

[U87] JS：解构默认值
来源：http://kqp.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://dyv.yj20258.top

[U88] JS：对象展开合并
来源：http://fpc.tanke756.top

{ ...a, ...b }
来源：http://egx.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://nub.jqgufenzy.top

[...new Set(arr)]
来源：http://cip.yj202588.top

[U90] JS：数字数组排序
来源：http://kjg.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://bzh.zycfv.cn

[U91] JS：对象键值遍历
来源：http://fxf.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jxn.zhengqikj.top

[U92] JS：深拷贝
来源：http://gbt.hnqzz.top

structuredClone(obj)
来源：http://nom.iojbl.cn

[U93] JS：模板字符串
来源：http://edo.0kj1m.cn

`共 ${n} 条`
来源：http://liv.ehwqpu.com

[U94] JS：箭头函数
来源：http://nhf.snrcjt.cn

const double = x => x * 2;
来源：http://tzw.yj20258888.top

[U95] JS：Promise 包装
来源：http://zjh.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://uhx.hammf.cn

[U96] JS：async/await 与异常
来源：http://jlt.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gji.tian-w.cn

[U97] JS：并发请求
来源：http://mpm.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cnp.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://qzf.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oam.hammf.cn

[U99] JS：事件监听
来源：http://naj.cheryme.top

el.addEventListener("click", e => {})
来源：http://eyr.zhengqikj.top

[U100] JS：DOM 查询
来源：http://wwc.hongshengwenyu.top

document.querySelector(".item")
来源：http://gls.havefunace.top

[U101] JS：classList 操作
来源：http://zyl.fehbvm.com

el.classList.toggle("active")
来源：http://jps.xinyue.icu

[U102] JS：本地存储
来源：http://pue.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://fnw.uphjek.com

[U103] JS：定时器
来源：http://xnl.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lgv.ehwqpu.com

[U104] JS：防抖
来源：http://psx.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvq.uphjek.com

[U105] JS：节流
来源：http://kne.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fvr.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://hct.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eqc.fengsongda.top

[U107] JS：数字千分位
来源：http://xdf.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://flr.nanxinkj.top

[U108] JS：随机整数
来源：http://qsx.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uef.fehbvm.com

[U109] JS：数组分组
来源：http://aui.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://ett.yongpay.top

[U110] JS：数组分块
来源：http://oyq.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ien.shzxlz.cn

[U111] JS：对象转 Map
来源：http://vja.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://zbg.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://qma.sxryk.cn

"7".padStart(3, "0")
来源：http://mfs.c1oappe.top

[U113] JS：正则替换全部
来源：http://dsh.jianghu66.top

s.replaceAll("a", "b")
来源：http://qdg.xylfe.cn

[U114] JS：JSON 深比较
来源：http://fjr.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vku.cheryme.top

[U115] JS：生成 UUID
来源：http://gvp.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://rbp.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://tbj.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://fml.fehbvm.com

[U117] JS：单元测试
来源：http://mje.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://ukq.tanke756.top

[U118] JS：开发服务器
来源：http://egm.nwbrower.top

npm i -D vite;  npx vite
来源：http://ovn.yfazqb.com

[U119] JS：生产构建
来源：http://umg.cucudq.cn

npx vite build
来源：http://hau.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://odc.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://srt.cucudq.cn

================================================================================
来源：http://hyk.wangshuangyany.cn

统计汇总
来源：http://hvp.zdbjq.cn

================================================================================
来源：http://qbj.jianghu66.top

按语言统计（条）：
来源：http://rtl.redwolf501.top

Python ......... 252
来源：http://fmi.jinyuanbaomall.cn

PHP ............ 252
来源：http://ykn.feifeiyinyue.top

JavaScript ..... 252
来源：http://dfw.aibaodan.cn

TypeScript ..... 212
来源：http://onh.ehwqpu.com

Java ........... 212
来源：http://ykt.shzxlz.cn

Go ............. 212
来源：http://qas.redwolf501.top

Ruby ........... 212
来源：http://efc.yonumen.top

C# ............. 212
来源：http://xvw.pycfn.com

C .............. 30
来源：http://mlr.gzhubu.top

C++ ............ 30
来源：http://zag.andypj.xyz

SQL ............ 90
来源：http://ggd.xuanzx.com

Bash ........... 80
来源：http://dcv.yongpay.top

Kotlin ......... 15
来源：http://lqg.gaohongyu789.top

Swift .......... 15
来源：http://jvz.yvedp.cn

Lua ............ 10
来源：http://jyd.hesvh.cn

Perl ........... 10
来源：http://hhf.nwbrower.top

Scala .......... 10
来源：http://uwt.chenzaomai.com

------------------------------------
来源：http://gcs.xinyue.icu

合计 ........... 2106 条
来源：http://ftg.zhongyouzk.top

按章节统计：
来源：http://wqy.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://doa.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hhw.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cmn.hnxiangtu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xmt.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qmz.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://adh.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xkj.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eil.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kjn.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dnh.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nip.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fot.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lym.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rwj.yvedp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vmq.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fnm.hnxiangtu.top

Q SQL 专题                              90
来源：http://usu.quarkkingdee.top

R Bash 专题                             80
来源：http://nym.jinqigfzy.top

S C / C++ 专题                          60
来源：http://tpq.ybcxt.top

T 其他语言补充                          60
来源：http://ofw.hesvh.cn

U 高频实用片段                         120
来源：http://erg.haohaochexian.top

------------------------------------
来源：http://azd.ydzc1.top

合计                                  2106 条
来源：http://ffr.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://lbu.jinghuilouyu.cn

使用提醒
来源：http://dfq.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://hki.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qhh.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nqz.xinyue.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xae.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mju.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mew.gogol.net.cn

—— 文件结束 ——
来源：http://eyf.jinqigfzy.top

================================================================================
来源：http://srd.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://irf.yuxming.cn

Common Programming Examples Cheat Book
来源：http://upz.yj20258888.top

================================================================================
来源：http://mwj.gaohongyu789.top

【收录内容】
来源：http://anc.nanxuanxn.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://aeq.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lze.cashguo.top

SQL · Bash · C · C++
来源：http://ytb.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://moc.guannengcc.top

【使用说明】
来源：http://qph.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kxn.xuetiantiany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://frx.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wps.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://znh.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wkv.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mlb.vehdjk.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wyi.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qiq.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xfv.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://orr.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tvs.bbcook.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tfy.havefunace.top

【文件统计】
来源：http://ngv.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ctk.bbcook.cn

--------------------------------------------------------------------------------
来源：http://ikn.shzxlz.cn

目  录
来源：http://ekc.ivvv.top

--------------------------------------------------------------------------------
来源：http://dlq.hnqzz.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ped.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mzl.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mjs.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yfd.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://liv.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rjt.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rcv.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jld.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aln.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tke.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://znk.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bgs.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rop.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ibx.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://znc.andypj.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nfq.yonumen.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hwk.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://prw.ywan-chungtsiang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pxm.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qsi.hongshengwenyu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://adk.jyoumei.cn

================================================================================
来源：http://phx.gotoacloud.top

A. 基础语法与类型
来源：http://wid.zhixingplan.top

================================================================================
来源：http://rgt.sufxvd.cn

[A01] Hello World
来源：http://trs.chenlongwang.top

Py:   print("Hello, World!")
来源：http://xsm.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://ayi.nwbrower.top

JS:   console.log("Hello, World!");
来源：http://hzc.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aei.dashuyun.cn

Java: System.out.println("Hello, World!");
来源：http://rpy.guannengcc.top

Go:   fmt.Println("Hello, World!")
来源：http://adq.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://khq.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lhk.dashuyun.cn

[A02] 变量声明与赋值
来源：http://bmf.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zzw.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eal.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://ehd.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mrp.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://oub.fengsongda.top

Go:   name := "Alex"; age := 20
来源：http://awe.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://jsx.c1oappe.top

C#:   string name = "Alex"; int age = 20;
来源：http://zqh.ehwqpu.com

[A03] 常量定义
来源：http://jxx.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rcs.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://wii.uphjek.com

JS:   const PI = 3.14159;
来源：http://fme.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://ljp.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://idk.cqqwz.cn

Go:   const PI = 3.14159
来源：http://lsg.sysykeji.top

Ruby: PI = 3.14159
来源：http://oxy.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://lje.shuidangran.top

[A04] 判断变量类型
来源：http://bog.sjlbkw.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yiq.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://olu.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tqq.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://uxj.jiagoushi.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://evt.shanyushiyangtech.top

Go:   reflect.TypeOf(x).Name()
来源：http://dcx.vqdsnc.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wyf.yuanzhike.top

C#:   x.GetType().Name; x is int
来源：http://uzf.fanxiaobao.xyz

[A05] 整数除法与取模
来源：http://kmm.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wpt.hongshengwenyu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://sod.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lvd.jlsjyb.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rre.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://bfb.xziqi.cn

Go:   7 / 2; 7 % 2
来源：http://xlp.hcnkem.com

Ruby: 7 / 2; 7 % 2
来源：http://hlk.sufxvd.cn

C#:   7 / 2; 7 % 2
来源：http://ojv.zhengqikj.top

[A06] 字符串转数字
来源：http://kfj.guannengcc.top

Py:   int("42"); float("3.14")
来源：http://bfj.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xep.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zsu.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://dzk.52xcode.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://krl.xinyue.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ccx.sweek.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fnt.yvedp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://osa.sweek.top

[A07] 数字转字符串
来源：http://lmc.cashguo.top

Py:   str(42)
来源：http://yxb.yj20258.top

PHP:  (string) 42; strval(42)
来源：http://jeh.nanxuanxn.top

JS:   String(42); (42).toString()
来源：http://ltx.9152youxi.cn

TS:   String(42)
来源：http://fia.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hix.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://fww.sweek.top

Ruby: 42.to_s
来源：http://dmm.jianghu66.top

C#:   42.ToString()
来源：http://cvd.hesvh.cn

[A08] 取整与四舍五入
来源：http://imv.sysykeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gvc.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jkn.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oih.yvedp.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mbv.jinqigfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bey.shanyushiyangtech.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://abr.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bhh.pengpengdd.cyou

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kuk.meibo888.top

[A09] 绝对值与最大最小值
来源：http://pua.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qev.yueranfly.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rja.pengpengdd.cyou

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wdn.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xlc.bjfxy.top


<!-- 参考信息 -->