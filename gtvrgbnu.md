代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://pao.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qeq.tarul.cn

[U42] PHP：PSR-4 自动加载
来源：http://ncr.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hlo.andypj.xyz

[U43] PHP：声明命名空间
来源：http://hvg.dashuyun.cn

namespace App\Http;
来源：http://ukn.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://swx.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://ale.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://roj.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://egg.chenzaomai.com

[U46] PHP：可空类型
来源：http://fmq.sxryk.cn

?string $name = null
来源：http://qra.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://wfj.jinqigfzy.top

int|string $id
来源：http://maq.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://igc.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fjo.aizwys.cn

[U49] PHP：只读属性
来源：http://suo.tarul.cn

public readonly string $name
来源：http://ekl.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://zec.nanxinkj.top

public function __construct(private int $id) {}
来源：http://kxj.vqdsnc.cn

[U51] PHP：数组解构
来源：http://cjj.aibaodan.cn

[$a, $b] = $arr;
来源：http://gqj.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://wsx.uphjek.com

$double = fn($x) => $x * 2;
来源：http://agw.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://msq.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://xiz.fehbvm.com

[U54] PHP：空安全调用
来源：http://pjj.jlsjyb.cn

$obj?->method()
来源：http://mcc.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://rmf.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rew.hywenlv.cn

[U56] PHP：命名参数
来源：http://ekz.zdbjq.cn

f(a: 1, b: 2)
来源：http://avi.yuxming.cn

[U57] PHP：字符串插值
来源：http://cqd.gotoacloud.top

"值: {$a}"
来源：http://mix.fehbvm.com

[U58] PHP：数组三件套
来源：http://tjy.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tqn.ydzc1.top

[U59] PHP：自定义排序
来源：http://vsf.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://umv.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://oov.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ctb.kuanghao11.cn

[U61] PHP：正则
来源：http://nli.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tvd.ehwqpu.com

[U62] PHP：日期对象
来源：http://jyv.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yyh.yfazqb.com

[U63] PHP：文件读写
来源：http://fsb.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://etd.hcnkem.com

[U64] PHP：目录遍历
来源：http://pnb.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://rii.sjlbkw.cn

[U65] PHP：会话
来源：http://tbm.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hxv.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://cpv.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://luf.hnqzz.top

[U67] PHP：处理文件上传
来源：http://svk.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zve.tarul.cn

[U68] PHP：PDO 连接
来源：http://khs.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wbh.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://gkz.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jar.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://qjq.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tpf.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://hqy.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://hgb.sysykeji.top

[U72] PHP：写错误日志
来源：http://jwe.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://bmi.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://zeg.birdmap.top

parse_ini_file("config.ini", true)
来源：http://trq.ivvv.top

[U74] PHP：读取环境变量
来源：http://zsu.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://wyt.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://qph.hongshengwenyu.top

composer require psr/container
来源：http://kal.jinqigfzy.top

[U76] PHP：简单路由
来源：http://nqp.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qtn.hysaishi.cn

[U77] PHP：模板渲染
来源：http://slw.quarkkingdee.top

composer require twig/twig
来源：http://lgd.yj20258888.top

[U78] PHP：单元测试
来源：http://dpp.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://kvb.ybcxt.top

[U79] PHP：静态分析
来源：http://ajl.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://mef.smart0.xyz

[U80] PHP：代码规范修复
来源：http://leu.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wfg.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://nza.feifeiyinyue.top

npm init -y;  npm i express
来源：http://fzj.fzhhl.top

[U82] JS：package.json 脚本
来源：http://iub.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rxi.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://rgc.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ucd.ivvv.top

[U84] JS：CommonJS 写法
来源：http://odg.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uyx.shanyushiyangtech.top

[U85] JS：可选链
来源：http://yak.zdbjq.cn

a?.b?.c
来源：http://vwm.chenzaomai.com

[U86] JS：空值合并
来源：http://wbb.dashuyun.cn

a ?? b
来源：http://qjt.birdmap.top

[U87] JS：解构默认值
来源：http://vvu.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://xwm.nwbrower.top

[U88] JS：对象展开合并
来源：http://uuw.guannengcc.top

{ ...a, ...b }
来源：http://bsn.yangfankeji.com

[U89] JS：数组去重
来源：http://znk.shangyingyoupin.top

[...new Set(arr)]
来源：http://shk.birdmap.top

[U90] JS：数字数组排序
来源：http://zyc.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://zvg.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://wbu.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nct.hysaishi.cn

[U92] JS：深拷贝
来源：http://dcv.nanxuanxn.top

structuredClone(obj)
来源：http://hfk.sjlbkw.cn

[U93] JS：模板字符串
来源：http://yto.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://osb.yj20258888.top

[U94] JS：箭头函数
来源：http://lnw.shzxlz.cn

const double = x => x * 2;
来源：http://ltz.guannengcc.top

[U95] JS：Promise 包装
来源：http://dfc.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://qwk.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://ivr.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://udm.shzxlz.cn

[U97] JS：并发请求
来源：http://jki.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://urz.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://lum.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://avf.cqqwz.cn

[U99] JS：事件监听
来源：http://vlo.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://lcn.aibaodan.cn

[U100] JS：DOM 查询
来源：http://hpf.guowangkeji.top

document.querySelector(".item")
来源：http://jqd.ydzc1.top

[U101] JS：classList 操作
来源：http://bpm.hnqzz.top

el.classList.toggle("active")
来源：http://gkj.zhiwuduotai.top

[U102] JS：本地存储
来源：http://aqr.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://saz.zycfv.cn

[U103] JS：定时器
来源：http://coo.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vdu.xuetiantiany.cn

[U104] JS：防抖
来源：http://qbd.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvq.dashuyun.cn

[U105] JS：节流
来源：http://jzi.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lbh.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://znk.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://exm.bbcook.cn

[U107] JS：数字千分位
来源：http://gvq.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://duo.jqgfzy.top

[U108] JS：随机整数
来源：http://jci.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mcf.zdbjq.cn

[U109] JS：数组分组
来源：http://qit.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://fiv.daxiang520.top

[U110] JS：数组分块
来源：http://nqn.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ohp.yangfankeji.com

[U111] JS：对象转 Map
来源：http://oqr.yuanzhike.top

new Map(Object.entries(obj))
来源：http://xey.andypj.xyz

[U112] JS：字符串补位
来源：http://fys.jqgfzy.top

"7".padStart(3, "0")
来源：http://euf.yfazqb.com

[U113] JS：正则替换全部
来源：http://ijw.cqqwz.cn

s.replaceAll("a", "b")
来源：http://fog.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://cfi.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://erd.shzxlz.cn

[U115] JS：生成 UUID
来源：http://mag.mhx1999.top

crypto.randomUUID()
来源：http://ylq.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://yxi.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://azc.xuetiantiany.cn

[U117] JS：单元测试
来源：http://hfv.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://zoo.9152youxi.cn

[U118] JS：开发服务器
来源：http://dyj.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://nbr.chenlongwang.top

[U119] JS：生产构建
来源：http://wpv.ctjpmb.com

npx vite build
来源：http://xop.cdnleiting.top

[U120] JS：读取环境变量（Vite）
来源：http://dsp.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://xei.sufxvd.cn

================================================================================
来源：http://zhh.fehbvm.com

统计汇总
来源：http://zqb.jinyuanbaomall.cn

================================================================================
来源：http://jzx.316326.xyz

按语言统计（条）：
来源：http://dvq.0kj1m.cn

Python ......... 252
来源：http://fsz.jinyuanbaomall.cn

PHP ............ 252
来源：http://nsz.hnxiangtu.top

JavaScript ..... 252
来源：http://prt.aizwys.cn

TypeScript ..... 212
来源：http://mln.jyoumei.cn

Java ........... 212
来源：http://qye.fehbvm.com

Go ............. 212
来源：http://ogf.ydjk.org.cn

Ruby ........... 212
来源：http://pog.jlsjyb.cn

C# ............. 212
来源：http://bna.pycfn.com

C .............. 30
来源：http://cnp.cdnleiting.top

C++ ............ 30
来源：http://zmn.kuanghao11.cn

SQL ............ 90
来源：http://mdy.bjfxy.top

Bash ........... 80
来源：http://kyh.ydzc1.top

Kotlin ......... 15
来源：http://jqb.hywenlv.cn

Swift .......... 15
来源：http://ndh.tarul.cn

Lua ............ 10
来源：http://yaa.andypj.xyz

Perl ........... 10
来源：http://uhx.52xcode.cn

Scala .......... 10
来源：http://yuj.cucudq.cn

------------------------------------
来源：http://wwg.dashuyun.cn

合计 ........... 2106 条
来源：http://fvb.iojbl.cn

按章节统计：
来源：http://aoo.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fuo.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zyh.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gfr.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sem.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fku.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yjt.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zra.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gws.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nei.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vmh.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hii.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kew.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pno.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ylh.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mkp.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jes.yj20258.top

Q SQL 专题                              90
来源：http://mag.c1oappe.top

R Bash 专题                             80
来源：http://kxx.9152youxi.cn

S C / C++ 专题                          60
来源：http://jdr.jianghu66.top

T 其他语言补充                          60
来源：http://leg.c1oappe.top

U 高频实用片段                         120
来源：http://hjj.wangshuangyany.cn

------------------------------------
来源：http://gjz.cheryme.top

合计                                  2106 条
来源：http://aub.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://bmd.52xcode.cn

使用提醒
来源：http://ymm.yvedp.cn

--------------------------------------------------------------------------------
来源：http://slh.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jsc.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nnh.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mri.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://okm.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fqc.sysykeji.top

—— 文件结束 ——
来源：http://kqj.guowangkeji.top

================================================================================
来源：http://myi.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://dsk.xylfe.cn

Common Programming Examples Cheat Book
来源：http://bhc.redwolf501.top

================================================================================
来源：http://tqo.sweek.top

【收录内容】
来源：http://oex.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hfa.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ewc.kuanghao11.cn

SQL · Bash · C · C++
来源：http://qik.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://utb.guowangkeji.top

【使用说明】
来源：http://mql.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://miq.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ila.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pub.fengsongda.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://exi.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mqy.redwolf501.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vvv.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xgm.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ykp.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cyq.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ycl.cdnleiting.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jnd.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lur.chenjidiqi.icu

【文件统计】
来源：http://nkz.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ywy.hammf.cn

--------------------------------------------------------------------------------
来源：http://ozq.ivvv.top

目  录
来源：http://vvu.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://gnu.sjlbkw.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://edg.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jma.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vtq.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ruu.andypj.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xui.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cwh.52xcode.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yje.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qae.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://enj.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zbd.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gel.nwbrower.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bmj.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kxh.pycfn.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rif.ivvv.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hpg.daxiang520.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fdd.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://giw.daria6918.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mty.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mir.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ije.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eox.haohaochexian.top

================================================================================
来源：http://lwx.ppjwa.cn

A. 基础语法与类型
来源：http://svk.tianlin.xyz

================================================================================
来源：http://tbl.yangfankeji.com

[A01] Hello World
来源：http://jyk.yvedp.cn

Py:   print("Hello, World!")
来源：http://hua.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://tlj.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://rmf.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yfg.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://ihf.nanxuanxn.top

Go:   fmt.Println("Hello, World!")
来源：http://mzz.yangfankeji.com

Ruby: puts "Hello, World!"
来源：http://fen.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://huk.ywan-chungtsiang.top

[A02] 变量声明与赋值
来源：http://ggo.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xda.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zbu.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://hud.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vrz.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://flh.zdbjq.cn

Go:   name := "Alex"; age := 20
来源：http://gdl.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://dvw.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://sej.fehbvm.com

[A03] 常量定义
来源：http://gmk.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pkk.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://vtn.vqdsnc.cn

JS:   const PI = 3.14159;
来源：http://wgj.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://epd.tarul.cn

Java: static final double PI = 3.14159;
来源：http://ywc.gotoacloud.top

Go:   const PI = 3.14159
来源：http://pjn.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://qve.yj202588.top

C#:   const double PI = 3.14159;
来源：http://pxd.316326.xyz

[A04] 判断变量类型
来源：http://obw.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kyb.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tqr.tanke756.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vyg.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://ydq.ehwqpu.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hdj.tanke756.top


<!-- 参考信息 -->