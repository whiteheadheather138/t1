代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://omb.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wtu.bjfxy.top

[U46] PHP：可空类型
来源：http://lce.yj202588.top

?string $name = null
来源：http://ztk.jinqigufen.top

[U47] PHP：联合类型
来源：http://syb.sysykeji.top

int|string $id
来源：http://kwb.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://hav.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vrn.jinqigufen.top

[U49] PHP：只读属性
来源：http://vhl.ybcxt.top

public readonly string $name
来源：http://kwa.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://evd.birdmap.top

public function __construct(private int $id) {}
来源：http://pxb.iojbl.cn

[U51] PHP：数组解构
来源：http://azm.jqgfzy.top

[$a, $b] = $arr;
来源：http://cnx.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://fay.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://qld.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://afe.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://ion.jianghu66.top

[U54] PHP：空安全调用
来源：http://wzp.xuetiantiany.cn

$obj?->method()
来源：http://gmy.ctjpmb.com

[U55] PHP：match 表达式
来源：http://eiz.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://org.yj202588.top

[U56] PHP：命名参数
来源：http://nfx.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://siu.zdbjq.cn

[U57] PHP：字符串插值
来源：http://bgd.yuxming.cn

"值: {$a}"
来源：http://vzb.jqgfzy.top

[U58] PHP：数组三件套
来源：http://spg.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mzf.wangdashe.top

[U59] PHP：自定义排序
来源：http://gai.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wor.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://mlo.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wtg.snrcjt.cn

[U61] PHP：正则
来源：http://fag.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yym.zhixingplan.top

[U62] PHP：日期对象
来源：http://bqo.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gfg.jinqigfzy.top

[U63] PHP：文件读写
来源：http://nwh.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jwk.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://izz.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://omw.zdqjudy.top

[U65] PHP：会话
来源：http://mnu.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cin.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://eyw.jqgfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lvy.wangdashe.top

[U67] PHP：处理文件上传
来源：http://nms.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://woa.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://ztk.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://icj.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://xja.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pbz.daxiang520.top

[U70] PHP：PDO 事务
来源：http://yyc.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jyi.fktsv.cn

[U71] PHP：抛出异常
来源：http://ypz.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://mgg.zhixingplan.top

[U72] PHP：写错误日志
来源：http://hie.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://esk.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://wjq.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://fsl.sweek.top

[U74] PHP：读取环境变量
来源：http://lci.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://iyr.nanxinkj.top

[U75] PHP：依赖注入
来源：http://ggp.yuxming.cn

composer require psr/container
来源：http://bto.guannengcc.top

[U76] PHP：简单路由
来源：http://zsa.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qnx.316326.xyz

[U77] PHP：模板渲染
来源：http://uon.meibo888.top

composer require twig/twig
来源：http://mgs.hesvh.cn

[U78] PHP：单元测试
来源：http://yqr.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://jrm.quarkkingdee.top

[U79] PHP：静态分析
来源：http://fmb.cheryme.top

composer require --dev phpstan/phpstan
来源：http://mdd.vehdjk.com

[U80] PHP：代码规范修复
来源：http://flx.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://syj.vehdjk.com

[U81] JS：初始化项目
来源：http://nby.chenlongwang.top

npm init -y;  npm i express
来源：http://skt.xinyue.icu

[U82] JS：package.json 脚本
来源：http://dmb.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sil.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://txq.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://fav.sweek.top

[U84] JS：CommonJS 写法
来源：http://rqb.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xwg.tian-w.cn

[U85] JS：可选链
来源：http://vml.cdnleiting.top

a?.b?.c
来源：http://aaw.tanke756.top

[U86] JS：空值合并
来源：http://ssw.zhijiandao.cn

a ?? b
来源：http://cem.quarkkingdee.top

[U87] JS：解构默认值
来源：http://cah.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://aon.yfazqb.com

[U88] JS：对象展开合并
来源：http://ame.xinyue.icu

{ ...a, ...b }
来源：http://dtv.fengsongda.top

[U89] JS：数组去重
来源：http://wph.fzhhl.top

[...new Set(arr)]
来源：http://wdn.fzhhl.top

[U90] JS：数字数组排序
来源：http://mpy.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://raq.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://mkc.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ogk.chenlongwang.top

[U92] JS：深拷贝
来源：http://vxs.yj202588.top

structuredClone(obj)
来源：http://ygt.cashguo.top

[U93] JS：模板字符串
来源：http://qov.jlsjyb.cn

`共 ${n} 条`
来源：http://jpc.bjfxy.top

[U94] JS：箭头函数
来源：http://pzn.ppjwa.cn

const double = x => x * 2;
来源：http://ctc.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://dfx.tarul.cn

new Promise((resolve, reject) => {})
来源：http://osg.bbcook.cn

[U96] JS：async/await 与异常
来源：http://uzf.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wdt.hnxiangtu.top

[U97] JS：并发请求
来源：http://wkh.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iaq.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://frs.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yls.yangfankeji.com

[U99] JS：事件监听
来源：http://nax.xziqi.cn

el.addEventListener("click", e => {})
来源：http://ldz.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://rba.sysykeji.top

document.querySelector(".item")
来源：http://rhx.tianlin.xyz

[U101] JS：classList 操作
来源：http://fbm.fktsv.cn

el.classList.toggle("active")
来源：http://nnj.zhoulong.xyz

[U102] JS：本地存储
来源：http://uce.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tzw.shanyushiyangtech.top

[U103] JS：定时器
来源：http://vmo.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lbc.dashuyun.cn

[U104] JS：防抖
来源：http://hkm.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euh.chenjidiqi.icu

[U105] JS：节流
来源：http://wxw.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yib.0kj1m.cn

[U106] JS：日期格式化
来源：http://afh.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hep.fehbvm.com

[U107] JS：数字千分位
来源：http://wij.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://drn.sweek.top

[U108] JS：随机整数
来源：http://ezh.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wvd.yj202588.top

[U109] JS：数组分组
来源：http://ftd.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://aca.ppjwa.cn

[U110] JS：数组分块
来源：http://xwc.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qww.cucudq.cn

[U111] JS：对象转 Map
来源：http://qhe.ctjpmb.com

new Map(Object.entries(obj))
来源：http://yre.fzhhl.top

[U112] JS：字符串补位
来源：http://ezm.xuanzx.com

"7".padStart(3, "0")
来源：http://rao.haohaochexian.top

[U113] JS：正则替换全部
来源：http://hsx.havefunace.top

s.replaceAll("a", "b")
来源：http://ppr.yvedp.cn

[U114] JS：JSON 深比较
来源：http://tag.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zkm.pycfn.com

[U115] JS：生成 UUID
来源：http://psz.gotoacloud.top

crypto.randomUUID()
来源：http://phg.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://ysm.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://pxn.316326.xyz

[U117] JS：单元测试
来源：http://uoh.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://wgo.ppjwa.cn

[U118] JS：开发服务器
来源：http://xdj.tanke756.top

npm i -D vite;  npx vite
来源：http://uso.hywenlv.cn

[U119] JS：生产构建
来源：http://qiv.zhixingplan.top

npx vite build
来源：http://pvi.zhijiandao.cn

[U120] JS：读取环境变量（Vite）
来源：http://ame.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://skd.yj20258888.top

================================================================================
来源：http://fpz.xuetiantiany.cn

统计汇总
来源：http://kqu.gaohongyu789.top

================================================================================
来源：http://bco.yonumen.top

按语言统计（条）：
来源：http://dcg.smart0.xyz

Python ......... 252
来源：http://fzg.ppjwa.cn

PHP ............ 252
来源：http://rgj.ppjwa.cn

JavaScript ..... 252
来源：http://gbc.zdqjudy.top

TypeScript ..... 212
来源：http://rzf.yueranfly.top

Java ........... 212
来源：http://yct.haohaochexian.top

Go ............. 212
来源：http://oay.yuanzhike.top

Ruby ........... 212
来源：http://tun.tian-w.cn

C# ............. 212
来源：http://feq.yvedp.cn

C .............. 30
来源：http://gck.shangyingyoupin.top

C++ ............ 30
来源：http://rec.jinghuilouyu.cn

SQL ............ 90
来源：http://xvh.hongshengwenyu.top

Bash ........... 80
来源：http://swu.daria6918.cn

Kotlin ......... 15
来源：http://wjk.cqqwz.cn

Swift .......... 15
来源：http://pzn.yanxiufei.cn

Lua ............ 10
来源：http://jhg.vqdsnc.cn

Perl ........... 10
来源：http://jsn.xziqi.cn

Scala .......... 10
来源：http://pox.zhiwuduotai.top

------------------------------------
来源：http://ypt.ppjwa.cn

合计 ........... 2106 条
来源：http://mhz.jyoumei.cn

按章节统计：
来源：http://pep.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kmx.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qaq.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wkj.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://end.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ebg.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rbt.tanke756.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hhl.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://idp.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gxv.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vyu.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gcs.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://prg.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yvg.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://akn.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qfo.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://doz.yj20258888.top

Q SQL 专题                              90
来源：http://svc.epnwcf.com

R Bash 专题                             80
来源：http://trs.sufxvd.cn

S C / C++ 专题                          60
来源：http://czz.316326.xyz

T 其他语言补充                          60
来源：http://eyu.wangshuangyany.cn

U 高频实用片段                         120
来源：http://bsu.xylfe.cn

------------------------------------
来源：http://obw.yueranfly.top

合计                                  2106 条
来源：http://top.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://xjr.nwbrower.top

使用提醒
来源：http://hes.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://ccs.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dvl.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cja.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://smc.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dcq.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://szv.vqdsnc.cn

—— 文件结束 ——
来源：http://zuf.shanyushiyangkeji.top

================================================================================
来源：http://yft.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://nfg.kuanghao11.cn

Common Programming Examples Cheat Book
来源：http://zzu.birdmap.top

================================================================================
来源：http://yao.vqdsnc.cn

【收录内容】
来源：http://njt.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ctm.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jqe.sufxvd.cn

SQL · Bash · C · C++
来源：http://gib.yonumen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ojl.xingfuxueyuan.xyz

【使用说明】
来源：http://nep.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ctj.daxiang520.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dej.pycfn.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hxu.yvedp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fab.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://onb.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mdh.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://spn.316326.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rno.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://flf.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mgo.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rxy.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yio.quarkkingdee.top

【文件统计】
来源：http://xoi.jqgfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gof.mhx1999.top

--------------------------------------------------------------------------------
来源：http://wey.fehbvm.com

目  录
来源：http://ywd.fengsongda.top

--------------------------------------------------------------------------------
来源：http://dln.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eel.meibo888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ulp.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fox.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sid.xingfuxueyuan.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ngu.hysaishi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aor.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dqe.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baj.hfpthk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aor.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uil.meibo888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ekx.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ztx.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://til.pycfn.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jot.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rvq.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://spd.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ull.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oyp.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vqf.zhijiandao.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zya.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cuk.mhx1999.top

================================================================================
来源：http://lad.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://yse.yueranfly.top

================================================================================
来源：http://alb.yonumen.top

[A01] Hello World
来源：http://fcu.jlsjyb.cn

Py:   print("Hello, World!")
来源：http://wub.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://hhj.sweek.top

JS:   console.log("Hello, World!");
来源：http://dko.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ksa.0kj1m.cn

Java: System.out.println("Hello, World!");
来源：http://gpb.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://shr.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://lxx.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dwx.bjfxy.top

[A02] 变量声明与赋值
来源：http://ble.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vpa.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xtj.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://jvt.redwolf501.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yzo.sjlbkw.cn

Java: String name = "Alex"; int age = 20;
来源：http://fer.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://etk.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://wcq.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cdw.tian-w.cn

[A03] 常量定义
来源：http://ojn.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cck.guowangkeji.top

PHP:  const PI = 3.14159;
来源：http://nxa.tanke756.top

JS:   const PI = 3.14159;
来源：http://yjx.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://kyd.nanxinkj.top

Java: static final double PI = 3.14159;
来源：http://bcq.zdqjudy.top

Go:   const PI = 3.14159
来源：http://kvi.andypj.xyz

Ruby: PI = 3.14159
来源：http://sbl.jinyuanbaomall.cn

C#:   const double PI = 3.14159;
来源：http://inq.fengsongda.top

[A04] 判断变量类型
来源：http://frm.ybcxt.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://map.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vek.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tuz.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://lmn.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qfq.snrcjt.cn

Go:   reflect.TypeOf(x).Name()
来源：http://okw.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fde.sweek.top

C#:   x.GetType().Name; x is int
来源：http://fjq.zycfv.cn

[A05] 整数除法与取模
来源：http://axi.hesvh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dec.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ohk.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yup.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rdj.tanke756.top


<!-- 参考信息 -->