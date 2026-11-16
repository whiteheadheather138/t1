代发 wailian999

[U59] PHP：自定义排序
来源：http://esx.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oyq.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://uoq.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yud.nanxinkj.top

[U61] PHP：正则
来源：http://cjg.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fty.jyoumei.cn

[U62] PHP：日期对象
来源：http://bwb.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ztf.cqqwz.cn

[U63] PHP：文件读写
来源：http://irb.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gcz.meibo888.top

[U64] PHP：目录遍历
来源：http://xeg.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://lst.jqgufenzy.top

[U65] PHP：会话
来源：http://biw.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fpw.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://uji.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://obj.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://dsu.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tbe.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://ons.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gea.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://yky.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fah.tarul.cn

[U70] PHP：PDO 事务
来源：http://zcv.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vcj.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://jca.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://ncm.xinyue.icu

[U72] PHP：写错误日志
来源：http://vfo.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://dsz.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://odl.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://szu.hesvh.cn

[U74] PHP：读取环境变量
来源：http://bgq.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://ovd.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://dgs.gotoacloud.top

composer require psr/container
来源：http://ebr.meibo888.top

[U76] PHP：简单路由
来源：http://hkx.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zjt.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://akn.epnwcf.com

composer require twig/twig
来源：http://ymr.cdnleiting.top

[U78] PHP：单元测试
来源：http://bqx.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://nhd.ctjpmb.com

[U79] PHP：静态分析
来源：http://ypn.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://uab.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://piy.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jpk.hcnkem.com

[U81] JS：初始化项目
来源：http://mxd.iojbl.cn

npm init -y;  npm i express
来源：http://zjq.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://msk.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tmx.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://fdv.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://phy.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://osy.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://chw.yfazqb.com

[U85] JS：可选链
来源：http://sek.zdqjudy.top

a?.b?.c
来源：http://poj.tarul.cn

[U86] JS：空值合并
来源：http://xoe.shuidangran.top

a ?? b
来源：http://qik.sysykeji.top

[U87] JS：解构默认值
来源：http://jbx.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://jnk.c1oappe.top

[U88] JS：对象展开合并
来源：http://yoc.iojbl.cn

{ ...a, ...b }
来源：http://yma.shangyingyoupin.top

[U89] JS：数组去重
来源：http://pdo.cqqwz.cn

[...new Set(arr)]
来源：http://mvr.yvedp.cn

[U90] JS：数字数组排序
来源：http://wfg.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://kon.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://ohq.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://deq.uphjek.com

[U92] JS：深拷贝
来源：http://ryd.xuanzx.com

structuredClone(obj)
来源：http://krd.hfpthk.cn

[U93] JS：模板字符串
来源：http://jbf.tian-w.cn

`共 ${n} 条`
来源：http://rih.jianghu66.top

[U94] JS：箭头函数
来源：http://jpn.52xcode.cn

const double = x => x * 2;
来源：http://pnr.zhixingplan.top

[U95] JS：Promise 包装
来源：http://uot.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://wpy.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://reu.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://olp.meibo888.top

[U97] JS：并发请求
来源：http://agg.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jbr.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://alh.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zij.kuanghao11.cn

[U99] JS：事件监听
来源：http://zgn.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://cru.sxryk.cn

[U100] JS：DOM 查询
来源：http://rql.ivvv.top

document.querySelector(".item")
来源：http://tsd.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://thd.yuanzhike.top

el.classList.toggle("active")
来源：http://fzq.epnwcf.com

[U102] JS：本地存储
来源：http://uhh.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dpq.hfpthk.cn

[U103] JS：定时器
来源：http://jpi.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mxs.bbcook.cn

[U104] JS：防抖
来源：http://puw.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aag.nanxuanxn.top

[U105] JS：节流
来源：http://qie.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bud.xziqi.cn

[U106] JS：日期格式化
来源：http://cgh.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hiw.fktsv.cn

[U107] JS：数字千分位
来源：http://you.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aqv.chenzaomai.com

[U108] JS：随机整数
来源：http://azn.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gnf.xylfe.cn

[U109] JS：数组分组
来源：http://rcb.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://dko.fengsongda.top

[U110] JS：数组分块
来源：http://tfh.jinyuanbaomall.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://usw.bjfxy.top

[U111] JS：对象转 Map
来源：http://kxg.yuxming.cn

new Map(Object.entries(obj))
来源：http://qcr.yonumen.top

[U112] JS：字符串补位
来源：http://gsg.iojbl.cn

"7".padStart(3, "0")
来源：http://dre.tarul.cn

[U113] JS：正则替换全部
来源：http://bjx.ctjpmb.com

s.replaceAll("a", "b")
来源：http://xrj.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://chu.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://dkh.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://kzx.yangfankeji.com

crypto.randomUUID()
来源：http://spn.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://slp.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://nbt.fengsongda.top

[U117] JS：单元测试
来源：http://kas.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://ksb.316326.xyz

[U118] JS：开发服务器
来源：http://hic.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://hdx.cqqwz.cn

[U119] JS：生产构建
来源：http://eeb.sxryk.cn

npx vite build
来源：http://bvy.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://xjv.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://nbk.zhixingplan.top

================================================================================
来源：http://llh.xuanzx.com

统计汇总
来源：http://jzf.jinyuanbaomall.cn

================================================================================
来源：http://wuy.yonumen.top

按语言统计（条）：
来源：http://jkw.jyoumei.cn

Python ......... 252
来源：http://ygk.jqgufenzy.top

PHP ............ 252
来源：http://mfq.ppjwa.cn

JavaScript ..... 252
来源：http://qik.zdbjq.cn

TypeScript ..... 212
来源：http://fqd.wangshuangyany.cn

Java ........... 212
来源：http://ngn.birdmap.top

Go ............. 212
来源：http://mdv.hnxiangtu.top

Ruby ........... 212
来源：http://luc.gaohongyu789.top

C# ............. 212
来源：http://rii.tarul.cn

C .............. 30
来源：http://boz.fzhhl.top

C++ ............ 30
来源：http://zoe.fehbvm.com

SQL ............ 90
来源：http://yoe.kuanghao11.cn

Bash ........... 80
来源：http://kyg.nanxinkj.top

Kotlin ......... 15
来源：http://wqd.hammf.cn

Swift .......... 15
来源：http://yyg.meibo888.top

Lua ............ 10
来源：http://ypm.sufxvd.cn

Perl ........... 10
来源：http://zfb.jqgfzy.top

Scala .......... 10
来源：http://qxt.zhixingplan.top

------------------------------------
来源：http://esb.nanxuanxn.top

合计 ........... 2106 条
来源：http://qrk.zhengqikj.top

按章节统计：
来源：http://qlm.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mox.guannengcc.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fwl.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jrf.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tru.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vqf.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ryk.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zfv.uphjek.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rgj.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kht.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mvi.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gal.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sob.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bht.sysykeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hia.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bgc.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xum.c1oappe.top

Q SQL 专题                              90
来源：http://gdd.meibo888.top

R Bash 专题                             80
来源：http://nou.redwolf501.top

S C / C++ 专题                          60
来源：http://qca.ybcxt.top

T 其他语言补充                          60
来源：http://bwc.hywenlv.cn

U 高频实用片段                         120
来源：http://ybp.gogol.net.cn

------------------------------------
来源：http://zfi.hammf.cn

合计                                  2106 条
来源：http://poa.daxiang520.top

--------------------------------------------------------------------------------
来源：http://qup.gaohongyu789.top

使用提醒
来源：http://pyg.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://nos.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oqb.chenjidiqi.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bxu.guowangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yxt.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://azs.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ymg.yfazqb.com

—— 文件结束 ——
来源：http://xdr.quarkkingdee.top

================================================================================
来源：http://bce.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://dej.jianghu66.top

Common Programming Examples Cheat Book
来源：http://cpk.jinghuilouyu.cn

================================================================================
来源：http://oqa.iojbl.cn

【收录内容】
来源：http://zzr.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vqx.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kfr.quarkkingdee.top

SQL · Bash · C · C++
来源：http://bjz.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hhf.daria6918.cn

【使用说明】
来源：http://agc.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ksi.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wxz.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yva.xuetiantiany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fyr.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://idx.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qol.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eoz.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uyo.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://etu.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://meh.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eka.vehdjk.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rsp.ywan-chungtsiang.top

【文件统计】
来源：http://aok.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://caz.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://iwg.quarkkingdee.top

目  录
来源：http://jjx.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://run.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ffx.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aib.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ylx.fengsongda.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gna.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bub.hcnkem.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eva.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wgw.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cba.tian-w.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://frk.snrcjt.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vkn.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bob.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ovq.jinghuilouyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ujc.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vtc.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qpq.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hrq.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yzq.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://esn.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rei.chenlongwang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sye.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://myg.xylfe.cn

================================================================================
来源：http://cfa.nwbrower.top

A. 基础语法与类型
来源：http://ycv.sysykeji.top

================================================================================
来源：http://zcy.jinqigufen.top

[A01] Hello World
来源：http://wmq.tianlin.xyz

Py:   print("Hello, World!")
来源：http://bfq.zhoulong.xyz

PHP:  echo "Hello, World!";
来源：http://tej.sufxvd.cn

JS:   console.log("Hello, World!");
来源：http://ahn.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://twg.jinqigfzy.top

Java: System.out.println("Hello, World!");
来源：http://tsc.yuanzhike.top

Go:   fmt.Println("Hello, World!")
来源：http://xpt.sysykeji.top

Ruby: puts "Hello, World!"
来源：http://khf.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tpi.cqqwz.cn

[A02] 变量声明与赋值
来源：http://hpa.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xrf.epnwcf.com

PHP:  $name = "Alex"; $age = 20;
来源：http://hsa.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://ccy.haohaochexian.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tbs.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://wqp.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://gpa.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://nlv.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gbr.wangdashe.top

[A03] 常量定义
来源：http://rvw.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mab.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://oqt.ybcxt.top

JS:   const PI = 3.14159;
来源：http://npf.zycfv.cn

TS:   const PI: number = 3.14159;
来源：http://rgh.zhengqikj.top

Java: static final double PI = 3.14159;
来源：http://vpn.zhoulong.xyz

Go:   const PI = 3.14159
来源：http://zbo.sjlbkw.cn

Ruby: PI = 3.14159
来源：http://wys.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://ite.aizwys.cn

[A04] 判断变量类型
来源：http://bbk.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://boy.smart0.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bxg.xuanzx.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uuk.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://lre.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kfb.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://ytl.hnxiangtu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://unb.yfazqb.com

C#:   x.GetType().Name; x is int
来源：http://pvb.c1oappe.top

[A05] 整数除法与取模
来源：http://tvq.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zhp.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://chu.guannengcc.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://phb.quarkkingdee.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://emx.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://xnk.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://mbw.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://fcg.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://bsk.snrcjt.cn

[A06] 字符串转数字
来源：http://ftg.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://gcv.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nwy.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ivt.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://pwl.dianchejie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ydz.sjlbkw.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ywm.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bil.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rdt.xylfe.cn

[A07] 数字转字符串
来源：http://bbz.gzhubu.top

Py:   str(42)
来源：http://htr.fktsv.cn

PHP:  (string) 42; strval(42)
来源：http://njh.yj202588.top

JS:   String(42); (42).toString()
来源：http://soj.c1oappe.top

TS:   String(42)
来源：http://xeb.chenjidiqi.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://ngm.guannengcc.top

Go:   strconv.Itoa(42)
来源：http://ffe.quarkkingdee.top

Ruby: 42.to_s
来源：http://fwq.birdmap.top

C#:   42.ToString()
来源：http://rrz.jqgufenzy.top

[A08] 取整与四舍五入
来源：http://ihu.zhongyouzk.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yzw.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zvj.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zdt.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ace.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hhx.dashuyun.cn


<!-- 参考信息 -->