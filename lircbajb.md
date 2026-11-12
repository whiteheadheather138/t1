代发 wailian999

[U59] PHP：自定义排序
来源：http://xam.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xri.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://nyd.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://olz.shuidangran.top

[U61] PHP：正则
来源：http://oph.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tbr.dianchejie.cn

[U62] PHP：日期对象
来源：http://bjj.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hvd.hnxiangtu.top

[U63] PHP：文件读写
来源：http://wuy.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zle.uphjek.com

[U64] PHP：目录遍历
来源：http://otm.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://pmp.cashguo.top

[U65] PHP：会话
来源：http://hzg.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://atc.sjlbkw.cn

[U66] PHP：设置 Cookie
来源：http://okd.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kol.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://zpa.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fil.yfazqb.com

[U68] PHP：PDO 连接
来源：http://khy.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kwt.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://gts.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mtd.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://wfn.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jpi.yj202588.top

[U71] PHP：抛出异常
来源：http://lzn.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://swl.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://hol.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://aqg.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://ygj.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://lhz.ydzc1.top

[U74] PHP：读取环境变量
来源：http://nvk.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://gvm.pycfn.com

[U75] PHP：依赖注入
来源：http://zsd.wangdashe.top

composer require psr/container
来源：http://vmq.dashuyun.cn

[U76] PHP：简单路由
来源：http://ktb.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tys.yonumen.top

[U77] PHP：模板渲染
来源：http://kbj.tianlin.xyz

composer require twig/twig
来源：http://jkc.tarul.cn

[U78] PHP：单元测试
来源：http://lro.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://yay.havefunace.top

[U79] PHP：静态分析
来源：http://vie.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://dkb.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://dhc.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dmg.zhengqikj.top

[U81] JS：初始化项目
来源：http://pbw.zdqjudy.top

npm init -y;  npm i express
来源：http://nbj.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://tbk.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wkz.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://ftk.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pzg.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://xpb.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://iqr.yuanzhike.top

[U85] JS：可选链
来源：http://zwy.hnxiangtu.top

a?.b?.c
来源：http://lkc.vqdsnc.cn

[U86] JS：空值合并
来源：http://nqc.quarkkingdee.top

a ?? b
来源：http://wov.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://tox.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://tus.zhengqikj.top

[U88] JS：对象展开合并
来源：http://obv.snrcjt.cn

{ ...a, ...b }
来源：http://tps.yanxiufei.cn

[U89] JS：数组去重
来源：http://fbd.fktsv.cn

[...new Set(arr)]
来源：http://yci.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://ova.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://ekz.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://rfo.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://icc.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://kyk.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://tum.yj202588.top

[U93] JS：模板字符串
来源：http://boq.xylfe.cn

`共 ${n} 条`
来源：http://fwr.sweek.top

[U94] JS：箭头函数
来源：http://smj.yvedp.cn

const double = x => x * 2;
来源：http://kkm.fktsv.cn

[U95] JS：Promise 包装
来源：http://tka.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://iqh.tanke756.top

[U96] JS：async/await 与异常
来源：http://ret.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fxp.c1oappe.top

[U97] JS：并发请求
来源：http://ujr.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://bgm.wangshuangyany.cn

[U98] JS：fetch 带 JSON
来源：http://wgg.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bpq.tanke756.top

[U99] JS：事件监听
来源：http://hbp.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://zkx.gogol.net.cn

[U100] JS：DOM 查询
来源：http://bia.zhiwuduotai.top

document.querySelector(".item")
来源：http://xiq.gotoacloud.top

[U101] JS：classList 操作
来源：http://cze.chenlongwang.top

el.classList.toggle("active")
来源：http://uqv.ctjpmb.com

[U102] JS：本地存储
来源：http://jfu.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cac.tanke756.top

[U103] JS：定时器
来源：http://rbw.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rbd.cdnleiting.top

[U104] JS：防抖
来源：http://nad.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyy.shuidangran.top

[U105] JS：节流
来源：http://avt.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cll.0kj1m.cn

[U106] JS：日期格式化
来源：http://ppl.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://knj.jiagoushi.top

[U107] JS：数字千分位
来源：http://teo.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://srw.hongshengwenyu.top

[U108] JS：随机整数
来源：http://uys.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kzs.iojbl.cn

[U109] JS：数组分组
来源：http://wsh.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://yhb.gogol.net.cn

[U110] JS：数组分块
来源：http://fgu.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vor.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://fqy.bbcook.cn

new Map(Object.entries(obj))
来源：http://mao.daria6918.cn

[U112] JS：字符串补位
来源：http://euj.daxiang520.top

"7".padStart(3, "0")
来源：http://kti.jqgfzy.top

[U113] JS：正则替换全部
来源：http://hdi.jiagoushi.top

s.replaceAll("a", "b")
来源：http://gyd.fehbvm.com

[U114] JS：JSON 深比较
来源：http://hjn.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sev.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://kqs.52xcode.cn

crypto.randomUUID()
来源：http://mos.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://oxn.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://oft.yangfankeji.com

[U117] JS：单元测试
来源：http://mgl.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://ykp.yj20258.top

[U118] JS：开发服务器
来源：http://kpb.chenlongwang.top

npm i -D vite;  npx vite
来源：http://rmk.ivvv.top

[U119] JS：生产构建
来源：http://pls.ctjpmb.com

npx vite build
来源：http://szm.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://hts.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://bed.gaohongyu789.top

================================================================================
来源：http://dcp.nanxinkj.top

统计汇总
来源：http://ykp.xuanzx.com

================================================================================
来源：http://rdg.tarul.cn

按语言统计（条）：
来源：http://umf.iojbl.cn

Python ......... 252
来源：http://mib.tanke756.top

PHP ............ 252
来源：http://epw.bjfxy.top

JavaScript ..... 252
来源：http://fph.sxryk.cn

TypeScript ..... 212
来源：http://zkw.shangyingyoupin.top

Java ........... 212
来源：http://vgy.fanxiaobao.xyz

Go ............. 212
来源：http://wji.9152youxi.cn

Ruby ........... 212
来源：http://txj.ydzc1.top

C# ............. 212
来源：http://wcj.smart0.xyz

C .............. 30
来源：http://lay.tarul.cn

C++ ............ 30
来源：http://igd.daxiang520.top

SQL ............ 90
来源：http://sba.snrcjt.cn

Bash ........... 80
来源：http://eqr.sysykeji.top

Kotlin ......... 15
来源：http://vgm.hcnkem.com

Swift .......... 15
来源：http://ytf.hesvh.cn

Lua ............ 10
来源：http://qrj.nwbrower.top

Perl ........... 10
来源：http://igk.cdnleiting.top

Scala .......... 10
来源：http://gif.hnxiangtu.top

------------------------------------
来源：http://tey.yj20258.top

合计 ........... 2106 条
来源：http://ohv.guowangkeji.top

按章节统计：
来源：http://cby.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vqp.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hep.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gkj.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ikd.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://emg.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jwf.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ybt.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ngj.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vva.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dkp.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://djb.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vjw.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://irt.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ufc.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wzk.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lfe.daxiang520.top

Q SQL 专题                              90
来源：http://uzb.birdmap.top

R Bash 专题                             80
来源：http://ybd.yanxiufei.cn

S C / C++ 专题                          60
来源：http://xze.ivvv.top

T 其他语言补充                          60
来源：http://nma.andypj.xyz

U 高频实用片段                         120
来源：http://llq.xylfe.cn

------------------------------------
来源：http://qpo.bjfxy.top

合计                                  2106 条
来源：http://tlj.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://mgx.yonumen.top

使用提醒
来源：http://aum.yonumen.top

--------------------------------------------------------------------------------
来源：http://txn.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cdr.xingfuxueyuan.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pza.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nlm.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://onp.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dwj.shzxlz.cn

—— 文件结束 ——
来源：http://tzh.feifeiyinyue.top

================================================================================
来源：http://jrx.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://rsm.gzhubu.top

Common Programming Examples Cheat Book
来源：http://chy.yj202588.top

================================================================================
来源：http://svz.sysykeji.top

【收录内容】
来源：http://riq.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://rgy.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://boy.mhx1999.top

SQL · Bash · C · C++
来源：http://qyx.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gss.tianlin.xyz

【使用说明】
来源：http://jzy.yj202588.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://deg.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zqy.hnqzz.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xfz.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qot.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zni.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tce.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://meo.haohaochexian.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hvx.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uir.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xgs.svipenyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pik.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ypj.xziqi.cn

【文件统计】
来源：http://xst.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ogj.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://sjk.bbcook.cn

目  录
来源：http://ayg.shuidangran.top

--------------------------------------------------------------------------------
来源：http://oqy.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ovd.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kcs.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uhh.yanxiufei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nby.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pfa.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pwk.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://btv.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xdp.nwbrower.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rdg.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cqv.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dce.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fln.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tdy.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qiu.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uhp.tarul.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ykt.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vpm.xingfuxueyuan.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://fqc.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rcw.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://glf.andypj.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mer.hnqzz.top

================================================================================
来源：http://hli.zhengqikj.top

A. 基础语法与类型
来源：http://cgj.yuxming.cn

================================================================================
来源：http://tyw.xziqi.cn

[A01] Hello World
来源：http://pwk.bbcook.cn

Py:   print("Hello, World!")
来源：http://edz.fehbvm.com

PHP:  echo "Hello, World!";
来源：http://imp.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://szp.nwbrower.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vtu.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://yru.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://xva.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://zra.chenjidiqi.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://ylj.pengpengdd.cyou

[A02] 变量声明与赋值
来源：http://sjv.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wzr.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ngv.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://fxc.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fbq.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://hbc.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://wbz.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://czu.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://hmw.fengsongda.top

[A03] 常量定义
来源：http://qnj.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://urc.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://ftj.guannengcc.top

JS:   const PI = 3.14159;
来源：http://dbk.chenlongwang.top

TS:   const PI: number = 3.14159;
来源：http://xuh.redwolf501.top

Java: static final double PI = 3.14159;
来源：http://dfl.shangyingyoupin.top

Go:   const PI = 3.14159
来源：http://tji.ydzc1.top

Ruby: PI = 3.14159
来源：http://wff.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://wca.xinyue.icu

[A04] 判断变量类型
来源：http://bzt.vehdjk.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://gqx.hnxiangtu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://szw.tianlin.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://azy.nwbrower.top

TS:   typeof x; x instanceof Date
来源：http://lot.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mda.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://age.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yrj.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://dak.daria6918.cn

[A05] 整数除法与取模
来源：http://sih.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tqh.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xyf.jinghuilouyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wbl.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kbd.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://sdl.xingfuxueyuan.xyz

Go:   7 / 2; 7 % 2
来源：http://sgy.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://kmz.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://gkl.hfpthk.cn

[A06] 字符串转数字
来源：http://amk.tianlin.xyz

Py:   int("42"); float("3.14")
来源：http://yvv.daxiang520.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qdv.dianchejie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ekr.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://mvb.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yiz.fzhhl.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mrn.zdbjq.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yfl.tanke756.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fmz.hcnkem.com

[A07] 数字转字符串
来源：http://kpz.epnwcf.com

Py:   str(42)
来源：http://iwy.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://tcm.yvedp.cn

JS:   String(42); (42).toString()
来源：http://loq.guowangkeji.top

TS:   String(42)
来源：http://sbu.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://pyn.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://rza.yj202588.top

Ruby: 42.to_s
来源：http://efr.cucudq.cn

C#:   42.ToString()
来源：http://uax.zhengqikj.top

[A08] 取整与四舍五入
来源：http://bzg.sweek.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lga.fanxiaobao.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://prf.zdbjq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ttk.haohaochexian.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://raf.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://edn.hnqzz.top


<!-- 参考信息 -->