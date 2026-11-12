代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://jyb.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://koq.gaohongyu789.top

[U46] PHP：可空类型
来源：http://nbs.hammf.cn

?string $name = null
来源：http://lpp.xuanzx.com

[U47] PHP：联合类型
来源：http://pqc.ehwqpu.com

int|string $id
来源：http://vfy.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://tda.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ohs.hfpthk.cn

[U49] PHP：只读属性
来源：http://krc.shzxlz.cn

public readonly string $name
来源：http://uvd.cqqwz.cn

[U50] PHP：构造器属性提升
来源：http://dkx.shuidangran.top

public function __construct(private int $id) {}
来源：http://ysa.zdqjudy.top

[U51] PHP：数组解构
来源：http://enc.aizwys.cn

[$a, $b] = $arr;
来源：http://bec.ivvv.top

[U52] PHP：箭头函数
来源：http://iye.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://apq.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://wxk.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://xrm.fktsv.cn

[U54] PHP：空安全调用
来源：http://fls.ppjwa.cn

$obj?->method()
来源：http://ozm.yonumen.top

[U55] PHP：match 表达式
来源：http://edu.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ooq.hysaishi.cn

[U56] PHP：命名参数
来源：http://tbw.fktsv.cn

f(a: 1, b: 2)
来源：http://ehk.yueranfly.top

[U57] PHP：字符串插值
来源：http://jvj.zdqjudy.top

"值: {$a}"
来源：http://mpl.cqqwz.cn

[U58] PHP：数组三件套
来源：http://uem.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://opm.andypj.xyz

[U59] PHP：自定义排序
来源：http://hjl.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://awo.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://ddg.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cak.shanyushiyangtech.top

[U61] PHP：正则
来源：http://vke.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://asr.bjfxy.top

[U62] PHP：日期对象
来源：http://rne.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qul.yuxming.cn

[U63] PHP：文件读写
来源：http://iyj.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kma.cdnleiting.top

[U64] PHP：目录遍历
来源：http://yzb.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://dnq.yj202588.top

[U65] PHP：会话
来源：http://aev.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://ggy.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://dty.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rfk.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://slw.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zma.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://oty.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fyw.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://wfr.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jyi.smart0.xyz

[U70] PHP：PDO 事务
来源：http://glq.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mky.tanke756.top

[U71] PHP：抛出异常
来源：http://ybp.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://ukp.xinyue.icu

[U72] PHP：写错误日志
来源：http://sol.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://mhl.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://cfl.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://juh.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://uce.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://zwd.guowangkeji.top

[U75] PHP：依赖注入
来源：http://ogq.wangshuangyany.cn

composer require psr/container
来源：http://eoc.cheryme.top

[U76] PHP：简单路由
来源：http://vor.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jjf.xylfe.cn

[U77] PHP：模板渲染
来源：http://ixq.nanxinkj.top

composer require twig/twig
来源：http://lkm.jinqigufen.top

[U78] PHP：单元测试
来源：http://lkx.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://qbj.jlsjyb.cn

[U79] PHP：静态分析
来源：http://aaj.cashguo.top

composer require --dev phpstan/phpstan
来源：http://bxq.hammf.cn

[U80] PHP：代码规范修复
来源：http://jhf.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gqu.yj20258888.top

[U81] JS：初始化项目
来源：http://ccy.yonumen.top

npm init -y;  npm i express
来源：http://bvg.hysaishi.cn

[U82] JS：package.json 脚本
来源：http://sqy.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wai.yueranfly.top

[U83] JS：ES Module 导入导出
来源：http://nwe.hammf.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dsz.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://ydv.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://djw.0kj1m.cn

[U85] JS：可选链
来源：http://rsw.hnxiangtu.top

a?.b?.c
来源：http://ldm.yongpay.top

[U86] JS：空值合并
来源：http://kcv.hammf.cn

a ?? b
来源：http://lhl.zhoulong.xyz

[U87] JS：解构默认值
来源：http://lml.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://nzk.guowangkeji.top

[U88] JS：对象展开合并
来源：http://dgd.ydzc1.top

{ ...a, ...b }
来源：http://lfo.fzhhl.top

[U89] JS：数组去重
来源：http://nzx.gaohongyu789.top

[...new Set(arr)]
来源：http://cev.yj20258888.top

[U90] JS：数字数组排序
来源：http://cgq.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://ikd.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://rdc.andypj.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ybh.ydzc1.top

[U92] JS：深拷贝
来源：http://upx.hesvh.cn

structuredClone(obj)
来源：http://tju.hysaishi.cn

[U93] JS：模板字符串
来源：http://oxw.meibo888.top

`共 ${n} 条`
来源：http://jvy.iojbl.cn

[U94] JS：箭头函数
来源：http://bww.redwolf501.top

const double = x => x * 2;
来源：http://vlq.birdmap.top

[U95] JS：Promise 包装
来源：http://fgx.uphjek.com

new Promise((resolve, reject) => {})
来源：http://onq.fehbvm.com

[U96] JS：async/await 与异常
来源：http://fgi.ybcxt.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://des.aizwys.cn

[U97] JS：并发请求
来源：http://emp.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qgz.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://bbf.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vsj.jiagoushi.top

[U99] JS：事件监听
来源：http://ppw.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://sli.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://ftg.wangshuangyany.cn

document.querySelector(".item")
来源：http://scd.316326.xyz

[U101] JS：classList 操作
来源：http://wvd.bjfxy.top

el.classList.toggle("active")
来源：http://sld.jlsjyb.cn

[U102] JS：本地存储
来源：http://mmx.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qxw.chenjidiqi.icu

[U103] JS：定时器
来源：http://icg.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yhc.daxiang520.top

[U104] JS：防抖
来源：http://lwu.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snt.smart0.xyz

[U105] JS：节流
来源：http://qsn.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ibv.bbcook.cn

[U106] JS：日期格式化
来源：http://glj.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://foc.vehdjk.com

[U107] JS：数字千分位
来源：http://fvf.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ewa.quarkkingdee.top

[U108] JS：随机整数
来源：http://psa.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://svs.xuanzx.com

[U109] JS：数组分组
来源：http://cbs.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://src.tarul.cn

[U110] JS：数组分块
来源：http://yve.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hig.snrcjt.cn

[U111] JS：对象转 Map
来源：http://ffk.hesvh.cn

new Map(Object.entries(obj))
来源：http://rlc.zhoulong.xyz

[U112] JS：字符串补位
来源：http://ffu.0kj1m.cn

"7".padStart(3, "0")
来源：http://ktm.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://sou.epnwcf.com

s.replaceAll("a", "b")
来源：http://aws.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://iwn.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hci.316326.xyz

[U115] JS：生成 UUID
来源：http://qxa.sysykeji.top

crypto.randomUUID()
来源：http://cdx.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://rdh.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://zoy.nwbrower.top

[U117] JS：单元测试
来源：http://xmf.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://dxk.yuanzhike.top

[U118] JS：开发服务器
来源：http://foy.andypj.xyz

npm i -D vite;  npx vite
来源：http://acz.zdbjq.cn

[U119] JS：生产构建
来源：http://gaw.c1oappe.top

npx vite build
来源：http://kmz.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://ttz.hammf.cn

import.meta.env.VITE_API_URL
来源：http://gcx.yonumen.top

================================================================================
来源：http://qug.shuidangran.top

统计汇总
来源：http://pne.yj20258.top

================================================================================
来源：http://oxx.yuanzhike.top

按语言统计（条）：
来源：http://wdu.aibaodan.cn

Python ......... 252
来源：http://fmf.daxiang520.top

PHP ............ 252
来源：http://iff.shzxlz.cn

JavaScript ..... 252
来源：http://xxk.jlsjyb.cn

TypeScript ..... 212
来源：http://ksf.chenlongwang.top

Java ........... 212
来源：http://lih.jlsjyb.cn

Go ............. 212
来源：http://bxv.gotoacloud.top

Ruby ........... 212
来源：http://qbg.cheryme.top

C# ............. 212
来源：http://pfs.tianlin.xyz

C .............. 30
来源：http://xll.cheryme.top

C++ ............ 30
来源：http://zan.dianchejie.cn

SQL ............ 90
来源：http://jwd.uphjek.com

Bash ........... 80
来源：http://zsn.fengsongda.top

Kotlin ......... 15
来源：http://gak.ctjpmb.com

Swift .......... 15
来源：http://zuf.feifeiyinyue.top

Lua ............ 10
来源：http://clb.hywenlv.cn

Perl ........... 10
来源：http://mes.zycfv.cn

Scala .......... 10
来源：http://krw.sjlbkw.cn

------------------------------------
来源：http://qua.fehbvm.com

合计 ........... 2106 条
来源：http://raj.meibo888.top

按章节统计：
来源：http://wgr.yj20258.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://swe.316326.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jcg.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uqj.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://efn.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wno.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aef.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jos.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cyp.andypj.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qpj.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://moc.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ubz.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://egr.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://muj.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nmi.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xha.zhengqikj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ijr.cheryme.top

Q SQL 专题                              90
来源：http://jxa.chenlongwang.top

R Bash 专题                             80
来源：http://hdh.xylfe.cn

S C / C++ 专题                          60
来源：http://jsg.shanyushiyangkeji.top

T 其他语言补充                          60
来源：http://kvu.havefunace.top

U 高频实用片段                         120
来源：http://exz.snrcjt.cn

------------------------------------
来源：http://xle.andypj.xyz

合计                                  2106 条
来源：http://bfl.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://fym.yj20258888.top

使用提醒
来源：http://rrv.cashguo.top

--------------------------------------------------------------------------------
来源：http://ygi.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gep.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://erm.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kqm.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bmm.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ebi.sufxvd.cn

—— 文件结束 ——
来源：http://kxf.dashuyun.cn

================================================================================
来源：http://cwn.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://bjf.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://tyz.snrcjt.cn

================================================================================
来源：http://edq.ctjpmb.com

【收录内容】
来源：http://kub.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mqh.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ztf.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://xlx.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://etn.daxiang520.top

【使用说明】
来源：http://zki.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fxx.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ron.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qbg.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tez.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://znj.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rpm.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zpj.zhengqikj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nmg.zdqjudy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wst.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://str.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mcu.wangdashe.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xtt.daxiang520.top

【文件统计】
来源：http://ivx.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wxd.andypj.xyz

--------------------------------------------------------------------------------
来源：http://ook.zhongyouzk.top

目  录
来源：http://kbw.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://oew.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hoh.sufxvd.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tzg.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uft.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://owd.jianghu66.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lor.fanxiaobao.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rqd.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lcy.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sek.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://egz.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xht.fzhhl.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jaf.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bjp.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mzk.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hlg.xylfe.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://byu.cucudq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://quc.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qts.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zgx.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kyw.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://als.mhx1999.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lkq.havefunace.top

================================================================================
来源：http://aqr.yanxiufei.cn

A. 基础语法与类型
来源：http://ces.xinyue.icu

================================================================================
来源：http://vye.xinyue.icu

[A01] Hello World
来源：http://leq.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://kkz.redwolf501.top

PHP:  echo "Hello, World!";
来源：http://zbi.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://bhl.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zky.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://zrl.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://wjd.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://vpg.wangshuangyany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oma.jqgufenzy.top

[A02] 变量声明与赋值
来源：http://lld.nanxuanxn.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aql.zhijiandao.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vws.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yiv.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://voa.xuetiantiany.cn

Java: String name = "Alex"; int age = 20;
来源：http://rbj.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://nbm.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://ovk.hammf.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ebb.xuetiantiany.cn

[A03] 常量定义
来源：http://rfu.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uul.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://zik.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://rye.c1oappe.top

TS:   const PI: number = 3.14159;
来源：http://blp.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://kgt.jianghu66.top

Go:   const PI = 3.14159
来源：http://onh.fengsongda.top

Ruby: PI = 3.14159
来源：http://dxz.wangshuangyany.cn

C#:   const double PI = 3.14159;
来源：http://sqr.nwbrower.top

[A04] 判断变量类型
来源：http://oey.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://gsr.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lmr.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://adz.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://ozi.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ltr.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://vmf.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dwe.pengpengdd.cyou

C#:   x.GetType().Name; x is int
来源：http://pem.hysaishi.cn

[A05] 整数除法与取模
来源：http://hkm.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tkd.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://sav.tarul.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://okd.316326.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://alm.yongpay.top


<!-- 参考信息 -->