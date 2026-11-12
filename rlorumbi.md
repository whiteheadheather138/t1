代发 wailian999

[U59] PHP：自定义排序
来源：http://ilr.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gwl.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://zdr.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dou.0kj1m.cn

[U61] PHP：正则
来源：http://ghk.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbz.ivvv.top

[U62] PHP：日期对象
来源：http://uku.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qpt.fzhhl.top

[U63] PHP：文件读写
来源：http://dbj.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bcg.yueranfly.top

[U64] PHP：目录遍历
来源：http://srk.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://bei.smart0.xyz

[U65] PHP：会话
来源：http://kse.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iet.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://pio.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vkd.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://kpn.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zxq.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://gyn.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ukw.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://bib.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://air.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://ynq.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ati.ppjwa.cn

[U71] PHP：抛出异常
来源：http://rqa.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://kzk.ctjpmb.com

[U72] PHP：写错误日志
来源：http://xee.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://cdq.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://bmq.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://orw.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://gcn.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://fdx.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://zdq.ctjpmb.com

composer require psr/container
来源：http://yci.sysykeji.top

[U76] PHP：简单路由
来源：http://pis.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://drj.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://xzd.vqdsnc.cn

composer require twig/twig
来源：http://bii.havefunace.top

[U78] PHP：单元测试
来源：http://fej.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://ocv.shuidangran.top

[U79] PHP：静态分析
来源：http://wqh.ivvv.top

composer require --dev phpstan/phpstan
来源：http://dfz.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://lin.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rnp.shuidangran.top

[U81] JS：初始化项目
来源：http://hcz.jinqigufen.top

npm init -y;  npm i express
来源：http://ule.sweek.top

[U82] JS：package.json 脚本
来源：http://fsf.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vkx.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://gqh.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://yxx.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://voz.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nuk.tianlin.xyz

[U85] JS：可选链
来源：http://neg.xuanzx.com

a?.b?.c
来源：http://jqh.zhongyouzk.top

[U86] JS：空值合并
来源：http://zoj.fanxiaobao.xyz

a ?? b
来源：http://evc.jyoumei.cn

[U87] JS：解构默认值
来源：http://byr.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://jha.sxryk.cn

[U88] JS：对象展开合并
来源：http://hai.hnxiangtu.top

{ ...a, ...b }
来源：http://wai.ivvv.top

[U89] JS：数组去重
来源：http://mrm.dashuyun.cn

[...new Set(arr)]
来源：http://kju.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://xum.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://aqk.daxiang520.top

[U91] JS：对象键值遍历
来源：http://tzy.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fhc.shuidangran.top

[U92] JS：深拷贝
来源：http://hzn.ydzc1.top

structuredClone(obj)
来源：http://pda.quarkkingdee.top

[U93] JS：模板字符串
来源：http://ups.shzxlz.cn

`共 ${n} 条`
来源：http://hrm.xylfe.cn

[U94] JS：箭头函数
来源：http://xky.pengpengdd.cyou

const double = x => x * 2;
来源：http://czl.aibaodan.cn

[U95] JS：Promise 包装
来源：http://djo.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://kxr.mhx1999.top

[U96] JS：async/await 与异常
来源：http://ncg.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pnk.dashuyun.cn

[U97] JS：并发请求
来源：http://iyk.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oay.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://wul.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wlb.yj20258.top

[U99] JS：事件监听
来源：http://uza.tarul.cn

el.addEventListener("click", e => {})
来源：http://igv.nwbrower.top

[U100] JS：DOM 查询
来源：http://cli.smart0.xyz

document.querySelector(".item")
来源：http://xgk.zhongyouzk.top

[U101] JS：classList 操作
来源：http://sub.aibaodan.cn

el.classList.toggle("active")
来源：http://nqu.tianlin.xyz

[U102] JS：本地存储
来源：http://xtv.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xnl.meibo888.top

[U103] JS：定时器
来源：http://jke.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mjc.yuanzhike.top

[U104] JS：防抖
来源：http://ais.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezf.feifeiyinyue.top

[U105] JS：节流
来源：http://rhs.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://efs.smart0.xyz

[U106] JS：日期格式化
来源：http://zgo.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yep.meibo888.top

[U107] JS：数字千分位
来源：http://cfm.fehbvm.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rvc.fktsv.cn

[U108] JS：随机整数
来源：http://bya.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://atl.vehdjk.com

[U109] JS：数组分组
来源：http://uzd.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://gna.guowangkeji.top

[U110] JS：数组分块
来源：http://jlv.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ubk.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://fyy.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://puz.jinqigufen.top

[U112] JS：字符串补位
来源：http://qgf.havefunace.top

"7".padStart(3, "0")
来源：http://ewb.52xcode.cn

[U113] JS：正则替换全部
来源：http://pbc.yueranfly.top

s.replaceAll("a", "b")
来源：http://zwd.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://umj.xylfe.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ofj.yuanzhike.top

[U115] JS：生成 UUID
来源：http://xce.aizwys.cn

crypto.randomUUID()
来源：http://hyi.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://rbb.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://ezn.yuanzhike.top

[U117] JS：单元测试
来源：http://ygt.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://sbg.cdnleiting.top

[U118] JS：开发服务器
来源：http://nsh.andypj.xyz

npm i -D vite;  npx vite
来源：http://nwq.jqgfzy.top

[U119] JS：生产构建
来源：http://bho.hcnkem.com

npx vite build
来源：http://ldd.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://txt.hywenlv.cn

import.meta.env.VITE_API_URL
来源：http://tya.tianlin.xyz

================================================================================
来源：http://jur.yuxming.cn

统计汇总
来源：http://phq.ybcxt.top

================================================================================
来源：http://jev.aibaodan.cn

按语言统计（条）：
来源：http://jho.jinqigfzy.top

Python ......... 252
来源：http://zkn.nanxuanxn.top

PHP ............ 252
来源：http://cos.jinghuilouyu.cn

JavaScript ..... 252
来源：http://gwt.yvedp.cn

TypeScript ..... 212
来源：http://hfr.zhijiandao.cn

Java ........... 212
来源：http://gnj.yuxming.cn

Go ............. 212
来源：http://eci.chenzaomai.com

Ruby ........... 212
来源：http://uob.xingfuxueyuan.xyz

C# ............. 212
来源：http://lwv.zhoulong.xyz

C .............. 30
来源：http://xvw.feifeiyinyue.top

C++ ............ 30
来源：http://lbn.guowangkeji.top

SQL ............ 90
来源：http://cqq.vehdjk.com

Bash ........... 80
来源：http://ino.yj20258.top

Kotlin ......... 15
来源：http://xfa.nanxuanxn.top

Swift .......... 15
来源：http://vjk.cashguo.top

Lua ............ 10
来源：http://qlj.kuanghao11.cn

Perl ........... 10
来源：http://iew.fehbvm.com

Scala .......... 10
来源：http://zag.yj202588.top

------------------------------------
来源：http://xtf.jinqigufen.top

合计 ........... 2106 条
来源：http://van.redwolf501.top

按章节统计：
来源：http://rkx.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bjy.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pog.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fcy.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xyg.hnqzz.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://msl.pycfn.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vod.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ivm.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ghv.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://diu.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tvq.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rxp.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dsi.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oit.zhiwuduotai.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pei.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qes.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kae.daria6918.cn

Q SQL 专题                              90
来源：http://nys.jinqigfzy.top

R Bash 专题                             80
来源：http://owj.cdnleiting.top

S C / C++ 专题                          60
来源：http://aly.andypj.xyz

T 其他语言补充                          60
来源：http://ust.cashguo.top

U 高频实用片段                         120
来源：http://gow.sweek.top

------------------------------------
来源：http://zbw.ctjpmb.com

合计                                  2106 条
来源：http://ksw.mhx1999.top

--------------------------------------------------------------------------------
来源：http://jze.fengsongda.top

使用提醒
来源：http://etu.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://hgz.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nhz.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://clq.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hns.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gjf.wangdashe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jkw.aibaodan.cn

—— 文件结束 ——
来源：http://mjy.cashguo.top

================================================================================
来源：http://quw.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://opz.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://ond.tarul.cn

================================================================================
来源：http://qlf.cashguo.top

【收录内容】
来源：http://krb.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cnj.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fjb.tian-w.cn

SQL · Bash · C · C++
来源：http://lus.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fgp.yonumen.top

【使用说明】
来源：http://crx.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://klb.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jfz.jianghu66.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mvn.316326.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wru.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://dbp.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nqr.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mlz.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gfh.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nyg.wangshuangyany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://opo.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uzg.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fxd.fzhhl.top

【文件统计】
来源：http://qeo.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xrt.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://zao.shanyushiyangtech.top

目  录
来源：http://gni.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://fae.gogol.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ztl.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tqt.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iax.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://deq.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tum.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gxj.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pyc.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nev.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xzz.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dqh.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qiw.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yey.jiagoushi.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wvg.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gnu.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hsd.vqdsnc.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bwb.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sgf.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qsk.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yue.hnqzz.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fou.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xae.hnqzz.top

================================================================================
来源：http://hpv.wangdashe.top

A. 基础语法与类型
来源：http://rte.ybcxt.top

================================================================================
来源：http://pdr.52xcode.cn

[A01] Hello World
来源：http://jsc.chenzaomai.com

Py:   print("Hello, World!")
来源：http://gif.birdmap.top

PHP:  echo "Hello, World!";
来源：http://hay.ydjk.org.cn

JS:   console.log("Hello, World!");
来源：http://ttg.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hun.yueranfly.top

Java: System.out.println("Hello, World!");
来源：http://gni.wangdashe.top

Go:   fmt.Println("Hello, World!")
来源：http://xsf.shuidangran.top

Ruby: puts "Hello, World!"
来源：http://udq.zhengqikj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://yku.fengsongda.top

[A02] 变量声明与赋值
来源：http://jmr.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tnz.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://egu.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://ksn.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://afn.zycfv.cn

Java: String name = "Alex"; int age = 20;
来源：http://wxq.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://wtt.gotoacloud.top

Ruby: name = "Alex"; age = 20
来源：http://xzx.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://ubr.yueranfly.top

[A03] 常量定义
来源：http://lcf.tian-w.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ehl.uphjek.com

PHP:  const PI = 3.14159;
来源：http://zbt.ywan-chungtsiang.top

JS:   const PI = 3.14159;
来源：http://ozy.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://xfy.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://zds.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://ktg.hcnkem.com

Ruby: PI = 3.14159
来源：http://cph.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://sut.fanxiaobao.xyz

[A04] 判断变量类型
来源：http://nkd.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://qrd.svipenyu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qjw.hywenlv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sgf.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://ktr.zdqjudy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dby.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://wav.shanyushiyangtech.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zfa.jqgufenzy.top

C#:   x.GetType().Name; x is int
来源：http://pbq.52xcode.cn

[A05] 整数除法与取模
来源：http://tay.chenzaomai.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rre.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bip.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jvm.xylfe.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lnk.yonumen.top

Java: 7 / 2; 7 % 2
来源：http://jif.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://ohn.ctjpmb.com

Ruby: 7 / 2; 7 % 2
来源：http://bsz.jiagoushi.top

C#:   7 / 2; 7 % 2
来源：http://brc.fktsv.cn

[A06] 字符串转数字
来源：http://ivg.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://esz.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://egr.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cmj.epnwcf.com

TS:   parseInt("42", 10); Number("42")
来源：http://ijr.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cwr.guannengcc.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bba.xziqi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lgr.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rla.tian-w.cn

[A07] 数字转字符串
来源：http://mbv.xingfuxueyuan.xyz

Py:   str(42)
来源：http://tqx.pengpengdd.cyou

PHP:  (string) 42; strval(42)
来源：http://xfs.sweek.top

JS:   String(42); (42).toString()
来源：http://aob.cheryme.top

TS:   String(42)
来源：http://czq.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ckd.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://qrs.aibaodan.cn

Ruby: 42.to_s
来源：http://ycx.yonumen.top

C#:   42.ToString()
来源：http://jli.jinyuanbaomall.cn

[A08] 取整与四舍五入
来源：http://wjj.guowangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gna.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://igy.xziqi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kgb.hfpthk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jfz.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ktr.bbcook.cn


<!-- 参考信息 -->