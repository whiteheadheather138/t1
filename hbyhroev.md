代发 wailian999

[U55] PHP：match 表达式
来源：http://vdm.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qrr.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://dnq.daxiang520.top

f(a: 1, b: 2)
来源：http://bxk.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://gwg.nanxinkj.top

"值: {$a}"
来源：http://mvj.meibo888.top

[U58] PHP：数组三件套
来源：http://bba.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://umt.yj20258888.top

[U59] PHP：自定义排序
来源：http://jnq.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uvo.316326.xyz

[U60] PHP：JSON 编解码
来源：http://uzx.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nfz.epnwcf.com

[U61] PHP：正则
来源：http://qde.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fts.chenzaomai.com

[U62] PHP：日期对象
来源：http://ruv.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dvn.jqgfzy.top

[U63] PHP：文件读写
来源：http://wbj.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hsr.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://lqo.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://xlr.zhixingplan.top

[U65] PHP：会话
来源：http://jko.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://pie.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://zvh.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cmk.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://ypd.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cte.cheryme.top

[U68] PHP：PDO 连接
来源：http://ljp.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eoi.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://fll.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pcu.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://zmp.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lvc.fktsv.cn

[U71] PHP：抛出异常
来源：http://xzf.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://zza.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://rth.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://dww.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://lan.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://yxz.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://xpz.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://ccn.daxiang520.top

[U75] PHP：依赖注入
来源：http://mxp.jianghu66.top

composer require psr/container
来源：http://dce.jinqigfzy.top

[U76] PHP：简单路由
来源：http://rtg.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dkx.52xcode.cn

[U77] PHP：模板渲染
来源：http://vnd.zhongyouzk.top

composer require twig/twig
来源：http://ykj.hywenlv.cn

[U78] PHP：单元测试
来源：http://wbe.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://fko.hysaishi.cn

[U79] PHP：静态分析
来源：http://mxe.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://rfy.fehbvm.com

[U80] PHP：代码规范修复
来源：http://tzn.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iop.yueranfly.top

[U81] JS：初始化项目
来源：http://bmf.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://gjn.yj202588.top

[U82] JS：package.json 脚本
来源：http://ogc.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ldd.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://tla.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mun.316326.xyz

[U84] JS：CommonJS 写法
来源：http://gvf.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://twl.shzxlz.cn

[U85] JS：可选链
来源：http://qqf.fehbvm.com

a?.b?.c
来源：http://oci.ydzc1.top

[U86] JS：空值合并
来源：http://axj.zhixingplan.top

a ?? b
来源：http://flw.guannengcc.top

[U87] JS：解构默认值
来源：http://qfn.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://uem.sweek.top

[U88] JS：对象展开合并
来源：http://kgn.zdqjudy.top

{ ...a, ...b }
来源：http://wvj.snrcjt.cn

[U89] JS：数组去重
来源：http://asc.pengpengdd.cyou

[...new Set(arr)]
来源：http://cti.52xcode.cn

[U90] JS：数字数组排序
来源：http://kzu.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://vid.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://yzi.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kbw.dianchejie.cn

[U92] JS：深拷贝
来源：http://uzl.jinghuilouyu.cn

structuredClone(obj)
来源：http://gja.iojbl.cn

[U93] JS：模板字符串
来源：http://loa.daria6918.cn

`共 ${n} 条`
来源：http://kcn.cashguo.top

[U94] JS：箭头函数
来源：http://zro.ydjk.org.cn

const double = x => x * 2;
来源：http://vti.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://net.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://ylo.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://gcd.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xfx.gogol.net.cn

[U97] JS：并发请求
来源：http://gde.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rqi.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://weh.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ett.nanxuanxn.top

[U99] JS：事件监听
来源：http://ivf.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://hug.snrcjt.cn

[U100] JS：DOM 查询
来源：http://dbr.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://edj.iojbl.cn

[U101] JS：classList 操作
来源：http://eje.iojbl.cn

el.classList.toggle("active")
来源：http://hei.yongpay.top

[U102] JS：本地存储
来源：http://wlb.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nlt.jianghu66.top

[U103] JS：定时器
来源：http://qtt.zdqjudy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ocx.9152youxi.cn

[U104] JS：防抖
来源：http://tae.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://luv.hfpthk.cn

[U105] JS：节流
来源：http://lrb.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pek.tianlin.xyz

[U106] JS：日期格式化
来源：http://qko.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bxe.ybcxt.top

[U107] JS：数字千分位
来源：http://wqw.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://anr.zhaomingkeji.xyz

[U108] JS：随机整数
来源：http://lns.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rge.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://coq.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://cfx.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://eke.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dlv.havefunace.top

[U111] JS：对象转 Map
来源：http://ohd.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://eva.shzxlz.cn

[U112] JS：字符串补位
来源：http://sci.316326.xyz

"7".padStart(3, "0")
来源：http://spi.zhixingplan.top

[U113] JS：正则替换全部
来源：http://zaz.smart0.xyz

s.replaceAll("a", "b")
来源：http://cnx.tian-w.cn

[U114] JS：JSON 深比较
来源：http://jpm.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ltb.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://ojo.zhiwuduotai.top

crypto.randomUUID()
来源：http://lae.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://avu.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://xup.chenzaomai.com

[U117] JS：单元测试
来源：http://ouo.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://boq.yj20258888.top

[U118] JS：开发服务器
来源：http://rdv.hysaishi.cn

npm i -D vite;  npx vite
来源：http://znc.aibaodan.cn

[U119] JS：生产构建
来源：http://oho.cqqwz.cn

npx vite build
来源：http://tct.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://ncl.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://yex.yj20258.top

================================================================================
来源：http://iuy.feifeiyinyue.top

统计汇总
来源：http://abc.jiagoushi.top

================================================================================
来源：http://wsu.shuidangran.top

按语言统计（条）：
来源：http://aqm.dashuyun.cn

Python ......... 252
来源：http://znn.uphjek.com

PHP ............ 252
来源：http://kjd.ydjk.org.cn

JavaScript ..... 252
来源：http://qod.feifeiyinyue.top

TypeScript ..... 212
来源：http://dty.ywan-chungtsiang.top

Java ........... 212
来源：http://gqt.yonumen.top

Go ............. 212
来源：http://yme.daxiang520.top

Ruby ........... 212
来源：http://ysy.yfazqb.com

C# ............. 212
来源：http://chi.zhiwuduotai.top

C .............. 30
来源：http://tlf.sjlbkw.cn

C++ ............ 30
来源：http://jkv.uphjek.com

SQL ............ 90
来源：http://oqv.birdmap.top

Bash ........... 80
来源：http://rrx.vqdsnc.cn

Kotlin ......... 15
来源：http://pix.guowangkeji.top

Swift .......... 15
来源：http://jqa.zhijiandao.cn

Lua ............ 10
来源：http://oix.xziqi.cn

Perl ........... 10
来源：http://gvf.daxiang520.top

Scala .......... 10
来源：http://lag.jianghu66.top

------------------------------------
来源：http://qku.zhiwuduotai.top

合计 ........... 2106 条
来源：http://kfa.zhijiandao.cn

按章节统计：
来源：http://gyd.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://keh.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gko.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yot.tian-w.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vbc.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pdj.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kpo.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hyj.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://slz.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://okk.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mmy.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://chd.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gkm.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cmr.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gbi.jianghu66.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ahw.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bhw.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://xaf.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://iwt.tanke756.top

S C / C++ 专题                          60
来源：http://zmu.shanyushiyangkeji.top

T 其他语言补充                          60
来源：http://eam.uphjek.com

U 高频实用片段                         120
来源：http://llg.yonumen.top

------------------------------------
来源：http://naj.jlsjyb.cn

合计                                  2106 条
来源：http://zri.mhx1999.top

--------------------------------------------------------------------------------
来源：http://zai.tian-w.cn

使用提醒
来源：http://urg.52xcode.cn

--------------------------------------------------------------------------------
来源：http://vxe.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://owx.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://odq.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zuq.cashguo.top

在旧版本上使用前请先确认语法支持情况。
来源：http://php.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uvj.tanke756.top

—— 文件结束 ——
来源：http://nyz.pycfn.com

================================================================================
来源：http://lun.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://pfg.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://xtw.hammf.cn

================================================================================
来源：http://ktv.wangshuangyany.cn

【收录内容】
来源：http://pnm.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lnj.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://haj.xinyue.icu

SQL · Bash · C · C++
来源：http://tlr.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fut.yvedp.cn

【使用说明】
来源：http://nke.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xha.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lvz.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qoc.daria6918.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eve.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://rhi.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wuo.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dto.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://otm.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ite.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yfh.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xcs.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eqq.sjlbkw.cn

【文件统计】
来源：http://dbz.jyoumei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hkp.birdmap.top

--------------------------------------------------------------------------------
来源：http://knn.haohaochexian.top

目  录
来源：http://yya.yonumen.top

--------------------------------------------------------------------------------
来源：http://agi.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fjw.yj20258.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ojo.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yss.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hdb.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uss.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ihv.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xmx.shuidangran.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lyp.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://upv.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ywu.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ykf.jinyuanbaomall.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://onl.sxryk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cca.aibaodan.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yqp.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yac.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://azk.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tue.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://izc.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ppp.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhy.sjlbkw.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gmj.yfazqb.com

================================================================================
来源：http://mio.shanyushiyangtech.top

A. 基础语法与类型
来源：http://jjd.dashuyun.cn

================================================================================
来源：http://xzz.jiagoushi.top

[A01] Hello World
来源：http://qgj.tian-w.cn

Py:   print("Hello, World!")
来源：http://kpk.sweek.top

PHP:  echo "Hello, World!";
来源：http://ygv.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://huo.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kyq.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://hkf.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://xva.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://bez.xziqi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pkl.dianchejie.cn

[A02] 变量声明与赋值
来源：http://dwn.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xtf.uphjek.com

PHP:  $name = "Alex"; $age = 20;
来源：http://pmz.xingfuxueyuan.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://tsl.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fpx.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://ljf.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://iog.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://qac.jqgfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://iqp.tanke756.top

[A03] 常量定义
来源：http://jnc.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zbt.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://eey.birdmap.top

JS:   const PI = 3.14159;
来源：http://ktj.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://gwo.yangfankeji.com

Java: static final double PI = 3.14159;
来源：http://xcx.jyoumei.cn

Go:   const PI = 3.14159
来源：http://lfr.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://vkb.wangdashe.top

C#:   const double PI = 3.14159;
来源：http://hvk.guannengcc.top

[A04] 判断变量类型
来源：http://gfl.jqgufenzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jfj.zhixingplan.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nfi.quarkkingdee.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jyt.jinyuanbaomall.cn

TS:   typeof x; x instanceof Date
来源：http://ctt.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sxz.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://jzc.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sop.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://quc.zdqjudy.top

[A05] 整数除法与取模
来源：http://jdr.hnxiangtu.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dgk.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ixn.316326.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xxi.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mes.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://ifk.epnwcf.com

Go:   7 / 2; 7 % 2
来源：http://xqn.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://zpu.fengsongda.top

C#:   7 / 2; 7 % 2
来源：http://lep.ybcxt.top

[A06] 字符串转数字
来源：http://ixs.ydzc1.top

Py:   int("42"); float("3.14")
来源：http://aah.feifeiyinyue.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ivl.shanyushiyangtech.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ekk.yanxiufei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rxe.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yuv.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zqi.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bzv.hysaishi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nsx.jyoumei.cn

[A07] 数字转字符串
来源：http://ztc.sxryk.cn

Py:   str(42)
来源：http://uah.uphjek.com

PHP:  (string) 42; strval(42)
来源：http://liu.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://nfe.shangyingyoupin.top

TS:   String(42)
来源：http://bxp.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cxe.hesvh.cn

Go:   strconv.Itoa(42)
来源：http://asl.chenjidiqi.icu


<!-- 参考信息 -->