代发 wailian999

[U57] PHP：字符串插值
来源：http://kau.zhiwuduotai.top

"值: {$a}"
来源：http://obf.nanxinkj.top

[U58] PHP：数组三件套
来源：http://fqk.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://utt.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://vza.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dvr.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://ypv.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lbp.hywenlv.cn

[U61] PHP：正则
来源：http://pnq.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sce.aizwys.cn

[U62] PHP：日期对象
来源：http://ccg.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zfa.nwbrower.top

[U63] PHP：文件读写
来源：http://zke.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qhp.zhixingplan.top

[U64] PHP：目录遍历
来源：http://hdp.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://yin.wangdashe.top

[U65] PHP：会话
来源：http://frl.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://als.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://elv.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://awu.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://hnx.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wlb.cheryme.top

[U68] PHP：PDO 连接
来源：http://tjw.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zcb.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://eeb.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ksr.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://olo.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dqy.chenzaomai.com

[U71] PHP：抛出异常
来源：http://qta.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://ljx.nwbrower.top

[U72] PHP：写错误日志
来源：http://xam.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://eoo.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://gsg.cheryme.top

parse_ini_file("config.ini", true)
来源：http://ylv.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://mrx.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://xxl.jinqigufen.top

[U75] PHP：依赖注入
来源：http://jae.tanke756.top

composer require psr/container
来源：http://sox.cheryme.top

[U76] PHP：简单路由
来源：http://sbb.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uth.vehdjk.com

[U77] PHP：模板渲染
来源：http://agj.dashuyun.cn

composer require twig/twig
来源：http://wyo.havefunace.top

[U78] PHP：单元测试
来源：http://pcw.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://isy.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://nzp.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://ing.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://mww.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://byv.haohaochexian.top

[U81] JS：初始化项目
来源：http://yls.yj20258.top

npm init -y;  npm i express
来源：http://nqu.xinyue.icu

[U82] JS：package.json 脚本
来源：http://whc.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://afy.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://hpx.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://gwx.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://oaq.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://drh.xylfe.cn

[U85] JS：可选链
来源：http://ael.jinqigfzy.top

a?.b?.c
来源：http://rxa.bbcook.cn

[U86] JS：空值合并
来源：http://ksv.yj20258888.top

a ?? b
来源：http://rkd.9152youxi.cn

[U87] JS：解构默认值
来源：http://xiy.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://glc.aibaodan.cn

[U88] JS：对象展开合并
来源：http://ilc.birdmap.top

{ ...a, ...b }
来源：http://uvk.andypj.xyz

[U89] JS：数组去重
来源：http://flw.wangshuangyany.cn

[...new Set(arr)]
来源：http://fvn.sweek.top

[U90] JS：数字数组排序
来源：http://lvd.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://vdv.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://qgk.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xlo.hnqzz.top

[U92] JS：深拷贝
来源：http://ynr.iojbl.cn

structuredClone(obj)
来源：http://hsq.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://byc.yongpay.top

`共 ${n} 条`
来源：http://oou.shuidangran.top

[U94] JS：箭头函数
来源：http://gvw.316326.xyz

const double = x => x * 2;
来源：http://ejj.gzhubu.top

[U95] JS：Promise 包装
来源：http://fqx.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://tcl.birdmap.top

[U96] JS：async/await 与异常
来源：http://mzc.c1oappe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yyf.ivvv.top

[U97] JS：并发请求
来源：http://abs.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gui.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://ycc.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uvf.meibo888.top

[U99] JS：事件监听
来源：http://yyh.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://jho.fzhhl.top

[U100] JS：DOM 查询
来源：http://vaf.jinghuilouyu.cn

document.querySelector(".item")
来源：http://svk.yj202588.top

[U101] JS：classList 操作
来源：http://hrv.tian-w.cn

el.classList.toggle("active")
来源：http://vnk.cashguo.top

[U102] JS：本地存储
来源：http://sjh.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kdj.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://shq.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cas.fzhhl.top

[U104] JS：防抖
来源：http://asr.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xje.hesvh.cn

[U105] JS：节流
来源：http://cpa.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oet.yonumen.top

[U106] JS：日期格式化
来源：http://jxu.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hps.yueranfly.top

[U107] JS：数字千分位
来源：http://rtm.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oon.ybcxt.top

[U108] JS：随机整数
来源：http://vjn.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bcp.jiagoushi.top

[U109] JS：数组分组
来源：http://yvi.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://fsk.bjfxy.top

[U110] JS：数组分块
来源：http://vos.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xlf.yj20258.top

[U111] JS：对象转 Map
来源：http://buo.jqgfzy.top

new Map(Object.entries(obj))
来源：http://tfs.zhengqikj.top

[U112] JS：字符串补位
来源：http://ysn.tarul.cn

"7".padStart(3, "0")
来源：http://wze.sweek.top

[U113] JS：正则替换全部
来源：http://utx.svipenyu.cn

s.replaceAll("a", "b")
来源：http://mtl.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://pfz.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jku.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://llq.gogol.net.cn

crypto.randomUUID()
来源：http://jzm.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://qan.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://ecf.epnwcf.com

[U117] JS：单元测试
来源：http://fkf.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://izl.yj202588.top

[U118] JS：开发服务器
来源：http://vrg.hnqzz.top

npm i -D vite;  npx vite
来源：http://syd.zhijiandao.cn

[U119] JS：生产构建
来源：http://btn.dianchejie.cn

npx vite build
来源：http://gxu.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ehk.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://ppr.cdnleiting.top

================================================================================
来源：http://vda.zdbjq.cn

统计汇总
来源：http://jna.sweek.top

================================================================================
来源：http://kuk.c1oappe.top

按语言统计（条）：
来源：http://sqh.chenlongwang.top

Python ......... 252
来源：http://xwz.shzxlz.cn

PHP ............ 252
来源：http://zzw.pengpengdd.cyou

JavaScript ..... 252
来源：http://jcz.jqgfzy.top

TypeScript ..... 212
来源：http://eeh.andypj.xyz

Java ........... 212
来源：http://jom.yongpay.top

Go ............. 212
来源：http://vyt.pycfn.com

Ruby ........... 212
来源：http://rua.guannengcc.top

C# ............. 212
来源：http://ncp.pengpengdd.cyou

C .............. 30
来源：http://opf.fktsv.cn

C++ ............ 30
来源：http://ovj.quarkkingdee.top

SQL ............ 90
来源：http://hfj.chenlongwang.top

Bash ........... 80
来源：http://dro.gaohongyu789.top

Kotlin ......... 15
来源：http://ovo.316326.xyz

Swift .......... 15
来源：http://dvp.zhengqikj.top

Lua ............ 10
来源：http://rqg.uphjek.com

Perl ........... 10
来源：http://wnq.guowangkeji.top

Scala .......... 10
来源：http://iim.bbcook.cn

------------------------------------
来源：http://sfo.yuxming.cn

合计 ........... 2106 条
来源：http://jet.tianlin.xyz

按章节统计：
来源：http://pad.tarul.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uhu.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nqx.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rgx.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gmc.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ktp.guowangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zhk.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sru.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mrx.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://frx.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://syh.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ifk.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eer.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zsx.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tjn.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jiw.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lcm.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://qjn.epnwcf.com

R Bash 专题                             80
来源：http://ckt.cheryme.top

S C / C++ 专题                          60
来源：http://tdb.aibaodan.cn

T 其他语言补充                          60
来源：http://xcx.aizwys.cn

U 高频实用片段                         120
来源：http://pnp.chenlongwang.top

------------------------------------
来源：http://fsq.sweek.top

合计                                  2106 条
来源：http://jsq.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://bxu.feifeiyinyue.top

使用提醒
来源：http://xkd.wangdashe.top

--------------------------------------------------------------------------------
来源：http://lsc.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ems.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tcs.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vwa.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wwp.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qxh.gotoacloud.top

—— 文件结束 ——
来源：http://pzg.xuetiantiany.cn

================================================================================
来源：http://cqk.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://hps.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://vel.ppjwa.cn

================================================================================
来源：http://kmf.dashuyun.cn

【收录内容】
来源：http://tim.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rcr.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://can.zhoulong.xyz

SQL · Bash · C · C++
来源：http://vxy.tanke756.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yxm.hesvh.cn

【使用说明】
来源：http://rpl.zhiwuduotai.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vrx.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bbv.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ocs.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wbj.bbcook.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ilj.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ljm.jianghu66.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lqd.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ikw.nwbrower.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://enw.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ngq.redwolf501.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://krr.shanyushiyangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tqu.yueranfly.top

【文件统计】
来源：http://rzy.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iak.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://riu.yongpay.top

目  录
来源：http://agk.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://iza.yuxming.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ktn.tarul.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qhs.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://adr.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ver.chenlongwang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nyx.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uqc.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fzd.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yux.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sru.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nqe.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wqc.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jbb.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nce.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://txm.shuidangran.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fdp.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lol.yj20258888.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kdz.haohaochexian.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ibk.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tmb.jlsjyb.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hwe.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pgh.gotoacloud.top

================================================================================
来源：http://qtr.sysykeji.top

A. 基础语法与类型
来源：http://xna.gotoacloud.top

================================================================================
来源：http://sfz.chenzaomai.com

[A01] Hello World
来源：http://sah.yj202588.top

Py:   print("Hello, World!")
来源：http://btf.fehbvm.com

PHP:  echo "Hello, World!";
来源：http://lpa.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://cqj.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bac.52xcode.cn

Java: System.out.println("Hello, World!");
来源：http://sus.fanxiaobao.xyz

Go:   fmt.Println("Hello, World!")
来源：http://jlx.yongpay.top

Ruby: puts "Hello, World!"
来源：http://snk.feifeiyinyue.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tzw.tianlin.xyz

[A02] 变量声明与赋值
来源：http://niz.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iyv.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qrm.zdbjq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hvh.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rrq.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://mlg.gaohongyu789.top

Go:   name := "Alex"; age := 20
来源：http://kwc.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://con.shuidangran.top

C#:   string name = "Alex"; int age = 20;
来源：http://nts.zhixingplan.top

[A03] 常量定义
来源：http://qut.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lqb.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://slv.bbcook.cn

JS:   const PI = 3.14159;
来源：http://dgw.jqgfzy.top

TS:   const PI: number = 3.14159;
来源：http://qju.meibo888.top

Java: static final double PI = 3.14159;
来源：http://hsd.jiagoushi.top

Go:   const PI = 3.14159
来源：http://moh.daria6918.cn

Ruby: PI = 3.14159
来源：http://wdx.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://otm.iojbl.cn

[A04] 判断变量类型
来源：http://voo.xylfe.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mre.jinyuanbaomall.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gci.nwbrower.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jna.jianghu66.top

TS:   typeof x; x instanceof Date
来源：http://phm.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rjl.yanxiufei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iqz.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rrx.hywenlv.cn

C#:   x.GetType().Name; x is int
来源：http://fdr.cdnleiting.top

[A05] 整数除法与取模
来源：http://amk.guowangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bxm.pengpengdd.cyou

PHP:  intdiv(7, 2); 7 % 2
来源：http://azx.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yst.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://acw.jqgfzy.top

Java: 7 / 2; 7 % 2
来源：http://ijy.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://dmv.fktsv.cn

Ruby: 7 / 2; 7 % 2
来源：http://kvt.c1oappe.top

C#:   7 / 2; 7 % 2
来源：http://yrt.shzxlz.cn

[A06] 字符串转数字
来源：http://gxo.cheryme.top

Py:   int("42"); float("3.14")
来源：http://edk.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vtu.mhx1999.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uss.guowangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://cif.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kce.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gnc.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://teg.yj20258.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tyg.chenlongwang.top

[A07] 数字转字符串
来源：http://nnq.zdbjq.cn

Py:   str(42)
来源：http://qkh.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://mmd.zycfv.cn

JS:   String(42); (42).toString()
来源：http://lsb.hfpthk.cn

TS:   String(42)
来源：http://kqu.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vpd.iojbl.cn

Go:   strconv.Itoa(42)
来源：http://rdf.jinqigfzy.top

Ruby: 42.to_s
来源：http://plt.zhaomingkeji.xyz

C#:   42.ToString()
来源：http://yot.xuetiantiany.cn

[A08] 取整与四舍五入
来源：http://zhf.xylfe.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kxx.dashuyun.cn


<!-- 参考信息 -->