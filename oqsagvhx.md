代发 wailian999

[U61] PHP：正则
来源：http://nke.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ocr.shzxlz.cn

[U62] PHP：日期对象
来源：http://wez.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ioo.sjlbkw.cn

[U63] PHP：文件读写
来源：http://ynu.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ofl.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://gze.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://nlq.sxryk.cn

[U65] PHP：会话
来源：http://ukc.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ico.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://ptu.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qtd.bbcook.cn

[U67] PHP：处理文件上传
来源：http://epu.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tje.smart0.xyz

[U68] PHP：PDO 连接
来源：http://mhf.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ptb.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://eiu.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cse.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://zra.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://stq.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://dab.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://dji.hfpthk.cn

[U72] PHP：写错误日志
来源：http://mee.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://ill.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://ejd.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://fmk.havefunace.top

[U74] PHP：读取环境变量
来源：http://crl.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://kko.iojbl.cn

[U75] PHP：依赖注入
来源：http://dkl.jqgufenzy.top

composer require psr/container
来源：http://off.tian-w.cn

[U76] PHP：简单路由
来源：http://oos.svipenyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kjk.gzhubu.top

[U77] PHP：模板渲染
来源：http://klr.zhengqikj.top

composer require twig/twig
来源：http://gyx.sjlbkw.cn

[U78] PHP：单元测试
来源：http://oot.uphjek.com

composer require --dev phpunit/phpunit
来源：http://umi.fzhhl.top

[U79] PHP：静态分析
来源：http://nlp.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://qlk.cheryme.top

[U80] PHP：代码规范修复
来源：http://ohz.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tzi.chenzaomai.com

[U81] JS：初始化项目
来源：http://lih.tian-w.cn

npm init -y;  npm i express
来源：http://vdf.hcnkem.com

[U82] JS：package.json 脚本
来源：http://dbz.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qtg.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://bbz.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://yog.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://heo.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zuq.bbcook.cn

[U85] JS：可选链
来源：http://kxy.ppjwa.cn

a?.b?.c
来源：http://yhs.ehwqpu.com

[U86] JS：空值合并
来源：http://jae.nwbrower.top

a ?? b
来源：http://qdj.hcnkem.com

[U87] JS：解构默认值
来源：http://jsl.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://uia.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://iba.zhengqikj.top

{ ...a, ...b }
来源：http://lkc.sjlbkw.cn

[U89] JS：数组去重
来源：http://kvz.yj20258888.top

[...new Set(arr)]
来源：http://fmp.gogol.net.cn

[U90] JS：数字数组排序
来源：http://ahr.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://ykm.shuidangran.top

[U91] JS：对象键值遍历
来源：http://hup.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wcg.jiagoushi.top

[U92] JS：深拷贝
来源：http://tyk.zdqjudy.top

structuredClone(obj)
来源：http://jlz.vehdjk.com

[U93] JS：模板字符串
来源：http://ywb.c1oappe.top

`共 ${n} 条`
来源：http://mei.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://dpp.shangyingyoupin.top

const double = x => x * 2;
来源：http://mof.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://hnz.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://sam.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://gqy.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://afj.chenzaomai.com

[U97] JS：并发请求
来源：http://pqe.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ghe.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://jlo.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mwe.vqdsnc.cn

[U99] JS：事件监听
来源：http://ict.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://kux.hcnkem.com

[U100] JS：DOM 查询
来源：http://bgh.jinghuilouyu.cn

document.querySelector(".item")
来源：http://sgh.shzxlz.cn

[U101] JS：classList 操作
来源：http://jrl.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://dwg.chenlongwang.top

[U102] JS：本地存储
来源：http://vef.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xkg.iojbl.cn

[U103] JS：定时器
来源：http://egm.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nlj.52xcode.cn

[U104] JS：防抖
来源：http://usj.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nky.ctjpmb.com

[U105] JS：节流
来源：http://fen.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tvg.nanxuanxn.top

[U106] JS：日期格式化
来源：http://vvz.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://muf.gotoacloud.top

[U107] JS：数字千分位
来源：http://xnq.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vnd.xuanzx.com

[U108] JS：随机整数
来源：http://cba.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xjc.gotoacloud.top

[U109] JS：数组分组
来源：http://tnm.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://shj.gotoacloud.top

[U110] JS：数组分块
来源：http://mwl.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://amt.aibaodan.cn

[U111] JS：对象转 Map
来源：http://cuz.yj20258.top

new Map(Object.entries(obj))
来源：http://ido.daxiang520.top

[U112] JS：字符串补位
来源：http://jfu.hywenlv.cn

"7".padStart(3, "0")
来源：http://itu.sysykeji.top

[U113] JS：正则替换全部
来源：http://lio.cucudq.cn

s.replaceAll("a", "b")
来源：http://cxs.yfazqb.com

[U114] JS：JSON 深比较
来源：http://jjg.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iol.yueranfly.top

[U115] JS：生成 UUID
来源：http://vdy.hywenlv.cn

crypto.randomUUID()
来源：http://rai.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://yzf.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://ltx.uphjek.com

[U117] JS：单元测试
来源：http://epj.sweek.top

npm i -D vitest;  npx vitest
来源：http://jep.aibaodan.cn

[U118] JS：开发服务器
来源：http://bpf.zhixingplan.top

npm i -D vite;  npx vite
来源：http://gvf.zhijiandao.cn

[U119] JS：生产构建
来源：http://brj.yanxiufei.cn

npx vite build
来源：http://hvn.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://ail.hnxiangtu.top

import.meta.env.VITE_API_URL
来源：http://cgq.hongshengwenyu.top

================================================================================
来源：http://dqy.meibo888.top

统计汇总
来源：http://zub.chenzaomai.com

================================================================================
来源：http://jql.tianlin.xyz

按语言统计（条）：
来源：http://gbg.tanke756.top

Python ......... 252
来源：http://ijj.xuetiantiany.cn

PHP ............ 252
来源：http://rfg.nwbrower.top

JavaScript ..... 252
来源：http://ccj.yfazqb.com

TypeScript ..... 212
来源：http://gba.daria6918.cn

Java ........... 212
来源：http://owf.jinqigufen.top

Go ............. 212
来源：http://xss.aibaodan.cn

Ruby ........... 212
来源：http://xwb.cheryme.top

C# ............. 212
来源：http://yca.svipenyu.cn

C .............. 30
来源：http://ovf.iojbl.cn

C++ ............ 30
来源：http://lpu.wangshuangyany.cn

SQL ............ 90
来源：http://guf.sxryk.cn

Bash ........... 80
来源：http://wqk.fehbvm.com

Kotlin ......... 15
来源：http://ntq.fanxiaobao.xyz

Swift .......... 15
来源：http://jmp.hnxiangtu.top

Lua ............ 10
来源：http://bak.zhiwuduotai.top

Perl ........... 10
来源：http://qnu.yongpay.top

Scala .......... 10
来源：http://wtm.jyoumei.cn

------------------------------------
来源：http://cui.havefunace.top

合计 ........... 2106 条
来源：http://bsh.cheryme.top

按章节统计：
来源：http://xgt.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kul.zdbjq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pxo.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iqu.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wrq.yangfankeji.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jho.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vkq.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tia.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://njb.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nyw.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cjy.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tto.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://orl.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pgt.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pim.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kqa.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://liz.zhiwuduotai.top

Q SQL 专题                              90
来源：http://gup.jiagoushi.top

R Bash 专题                             80
来源：http://mer.zdbjq.cn

S C / C++ 专题                          60
来源：http://zhs.gaohongyu789.top

T 其他语言补充                          60
来源：http://dcr.yj20258.top

U 高频实用片段                         120
来源：http://skg.yangfankeji.com

------------------------------------
来源：http://jri.bjfxy.top

合计                                  2106 条
来源：http://fda.tarul.cn

--------------------------------------------------------------------------------
来源：http://cge.ywan-chungtsiang.top

使用提醒
来源：http://gwk.hammf.cn

--------------------------------------------------------------------------------
来源：http://ffr.chenjidiqi.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qcy.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xoc.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ddf.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jdm.kuanghao11.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://snw.sysykeji.top

—— 文件结束 ——
来源：http://jdl.cucudq.cn

================================================================================
来源：http://uxd.daria6918.cn

程序语言常见例子速查手册（2024 版）
来源：http://clf.yfazqb.com

Common Programming Examples Cheat Book
来源：http://tni.wangshuangyany.cn

================================================================================
来源：http://nto.iojbl.cn

【收录内容】
来源：http://kdb.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ovd.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ywl.ehwqpu.com

SQL · Bash · C · C++
来源：http://fvu.tianlin.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iqo.ivvv.top

【使用说明】
来源：http://qwe.chenjidiqi.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://erp.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oda.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fij.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://slf.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tiw.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://doy.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ejy.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cse.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eft.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zhk.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bkr.mhx1999.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qxn.cqqwz.cn

【文件统计】
来源：http://zsq.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yxz.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://pgw.chenzaomai.com

目  录
来源：http://enz.sxryk.cn

--------------------------------------------------------------------------------
来源：http://rmw.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nja.jyoumei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ims.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iex.fktsv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uwm.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lpp.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ete.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://knv.ehwqpu.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xrh.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eop.wangshuangyany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ajf.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://okv.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fdb.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jlc.hongshengwenyu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pur.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wkr.jianghu66.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://loh.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://drl.yuanzhike.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jlm.ctjpmb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uzs.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://shm.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eud.ppjwa.cn

================================================================================
来源：http://crp.fehbvm.com

A. 基础语法与类型
来源：http://xfk.birdmap.top

================================================================================
来源：http://mrr.zdbjq.cn

[A01] Hello World
来源：http://ikt.hongshengwenyu.top

Py:   print("Hello, World!")
来源：http://afc.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://otj.dashuyun.cn

JS:   console.log("Hello, World!");
来源：http://otb.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eao.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://gly.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://yjx.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://pbv.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://sbd.316326.xyz

[A02] 变量声明与赋值
来源：http://uwj.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zir.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://eoe.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eid.meibo888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wzj.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://syi.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://icx.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://azu.shuidangran.top

C#:   string name = "Alex"; int age = 20;
来源：http://ipp.bbcook.cn

[A03] 常量定义
来源：http://fkf.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qfv.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://hzy.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://tib.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://cmm.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://hzc.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://qwn.xuanzx.com

Ruby: PI = 3.14159
来源：http://uxw.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://qex.hysaishi.cn

[A04] 判断变量类型
来源：http://bxn.nanxuanxn.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rdb.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nzs.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zju.redwolf501.top

TS:   typeof x; x instanceof Date
来源：http://hxg.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rkf.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://fgh.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://liq.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://nnc.dianchejie.cn

[A05] 整数除法与取模
来源：http://mqv.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bbz.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nss.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ecr.nanxinkj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zux.jqgufenzy.top

Java: 7 / 2; 7 % 2
来源：http://fbi.shanyushiyangkeji.top

Go:   7 / 2; 7 % 2
来源：http://ycy.ydjk.org.cn

Ruby: 7 / 2; 7 % 2
来源：http://hhz.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://dbo.dashuyun.cn

[A06] 字符串转数字
来源：http://zkq.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://gjs.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wtf.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mpz.snrcjt.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wyy.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ydw.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rvs.guannengcc.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zjd.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ubg.cheryme.top

[A07] 数字转字符串
来源：http://yzf.c1oappe.top

Py:   str(42)
来源：http://utf.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://ifm.nwbrower.top

JS:   String(42); (42).toString()
来源：http://pqi.hnqzz.top

TS:   String(42)
来源：http://tll.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xrs.guowangkeji.top

Go:   strconv.Itoa(42)
来源：http://srl.zhiwuduotai.top

Ruby: 42.to_s
来源：http://kfw.aibaodan.cn

C#:   42.ToString()
来源：http://eyv.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://yvk.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vbi.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://txg.xuetiantiany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mjb.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xiv.9152youxi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rnu.pycfn.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wdl.guannengcc.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xcu.hywenlv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ffn.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://muz.yongpay.top


<!-- 参考信息 -->