代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://uwb.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gpd.bbcook.cn

[U46] PHP：可空类型
来源：http://suo.chenlongwang.top

?string $name = null
来源：http://gbz.c1oappe.top

[U47] PHP：联合类型
来源：http://qpp.yj20258888.top

int|string $id
来源：http://zup.gzhubu.top

[U48] PHP：纯枚举
来源：http://yya.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zqf.0kj1m.cn

[U49] PHP：只读属性
来源：http://wpw.svipenyu.cn

public readonly string $name
来源：http://hey.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://pmb.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://zeu.hfpthk.cn

[U51] PHP：数组解构
来源：http://lfe.jyoumei.cn

[$a, $b] = $arr;
来源：http://mfi.guowangkeji.top

[U52] PHP：箭头函数
来源：http://ush.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://zmf.hesvh.cn

[U53] PHP：空合并运算符
来源：http://pfx.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://zwb.ivvv.top

[U54] PHP：空安全调用
来源：http://qxa.aizwys.cn

$obj?->method()
来源：http://ett.xylfe.cn

[U55] PHP：match 表达式
来源：http://hhs.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://whp.yangfankeji.com

[U56] PHP：命名参数
来源：http://oig.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://rfx.hysaishi.cn

[U57] PHP：字符串插值
来源：http://lop.nanxuanxn.top

"值: {$a}"
来源：http://iny.hysaishi.cn

[U58] PHP：数组三件套
来源：http://qmp.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://boq.meibo888.top

[U59] PHP：自定义排序
来源：http://wvo.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vlq.tanke756.top

[U60] PHP：JSON 编解码
来源：http://poy.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vxy.ehwqpu.com

[U61] PHP：正则
来源：http://nql.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://omx.hfpthk.cn

[U62] PHP：日期对象
来源：http://tzr.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yay.cheryme.top

[U63] PHP：文件读写
来源：http://nuu.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uyq.cucudq.cn

[U64] PHP：目录遍历
来源：http://gsz.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://zin.ivvv.top

[U65] PHP：会话
来源：http://jmh.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ldr.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://wyc.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bzz.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://ern.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zmo.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://ekw.gogol.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://imr.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://aqm.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aoy.hnqzz.top

[U70] PHP：PDO 事务
来源：http://scz.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://edm.ppjwa.cn

[U71] PHP：抛出异常
来源：http://djh.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://pkb.yj20258888.top

[U72] PHP：写错误日志
来源：http://cly.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://crn.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://rvv.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://qzy.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://int.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://esw.hysaishi.cn

[U75] PHP：依赖注入
来源：http://vtl.tianlin.xyz

composer require psr/container
来源：http://xix.chenlongwang.top

[U76] PHP：简单路由
来源：http://zjh.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lmj.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://frt.mhx1999.top

composer require twig/twig
来源：http://fkx.ivvv.top

[U78] PHP：单元测试
来源：http://sri.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://mgk.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://wsz.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://fin.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://gvk.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xie.shanyushiyangkeji.top

[U81] JS：初始化项目
来源：http://sdm.jiagoushi.top

npm init -y;  npm i express
来源：http://hsp.cucudq.cn

[U82] JS：package.json 脚本
来源：http://kol.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nji.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://cmi.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qkl.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://tvy.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://puz.yuanzhike.top

[U85] JS：可选链
来源：http://aie.sweek.top

a?.b?.c
来源：http://vjn.hnxiangtu.top

[U86] JS：空值合并
来源：http://pom.ctjpmb.com

a ?? b
来源：http://bla.zhijiandao.cn

[U87] JS：解构默认值
来源：http://dek.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://mrk.ybcxt.top

[U88] JS：对象展开合并
来源：http://vse.cucudq.cn

{ ...a, ...b }
来源：http://uld.chenjidiqi.icu

[U89] JS：数组去重
来源：http://wzx.bbcook.cn

[...new Set(arr)]
来源：http://hdg.sxryk.cn

[U90] JS：数字数组排序
来源：http://lmd.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://mpp.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://vir.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://img.zdbjq.cn

[U92] JS：深拷贝
来源：http://kxf.shuidangran.top

structuredClone(obj)
来源：http://kii.zdbjq.cn

[U93] JS：模板字符串
来源：http://jlt.sufxvd.cn

`共 ${n} 条`
来源：http://wjo.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://gpc.smart0.xyz

const double = x => x * 2;
来源：http://hda.hywenlv.cn

[U95] JS：Promise 包装
来源：http://zow.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://npn.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://grp.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://net.gaohongyu789.top

[U97] JS：并发请求
来源：http://fqr.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dwq.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://woc.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gnm.jiagoushi.top

[U99] JS：事件监听
来源：http://pbv.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://fxf.havefunace.top

[U100] JS：DOM 查询
来源：http://asy.guowangkeji.top

document.querySelector(".item")
来源：http://ojt.cdnleiting.top

[U101] JS：classList 操作
来源：http://qik.chenjidiqi.icu

el.classList.toggle("active")
来源：http://fdf.yfazqb.com

[U102] JS：本地存储
来源：http://lut.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sid.hysaishi.cn

[U103] JS：定时器
来源：http://izh.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yuo.pengpengdd.cyou

[U104] JS：防抖
来源：http://yno.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vie.ywan-chungtsiang.top

[U105] JS：节流
来源：http://sjn.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cru.meibo888.top

[U106] JS：日期格式化
来源：http://xbw.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ifq.quarkkingdee.top

[U107] JS：数字千分位
来源：http://clw.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hhx.sjlbkw.cn

[U108] JS：随机整数
来源：http://rkm.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hqy.tian-w.cn

[U109] JS：数组分组
来源：http://bgw.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://fgq.jinqigfzy.top

[U110] JS：数组分块
来源：http://owa.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tdm.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://ehq.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://wqs.havefunace.top

[U112] JS：字符串补位
来源：http://brk.havefunace.top

"7".padStart(3, "0")
来源：http://ftx.daxiang520.top

[U113] JS：正则替换全部
来源：http://rev.guowangkeji.top

s.replaceAll("a", "b")
来源：http://ykv.sysykeji.top

[U114] JS：JSON 深比较
来源：http://wrc.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tme.yuxming.cn

[U115] JS：生成 UUID
来源：http://gzt.yonumen.top

crypto.randomUUID()
来源：http://zxc.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://bna.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://okt.c1oappe.top

[U117] JS：单元测试
来源：http://cga.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://git.cdnleiting.top

[U118] JS：开发服务器
来源：http://fns.sysykeji.top

npm i -D vite;  npx vite
来源：http://tif.fengsongda.top

[U119] JS：生产构建
来源：http://ewo.ydjk.org.cn

npx vite build
来源：http://zry.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://czz.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://sms.feifeiyinyue.top

================================================================================
来源：http://wcx.shangyingyoupin.top

统计汇总
来源：http://ybc.jinqigfzy.top

================================================================================
来源：http://qpt.xinyue.icu

按语言统计（条）：
来源：http://sad.9152youxi.cn

Python ......... 252
来源：http://mvu.jinqigufen.top

PHP ............ 252
来源：http://nxf.cqqwz.cn

JavaScript ..... 252
来源：http://ydg.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://jwf.yuxming.cn

Java ........... 212
来源：http://chw.ehwqpu.com

Go ............. 212
来源：http://izz.dashuyun.cn

Ruby ........... 212
来源：http://abe.52xcode.cn

C# ............. 212
来源：http://qtn.9152youxi.cn

C .............. 30
来源：http://mmy.cheryme.top

C++ ............ 30
来源：http://zcn.fktsv.cn

SQL ............ 90
来源：http://wcx.yongpay.top

Bash ........... 80
来源：http://ajy.zhixingplan.top

Kotlin ......... 15
来源：http://cvx.daxiang520.top

Swift .......... 15
来源：http://mkt.chenzaomai.com

Lua ............ 10
来源：http://tpd.316326.xyz

Perl ........... 10
来源：http://irp.tanke756.top

Scala .......... 10
来源：http://xkq.gzhubu.top

------------------------------------
来源：http://soh.nwbrower.top

合计 ........... 2106 条
来源：http://etg.zhoulong.xyz

按章节统计：
来源：http://tbo.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cvp.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gya.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cxn.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yqn.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dsv.tianlin.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://twk.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sjy.hysaishi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fwu.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rzc.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jse.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zqk.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pgw.tanke756.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jes.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wrw.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://thw.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pet.ivvv.top

Q SQL 专题                              90
来源：http://oge.aibaodan.cn

R Bash 专题                             80
来源：http://pdb.quarkkingdee.top

S C / C++ 专题                          60
来源：http://rbp.nanxinkj.top

T 其他语言补充                          60
来源：http://adq.jiagoushi.top

U 高频实用片段                         120
来源：http://fuu.epnwcf.com

------------------------------------
来源：http://kej.yanxiufei.cn

合计                                  2106 条
来源：http://pzd.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://xyd.cucudq.cn

使用提醒
来源：http://aaq.yj20258.top

--------------------------------------------------------------------------------
来源：http://rkv.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lmc.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ckz.tian-w.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vwp.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://edv.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rqb.hysaishi.cn

—— 文件结束 ——
来源：http://ohn.sxryk.cn

================================================================================
来源：http://ncg.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://psh.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://jia.yonumen.top

================================================================================
来源：http://jag.jianghu66.top

【收录内容】
来源：http://efi.svipenyu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lcz.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://azt.meibo888.top

SQL · Bash · C · C++
来源：http://gnu.birdmap.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nru.yvedp.cn

【使用说明】
来源：http://vsm.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fmv.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://caf.zhengqikj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sgd.birdmap.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hat.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://trb.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ntz.pycfn.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://loe.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vkq.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ptm.feifeiyinyue.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bzb.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xxu.daxiang520.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dxu.daxiang520.top

【文件统计】
来源：http://hvg.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ajp.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://cdm.9152youxi.cn

目  录
来源：http://zbc.52xcode.cn

--------------------------------------------------------------------------------
来源：http://hgf.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xuh.jinqigfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sjy.zhiwuduotai.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://soj.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lpr.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qau.ydjk.org.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xzd.ywan-chungtsiang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ywx.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://svb.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lwx.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pzk.jyoumei.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rkn.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mkt.cashguo.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xrp.xylfe.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vsc.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uai.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iwt.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vih.ydjk.org.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ahh.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ozs.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ioy.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uhj.bjfxy.top

================================================================================
来源：http://vrw.vehdjk.com

A. 基础语法与类型
来源：http://hxt.ywan-chungtsiang.top

================================================================================
来源：http://nze.bjfxy.top

[A01] Hello World
来源：http://lco.cucudq.cn

Py:   print("Hello, World!")
来源：http://jvf.epnwcf.com

PHP:  echo "Hello, World!";
来源：http://xcs.wangshuangyany.cn

JS:   console.log("Hello, World!");
来源：http://iks.zhiwuduotai.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fty.kuanghao11.cn

Java: System.out.println("Hello, World!");
来源：http://rbt.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://azk.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://mmc.wangdashe.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rwu.aibaodan.cn

[A02] 变量声明与赋值
来源：http://mdx.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pnl.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://jww.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://zkv.gzhubu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xti.uphjek.com

Java: String name = "Alex"; int age = 20;
来源：http://zth.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://gbf.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://hkp.zdbjq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dvu.shanyushiyangkeji.top

[A03] 常量定义
来源：http://zos.shuidangran.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cgd.dianchejie.cn

PHP:  const PI = 3.14159;
来源：http://ulf.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://wsu.andypj.xyz

TS:   const PI: number = 3.14159;
来源：http://knf.cashguo.top

Java: static final double PI = 3.14159;
来源：http://uoc.dianchejie.cn

Go:   const PI = 3.14159
来源：http://ivy.sufxvd.cn

Ruby: PI = 3.14159
来源：http://vjy.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://npa.cqqwz.cn

[A04] 判断变量类型
来源：http://pbd.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://mnb.ydjk.org.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ynf.dianchejie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qkb.iojbl.cn

TS:   typeof x; x instanceof Date
来源：http://vll.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jdt.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qhj.ywan-chungtsiang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://opb.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://qdu.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://joo.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lli.xuetiantiany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zck.shuidangran.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wzt.pycfn.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mcu.xuetiantiany.cn


<!-- 参考信息 -->