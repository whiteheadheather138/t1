代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://ykx.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rzc.sysykeji.top

[U46] PHP：可空类型
来源：http://iar.zhongyouzk.top

?string $name = null
来源：http://zhe.ydjk.org.cn

[U47] PHP：联合类型
来源：http://qua.hfpthk.cn

int|string $id
来源：http://ldu.shuidangran.top

[U48] PHP：纯枚举
来源：http://fgq.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pqv.smart0.xyz

[U49] PHP：只读属性
来源：http://elh.jinyuanbaomall.cn

public readonly string $name
来源：http://fcx.hammf.cn

[U50] PHP：构造器属性提升
来源：http://hme.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://tbw.zhijiandao.cn

[U51] PHP：数组解构
来源：http://ozh.jqgfzy.top

[$a, $b] = $arr;
来源：http://kpu.meibo888.top

[U52] PHP：箭头函数
来源：http://mrf.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://pob.52xcode.cn

[U53] PHP：空合并运算符
来源：http://dzj.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://miw.tarul.cn

[U54] PHP：空安全调用
来源：http://udo.yangfankeji.com

$obj?->method()
来源：http://zjt.pycfn.com

[U55] PHP：match 表达式
来源：http://ppx.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rsf.daria6918.cn

[U56] PHP：命名参数
来源：http://pur.jianghu66.top

f(a: 1, b: 2)
来源：http://wct.redwolf501.top

[U57] PHP：字符串插值
来源：http://vrn.sweek.top

"值: {$a}"
来源：http://vku.hywenlv.cn

[U58] PHP：数组三件套
来源：http://pis.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://byj.yonumen.top

[U59] PHP：自定义排序
来源：http://lgw.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whw.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://zax.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://web.yueranfly.top

[U61] PHP：正则
来源：http://wmk.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lcw.gogol.net.cn

[U62] PHP：日期对象
来源：http://app.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cuo.0kj1m.cn

[U63] PHP：文件读写
来源：http://nsd.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cir.ppjwa.cn

[U64] PHP：目录遍历
来源：http://pwk.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://jqh.gzhubu.top

[U65] PHP：会话
来源：http://awd.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ucp.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://emx.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vsh.jianghu66.top

[U67] PHP：处理文件上传
来源：http://jxc.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cby.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://xfd.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qbf.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://eil.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xdn.vehdjk.com

[U70] PHP：PDO 事务
来源：http://wxu.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lmf.sweek.top

[U71] PHP：抛出异常
来源：http://dap.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://ofe.hammf.cn

[U72] PHP：写错误日志
来源：http://ezx.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://kyx.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://fhw.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://ygt.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://wmi.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://xlz.haohaochexian.top

[U75] PHP：依赖注入
来源：http://vgy.aibaodan.cn

composer require psr/container
来源：http://tpp.yuxming.cn

[U76] PHP：简单路由
来源：http://ffa.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ntv.316326.xyz

[U77] PHP：模板渲染
来源：http://bdv.yangfankeji.com

composer require twig/twig
来源：http://ogr.hysaishi.cn

[U78] PHP：单元测试
来源：http://hxa.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://cyf.pycfn.com

[U79] PHP：静态分析
来源：http://qgh.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://xjh.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://utr.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://afc.xziqi.cn

[U81] JS：初始化项目
来源：http://ftx.hnxiangtu.top

npm init -y;  npm i express
来源：http://zpx.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://qxo.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ehd.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://ckb.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://zej.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://cpb.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://bxt.yj202588.top

[U85] JS：可选链
来源：http://ssw.uphjek.com

a?.b?.c
来源：http://lww.yangfankeji.com

[U86] JS：空值合并
来源：http://vre.zhiwuduotai.top

a ?? b
来源：http://lrd.sjlbkw.cn

[U87] JS：解构默认值
来源：http://iys.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://mbt.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://jcs.epnwcf.com

{ ...a, ...b }
来源：http://cjq.gaohongyu789.top

[U89] JS：数组去重
来源：http://rau.fktsv.cn

[...new Set(arr)]
来源：http://ies.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://qvf.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://ygs.yj20258888.top

[U91] JS：对象键值遍历
来源：http://ilx.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://awj.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://ssv.ehwqpu.com

structuredClone(obj)
来源：http://ziu.guowangkeji.top

[U93] JS：模板字符串
来源：http://bqb.zhoulong.xyz

`共 ${n} 条`
来源：http://xkb.iojbl.cn

[U94] JS：箭头函数
来源：http://wrw.ybcxt.top

const double = x => x * 2;
来源：http://phw.cdnleiting.top

[U95] JS：Promise 包装
来源：http://nph.jqgufenzy.top

new Promise((resolve, reject) => {})
来源：http://cfy.redwolf501.top

[U96] JS：async/await 与异常
来源：http://bhj.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ozq.chenjidiqi.icu

[U97] JS：并发请求
来源：http://uju.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://epi.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://uio.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wrb.kuanghao11.cn

[U99] JS：事件监听
来源：http://srj.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://zus.cheryme.top

[U100] JS：DOM 查询
来源：http://xlk.ctjpmb.com

document.querySelector(".item")
来源：http://zir.yj20258.top

[U101] JS：classList 操作
来源：http://jhe.yfazqb.com

el.classList.toggle("active")
来源：http://pyn.cashguo.top

[U102] JS：本地存储
来源：http://iqj.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bmv.shangyingyoupin.top

[U103] JS：定时器
来源：http://dqf.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gaz.0kj1m.cn

[U104] JS：防抖
来源：http://gsq.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onk.pengpengdd.cyou

[U105] JS：节流
来源：http://mcp.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pes.zhengqikj.top

[U106] JS：日期格式化
来源：http://rod.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bly.meibo888.top

[U107] JS：数字千分位
来源：http://qxq.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://otq.vehdjk.com

[U108] JS：随机整数
来源：http://ecf.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://byv.hysaishi.cn

[U109] JS：数组分组
来源：http://frh.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://rmh.quarkkingdee.top

[U110] JS：数组分块
来源：http://anr.jinyuanbaomall.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iyy.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://syg.zdbjq.cn

new Map(Object.entries(obj))
来源：http://sot.sjlbkw.cn

[U112] JS：字符串补位
来源：http://xiy.cqqwz.cn

"7".padStart(3, "0")
来源：http://dkh.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://gag.zycfv.cn

s.replaceAll("a", "b")
来源：http://mzw.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://ihu.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://jhc.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://eea.shzxlz.cn

crypto.randomUUID()
来源：http://pvv.sxryk.cn

[U116] JS：类型检查（JSDoc）
来源：http://lzl.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://cdf.jqgfzy.top

[U117] JS：单元测试
来源：http://vpq.sweek.top

npm i -D vitest;  npx vitest
来源：http://rah.aizwys.cn

[U118] JS：开发服务器
来源：http://ufi.sysykeji.top

npm i -D vite;  npx vite
来源：http://scl.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://pfm.chenlongwang.top

npx vite build
来源：http://gtw.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://bvf.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://uor.guannengcc.top

================================================================================
来源：http://xsa.pycfn.com

统计汇总
来源：http://bum.yongpay.top

================================================================================
来源：http://kqy.hesvh.cn

按语言统计（条）：
来源：http://lpu.cdnleiting.top

Python ......... 252
来源：http://jzh.ydzc1.top

PHP ............ 252
来源：http://yma.hfpthk.cn

JavaScript ..... 252
来源：http://pkd.daria6918.cn

TypeScript ..... 212
来源：http://eey.zhengqikj.top

Java ........... 212
来源：http://uxo.yanxiufei.cn

Go ............. 212
来源：http://qhj.dianchejie.cn

Ruby ........... 212
来源：http://eoq.ydjk.org.cn

C# ............. 212
来源：http://xol.zhaomingkeji.xyz

C .............. 30
来源：http://wut.guowangkeji.top

C++ ............ 30
来源：http://fwd.iojbl.cn

SQL ............ 90
来源：http://mlx.ywan-chungtsiang.top

Bash ........... 80
来源：http://sfu.kuanghao11.cn

Kotlin ......... 15
来源：http://xih.0kj1m.cn

Swift .......... 15
来源：http://ltg.hnxiangtu.top

Lua ............ 10
来源：http://zas.yvedp.cn

Perl ........... 10
来源：http://lze.guannengcc.top

Scala .......... 10
来源：http://efg.hnqzz.top

------------------------------------
来源：http://qys.c1oappe.top

合计 ........... 2106 条
来源：http://dqz.yj20258.top

按章节统计：
来源：http://afn.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tqu.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lrb.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xhe.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wxy.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wmq.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jov.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://coi.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://btf.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sck.hysaishi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ezi.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lnl.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mlh.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cdk.vehdjk.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ltu.zdqjudy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jjm.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bew.tanke756.top

Q SQL 专题                              90
来源：http://jrd.aibaodan.cn

R Bash 专题                             80
来源：http://lgi.sjlbkw.cn

S C / C++ 专题                          60
来源：http://pch.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://qww.feifeiyinyue.top

U 高频实用片段                         120
来源：http://imk.gotoacloud.top

------------------------------------
来源：http://asg.zhongyouzk.top

合计                                  2106 条
来源：http://wsn.hammf.cn

--------------------------------------------------------------------------------
来源：http://rsn.hfpthk.cn

使用提醒
来源：http://ggq.uphjek.com

--------------------------------------------------------------------------------
来源：http://zar.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jnh.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cni.316326.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eqs.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bkk.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pkt.shuidangran.top

—— 文件结束 ——
来源：http://hzk.yonumen.top

================================================================================
来源：http://fzh.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://zja.sjlbkw.cn

Common Programming Examples Cheat Book
来源：http://izq.zhiwuduotai.top

================================================================================
来源：http://xuu.fengsongda.top

【收录内容】
来源：http://ipp.snrcjt.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kks.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sht.yfazqb.com

SQL · Bash · C · C++
来源：http://trx.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jbd.yonumen.top

【使用说明】
来源：http://qyx.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qpi.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rnh.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ffi.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xun.jqgfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ymw.snrcjt.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bcc.mhx1999.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jsl.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bwn.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jby.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rpj.yonumen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://noq.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ubt.epnwcf.com

【文件统计】
来源：http://wwu.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qbk.iojbl.cn

--------------------------------------------------------------------------------
来源：http://oqt.hywenlv.cn

目  录
来源：http://vot.guannengcc.top

--------------------------------------------------------------------------------
来源：http://yan.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://txs.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hty.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xsh.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ksd.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zse.jinyuanbaomall.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lwv.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qyl.fzhhl.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nwr.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://atk.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oef.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://egd.svipenyu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qnj.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cwn.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tjj.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ivy.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ypk.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://guw.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vcc.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bbr.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wki.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rvc.yfazqb.com

================================================================================
来源：http://eiu.zhengqikj.top

A. 基础语法与类型
来源：http://krt.ybcxt.top

================================================================================
来源：http://cvi.bbcook.cn

[A01] Hello World
来源：http://xyx.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://mlz.guowangkeji.top

PHP:  echo "Hello, World!";
来源：http://ywp.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://rli.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tgw.yuxming.cn

Java: System.out.println("Hello, World!");
来源：http://amo.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://sns.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://mvh.yueranfly.top

C#:   Console.WriteLine("Hello, World!");
来源：http://oke.meibo888.top

[A02] 变量声明与赋值
来源：http://ewe.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ail.sufxvd.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dbg.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wcn.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ahc.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://wpz.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://yoj.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://kwc.jinyuanbaomall.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xbr.aibaodan.cn

[A03] 常量定义
来源：http://oxl.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rbd.wangdashe.top

PHP:  const PI = 3.14159;
来源：http://gfh.shanyushiyangtech.top

JS:   const PI = 3.14159;
来源：http://wtp.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://urq.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://vkc.c1oappe.top

Go:   const PI = 3.14159
来源：http://fbb.chenlongwang.top

Ruby: PI = 3.14159
来源：http://max.aizwys.cn

C#:   const double PI = 3.14159;
来源：http://lad.shzxlz.cn

[A04] 判断变量类型
来源：http://tpz.hcnkem.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://cjr.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nlk.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://azr.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://ryg.ywan-chungtsiang.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mvo.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://ifh.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cdh.xinyue.icu

C#:   x.GetType().Name; x is int
来源：http://bdd.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://siy.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://god.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mnm.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ush.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vvh.c1oappe.top


<!-- 参考信息 -->