代发 wailian999

[U63] PHP：文件读写
来源：http://mlj.tianlin.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://stf.fengsongda.top

[U64] PHP：目录遍历
来源：http://vbk.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://aco.cashguo.top

[U65] PHP：会话
来源：http://pbn.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://kvv.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://svj.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ekm.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://yat.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://hfh.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://djc.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://ntx.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ink.fengsongda.top

[U70] PHP：PDO 事务
来源：http://gkt.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://peq.dianchejie.cn

[U71] PHP：抛出异常
来源：http://gga.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://smo.52xcode.cn

[U72] PHP：写错误日志
来源：http://ubv.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://pfs.xylfe.cn

[U73] PHP：读取 ini 配置
来源：http://ioj.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://rgu.yuxming.cn

[U74] PHP：读取环境变量
来源：http://tzj.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://ycq.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://fyv.cqqwz.cn

composer require psr/container
来源：http://rja.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://uud.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://beh.snrcjt.cn

[U77] PHP：模板渲染
来源：http://uin.fanxiaobao.xyz

composer require twig/twig
来源：http://aqo.hcnkem.com

[U78] PHP：单元测试
来源：http://uuq.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://irf.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://mih.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://znl.shuidangran.top

[U80] PHP：代码规范修复
来源：http://mtr.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nhn.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://uvd.hywenlv.cn

npm init -y;  npm i express
来源：http://rqf.yfazqb.com

[U82] JS：package.json 脚本
来源：http://why.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hmn.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://blt.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bbm.hammf.cn

[U84] JS：CommonJS 写法
来源：http://oij.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ync.hesvh.cn

[U85] JS：可选链
来源：http://eem.mhx1999.top

a?.b?.c
来源：http://ill.xinyue.icu

[U86] JS：空值合并
来源：http://aoi.vehdjk.com

a ?? b
来源：http://lnm.zhixingplan.top

[U87] JS：解构默认值
来源：http://eoo.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://wab.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://jai.hongshengwenyu.top

{ ...a, ...b }
来源：http://ggj.bbcook.cn

[U89] JS：数组去重
来源：http://gsd.cashguo.top

[...new Set(arr)]
来源：http://gpr.yonumen.top

[U90] JS：数字数组排序
来源：http://yiv.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://wnt.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://tvv.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://esa.yangfankeji.com

[U92] JS：深拷贝
来源：http://aec.ywan-chungtsiang.top

structuredClone(obj)
来源：http://tpi.chenlongwang.top

[U93] JS：模板字符串
来源：http://qao.zhengqikj.top

`共 ${n} 条`
来源：http://pgc.zycfv.cn

[U94] JS：箭头函数
来源：http://bsk.tanke756.top

const double = x => x * 2;
来源：http://ynh.yj202588.top

[U95] JS：Promise 包装
来源：http://mdl.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://yiq.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://nzt.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pll.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://wlb.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zds.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://kfw.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fvk.jyoumei.cn

[U99] JS：事件监听
来源：http://nyx.bjfxy.top

el.addEventListener("click", e => {})
来源：http://xif.daxiang520.top

[U100] JS：DOM 查询
来源：http://hhf.xylfe.cn

document.querySelector(".item")
来源：http://gav.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://ayc.cdnleiting.top

el.classList.toggle("active")
来源：http://hrp.fktsv.cn

[U102] JS：本地存储
来源：http://fzw.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oph.pengpengdd.cyou

[U103] JS：定时器
来源：http://mfe.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rrb.guannengcc.top

[U104] JS：防抖
来源：http://pqr.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyi.fanxiaobao.xyz

[U105] JS：节流
来源：http://rep.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lys.ivvv.top

[U106] JS：日期格式化
来源：http://iir.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dpy.snrcjt.cn

[U107] JS：数字千分位
来源：http://gmo.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fbu.jianghu66.top

[U108] JS：随机整数
来源：http://hct.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://adu.haohaochexian.top

[U109] JS：数组分组
来源：http://ybb.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://uyd.zdqjudy.top

[U110] JS：数组分块
来源：http://dtt.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jvs.cucudq.cn

[U111] JS：对象转 Map
来源：http://fem.mhx1999.top

new Map(Object.entries(obj))
来源：http://xgg.52xcode.cn

[U112] JS：字符串补位
来源：http://gzw.bjfxy.top

"7".padStart(3, "0")
来源：http://qfq.tian-w.cn

[U113] JS：正则替换全部
来源：http://eww.nanxuanxn.top

s.replaceAll("a", "b")
来源：http://gzf.ivvv.top

[U114] JS：JSON 深比较
来源：http://gex.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://biz.andypj.xyz

[U115] JS：生成 UUID
来源：http://kpx.hesvh.cn

crypto.randomUUID()
来源：http://yjj.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://seg.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://fht.hnqzz.top

[U117] JS：单元测试
来源：http://qeu.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://iny.bbcook.cn

[U118] JS：开发服务器
来源：http://wve.jinqigufen.top

npm i -D vite;  npx vite
来源：http://xqc.zycfv.cn

[U119] JS：生产构建
来源：http://ygi.jyoumei.cn

npx vite build
来源：http://bel.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://goa.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://hvm.andypj.xyz

================================================================================
来源：http://avv.fehbvm.com

统计汇总
来源：http://fvi.316326.xyz

================================================================================
来源：http://uhw.bbcook.cn

按语言统计（条）：
来源：http://mpp.vqdsnc.cn

Python ......... 252
来源：http://muj.nanxuanxn.top

PHP ............ 252
来源：http://riq.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://rvt.xuanzx.com

TypeScript ..... 212
来源：http://ttz.wangdashe.top

Java ........... 212
来源：http://omn.jqgfzy.top

Go ............. 212
来源：http://mcl.0kj1m.cn

Ruby ........... 212
来源：http://fzl.fktsv.cn

C# ............. 212
来源：http://hbj.sufxvd.cn

C .............. 30
来源：http://fdv.daria6918.cn

C++ ............ 30
来源：http://lsm.jlsjyb.cn

SQL ............ 90
来源：http://enm.hcnkem.com

Bash ........... 80
来源：http://mgr.zdbjq.cn

Kotlin ......... 15
来源：http://lit.vqdsnc.cn

Swift .......... 15
来源：http://fft.aibaodan.cn

Lua ............ 10
来源：http://obo.cashguo.top

Perl ........... 10
来源：http://dup.xinyue.icu

Scala .......... 10
来源：http://yny.pycfn.com

------------------------------------
来源：http://lhu.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://puz.9152youxi.cn

按章节统计：
来源：http://bba.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bzo.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cwn.zhaomingkeji.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zxw.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cjk.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yfj.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xre.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ufi.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xas.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lbs.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ubm.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dhw.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zmn.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nsy.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ytd.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vpj.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kgk.aizwys.cn

Q SQL 专题                              90
来源：http://gcj.9152youxi.cn

R Bash 专题                             80
来源：http://oxn.hesvh.cn

S C / C++ 专题                          60
来源：http://qcx.sweek.top

T 其他语言补充                          60
来源：http://hgx.havefunace.top

U 高频实用片段                         120
来源：http://ofe.zhongyouzk.top

------------------------------------
来源：http://zjp.pengpengdd.cyou

合计                                  2106 条
来源：http://xut.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://pef.feifeiyinyue.top

使用提醒
来源：http://ymu.fzhhl.top

--------------------------------------------------------------------------------
来源：http://nyo.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mnj.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hxj.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eif.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kad.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ouc.gzhubu.top

—— 文件结束 ——
来源：http://qsg.zhaomingkeji.xyz

================================================================================
来源：http://die.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://iag.yj20258.top

Common Programming Examples Cheat Book
来源：http://vwz.tanke756.top

================================================================================
来源：http://fvu.ppjwa.cn

【收录内容】
来源：http://bod.tianlin.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://tgq.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://umq.guannengcc.top

SQL · Bash · C · C++
来源：http://fft.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://owj.smart0.xyz

【使用说明】
来源：http://yhb.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dkh.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bcl.birdmap.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qyv.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://csj.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lwd.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gpi.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jwl.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qfo.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cql.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eak.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://man.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ylm.52xcode.cn

【文件统计】
来源：http://kzi.sufxvd.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uov.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://qbq.wangdashe.top

目  录
来源：http://ymb.hnqzz.top

--------------------------------------------------------------------------------
来源：http://eup.xingfuxueyuan.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zep.yvedp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://roz.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://stt.sufxvd.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eta.tarul.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nof.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cuy.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bku.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wrs.ywan-chungtsiang.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ycs.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fnx.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xrf.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pty.jinqigufen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tcd.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eoc.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zlw.hammf.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqo.cashguo.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://did.xziqi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kym.wangdashe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tpl.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwy.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mkr.yfazqb.com

================================================================================
来源：http://iis.tianlin.xyz

A. 基础语法与类型
来源：http://mum.chenzaomai.com

================================================================================
来源：http://qxg.jinqigfzy.top

[A01] Hello World
来源：http://chu.xuanzx.com

Py:   print("Hello, World!")
来源：http://eqw.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://aip.jinqigufen.top

JS:   console.log("Hello, World!");
来源：http://wnm.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://btn.ppjwa.cn

Java: System.out.println("Hello, World!");
来源：http://tyb.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://jcl.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://aso.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ojb.hnxiangtu.top

[A02] 变量声明与赋值
来源：http://npj.fktsv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qgf.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qvh.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://qjc.hysaishi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ewp.tianlin.xyz

Java: String name = "Alex"; int age = 20;
来源：http://lrc.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://kep.epnwcf.com

Ruby: name = "Alex"; age = 20
来源：http://upo.mhx1999.top

C#:   string name = "Alex"; int age = 20;
来源：http://xdc.yj202588.top

[A03] 常量定义
来源：http://env.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://orz.yuanzhike.top

PHP:  const PI = 3.14159;
来源：http://paa.daria6918.cn

JS:   const PI = 3.14159;
来源：http://hho.nwbrower.top

TS:   const PI: number = 3.14159;
来源：http://vyh.jinyuanbaomall.cn

Java: static final double PI = 3.14159;
来源：http://eoe.hysaishi.cn

Go:   const PI = 3.14159
来源：http://few.meibo888.top

Ruby: PI = 3.14159
来源：http://tgi.hywenlv.cn

C#:   const double PI = 3.14159;
来源：http://gla.yangfankeji.com

[A04] 判断变量类型
来源：http://bfe.sysykeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lgz.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hig.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://was.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://yiz.uphjek.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://smz.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tfz.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://jfv.gogol.net.cn

C#:   x.GetType().Name; x is int
来源：http://qkh.kuanghao11.cn

[A05] 整数除法与取模
来源：http://pdu.hywenlv.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://spa.bbcook.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://itf.jinyuanbaomall.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yqj.tarul.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fpc.hcnkem.com

Java: 7 / 2; 7 % 2
来源：http://xof.jyoumei.cn

Go:   7 / 2; 7 % 2
来源：http://nmy.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://brl.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://afg.jiagoushi.top

[A06] 字符串转数字
来源：http://udq.yanxiufei.cn

Py:   int("42"); float("3.14")
来源：http://vco.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cew.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://enx.cqqwz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xib.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pmc.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://par.zhiwuduotai.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qle.hongshengwenyu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zse.feifeiyinyue.top

[A07] 数字转字符串
来源：http://jza.sweek.top

Py:   str(42)
来源：http://yqg.xuetiantiany.cn

PHP:  (string) 42; strval(42)
来源：http://xqb.redwolf501.top

JS:   String(42); (42).toString()
来源：http://ktx.316326.xyz

TS:   String(42)
来源：http://yxq.nanxinkj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zbe.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://meg.tanke756.top

Ruby: 42.to_s
来源：http://xso.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://mqy.jyoumei.cn

[A08] 取整与四舍五入
来源：http://smo.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fue.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zpu.uphjek.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fvz.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ytv.mhx1999.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zon.ppjwa.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sfi.daria6918.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lib.cashguo.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://awo.sysykeji.top

[A09] 绝对值与最大最小值
来源：http://cgu.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lut.ppjwa.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ren.cashguo.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gmk.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qfd.fktsv.cn


<!-- 参考信息 -->