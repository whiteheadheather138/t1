代发 wailian999

[U55] PHP：match 表达式
来源：http://ils.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tnk.cheryme.top

[U56] PHP：命名参数
来源：http://dns.redwolf501.top

f(a: 1, b: 2)
来源：http://ewb.ybcxt.top

[U57] PHP：字符串插值
来源：http://mvx.316326.xyz

"值: {$a}"
来源：http://hhg.sysykeji.top

[U58] PHP：数组三件套
来源：http://idn.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://obg.chenzaomai.com

[U59] PHP：自定义排序
来源：http://edf.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xgj.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://ivk.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lsb.jiagoushi.top

[U61] PHP：正则
来源：http://bov.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bxe.zhixingplan.top

[U62] PHP：日期对象
来源：http://kbv.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tgq.sxryk.cn

[U63] PHP：文件读写
来源：http://xue.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rtq.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://dgv.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://lev.52xcode.cn

[U65] PHP：会话
来源：http://zmo.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gsc.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://enf.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://trw.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://ljo.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://llc.zhengqikj.top

[U68] PHP：PDO 连接
来源：http://jii.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nhr.sweek.top

[U69] PHP：PDO 预处理
来源：http://svf.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vnz.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://ldp.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://esl.c1oappe.top

[U71] PHP：抛出异常
来源：http://arv.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://chi.fktsv.cn

[U72] PHP：写错误日志
来源：http://fsk.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://vku.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://nkp.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://pye.daxiang520.top

[U74] PHP：读取环境变量
来源：http://cwh.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://bwj.shzxlz.cn

[U75] PHP：依赖注入
来源：http://eva.shzxlz.cn

composer require psr/container
来源：http://vjw.aizwys.cn

[U76] PHP：简单路由
来源：http://bck.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uzv.shuidangran.top

[U77] PHP：模板渲染
来源：http://neg.daxiang520.top

composer require twig/twig
来源：http://lyt.havefunace.top

[U78] PHP：单元测试
来源：http://myu.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://kvi.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://hwr.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://viu.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://lhe.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ncm.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://wko.kuanghao11.cn

npm init -y;  npm i express
来源：http://wdx.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://sgr.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rdr.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://bbz.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://fqm.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://xra.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://pzm.jinghuilouyu.cn

[U85] JS：可选链
来源：http://fha.wangshuangyany.cn

a?.b?.c
来源：http://wsi.svipenyu.cn

[U86] JS：空值合并
来源：http://dqd.hongshengwenyu.top

a ?? b
来源：http://zna.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://sec.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://qzx.gotoacloud.top

[U88] JS：对象展开合并
来源：http://qam.zhoulong.xyz

{ ...a, ...b }
来源：http://whj.hnxiangtu.top

[U89] JS：数组去重
来源：http://foj.yongpay.top

[...new Set(arr)]
来源：http://qqe.fktsv.cn

[U90] JS：数字数组排序
来源：http://ero.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://rkr.andypj.xyz

[U91] JS：对象键值遍历
来源：http://srt.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nfq.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://vtk.bjfxy.top

structuredClone(obj)
来源：http://pgc.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://npz.hywenlv.cn

`共 ${n} 条`
来源：http://mgz.svipenyu.cn

[U94] JS：箭头函数
来源：http://czr.cucudq.cn

const double = x => x * 2;
来源：http://uyn.gotoacloud.top

[U95] JS：Promise 包装
来源：http://edj.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://rfz.yj202588.top

[U96] JS：async/await 与异常
来源：http://oyy.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://osr.hongshengwenyu.top

[U97] JS：并发请求
来源：http://afz.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pwi.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://bdj.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jsz.cashguo.top

[U99] JS：事件监听
来源：http://kep.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://bmv.zhoulong.xyz

[U100] JS：DOM 查询
来源：http://fbp.jqgfzy.top

document.querySelector(".item")
来源：http://sbq.daxiang520.top

[U101] JS：classList 操作
来源：http://yjd.vehdjk.com

el.classList.toggle("active")
来源：http://clv.xinyue.icu

[U102] JS：本地存储
来源：http://puw.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wzy.uphjek.com

[U103] JS：定时器
来源：http://skn.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wfr.guannengcc.top

[U104] JS：防抖
来源：http://gbd.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rql.bjfxy.top

[U105] JS：节流
来源：http://ckg.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lis.52xcode.cn

[U106] JS：日期格式化
来源：http://kcu.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mfn.zhijiandao.cn

[U107] JS：数字千分位
来源：http://aic.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vtr.wangshuangyany.cn

[U108] JS：随机整数
来源：http://myo.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://okm.sjlbkw.cn

[U109] JS：数组分组
来源：http://axt.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://bhg.wangdashe.top

[U110] JS：数组分块
来源：http://sts.kuanghao11.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ocd.smart0.xyz

[U111] JS：对象转 Map
来源：http://mjd.fengsongda.top

new Map(Object.entries(obj))
来源：http://esq.kuanghao11.cn

[U112] JS：字符串补位
来源：http://soo.shanyushiyangtech.top

"7".padStart(3, "0")
来源：http://qpg.birdmap.top

[U113] JS：正则替换全部
来源：http://ywb.xziqi.cn

s.replaceAll("a", "b")
来源：http://pdy.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://ivf.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://etf.hfpthk.cn

[U115] JS：生成 UUID
来源：http://lwi.yj202588.top

crypto.randomUUID()
来源：http://pbi.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://jgy.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://zyv.mhx1999.top

[U117] JS：单元测试
来源：http://pph.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://xsi.hammf.cn

[U118] JS：开发服务器
来源：http://yig.hesvh.cn

npm i -D vite;  npx vite
来源：http://ufd.xinyue.icu

[U119] JS：生产构建
来源：http://lgj.yj202588.top

npx vite build
来源：http://ksa.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://hbc.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://mic.ydjk.org.cn

================================================================================
来源：http://fix.cashguo.top

统计汇总
来源：http://all.hnxiangtu.top

================================================================================
来源：http://qof.sxryk.cn

按语言统计（条）：
来源：http://nea.hnqzz.top

Python ......... 252
来源：http://kuz.bbcook.cn

PHP ............ 252
来源：http://eym.yvedp.cn

JavaScript ..... 252
来源：http://szn.pycfn.com

TypeScript ..... 212
来源：http://fre.guannengcc.top

Java ........... 212
来源：http://yue.redwolf501.top

Go ............. 212
来源：http://nnz.tanke756.top

Ruby ........... 212
来源：http://ybc.ywan-chungtsiang.top

C# ............. 212
来源：http://qgq.epnwcf.com

C .............. 30
来源：http://vnm.cdnleiting.top

C++ ............ 30
来源：http://buv.yvedp.cn

SQL ............ 90
来源：http://efy.daxiang520.top

Bash ........... 80
来源：http://arw.52xcode.cn

Kotlin ......... 15
来源：http://xwl.haohaochexian.top

Swift .......... 15
来源：http://nay.cashguo.top

Lua ............ 10
来源：http://zyw.jinqigufen.top

Perl ........... 10
来源：http://zwx.chenlongwang.top

Scala .......... 10
来源：http://vca.tanke756.top

------------------------------------
来源：http://lvr.9152youxi.cn

合计 ........... 2106 条
来源：http://rqp.dashuyun.cn

按章节统计：
来源：http://mko.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bpk.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://knj.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://swv.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xgw.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cgl.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ivj.shanyushiyangtech.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vuk.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dia.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mfg.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zaw.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://koo.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rwf.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://onb.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hnu.aizwys.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sat.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bpz.aibaodan.cn

Q SQL 专题                              90
来源：http://qfp.nanxuanxn.top

R Bash 专题                             80
来源：http://uon.cucudq.cn

S C / C++ 专题                          60
来源：http://msf.jiagoushi.top

T 其他语言补充                          60
来源：http://oec.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://vku.ctjpmb.com

------------------------------------
来源：http://usj.hfpthk.cn

合计                                  2106 条
来源：http://buq.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://jna.cdnleiting.top

使用提醒
来源：http://ypg.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://acg.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tzl.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ito.andypj.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jeb.dashuyun.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jjb.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zcz.vehdjk.com

—— 文件结束 ——
来源：http://anb.svipenyu.cn

================================================================================
来源：http://jpg.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://rsn.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://qkd.jinghuilouyu.cn

================================================================================
来源：http://wuh.fzhhl.top

【收录内容】
来源：http://ncn.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bog.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rht.bjfxy.top

SQL · Bash · C · C++
来源：http://ysr.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xll.ctjpmb.com

【使用说明】
来源：http://yux.meibo888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tpl.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tgy.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wuu.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cwr.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lhl.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qpl.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fhi.tianlin.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ayd.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ebs.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vtx.daxiang520.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://obm.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mlg.shanyushiyangtech.top

【文件统计】
来源：http://nlv.yfazqb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://izm.yj20258.top

--------------------------------------------------------------------------------
来源：http://jls.yueranfly.top

目  录
来源：http://jjl.pycfn.com

--------------------------------------------------------------------------------
来源：http://giy.redwolf501.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vaa.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sxp.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://klk.ybcxt.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://scz.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jru.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jul.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zwz.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qxb.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rko.jinghuilouyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tyn.zdqjudy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://maw.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dpj.jqgfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mgk.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mgb.vqdsnc.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jct.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wzv.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tdc.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vvo.pycfn.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://viu.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ule.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gsf.gogol.net.cn

================================================================================
来源：http://zbd.gotoacloud.top

A. 基础语法与类型
来源：http://wzy.hcnkem.com

================================================================================
来源：http://fcq.cheryme.top

[A01] Hello World
来源：http://fns.birdmap.top

Py:   print("Hello, World!")
来源：http://eik.cdnleiting.top

PHP:  echo "Hello, World!";
来源：http://gxw.sysykeji.top

JS:   console.log("Hello, World!");
来源：http://agu.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wab.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://jqi.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://gpc.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://sfq.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eiy.shuidangran.top

[A02] 变量声明与赋值
来源：http://fiz.epnwcf.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xvu.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ntf.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://hgu.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fma.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://cly.birdmap.top

Go:   name := "Alex"; age := 20
来源：http://xlf.xylfe.cn

Ruby: name = "Alex"; age = 20
来源：http://gnw.hcnkem.com

C#:   string name = "Alex"; int age = 20;
来源：http://pli.jianghu66.top

[A03] 常量定义
来源：http://qes.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ypn.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://fri.ydzc1.top

JS:   const PI = 3.14159;
来源：http://hcd.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://iuj.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://uef.cqqwz.cn

Go:   const PI = 3.14159
来源：http://lrv.cheryme.top

Ruby: PI = 3.14159
来源：http://myf.yj20258.top

C#:   const double PI = 3.14159;
来源：http://teq.hnqzz.top

[A04] 判断变量类型
来源：http://guo.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gmj.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rut.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wmk.chenzaomai.com

TS:   typeof x; x instanceof Date
来源：http://tdh.hammf.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rep.wangdashe.top

Go:   reflect.TypeOf(x).Name()
来源：http://tnf.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://hqm.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://gup.yj20258888.top

[A05] 整数除法与取模
来源：http://ovx.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qia.zhijiandao.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://unq.52xcode.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fcg.chenlongwang.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yqx.jinqigufen.top

Java: 7 / 2; 7 % 2
来源：http://jjv.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://hed.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://ifa.52xcode.cn

C#:   7 / 2; 7 % 2
来源：http://kys.daria6918.cn

[A06] 字符串转数字
来源：http://nao.hywenlv.cn

Py:   int("42"); float("3.14")
来源：http://faa.ehwqpu.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xpg.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qve.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://vrs.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pyr.jinyuanbaomall.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gnv.birdmap.top

Ruby: "42".to_i; "3.14".to_f
来源：http://uaq.fehbvm.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://iib.cheryme.top

[A07] 数字转字符串
来源：http://fie.gzhubu.top

Py:   str(42)
来源：http://zzh.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://wkc.hesvh.cn

JS:   String(42); (42).toString()
来源：http://onz.yj202588.top

TS:   String(42)
来源：http://fgm.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xee.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://hsp.tianlin.xyz


<!-- 参考信息 -->