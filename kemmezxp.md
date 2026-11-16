代发 wailian999

[U47] PHP：联合类型
来源：http://pty.hongshengwenyu.top

int|string $id
来源：http://mpv.snrcjt.cn

[U48] PHP：纯枚举
来源：http://ugd.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rkg.zhengqikj.top

[U49] PHP：只读属性
来源：http://kzq.havefunace.top

public readonly string $name
来源：http://gkj.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://klv.aibaodan.cn

public function __construct(private int $id) {}
来源：http://pmr.hysaishi.cn

[U51] PHP：数组解构
来源：http://ymk.gzhubu.top

[$a, $b] = $arr;
来源：http://pmh.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://fug.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://vbp.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://syw.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://iug.cucudq.cn

[U54] PHP：空安全调用
来源：http://eiq.gzhubu.top

$obj?->method()
来源：http://ojn.haohaochexian.top

[U55] PHP：match 表达式
来源：http://ltq.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gab.epnwcf.com

[U56] PHP：命名参数
来源：http://ivb.uphjek.com

f(a: 1, b: 2)
来源：http://qqs.jyoumei.cn

[U57] PHP：字符串插值
来源：http://mec.yuxming.cn

"值: {$a}"
来源：http://cgw.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://poa.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bdw.zdbjq.cn

[U59] PHP：自定义排序
来源：http://msm.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxd.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://wdb.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rnq.yanxiufei.cn

[U61] PHP：正则
来源：http://eme.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cfu.jlsjyb.cn

[U62] PHP：日期对象
来源：http://jyr.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vrf.chenzaomai.com

[U63] PHP：文件读写
来源：http://ccf.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yky.yj20258.top

[U64] PHP：目录遍历
来源：http://ltg.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://ouv.yj202588.top

[U65] PHP：会话
来源：http://qbv.shuidangran.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wyu.sysykeji.top

[U66] PHP：设置 Cookie
来源：http://uhm.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://irb.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://vdp.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uew.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://lkw.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://odj.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://mge.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gjs.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://yqy.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pkv.birdmap.top

[U71] PHP：抛出异常
来源：http://fzd.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://mil.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://roo.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://btg.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://qvy.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://fzu.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://lwu.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://emo.0kj1m.cn

[U75] PHP：依赖注入
来源：http://mwn.guannengcc.top

composer require psr/container
来源：http://oxa.fehbvm.com

[U76] PHP：简单路由
来源：http://pfi.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sml.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://vnv.sweek.top

composer require twig/twig
来源：http://azb.ivvv.top

[U78] PHP：单元测试
来源：http://oju.ivvv.top

composer require --dev phpunit/phpunit
来源：http://ctb.zhengqikj.top

[U79] PHP：静态分析
来源：http://dtd.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://dyj.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://typ.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://aby.gzhubu.top

[U81] JS：初始化项目
来源：http://fzs.hfpthk.cn

npm init -y;  npm i express
来源：http://jii.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://vjg.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jcx.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://azh.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://pxl.jqgfzy.top

[U84] JS：CommonJS 写法
来源：http://gbe.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://ofd.quarkkingdee.top

[U85] JS：可选链
来源：http://hvx.zhengqikj.top

a?.b?.c
来源：http://gmb.hnqzz.top

[U86] JS：空值合并
来源：http://bya.feifeiyinyue.top

a ?? b
来源：http://pxl.hnqzz.top

[U87] JS：解构默认值
来源：http://gne.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://uvg.c1oappe.top

[U88] JS：对象展开合并
来源：http://hle.chenzaomai.com

{ ...a, ...b }
来源：http://gek.xylfe.cn

[U89] JS：数组去重
来源：http://jmr.shangyingyoupin.top

[...new Set(arr)]
来源：http://srs.smart0.xyz

[U90] JS：数字数组排序
来源：http://kja.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://lkj.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://cqy.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tzs.havefunace.top

[U92] JS：深拷贝
来源：http://ilv.yj20258.top

structuredClone(obj)
来源：http://hwj.sysykeji.top

[U93] JS：模板字符串
来源：http://xqt.vehdjk.com

`共 ${n} 条`
来源：http://zcm.nwbrower.top

[U94] JS：箭头函数
来源：http://hha.jlsjyb.cn

const double = x => x * 2;
来源：http://mfi.cheryme.top

[U95] JS：Promise 包装
来源：http://max.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://cpv.cheryme.top

[U96] JS：async/await 与异常
来源：http://ggq.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aav.zhijiandao.cn

[U97] JS：并发请求
来源：http://nvv.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bba.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://rvg.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://psq.smart0.xyz

[U99] JS：事件监听
来源：http://ehc.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://rzf.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://avc.vqdsnc.cn

document.querySelector(".item")
来源：http://vqm.guowangkeji.top

[U101] JS：classList 操作
来源：http://nms.hcnkem.com

el.classList.toggle("active")
来源：http://cuf.chenjidiqi.icu

[U102] JS：本地存储
来源：http://coh.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ddo.fanxiaobao.xyz

[U103] JS：定时器
来源：http://rab.shzxlz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mbh.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://gmd.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xkh.yj20258888.top

[U105] JS：节流
来源：http://fza.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vhy.zhoulong.xyz

[U106] JS：日期格式化
来源：http://ekw.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jui.nanxuanxn.top

[U107] JS：数字千分位
来源：http://xos.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jyt.c1oappe.top

[U108] JS：随机整数
来源：http://npk.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ewx.guannengcc.top

[U109] JS：数组分组
来源：http://vth.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://kkf.yongpay.top

[U110] JS：数组分块
来源：http://jci.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fgl.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://xkl.vehdjk.com

new Map(Object.entries(obj))
来源：http://kih.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://enj.zhixingplan.top

"7".padStart(3, "0")
来源：http://pii.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://kja.316326.xyz

s.replaceAll("a", "b")
来源：http://mzo.fzhhl.top

[U114] JS：JSON 深比较
来源：http://yqa.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ilo.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://qbz.zhengqikj.top

crypto.randomUUID()
来源：http://adl.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://wix.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://rou.havefunace.top

[U117] JS：单元测试
来源：http://ddp.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://ovp.hfpthk.cn

[U118] JS：开发服务器
来源：http://nek.gogol.net.cn

npm i -D vite;  npx vite
来源：http://wxs.nwbrower.top

[U119] JS：生产构建
来源：http://ttj.9152youxi.cn

npx vite build
来源：http://ykj.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://rmv.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://qhb.hnxiangtu.top

================================================================================
来源：http://hso.zdqjudy.top

统计汇总
来源：http://auy.yuxming.cn

================================================================================
来源：http://eiz.tarul.cn

按语言统计（条）：
来源：http://zbt.hfpthk.cn

Python ......... 252
来源：http://kot.jinghuilouyu.cn

PHP ............ 252
来源：http://swg.zhiwuduotai.top

JavaScript ..... 252
来源：http://jwi.chenlongwang.top

TypeScript ..... 212
来源：http://dsu.guowangkeji.top

Java ........... 212
来源：http://nfk.cdnleiting.top

Go ............. 212
来源：http://cav.zdbjq.cn

Ruby ........... 212
来源：http://fiu.shuidangran.top

C# ............. 212
来源：http://dhq.ydjk.org.cn

C .............. 30
来源：http://afs.aibaodan.cn

C++ ............ 30
来源：http://qbo.dashuyun.cn

SQL ............ 90
来源：http://ror.jinyuanbaomall.cn

Bash ........... 80
来源：http://rbt.hywenlv.cn

Kotlin ......... 15
来源：http://zes.zhiwuduotai.top

Swift .......... 15
来源：http://xnq.zhixingplan.top

Lua ............ 10
来源：http://ibo.vehdjk.com

Perl ........... 10
来源：http://pvj.shangyingyoupin.top

Scala .......... 10
来源：http://xqg.jinghuilouyu.cn

------------------------------------
来源：http://gqa.ctjpmb.com

合计 ........... 2106 条
来源：http://ubd.uphjek.com

按章节统计：
来源：http://gss.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jqk.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jsu.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wmf.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pni.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nxf.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kwf.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cjy.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tem.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gte.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zui.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rgj.daria6918.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xxy.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mag.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tlt.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bax.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://crk.jyoumei.cn

Q SQL 专题                              90
来源：http://jig.sjlbkw.cn

R Bash 专题                             80
来源：http://aay.yfazqb.com

S C / C++ 专题                          60
来源：http://owu.sjlbkw.cn

T 其他语言补充                          60
来源：http://ozm.tian-w.cn

U 高频实用片段                         120
来源：http://gdc.vqdsnc.cn

------------------------------------
来源：http://auc.aibaodan.cn

合计                                  2106 条
来源：http://jlm.fengsongda.top

--------------------------------------------------------------------------------
来源：http://pcj.316326.xyz

使用提醒
来源：http://rmu.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://ysh.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fap.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fju.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rlv.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yox.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sqv.gzhubu.top

—— 文件结束 ——
来源：http://kxv.svipenyu.cn

================================================================================
来源：http://dsd.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://kdj.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://spf.ehwqpu.com

================================================================================
来源：http://mjs.zhongyouzk.top

【收录内容】
来源：http://gxb.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oij.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lcp.ivvv.top

SQL · Bash · C · C++
来源：http://uis.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kji.bbcook.cn

【使用说明】
来源：http://loy.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pwa.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://edy.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kkw.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bmg.zycfv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://alq.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rlj.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qrp.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yog.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://swp.cheryme.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hce.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://owk.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oym.52xcode.cn

【文件统计】
来源：http://tdd.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fpe.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://jue.cheryme.top

目  录
来源：http://mlr.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://bus.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lyf.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lfg.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zdf.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://quo.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fif.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rvf.shanyushiyangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tcf.cashguo.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zmz.wangdashe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://thx.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bog.gogol.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wqu.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zoo.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rsw.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kga.iojbl.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ecu.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oql.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vlr.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iei.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vez.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://myu.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jof.bjfxy.top

================================================================================
来源：http://wtv.gaohongyu789.top

A. 基础语法与类型
来源：http://djj.jianghu66.top

================================================================================
来源：http://ehy.yj202588.top

[A01] Hello World
来源：http://bkr.fktsv.cn

Py:   print("Hello, World!")
来源：http://uwa.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://yoc.sysykeji.top

JS:   console.log("Hello, World!");
来源：http://ogd.jianghu66.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gbf.jinqigfzy.top

Java: System.out.println("Hello, World!");
来源：http://jgj.guowangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://fkj.wangshuangyany.cn

Ruby: puts "Hello, World!"
来源：http://bkd.snrcjt.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://woe.yonumen.top

[A02] 变量声明与赋值
来源：http://yas.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://umd.xuanzx.com

PHP:  $name = "Alex"; $age = 20;
来源：http://qaj.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://aza.sufxvd.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rjm.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://lvj.kuanghao11.cn

Go:   name := "Alex"; age := 20
来源：http://uqi.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://xrq.wangdashe.top

C#:   string name = "Alex"; int age = 20;
来源：http://ghc.aizwys.cn

[A03] 常量定义
来源：http://zbe.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zmg.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://mye.vehdjk.com

JS:   const PI = 3.14159;
来源：http://rxw.bjfxy.top

TS:   const PI: number = 3.14159;
来源：http://ojf.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://rxu.yj20258888.top

Go:   const PI = 3.14159
来源：http://ehx.zhaomingkeji.xyz

Ruby: PI = 3.14159
来源：http://qkl.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://jzr.iojbl.cn

[A04] 判断变量类型
来源：http://iuv.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mns.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pxa.hfpthk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nsa.yangfankeji.com

TS:   typeof x; x instanceof Date
来源：http://zfy.vehdjk.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://aer.cheryme.top

Go:   reflect.TypeOf(x).Name()
来源：http://vkd.mhx1999.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ulj.aizwys.cn

C#:   x.GetType().Name; x is int
来源：http://jco.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://rpv.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xeg.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://oqd.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rul.xingfuxueyuan.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wdf.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://kqk.xuanzx.com

Go:   7 / 2; 7 % 2
来源：http://bvw.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://myd.zhongyouzk.top

C#:   7 / 2; 7 % 2
来源：http://rzw.316326.xyz


<!-- 参考信息 -->