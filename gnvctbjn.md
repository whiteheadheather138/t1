代发 wailian999

[U53] PHP：空合并运算符
来源：http://ggz.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://xcs.pycfn.com

[U54] PHP：空安全调用
来源：http://jvt.pycfn.com

$obj?->method()
来源：http://qrk.hesvh.cn

[U55] PHP：match 表达式
来源：http://alf.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pht.mhx1999.top

[U56] PHP：命名参数
来源：http://bak.hywenlv.cn

f(a: 1, b: 2)
来源：http://ufu.hammf.cn

[U57] PHP：字符串插值
来源：http://xaw.sweek.top

"值: {$a}"
来源：http://jtc.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://dgn.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://asx.hysaishi.cn

[U59] PHP：自定义排序
来源：http://vre.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvi.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://bfn.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gro.yonumen.top

[U61] PHP：正则
来源：http://kqw.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fjo.yuxming.cn

[U62] PHP：日期对象
来源：http://rqi.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://igr.9152youxi.cn

[U63] PHP：文件读写
来源：http://dgl.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pqn.epnwcf.com

[U64] PHP：目录遍历
来源：http://npg.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://eqs.sysykeji.top

[U65] PHP：会话
来源：http://zoi.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://txt.havefunace.top

[U66] PHP：设置 Cookie
来源：http://iwu.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eyh.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://sqm.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pzv.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://tdi.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zjs.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://mcv.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rhr.hammf.cn

[U70] PHP：PDO 事务
来源：http://abq.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kmu.sweek.top

[U71] PHP：抛出异常
来源：http://tsa.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://hvq.chenzaomai.com

[U72] PHP：写错误日志
来源：http://ipi.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://rit.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://mcw.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://nsn.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://qrk.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://htc.sufxvd.cn

[U75] PHP：依赖注入
来源：http://ued.hnqzz.top

composer require psr/container
来源：http://hdo.jqgfzy.top

[U76] PHP：简单路由
来源：http://trs.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ldv.yuanzhike.top

[U77] PHP：模板渲染
来源：http://kdz.meibo888.top

composer require twig/twig
来源：http://xdf.fengsongda.top

[U78] PHP：单元测试
来源：http://gxq.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://dfy.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://twn.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://tjx.52xcode.cn

[U80] PHP：代码规范修复
来源：http://yhr.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hdq.ivvv.top

[U81] JS：初始化项目
来源：http://fvc.ydjk.org.cn

npm init -y;  npm i express
来源：http://uin.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://jwv.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://evk.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://fom.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://kwu.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://dcr.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://vol.jinghuilouyu.cn

[U85] JS：可选链
来源：http://upv.sysykeji.top

a?.b?.c
来源：http://yam.yuxming.cn

[U86] JS：空值合并
来源：http://dis.shzxlz.cn

a ?? b
来源：http://cqb.ivvv.top

[U87] JS：解构默认值
来源：http://aso.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://gui.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://fwv.ehwqpu.com

{ ...a, ...b }
来源：http://zbf.fehbvm.com

[U89] JS：数组去重
来源：http://hiw.zhongyouzk.top

[...new Set(arr)]
来源：http://bxt.zdbjq.cn

[U90] JS：数字数组排序
来源：http://hro.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://qrb.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://avt.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hoz.ehwqpu.com

[U92] JS：深拷贝
来源：http://qcf.hywenlv.cn

structuredClone(obj)
来源：http://rcd.zhongyouzk.top

[U93] JS：模板字符串
来源：http://shr.sxryk.cn

`共 ${n} 条`
来源：http://cdb.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://lim.epnwcf.com

const double = x => x * 2;
来源：http://cxc.yueranfly.top

[U95] JS：Promise 包装
来源：http://rzr.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://wws.xinyue.icu

[U96] JS：async/await 与异常
来源：http://miw.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ayt.zhijiandao.cn

[U97] JS：并发请求
来源：http://ujn.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://gcn.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://pwy.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ujy.cashguo.top

[U99] JS：事件监听
来源：http://pfq.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://kqx.hfpthk.cn

[U100] JS：DOM 查询
来源：http://pxe.jlsjyb.cn

document.querySelector(".item")
来源：http://fcl.hammf.cn

[U101] JS：classList 操作
来源：http://zfr.andypj.xyz

el.classList.toggle("active")
来源：http://ukx.jqgfzy.top

[U102] JS：本地存储
来源：http://inf.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ecu.cheryme.top

[U103] JS：定时器
来源：http://qkw.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mld.zhijiandao.cn

[U104] JS：防抖
来源：http://yru.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcb.shzxlz.cn

[U105] JS：节流
来源：http://lrb.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aur.redwolf501.top

[U106] JS：日期格式化
来源：http://udt.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mxh.daria6918.cn

[U107] JS：数字千分位
来源：http://ifv.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ebr.wangshuangyany.cn

[U108] JS：随机整数
来源：http://szd.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://duq.fehbvm.com

[U109] JS：数组分组
来源：http://rzm.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://eyq.ydzc1.top

[U110] JS：数组分块
来源：http://msz.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lec.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://oxk.yj20258.top

new Map(Object.entries(obj))
来源：http://rit.jqgufenzy.top

[U112] JS：字符串补位
来源：http://ukq.dianchejie.cn

"7".padStart(3, "0")
来源：http://cnz.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://drt.jqgfzy.top

s.replaceAll("a", "b")
来源：http://rny.daria6918.cn

[U114] JS：JSON 深比较
来源：http://ght.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wre.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://kcr.hfpthk.cn

crypto.randomUUID()
来源：http://oqo.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://nky.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://hyq.bjfxy.top

[U117] JS：单元测试
来源：http://naj.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://vzh.fktsv.cn

[U118] JS：开发服务器
来源：http://lup.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://jkw.gzhubu.top

[U119] JS：生产构建
来源：http://vba.tianlin.xyz

npx vite build
来源：http://aqh.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://zzp.yj202588.top

import.meta.env.VITE_API_URL
来源：http://mfc.ivvv.top

================================================================================
来源：http://qnw.daxiang520.top

统计汇总
来源：http://ciu.nanxuanxn.top

================================================================================
来源：http://zrx.jiagoushi.top

按语言统计（条）：
来源：http://ufx.quarkkingdee.top

Python ......... 252
来源：http://vxw.mhx1999.top

PHP ............ 252
来源：http://bjc.yuanzhike.top

JavaScript ..... 252
来源：http://ilg.fengsongda.top

TypeScript ..... 212
来源：http://wbg.sysykeji.top

Java ........... 212
来源：http://kru.haohaochexian.top

Go ............. 212
来源：http://lnt.hammf.cn

Ruby ........... 212
来源：http://chc.0kj1m.cn

C# ............. 212
来源：http://tkz.svipenyu.cn

C .............. 30
来源：http://dlo.quarkkingdee.top

C++ ............ 30
来源：http://gpx.sjlbkw.cn

SQL ............ 90
来源：http://qci.bbcook.cn

Bash ........... 80
来源：http://kxh.xinyue.icu

Kotlin ......... 15
来源：http://bzf.cdnleiting.top

Swift .......... 15
来源：http://rag.hywenlv.cn

Lua ............ 10
来源：http://muc.zhongyouzk.top

Perl ........... 10
来源：http://nin.snrcjt.cn

Scala .......... 10
来源：http://san.tian-w.cn

------------------------------------
来源：http://nmu.hfpthk.cn

合计 ........... 2106 条
来源：http://yvo.zhaomingkeji.xyz

按章节统计：
来源：http://cir.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jcx.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fwk.hnqzz.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kie.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ygl.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://icn.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jjr.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://weg.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kfq.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iyn.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://asa.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://axy.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pgv.cdnleiting.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ehj.zhongyouzk.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dky.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rud.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fpy.havefunace.top

Q SQL 专题                              90
来源：http://dtc.bjfxy.top

R Bash 专题                             80
来源：http://ank.guannengcc.top

S C / C++ 专题                          60
来源：http://vez.yj20258.top

T 其他语言补充                          60
来源：http://rzp.hesvh.cn

U 高频实用片段                         120
来源：http://hpt.zhengqikj.top

------------------------------------
来源：http://wwz.epnwcf.com

合计                                  2106 条
来源：http://jrd.meibo888.top

--------------------------------------------------------------------------------
来源：http://bjd.hywenlv.cn

使用提醒
来源：http://akw.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://zjx.ybcxt.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mlb.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://snx.shangyingyoupin.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xxm.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kws.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://muv.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://tfs.ppjwa.cn

================================================================================
来源：http://urz.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://ouk.gzhubu.top

Common Programming Examples Cheat Book
来源：http://ran.jinghuilouyu.cn

================================================================================
来源：http://uyp.zhoulong.xyz

【收录内容】
来源：http://nsf.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://plz.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gcg.yangfankeji.com

SQL · Bash · C · C++
来源：http://plo.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lkb.guowangkeji.top

【使用说明】
来源：http://jwr.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cxo.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yfc.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://udz.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nlk.fzhhl.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fjq.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yvi.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pih.guannengcc.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yqz.yj20258.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wau.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pdw.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xkq.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://teo.nanxuanxn.top

【文件统计】
来源：http://izu.redwolf501.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ezy.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://fbm.guowangkeji.top

目  录
来源：http://rhk.andypj.xyz

--------------------------------------------------------------------------------
来源：http://dvl.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tiv.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jib.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://inl.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ppo.tianlin.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://frw.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qzb.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xih.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ntz.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yea.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wmw.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bcp.pengpengdd.cyou

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xno.daxiang520.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jqg.hfpthk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kct.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xab.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rdw.zhoulong.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qoh.hammf.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gva.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uyr.zhijiandao.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tuo.shangyingyoupin.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mux.jqgfzy.top

================================================================================
来源：http://vga.dashuyun.cn

A. 基础语法与类型
来源：http://ufv.smart0.xyz

================================================================================
来源：http://bua.chenlongwang.top

[A01] Hello World
来源：http://ukn.yfazqb.com

Py:   print("Hello, World!")
来源：http://qvo.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://roo.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://ztq.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hgm.pengpengdd.cyou

Java: System.out.println("Hello, World!");
来源：http://zwg.vehdjk.com

Go:   fmt.Println("Hello, World!")
来源：http://isf.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://ivj.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ira.fktsv.cn

[A02] 变量声明与赋值
来源：http://xbo.yuxming.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lnl.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uwz.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://ctq.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qpa.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://nlb.sweek.top

Go:   name := "Alex"; age := 20
来源：http://hwr.wangshuangyany.cn

Ruby: name = "Alex"; age = 20
来源：http://wlh.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://skh.jinghuilouyu.cn

[A03] 常量定义
来源：http://cff.52xcode.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zww.yongpay.top

PHP:  const PI = 3.14159;
来源：http://vow.svipenyu.cn

JS:   const PI = 3.14159;
来源：http://enk.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://blk.yj20258.top

Java: static final double PI = 3.14159;
来源：http://oet.tanke756.top

Go:   const PI = 3.14159
来源：http://dsg.birdmap.top

Ruby: PI = 3.14159
来源：http://kea.daxiang520.top

C#:   const double PI = 3.14159;
来源：http://unn.dashuyun.cn

[A04] 判断变量类型
来源：http://mlc.gotoacloud.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qpj.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://maz.gaohongyu789.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bzf.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://mja.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nec.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://zdm.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lnz.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://tof.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://xau.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zkc.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rzz.hysaishi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://llu.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://psb.shzxlz.cn

Java: 7 / 2; 7 % 2
来源：http://mbe.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://nfe.svipenyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://fjr.havefunace.top

C#:   7 / 2; 7 % 2
来源：http://zae.yongpay.top

[A06] 字符串转数字
来源：http://sjy.yangfankeji.com

Py:   int("42"); float("3.14")
来源：http://nev.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://viq.hnqzz.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cax.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://uzz.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uum.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xnc.tarul.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rhe.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://scj.yuxming.cn

[A07] 数字转字符串
来源：http://mms.vehdjk.com

Py:   str(42)
来源：http://tbn.zhiwuduotai.top

PHP:  (string) 42; strval(42)
来源：http://rla.hesvh.cn


<!-- 参考信息 -->