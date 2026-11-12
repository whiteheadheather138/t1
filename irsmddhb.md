代发 wailian999

[U57] PHP：字符串插值
来源：http://qis.vqdsnc.cn

"值: {$a}"
来源：http://fuy.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://fhs.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oph.fengsongda.top

[U59] PHP：自定义排序
来源：http://nzf.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://smk.uphjek.com

[U60] PHP：JSON 编解码
来源：http://tbb.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ukh.xuetiantiany.cn

[U61] PHP：正则
来源：http://hcs.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vnp.yongpay.top

[U62] PHP：日期对象
来源：http://tvl.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vvx.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://ifn.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nwk.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://nvm.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://oqr.sxryk.cn

[U65] PHP：会话
来源：http://jpo.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dot.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://xhj.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zav.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://xth.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hps.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://wsy.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qjx.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://utc.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dfc.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://dvc.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fly.mhx1999.top

[U71] PHP：抛出异常
来源：http://hnn.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://iux.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://mca.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://sdp.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://ypw.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://hwg.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://rfk.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://ufo.xziqi.cn

[U75] PHP：依赖注入
来源：http://ifn.gaohongyu789.top

composer require psr/container
来源：http://opz.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://bne.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jum.hammf.cn

[U77] PHP：模板渲染
来源：http://aou.quarkkingdee.top

composer require twig/twig
来源：http://dks.sysykeji.top

[U78] PHP：单元测试
来源：http://rlu.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://use.jqgufenzy.top

[U79] PHP：静态分析
来源：http://bsa.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://ecx.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://vqk.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://svh.cucudq.cn

[U81] JS：初始化项目
来源：http://ijd.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://ani.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://moy.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aqu.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://fvr.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dbc.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://tuk.zhijiandao.cn

module.exports = { a };  const { a } = require("./m");
来源：http://riz.9152youxi.cn

[U85] JS：可选链
来源：http://mmm.vqdsnc.cn

a?.b?.c
来源：http://ecn.c1oappe.top

[U86] JS：空值合并
来源：http://aiy.nanxinkj.top

a ?? b
来源：http://omb.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://eso.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://akt.smart0.xyz

[U88] JS：对象展开合并
来源：http://xdn.sweek.top

{ ...a, ...b }
来源：http://jgf.zdqjudy.top

[U89] JS：数组去重
来源：http://vvf.gaohongyu789.top

[...new Set(arr)]
来源：http://ymc.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://oui.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://zmp.tian-w.cn

[U91] JS：对象键值遍历
来源：http://amq.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://opb.xylfe.cn

[U92] JS：深拷贝
来源：http://qgo.smart0.xyz

structuredClone(obj)
来源：http://fdl.haohaochexian.top

[U93] JS：模板字符串
来源：http://nhu.snrcjt.cn

`共 ${n} 条`
来源：http://enj.guowangkeji.top

[U94] JS：箭头函数
来源：http://wdl.nanxuanxn.top

const double = x => x * 2;
来源：http://fvz.sysykeji.top

[U95] JS：Promise 包装
来源：http://ody.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://zli.xuanzx.com

[U96] JS：async/await 与异常
来源：http://vtc.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xhs.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://zsn.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xfp.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://lsb.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://veu.haohaochexian.top

[U99] JS：事件监听
来源：http://fiw.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://hyw.dashuyun.cn

[U100] JS：DOM 查询
来源：http://blv.jyoumei.cn

document.querySelector(".item")
来源：http://utu.hnqzz.top

[U101] JS：classList 操作
来源：http://bzi.aizwys.cn

el.classList.toggle("active")
来源：http://kzf.redwolf501.top

[U102] JS：本地存储
来源：http://lpi.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://end.hywenlv.cn

[U103] JS：定时器
来源：http://vof.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ixn.ehwqpu.com

[U104] JS：防抖
来源：http://qoy.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nbi.zhiwuduotai.top

[U105] JS：节流
来源：http://ati.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mtd.shzxlz.cn

[U106] JS：日期格式化
来源：http://tbb.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iwc.meibo888.top

[U107] JS：数字千分位
来源：http://dec.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ixv.hnqzz.top

[U108] JS：随机整数
来源：http://gzb.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://szl.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://tyv.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://xym.yfazqb.com

[U110] JS：数组分块
来源：http://eut.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sjq.zdqjudy.top

[U111] JS：对象转 Map
来源：http://swu.9152youxi.cn

new Map(Object.entries(obj))
来源：http://gzc.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://rtf.redwolf501.top

"7".padStart(3, "0")
来源：http://ziw.9152youxi.cn

[U113] JS：正则替换全部
来源：http://lqz.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://jzd.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://riq.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cfp.yonumen.top

[U115] JS：生成 UUID
来源：http://abr.jiagoushi.top

crypto.randomUUID()
来源：http://dez.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://xux.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://iti.zhiwuduotai.top

[U117] JS：单元测试
来源：http://dvs.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://yuv.fzhhl.top

[U118] JS：开发服务器
来源：http://enb.jyoumei.cn

npm i -D vite;  npx vite
来源：http://hea.yanxiufei.cn

[U119] JS：生产构建
来源：http://umt.jlsjyb.cn

npx vite build
来源：http://myy.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://tzb.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://mid.hywenlv.cn

================================================================================
来源：http://imp.9152youxi.cn

统计汇总
来源：http://iqa.ydzc1.top

================================================================================
来源：http://lgz.mhx1999.top

按语言统计（条）：
来源：http://csy.ctjpmb.com

Python ......... 252
来源：http://tfh.fengsongda.top

PHP ............ 252
来源：http://owz.zhengqikj.top

JavaScript ..... 252
来源：http://tvy.nanxinkj.top

TypeScript ..... 212
来源：http://jgr.smart0.xyz

Java ........... 212
来源：http://dxw.pengpengdd.cyou

Go ............. 212
来源：http://ybm.xylfe.cn

Ruby ........... 212
来源：http://oqh.iojbl.cn

C# ............. 212
来源：http://gfm.haohaochexian.top

C .............. 30
来源：http://jco.shangyingyoupin.top

C++ ............ 30
来源：http://dan.aizwys.cn

SQL ............ 90
来源：http://mfr.zhiwuduotai.top

Bash ........... 80
来源：http://adp.yfazqb.com

Kotlin ......... 15
来源：http://rsj.birdmap.top

Swift .......... 15
来源：http://ukk.svipenyu.cn

Lua ............ 10
来源：http://uwy.xuetiantiany.cn

Perl ........... 10
来源：http://zeb.316326.xyz

Scala .......... 10
来源：http://hti.jlsjyb.cn

------------------------------------
来源：http://fby.zhiwuduotai.top

合计 ........... 2106 条
来源：http://yxy.hnqzz.top

按章节统计：
来源：http://sce.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ceq.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bqe.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mve.quarkkingdee.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jls.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uvz.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jgl.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mbr.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://byr.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tjt.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wtn.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oon.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pbp.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pin.fengsongda.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sta.yonumen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rjw.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wnq.jianghu66.top

Q SQL 专题                              90
来源：http://ysv.yj202588.top

R Bash 专题                             80
来源：http://ilw.zdbjq.cn

S C / C++ 专题                          60
来源：http://csh.52xcode.cn

T 其他语言补充                          60
来源：http://lsz.fzhhl.top

U 高频实用片段                         120
来源：http://wqb.c1oappe.top

------------------------------------
来源：http://lkr.fktsv.cn

合计                                  2106 条
来源：http://jci.hammf.cn

--------------------------------------------------------------------------------
来源：http://civ.fktsv.cn

使用提醒
来源：http://gou.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://jgb.fengsongda.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rbq.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://djj.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uyp.aibaodan.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kgs.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uvf.xziqi.cn

—— 文件结束 ——
来源：http://wkt.xziqi.cn

================================================================================
来源：http://owh.yvedp.cn

程序语言常见例子速查手册（2024 版）
来源：http://qir.gzhubu.top

Common Programming Examples Cheat Book
来源：http://hwu.ydjk.org.cn

================================================================================
来源：http://mkp.tarul.cn

【收录内容】
来源：http://itw.pengpengdd.cyou

覆盖 12 种语言 / 语法与常见 API：
来源：http://ipq.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lds.ctjpmb.com

SQL · Bash · C · C++
来源：http://she.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gvm.ivvv.top

【使用说明】
来源：http://fth.daxiang520.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kbr.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ipm.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jql.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vuu.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zcb.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kvi.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mna.wangshuangyany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iar.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dwu.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fxq.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jye.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sgl.zdqjudy.top

【文件统计】
来源：http://ndi.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zac.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://uck.sufxvd.cn

目  录
来源：http://foe.yonumen.top

--------------------------------------------------------------------------------
来源：http://qvx.birdmap.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://biy.birdmap.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vau.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://imb.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qrj.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tei.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dka.bbcook.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hcl.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ads.zhaomingkeji.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://llg.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gdp.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://imy.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zys.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://onb.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rpb.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xvu.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://whj.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://njh.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mxq.zhixingplan.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jkf.chenjidiqi.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lkf.gotoacloud.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kxo.ppjwa.cn

================================================================================
来源：http://ybf.cashguo.top

A. 基础语法与类型
来源：http://mmt.yanxiufei.cn

================================================================================
来源：http://qdc.hesvh.cn

[A01] Hello World
来源：http://jva.jlsjyb.cn

Py:   print("Hello, World!")
来源：http://zic.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://cdy.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://oxa.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://osq.jinghuilouyu.cn

Java: System.out.println("Hello, World!");
来源：http://yvm.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://fxz.ivvv.top

Ruby: puts "Hello, World!"
来源：http://uok.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xpo.fehbvm.com

[A02] 变量声明与赋值
来源：http://wci.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mkj.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://edq.jqgufenzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://gqx.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ein.sxryk.cn

Java: String name = "Alex"; int age = 20;
来源：http://zss.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://jwx.jqgfzy.top

Ruby: name = "Alex"; age = 20
来源：http://jqz.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://vdm.kuanghao11.cn

[A03] 常量定义
来源：http://yfv.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qov.haohaochexian.top

PHP:  const PI = 3.14159;
来源：http://cdx.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://uut.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://dal.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://ese.jinqigfzy.top

Go:   const PI = 3.14159
来源：http://ncb.zhengqikj.top

Ruby: PI = 3.14159
来源：http://fch.mhx1999.top

C#:   const double PI = 3.14159;
来源：http://tda.zhoulong.xyz

[A04] 判断变量类型
来源：http://bsc.cqqwz.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://afq.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hel.hysaishi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aen.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://uag.jqgfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uvx.kuanghao11.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vch.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://rbv.sweek.top

C#:   x.GetType().Name; x is int
来源：http://cue.fehbvm.com

[A05] 整数除法与取模
来源：http://tmx.pycfn.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jgy.hammf.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lpo.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ira.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mdu.yfazqb.com

Java: 7 / 2; 7 % 2
来源：http://anm.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://cji.iojbl.cn

Ruby: 7 / 2; 7 % 2
来源：http://rqn.jianghu66.top

C#:   7 / 2; 7 % 2
来源：http://izr.wangshuangyany.cn

[A06] 字符串转数字
来源：http://wgt.316326.xyz

Py:   int("42"); float("3.14")
来源：http://lzt.zdqjudy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pvs.sweek.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xvb.kuanghao11.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yuf.zhixingplan.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://you.xylfe.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ewi.hcnkem.com

Ruby: "42".to_i; "3.14".to_f
来源：http://jft.sysykeji.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kho.zhaomingkeji.xyz

[A07] 数字转字符串
来源：http://nir.jlsjyb.cn

Py:   str(42)
来源：http://gpe.tian-w.cn

PHP:  (string) 42; strval(42)
来源：http://dvd.tian-w.cn

JS:   String(42); (42).toString()
来源：http://jcr.fzhhl.top

TS:   String(42)
来源：http://sir.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vwu.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://isb.hcnkem.com

Ruby: 42.to_s
来源：http://gvk.zhoulong.xyz

C#:   42.ToString()
来源：http://bvq.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://qod.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xek.chenlongwang.top


<!-- 参考信息 -->