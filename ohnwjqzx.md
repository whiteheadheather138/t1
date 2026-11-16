代发 wailian999

[U51] PHP：数组解构
来源：http://zbt.hnqzz.top

[$a, $b] = $arr;
来源：http://gdy.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://yis.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://xyi.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://wqw.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://pry.hammf.cn

[U54] PHP：空安全调用
来源：http://dqc.hysaishi.cn

$obj?->method()
来源：http://cqj.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://das.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ucr.svipenyu.cn

[U56] PHP：命名参数
来源：http://qxo.yj20258888.top

f(a: 1, b: 2)
来源：http://tfk.fktsv.cn

[U57] PHP：字符串插值
来源：http://ybl.smart0.xyz

"值: {$a}"
来源：http://gaq.dashuyun.cn

[U58] PHP：数组三件套
来源：http://kex.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gey.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://pbq.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ynp.tanke756.top

[U60] PHP：JSON 编解码
来源：http://hqj.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tet.xuetiantiany.cn

[U61] PHP：正则
来源：http://kpg.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mju.ctjpmb.com

[U62] PHP：日期对象
来源：http://eqx.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mpx.shangyingyoupin.top

[U63] PHP：文件读写
来源：http://hfd.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ekp.jqgfzy.top

[U64] PHP：目录遍历
来源：http://oyj.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://znv.cdnleiting.top

[U65] PHP：会话
来源：http://okc.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wvz.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://rcf.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bfv.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://sdq.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jbl.52xcode.cn

[U68] PHP：PDO 连接
来源：http://cma.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aju.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://scx.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qgy.yonumen.top

[U70] PHP：PDO 事务
来源：http://hvu.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sss.havefunace.top

[U71] PHP：抛出异常
来源：http://yma.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://zte.zycfv.cn

[U72] PHP：写错误日志
来源：http://inc.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://jyn.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://kpp.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://jrk.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://toz.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://jos.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://gyx.aibaodan.cn

composer require psr/container
来源：http://kne.tanke756.top

[U76] PHP：简单路由
来源：http://yhd.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mxf.yj20258.top

[U77] PHP：模板渲染
来源：http://uuz.ppjwa.cn

composer require twig/twig
来源：http://gbd.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://qip.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://rpc.yanxiufei.cn

[U79] PHP：静态分析
来源：http://mvn.316326.xyz

composer require --dev phpstan/phpstan
来源：http://zdo.cheryme.top

[U80] PHP：代码规范修复
来源：http://gfw.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lkw.zdbjq.cn

[U81] JS：初始化项目
来源：http://jda.havefunace.top

npm init -y;  npm i express
来源：http://kea.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://hmr.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oej.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://sss.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tnz.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://teh.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iir.gotoacloud.top

[U85] JS：可选链
来源：http://ygw.sjlbkw.cn

a?.b?.c
来源：http://drs.gotoacloud.top

[U86] JS：空值合并
来源：http://zjq.kuanghao11.cn

a ?? b
来源：http://joo.tanke756.top

[U87] JS：解构默认值
来源：http://tve.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://hpl.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://tmz.yj202588.top

{ ...a, ...b }
来源：http://osh.ybcxt.top

[U89] JS：数组去重
来源：http://fdl.fzhhl.top

[...new Set(arr)]
来源：http://pjo.hywenlv.cn

[U90] JS：数字数组排序
来源：http://gaj.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://jwz.gzhubu.top

[U91] JS：对象键值遍历
来源：http://esm.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gwq.sjlbkw.cn

[U92] JS：深拷贝
来源：http://ctj.yuxming.cn

structuredClone(obj)
来源：http://rwr.vehdjk.com

[U93] JS：模板字符串
来源：http://lwz.fktsv.cn

`共 ${n} 条`
来源：http://dgu.smart0.xyz

[U94] JS：箭头函数
来源：http://gnr.nwbrower.top

const double = x => x * 2;
来源：http://tqh.316326.xyz

[U95] JS：Promise 包装
来源：http://oru.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://rxh.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://ppm.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gsa.cashguo.top

[U97] JS：并发请求
来源：http://laq.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://sxc.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://ogu.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fjo.shuidangran.top

[U99] JS：事件监听
来源：http://dez.aizwys.cn

el.addEventListener("click", e => {})
来源：http://xsf.cheryme.top

[U100] JS：DOM 查询
来源：http://fzl.yueranfly.top

document.querySelector(".item")
来源：http://xle.daxiang520.top

[U101] JS：classList 操作
来源：http://ddu.cashguo.top

el.classList.toggle("active")
来源：http://umn.yongpay.top

[U102] JS：本地存储
来源：http://wbs.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zri.sweek.top

[U103] JS：定时器
来源：http://cnz.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qgo.iojbl.cn

[U104] JS：防抖
来源：http://ime.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://plj.sysykeji.top

[U105] JS：节流
来源：http://kjn.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pro.sysykeji.top

[U106] JS：日期格式化
来源：http://vqu.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rln.yanxiufei.cn

[U107] JS：数字千分位
来源：http://asx.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://byz.iojbl.cn

[U108] JS：随机整数
来源：http://xni.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pjm.sweek.top

[U109] JS：数组分组
来源：http://phz.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://uek.cdnleiting.top

[U110] JS：数组分块
来源：http://kxx.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bip.yonumen.top

[U111] JS：对象转 Map
来源：http://oye.chenzaomai.com

new Map(Object.entries(obj))
来源：http://gve.yuanzhike.top

[U112] JS：字符串补位
来源：http://yme.pycfn.com

"7".padStart(3, "0")
来源：http://xwz.sweek.top

[U113] JS：正则替换全部
来源：http://xfm.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://dqr.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://ksd.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ftk.xuanzx.com

[U115] JS：生成 UUID
来源：http://uru.yfazqb.com

crypto.randomUUID()
来源：http://ybt.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://eyj.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://aso.cqqwz.cn

[U117] JS：单元测试
来源：http://tqj.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://faj.sufxvd.cn

[U118] JS：开发服务器
来源：http://mvl.ehwqpu.com

npm i -D vite;  npx vite
来源：http://dja.gogol.net.cn

[U119] JS：生产构建
来源：http://tzz.yongpay.top

npx vite build
来源：http://hzd.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://xtd.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://qhi.jqgfzy.top

================================================================================
来源：http://jvl.gzhubu.top

统计汇总
来源：http://ufh.guowangkeji.top

================================================================================
来源：http://zme.cqqwz.cn

按语言统计（条）：
来源：http://pqn.smart0.xyz

Python ......... 252
来源：http://wtn.daxiang520.top

PHP ............ 252
来源：http://tui.zdqjudy.top

JavaScript ..... 252
来源：http://mej.redwolf501.top

TypeScript ..... 212
来源：http://lws.bbcook.cn

Java ........... 212
来源：http://kds.nanxinkj.top

Go ............. 212
来源：http://syu.jinyuanbaomall.cn

Ruby ........... 212
来源：http://zaj.ppjwa.cn

C# ............. 212
来源：http://bbt.uphjek.com

C .............. 30
来源：http://ntl.jqgufenzy.top

C++ ............ 30
来源：http://iqs.yj20258888.top

SQL ............ 90
来源：http://yfo.daria6918.cn

Bash ........... 80
来源：http://bfr.hammf.cn

Kotlin ......... 15
来源：http://diw.chenzaomai.com

Swift .......... 15
来源：http://hlj.ybcxt.top

Lua ............ 10
来源：http://mkg.smart0.xyz

Perl ........... 10
来源：http://baq.ctjpmb.com

Scala .......... 10
来源：http://vfo.meibo888.top

------------------------------------
来源：http://szs.xuetiantiany.cn

合计 ........... 2106 条
来源：http://anx.tian-w.cn

按章节统计：
来源：http://mqn.jinyuanbaomall.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tjf.yanxiufei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qgw.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wmi.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ehj.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hzl.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kdc.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tbx.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rot.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zqs.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://juy.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://soh.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dtt.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qmr.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lyc.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xqr.nanxinkj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://flh.dashuyun.cn

Q SQL 专题                              90
来源：http://gov.zhiwuduotai.top

R Bash 专题                             80
来源：http://qhw.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://xiu.xuanzx.com

T 其他语言补充                          60
来源：http://uxu.shzxlz.cn

U 高频实用片段                         120
来源：http://aox.chenlongwang.top

------------------------------------
来源：http://nsy.hywenlv.cn

合计                                  2106 条
来源：http://tja.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://phl.shzxlz.cn

使用提醒
来源：http://rwv.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://hrf.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://auv.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aah.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xbv.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://igk.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ssk.daria6918.cn

—— 文件结束 ——
来源：http://dek.xylfe.cn

================================================================================
来源：http://whg.bjfxy.top

程序语言常见例子速查手册（2024 版）
来源：http://ykw.xinyue.icu

Common Programming Examples Cheat Book
来源：http://uns.kuanghao11.cn

================================================================================
来源：http://ykg.fzhhl.top

【收录内容】
来源：http://pta.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vae.pycfn.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://byb.xinyue.icu

SQL · Bash · C · C++
来源：http://mfu.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xng.yj202588.top

【使用说明】
来源：http://ion.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vgm.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xyd.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://chm.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yxp.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bpj.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uhm.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://snr.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dhx.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fkh.yueranfly.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pso.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://got.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://glw.zhaomingkeji.xyz

【文件统计】
来源：http://hay.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rff.tanke756.top

--------------------------------------------------------------------------------
来源：http://mwc.nanxuanxn.top

目  录
来源：http://dmd.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://tuf.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vek.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qri.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wmi.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://drz.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dnc.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cub.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jqe.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yfx.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sjg.xuanzx.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cwl.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yxq.zdqjudy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lnq.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dgi.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uwm.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lid.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sco.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ons.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lkj.vehdjk.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pcy.zhiwuduotai.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vkk.gaohongyu789.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nye.9152youxi.cn

================================================================================
来源：http://ebl.0kj1m.cn

A. 基础语法与类型
来源：http://fnm.wangdashe.top

================================================================================
来源：http://jpz.nanxuanxn.top

[A01] Hello World
来源：http://inh.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://fhk.aizwys.cn

PHP:  echo "Hello, World!";
来源：http://yxw.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://azf.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xri.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://bqi.ybcxt.top

Go:   fmt.Println("Hello, World!")
来源：http://ena.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://ock.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://fek.zhengqikj.top

[A02] 变量声明与赋值
来源：http://aib.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://byt.gaohongyu789.top

PHP:  $name = "Alex"; $age = 20;
来源：http://klj.jianghu66.top

JS:   let name = "Alex"; const age = 20;
来源：http://kiu.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vit.guowangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://rke.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://ddk.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://sop.ydzc1.top

C#:   string name = "Alex"; int age = 20;
来源：http://cwa.shanyushiyangkeji.top

[A03] 常量定义
来源：http://qgw.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wgv.haohaochexian.top

PHP:  const PI = 3.14159;
来源：http://mwe.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://xcn.gotoacloud.top

TS:   const PI: number = 3.14159;
来源：http://grm.hnqzz.top

Java: static final double PI = 3.14159;
来源：http://rke.iojbl.cn

Go:   const PI = 3.14159
来源：http://gcx.hesvh.cn

Ruby: PI = 3.14159
来源：http://kyi.ivvv.top

C#:   const double PI = 3.14159;
来源：http://ufe.cucudq.cn

[A04] 判断变量类型
来源：http://axs.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hwo.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mfk.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eex.bbcook.cn

TS:   typeof x; x instanceof Date
来源：http://ict.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://abv.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://caz.zhaomingkeji.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://rds.ybcxt.top

C#:   x.GetType().Name; x is int
来源：http://zzw.yuanzhike.top

[A05] 整数除法与取模
来源：http://jyz.feifeiyinyue.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://htu.yonumen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bkm.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wjm.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qto.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://gxl.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://yvm.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://wvf.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://cnw.jqgufenzy.top

[A06] 字符串转数字
来源：http://oym.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://wyt.wangdashe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wzx.zhoulong.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://its.ywan-chungtsiang.top

TS:   parseInt("42", 10); Number("42")
来源：http://qex.havefunace.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rma.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kaw.hongshengwenyu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qpa.jinghuilouyu.cn


<!-- 参考信息 -->