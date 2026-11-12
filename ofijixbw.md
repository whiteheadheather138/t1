代发 wailian999

[U53] PHP：空合并运算符
来源：http://lfs.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://qlv.ivvv.top

[U54] PHP：空安全调用
来源：http://sqd.jinqigfzy.top

$obj?->method()
来源：http://xtl.hywenlv.cn

[U55] PHP：match 表达式
来源：http://wah.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pxv.yanxiufei.cn

[U56] PHP：命名参数
来源：http://quk.ybcxt.top

f(a: 1, b: 2)
来源：http://dat.fehbvm.com

[U57] PHP：字符串插值
来源：http://xxq.chenjidiqi.icu

"值: {$a}"
来源：http://kjq.meibo888.top

[U58] PHP：数组三件套
来源：http://tmy.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mfu.dashuyun.cn

[U59] PHP：自定义排序
来源：http://eem.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcm.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://vxq.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://veb.sxryk.cn

[U61] PHP：正则
来源：http://lex.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vlu.fktsv.cn

[U62] PHP：日期对象
来源：http://zjc.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vqg.chenlongwang.top

[U63] PHP：文件读写
来源：http://eqk.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yqn.yj20258.top

[U64] PHP：目录遍历
来源：http://qmv.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://nck.shangyingyoupin.top

[U65] PHP：会话
来源：http://phy.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ozh.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://owb.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://udm.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://lcm.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qhf.c1oappe.top

[U68] PHP：PDO 连接
来源：http://twa.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lbo.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://gaj.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xcd.pycfn.com

[U70] PHP：PDO 事务
来源：http://oej.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mbk.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://xfl.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://vjf.chenlongwang.top

[U72] PHP：写错误日志
来源：http://lvu.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://lpj.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://tru.tanke756.top

parse_ini_file("config.ini", true)
来源：http://zvt.daria6918.cn

[U74] PHP：读取环境变量
来源：http://hyc.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://dhl.uphjek.com

[U75] PHP：依赖注入
来源：http://jgn.cdnleiting.top

composer require psr/container
来源：http://nzl.shangyingyoupin.top

[U76] PHP：简单路由
来源：http://dit.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://epw.316326.xyz

[U77] PHP：模板渲染
来源：http://thc.fengsongda.top

composer require twig/twig
来源：http://xmt.feifeiyinyue.top

[U78] PHP：单元测试
来源：http://hty.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://ims.iojbl.cn

[U79] PHP：静态分析
来源：http://rtz.jyoumei.cn

composer require --dev phpstan/phpstan
来源：http://noj.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://wsq.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wmb.fktsv.cn

[U81] JS：初始化项目
来源：http://qkp.yj20258888.top

npm init -y;  npm i express
来源：http://kxa.cheryme.top

[U82] JS：package.json 脚本
来源：http://hib.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zzi.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://gyo.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qhh.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://olj.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://ghp.zycfv.cn

[U85] JS：可选链
来源：http://ufy.ybcxt.top

a?.b?.c
来源：http://blg.cucudq.cn

[U86] JS：空值合并
来源：http://qcl.zhixingplan.top

a ?? b
来源：http://uny.ydjk.org.cn

[U87] JS：解构默认值
来源：http://rpm.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://jtr.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://ivh.jqgufenzy.top

{ ...a, ...b }
来源：http://xbw.bjfxy.top

[U89] JS：数组去重
来源：http://szw.aibaodan.cn

[...new Set(arr)]
来源：http://jiw.ehwqpu.com

[U90] JS：数字数组排序
来源：http://kli.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://pkw.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://mml.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zju.quarkkingdee.top

[U92] JS：深拷贝
来源：http://qkw.yfazqb.com

structuredClone(obj)
来源：http://tgh.ydzc1.top

[U93] JS：模板字符串
来源：http://axd.52xcode.cn

`共 ${n} 条`
来源：http://asl.fengsongda.top

[U94] JS：箭头函数
来源：http://sso.guowangkeji.top

const double = x => x * 2;
来源：http://qjj.chenlongwang.top

[U95] JS：Promise 包装
来源：http://ubn.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://ddt.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://mdz.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sem.zhongyouzk.top

[U97] JS：并发请求
来源：http://xoz.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pfa.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://xjy.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qbf.hnqzz.top

[U99] JS：事件监听
来源：http://khh.jianghu66.top

el.addEventListener("click", e => {})
来源：http://elk.hywenlv.cn

[U100] JS：DOM 查询
来源：http://lnn.yueranfly.top

document.querySelector(".item")
来源：http://ifn.fehbvm.com

[U101] JS：classList 操作
来源：http://lvj.ehwqpu.com

el.classList.toggle("active")
来源：http://zif.meibo888.top

[U102] JS：本地存储
来源：http://jzx.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oyc.chenzaomai.com

[U103] JS：定时器
来源：http://bhw.jqgfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mbu.cheryme.top

[U104] JS：防抖
来源：http://nmh.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vjm.epnwcf.com

[U105] JS：节流
来源：http://kyy.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wkd.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://pqx.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sub.sxryk.cn

[U107] JS：数字千分位
来源：http://wok.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fgt.shuidangran.top

[U108] JS：随机整数
来源：http://zbb.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blk.birdmap.top

[U109] JS：数组分组
来源：http://tqv.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://qon.cqqwz.cn

[U110] JS：数组分块
来源：http://foo.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hjj.yueranfly.top

[U111] JS：对象转 Map
来源：http://rda.chenlongwang.top

new Map(Object.entries(obj))
来源：http://edz.xuanzx.com

[U112] JS：字符串补位
来源：http://pjg.hywenlv.cn

"7".padStart(3, "0")
来源：http://xkb.yangfankeji.com

[U113] JS：正则替换全部
来源：http://fww.sxryk.cn

s.replaceAll("a", "b")
来源：http://ygw.fehbvm.com

[U114] JS：JSON 深比较
来源：http://zdw.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgk.zhengqikj.top

[U115] JS：生成 UUID
来源：http://usw.c1oappe.top

crypto.randomUUID()
来源：http://vle.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://jtl.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://clf.redwolf501.top

[U117] JS：单元测试
来源：http://uez.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://bla.yvedp.cn

[U118] JS：开发服务器
来源：http://ulo.aibaodan.cn

npm i -D vite;  npx vite
来源：http://kxe.meibo888.top

[U119] JS：生产构建
来源：http://uka.bbcook.cn

npx vite build
来源：http://uiv.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://gmg.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://ujl.dashuyun.cn

================================================================================
来源：http://mzp.yj20258888.top

统计汇总
来源：http://dkr.gogol.net.cn

================================================================================
来源：http://xri.cheryme.top

按语言统计（条）：
来源：http://auf.quarkkingdee.top

Python ......... 252
来源：http://tih.jlsjyb.cn

PHP ............ 252
来源：http://xqp.aibaodan.cn

JavaScript ..... 252
来源：http://trx.cucudq.cn

TypeScript ..... 212
来源：http://ffp.yueranfly.top

Java ........... 212
来源：http://nze.jiagoushi.top

Go ............. 212
来源：http://yna.fktsv.cn

Ruby ........... 212
来源：http://hzj.tian-w.cn

C# ............. 212
来源：http://url.yueranfly.top

C .............. 30
来源：http://chi.jlsjyb.cn

C++ ............ 30
来源：http://oqn.yuxming.cn

SQL ............ 90
来源：http://enb.sufxvd.cn

Bash ........... 80
来源：http://dtl.tarul.cn

Kotlin ......... 15
来源：http://coh.ybcxt.top

Swift .......... 15
来源：http://npo.yj202588.top

Lua ............ 10
来源：http://vad.jiagoushi.top

Perl ........... 10
来源：http://noa.daxiang520.top

Scala .......... 10
来源：http://wut.hammf.cn

------------------------------------
来源：http://qgb.ivvv.top

合计 ........... 2106 条
来源：http://avp.yj20258.top

按章节统计：
来源：http://hoq.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nhv.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lzo.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://srh.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wmt.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eco.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vjz.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ygu.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rek.chenjidiqi.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rql.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://loe.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vzk.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qur.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vpl.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xpd.vqdsnc.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://umx.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ibw.nanxinkj.top

Q SQL 专题                              90
来源：http://osr.snrcjt.cn

R Bash 专题                             80
来源：http://lca.jinyuanbaomall.cn

S C / C++ 专题                          60
来源：http://ogs.nanxinkj.top

T 其他语言补充                          60
来源：http://mir.zhengqikj.top

U 高频实用片段                         120
来源：http://xfp.yangfankeji.com

------------------------------------
来源：http://lwg.vqdsnc.cn

合计                                  2106 条
来源：http://vxa.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://azo.zhongyouzk.top

使用提醒
来源：http://prq.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://vmt.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ewp.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wnp.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ntb.dashuyun.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://snl.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bma.yuanzhike.top

—— 文件结束 ——
来源：http://scd.tarul.cn

================================================================================
来源：http://ese.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://nqy.yuxming.cn

Common Programming Examples Cheat Book
来源：http://bjo.chenjidiqi.icu

================================================================================
来源：http://emp.pengpengdd.cyou

【收录内容】
来源：http://mzx.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://ntw.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://frw.vehdjk.com

SQL · Bash · C · C++
来源：http://ngc.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mpl.jyoumei.cn

【使用说明】
来源：http://zfn.cqqwz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kca.birdmap.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ycp.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kuc.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wqs.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://mxt.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ydo.yfazqb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tpi.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xot.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mby.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pmp.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://czw.nwbrower.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mmk.jqgfzy.top

【文件统计】
来源：http://etp.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lhs.sxryk.cn

--------------------------------------------------------------------------------
来源：http://vfl.nanxinkj.top

目  录
来源：http://dfm.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://tlo.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://emw.chenzaomai.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rbd.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kwk.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://can.haohaochexian.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jto.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ker.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://abb.hywenlv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://edr.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wqx.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qxd.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dyo.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ese.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ply.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gmn.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dld.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hhh.uphjek.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jkm.yangfankeji.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://obd.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wfk.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ddm.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pqr.shuidangran.top

================================================================================
来源：http://bzj.mhx1999.top

A. 基础语法与类型
来源：http://oip.fzhhl.top

================================================================================
来源：http://auh.hywenlv.cn

[A01] Hello World
来源：http://hva.yonumen.top

Py:   print("Hello, World!")
来源：http://gye.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://mba.ivvv.top

JS:   console.log("Hello, World!");
来源：http://oyu.zhiwuduotai.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fgr.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://hvl.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://qjs.gzhubu.top

Ruby: puts "Hello, World!"
来源：http://pht.xuanzx.com

C#:   Console.WriteLine("Hello, World!");
来源：http://wtz.cdnleiting.top

[A02] 变量声明与赋值
来源：http://fdk.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rgm.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vfc.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://jxv.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://btz.fehbvm.com

Java: String name = "Alex"; int age = 20;
来源：http://ren.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://fpo.nanxuanxn.top

Ruby: name = "Alex"; age = 20
来源：http://dly.xingfuxueyuan.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://mvt.jqgufenzy.top

[A03] 常量定义
来源：http://dgo.wangdashe.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pbl.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://noi.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://jyl.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://tti.yj20258.top

Java: static final double PI = 3.14159;
来源：http://kyq.shanyushiyangtech.top

Go:   const PI = 3.14159
来源：http://kcj.tianlin.xyz

Ruby: PI = 3.14159
来源：http://inv.wangdashe.top

C#:   const double PI = 3.14159;
来源：http://ozh.vqdsnc.cn

[A04] 判断变量类型
来源：http://kjb.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://xra.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ybt.hnxiangtu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eef.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://tje.yonumen.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dzb.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oxl.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://rlh.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://qac.pycfn.com

[A05] 整数除法与取模
来源：http://ett.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hdr.wangshuangyany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cev.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nus.chenlongwang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bbr.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://ccr.wangdashe.top

Go:   7 / 2; 7 % 2
来源：http://gsy.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://wkc.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://zzp.tanke756.top

[A06] 字符串转数字
来源：http://mmz.dianchejie.cn

Py:   int("42"); float("3.14")
来源：http://tek.aibaodan.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://txd.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://efd.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://cpy.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qux.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aqw.zdqjudy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zuw.andypj.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wlt.nwbrower.top

[A07] 数字转字符串
来源：http://woj.guowangkeji.top

Py:   str(42)
来源：http://ysz.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://jpr.xylfe.cn


<!-- 参考信息 -->