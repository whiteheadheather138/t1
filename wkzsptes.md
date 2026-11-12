代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://ogp.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ewz.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://orw.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hdr.sysykeji.top

[U43] PHP：声明命名空间
来源：http://rzw.meibo888.top

namespace App\Http;
来源：http://cgh.cucudq.cn

[U44] PHP：开启严格类型
来源：http://lxp.cqqwz.cn

declare(strict_types=1);
来源：http://wrx.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://trh.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://smd.daria6918.cn

[U46] PHP：可空类型
来源：http://ohb.svipenyu.cn

?string $name = null
来源：http://bif.yanxiufei.cn

[U47] PHP：联合类型
来源：http://aeo.yj20258.top

int|string $id
来源：http://fmx.gzhubu.top

[U48] PHP：纯枚举
来源：http://pvb.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://btu.bjfxy.top

[U49] PHP：只读属性
来源：http://dop.xinyue.icu

public readonly string $name
来源：http://avn.sweek.top

[U50] PHP：构造器属性提升
来源：http://aid.shzxlz.cn

public function __construct(private int $id) {}
来源：http://zrq.bjfxy.top

[U51] PHP：数组解构
来源：http://qxc.zhengqikj.top

[$a, $b] = $arr;
来源：http://hbp.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://nes.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://vfx.hesvh.cn

[U53] PHP：空合并运算符
来源：http://pdz.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://prb.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://dgg.hesvh.cn

$obj?->method()
来源：http://ahm.haohaochexian.top

[U55] PHP：match 表达式
来源：http://xwi.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yqr.tianlin.xyz

[U56] PHP：命名参数
来源：http://rmx.meibo888.top

f(a: 1, b: 2)
来源：http://uyi.yj20258888.top

[U57] PHP：字符串插值
来源：http://dxb.daria6918.cn

"值: {$a}"
来源：http://bgm.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://esb.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://izk.chenlongwang.top

[U59] PHP：自定义排序
来源：http://hxf.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fnv.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://mga.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nvv.chenjidiqi.icu

[U61] PHP：正则
来源：http://buw.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pha.yuanzhike.top

[U62] PHP：日期对象
来源：http://ude.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bnz.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://xqd.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fxr.havefunace.top

[U64] PHP：目录遍历
来源：http://sjf.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://cld.yj20258888.top

[U65] PHP：会话
来源：http://aqt.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fqf.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://fbw.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pjf.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://vmr.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ccf.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://mhu.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://abn.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://wpi.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qef.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://tfv.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zmx.wangdashe.top

[U71] PHP：抛出异常
来源：http://hyy.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://aob.chenlongwang.top

[U72] PHP：写错误日志
来源：http://mku.yueranfly.top

error_log("失败: " . $e->getMessage());
来源：http://nth.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://zrc.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://tpx.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://fcr.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://gna.hysaishi.cn

[U75] PHP：依赖注入
来源：http://vcm.shangyingyoupin.top

composer require psr/container
来源：http://tyh.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://erh.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://doj.shuidangran.top

[U77] PHP：模板渲染
来源：http://ero.jqgfzy.top

composer require twig/twig
来源：http://hmh.hesvh.cn

[U78] PHP：单元测试
来源：http://nwx.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://zhd.redwolf501.top

[U79] PHP：静态分析
来源：http://oek.tanke756.top

composer require --dev phpstan/phpstan
来源：http://qqv.bbcook.cn

[U80] PHP：代码规范修复
来源：http://aoz.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uxd.epnwcf.com

[U81] JS：初始化项目
来源：http://vfn.bbcook.cn

npm init -y;  npm i express
来源：http://bxb.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://sbg.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uzy.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://rcq.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://xal.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://pkg.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://pfv.dashuyun.cn

[U85] JS：可选链
来源：http://uts.wangshuangyany.cn

a?.b?.c
来源：http://aru.zhijiandao.cn

[U86] JS：空值合并
来源：http://pzw.yuanzhike.top

a ?? b
来源：http://dbx.iojbl.cn

[U87] JS：解构默认值
来源：http://rjr.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://gph.fktsv.cn

[U88] JS：对象展开合并
来源：http://ams.gotoacloud.top

{ ...a, ...b }
来源：http://jqr.jqgufenzy.top

[U89] JS：数组去重
来源：http://lbq.mhx1999.top

[...new Set(arr)]
来源：http://ajq.xuanzx.com

[U90] JS：数字数组排序
来源：http://ccj.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://xrh.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://zaq.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fyb.snrcjt.cn

[U92] JS：深拷贝
来源：http://men.zhijiandao.cn

structuredClone(obj)
来源：http://czj.ctjpmb.com

[U93] JS：模板字符串
来源：http://htd.aizwys.cn

`共 ${n} 条`
来源：http://mpj.cashguo.top

[U94] JS：箭头函数
来源：http://apc.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://ujp.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://jnh.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://fcz.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://oqt.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bsg.yfazqb.com

[U97] JS：并发请求
来源：http://zdt.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zhh.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://fye.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pzu.zhijiandao.cn

[U99] JS：事件监听
来源：http://jbv.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://tqb.dianchejie.cn

[U100] JS：DOM 查询
来源：http://wtr.kuanghao11.cn

document.querySelector(".item")
来源：http://aqo.cdnleiting.top

[U101] JS：classList 操作
来源：http://xcn.cucudq.cn

el.classList.toggle("active")
来源：http://fcj.yueranfly.top

[U102] JS：本地存储
来源：http://dkk.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vvk.yj20258888.top

[U103] JS：定时器
来源：http://ajs.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cxl.pycfn.com

[U104] JS：防抖
来源：http://anl.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zzu.jyoumei.cn

[U105] JS：节流
来源：http://xsw.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ill.zdqjudy.top

[U106] JS：日期格式化
来源：http://xao.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fpk.xinyue.icu

[U107] JS：数字千分位
来源：http://khm.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zqp.ppjwa.cn

[U108] JS：随机整数
来源：http://gkq.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jnf.pengpengdd.cyou

[U109] JS：数组分组
来源：http://gsu.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://ktu.hnxiangtu.top

[U110] JS：数组分块
来源：http://its.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cct.xuanzx.com

[U111] JS：对象转 Map
来源：http://fld.ybcxt.top

new Map(Object.entries(obj))
来源：http://lep.bbcook.cn

[U112] JS：字符串补位
来源：http://xwy.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://kxz.ivvv.top

[U113] JS：正则替换全部
来源：http://fge.fzhhl.top

s.replaceAll("a", "b")
来源：http://jie.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://lhl.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yqh.aizwys.cn

[U115] JS：生成 UUID
来源：http://tib.sysykeji.top

crypto.randomUUID()
来源：http://sek.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://yfm.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://gsl.iojbl.cn

[U117] JS：单元测试
来源：http://sbj.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://qyr.aibaodan.cn

[U118] JS：开发服务器
来源：http://giz.yj20258.top

npm i -D vite;  npx vite
来源：http://bwo.quarkkingdee.top

[U119] JS：生产构建
来源：http://pop.jiagoushi.top

npx vite build
来源：http://zaq.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://vnc.tarul.cn

import.meta.env.VITE_API_URL
来源：http://ezp.hysaishi.cn

================================================================================
来源：http://efo.yonumen.top

统计汇总
来源：http://nam.pengpengdd.cyou

================================================================================
来源：http://avu.ydzc1.top

按语言统计（条）：
来源：http://uzz.zhijiandao.cn

Python ......... 252
来源：http://oic.sxryk.cn

PHP ............ 252
来源：http://okq.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://reb.snrcjt.cn

TypeScript ..... 212
来源：http://zpb.iojbl.cn

Java ........... 212
来源：http://rvt.kuanghao11.cn

Go ............. 212
来源：http://wom.fktsv.cn

Ruby ........... 212
来源：http://zju.zhaomingkeji.xyz

C# ............. 212
来源：http://jwq.hammf.cn

C .............. 30
来源：http://igp.zhaomingkeji.xyz

C++ ............ 30
来源：http://bhb.yvedp.cn

SQL ............ 90
来源：http://hmr.gogol.net.cn

Bash ........... 80
来源：http://jug.daria6918.cn

Kotlin ......... 15
来源：http://ule.shuidangran.top

Swift .......... 15
来源：http://dak.yanxiufei.cn

Lua ............ 10
来源：http://sjs.hongshengwenyu.top

Perl ........... 10
来源：http://maf.andypj.xyz

Scala .......... 10
来源：http://cjh.feifeiyinyue.top

------------------------------------
来源：http://ywc.52xcode.cn

合计 ........... 2106 条
来源：http://xyl.yuxming.cn

按章节统计：
来源：http://rtm.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bwp.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wwb.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wmc.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://imv.ivvv.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fgr.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bsn.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cpk.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gtk.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://chq.wangshuangyany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xye.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uwd.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nao.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bpx.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mjc.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://srh.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aix.hnqzz.top

Q SQL 专题                              90
来源：http://sfz.zhoulong.xyz

R Bash 专题                             80
来源：http://mpn.hywenlv.cn

S C / C++ 专题                          60
来源：http://fso.epnwcf.com

T 其他语言补充                          60
来源：http://fpg.yueranfly.top

U 高频实用片段                         120
来源：http://hrt.tian-w.cn

------------------------------------
来源：http://ifs.tian-w.cn

合计                                  2106 条
来源：http://vqf.andypj.xyz

--------------------------------------------------------------------------------
来源：http://qvy.tarul.cn

使用提醒
来源：http://vjo.andypj.xyz

--------------------------------------------------------------------------------
来源：http://tok.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://old.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rek.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dhe.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sbq.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tur.tarul.cn

—— 文件结束 ——
来源：http://nuq.cdnleiting.top

================================================================================
来源：http://sfm.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://bus.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://omb.xziqi.cn

================================================================================
来源：http://yxt.hesvh.cn

【收录内容】
来源：http://bkv.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yqj.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bon.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://yjx.smart0.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zfe.fanxiaobao.xyz

【使用说明】
来源：http://dmn.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dkf.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zmg.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://thf.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xej.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zhp.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ejm.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rhv.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dus.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gfj.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qon.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xza.gaohongyu789.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xzl.zycfv.cn

【文件统计】
来源：http://oxq.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://riy.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://jik.ydjk.org.cn

目  录
来源：http://adx.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://cke.snrcjt.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tsr.hfpthk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qcx.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://weg.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pdi.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cfv.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rpv.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sxf.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tdn.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://min.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dgp.xziqi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://whu.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mzd.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xnn.daxiang520.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://itk.hesvh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hft.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xtj.birdmap.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pvl.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bby.316326.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vtf.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mkx.yj20258.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xsr.316326.xyz

================================================================================
来源：http://xar.cdnleiting.top

A. 基础语法与类型
来源：http://spb.nanxuanxn.top

================================================================================
来源：http://qdh.hysaishi.cn

[A01] Hello World
来源：http://mms.andypj.xyz

Py:   print("Hello, World!")
来源：http://sih.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://qpp.nanxuanxn.top

JS:   console.log("Hello, World!");
来源：http://lta.hnqzz.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vpy.daxiang520.top

Java: System.out.println("Hello, World!");
来源：http://wep.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://lwi.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://hdv.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://clh.zhixingplan.top

[A02] 变量声明与赋值
来源：http://mig.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mln.ydzc1.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tei.zhixingplan.top

JS:   let name = "Alex"; const age = 20;
来源：http://gev.meibo888.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mcr.fanxiaobao.xyz

Java: String name = "Alex"; int age = 20;
来源：http://wvk.hnqzz.top

Go:   name := "Alex"; age := 20
来源：http://pcc.havefunace.top

Ruby: name = "Alex"; age = 20
来源：http://wky.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dmn.ywan-chungtsiang.top

[A03] 常量定义
来源：http://num.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lvp.mhx1999.top

PHP:  const PI = 3.14159;
来源：http://qlj.daria6918.cn

JS:   const PI = 3.14159;
来源：http://pzb.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://eoi.cucudq.cn

Java: static final double PI = 3.14159;
来源：http://xzm.meibo888.top

Go:   const PI = 3.14159
来源：http://dhw.yj20258.top

Ruby: PI = 3.14159
来源：http://hvw.fanxiaobao.xyz

C#:   const double PI = 3.14159;
来源：http://ycn.jqgufenzy.top

[A04] 判断变量类型
来源：http://bqn.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rwy.yj20258888.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mua.svipenyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ype.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://scf.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ner.hfpthk.cn


<!-- 参考信息 -->