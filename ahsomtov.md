代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://qil.chenjidiqi.icu

sys.stdout.isatty()
来源：http://bkb.yj202588.top

[U40] Py：打印到标准错误
来源：http://icx.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://wia.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://epe.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eod.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://fps.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ffg.bbcook.cn

[U43] PHP：声明命名空间
来源：http://eav.andypj.xyz

namespace App\Http;
来源：http://oij.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://jja.ybcxt.top

declare(strict_types=1);
来源：http://aft.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://ejq.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lzr.shzxlz.cn

[U46] PHP：可空类型
来源：http://vmc.jqgfzy.top

?string $name = null
来源：http://iye.zhoulong.xyz

[U47] PHP：联合类型
来源：http://pye.epnwcf.com

int|string $id
来源：http://fek.yfazqb.com

[U48] PHP：纯枚举
来源：http://lps.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kyc.pycfn.com

[U49] PHP：只读属性
来源：http://mta.daxiang520.top

public readonly string $name
来源：http://ept.cheryme.top

[U50] PHP：构造器属性提升
来源：http://xxm.c1oappe.top

public function __construct(private int $id) {}
来源：http://qtn.xuanzx.com

[U51] PHP：数组解构
来源：http://szm.aibaodan.cn

[$a, $b] = $arr;
来源：http://mra.zdbjq.cn

[U52] PHP：箭头函数
来源：http://iev.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://hfk.zycfv.cn

[U53] PHP：空合并运算符
来源：http://snu.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://htw.fengsongda.top

[U54] PHP：空安全调用
来源：http://elg.yonumen.top

$obj?->method()
来源：http://jdp.yj20258.top

[U55] PHP：match 表达式
来源：http://dot.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yva.jiagoushi.top

[U56] PHP：命名参数
来源：http://ctp.tian-w.cn

f(a: 1, b: 2)
来源：http://qde.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://wzd.shangyingyoupin.top

"值: {$a}"
来源：http://bau.iojbl.cn

[U58] PHP：数组三件套
来源：http://sme.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kmu.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://jvp.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fsq.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://scb.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sac.sufxvd.cn

[U61] PHP：正则
来源：http://cwf.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wwz.nanxinkj.top

[U62] PHP：日期对象
来源：http://riq.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://btj.gotoacloud.top

[U63] PHP：文件读写
来源：http://jzk.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qfc.hcnkem.com

[U64] PHP：目录遍历
来源：http://mzh.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://ncz.zdbjq.cn

[U65] PHP：会话
来源：http://cgd.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nha.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://sbq.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tno.sxryk.cn

[U67] PHP：处理文件上传
来源：http://ncp.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nzm.sxryk.cn

[U68] PHP：PDO 连接
来源：http://gxt.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://syi.xuetiantiany.cn

[U69] PHP：PDO 预处理
来源：http://hgf.jqgfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ysq.yvedp.cn

[U70] PHP：PDO 事务
来源：http://rwu.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nmt.redwolf501.top

[U71] PHP：抛出异常
来源：http://szg.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://kzg.hcnkem.com

[U72] PHP：写错误日志
来源：http://kne.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://qmu.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://tym.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://paz.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://bzq.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://erk.tarul.cn

[U75] PHP：依赖注入
来源：http://gkt.tianlin.xyz

composer require psr/container
来源：http://bol.0kj1m.cn

[U76] PHP：简单路由
来源：http://adq.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ygn.xylfe.cn

[U77] PHP：模板渲染
来源：http://pyb.uphjek.com

composer require twig/twig
来源：http://tyj.sjlbkw.cn

[U78] PHP：单元测试
来源：http://hkh.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://pco.sufxvd.cn

[U79] PHP：静态分析
来源：http://swa.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://bsy.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://qpq.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cct.ydzc1.top

[U81] JS：初始化项目
来源：http://sgg.sweek.top

npm init -y;  npm i express
来源：http://foh.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://ser.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ofj.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://xtg.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://noc.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://eex.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hen.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://zqo.chenzaomai.com

a?.b?.c
来源：http://muc.snrcjt.cn

[U86] JS：空值合并
来源：http://twv.hnxiangtu.top

a ?? b
来源：http://ykk.fehbvm.com

[U87] JS：解构默认值
来源：http://feo.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://rzy.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://zuk.zhoulong.xyz

{ ...a, ...b }
来源：http://nvl.hnxiangtu.top

[U89] JS：数组去重
来源：http://nql.zhongyouzk.top

[...new Set(arr)]
来源：http://goo.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://nap.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://ggf.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://eai.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ins.svipenyu.cn

[U92] JS：深拷贝
来源：http://rsl.vqdsnc.cn

structuredClone(obj)
来源：http://ahm.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://qrf.jinqigufen.top

`共 ${n} 条`
来源：http://pxb.cheryme.top

[U94] JS：箭头函数
来源：http://gam.zhoulong.xyz

const double = x => x * 2;
来源：http://exu.cheryme.top

[U95] JS：Promise 包装
来源：http://ivd.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://mtn.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://zcl.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://toj.xuanzx.com

[U97] JS：并发请求
来源：http://nrn.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://sac.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://eqp.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://shm.gzhubu.top

[U99] JS：事件监听
来源：http://hqi.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://taq.birdmap.top

[U100] JS：DOM 查询
来源：http://lzx.yangfankeji.com

document.querySelector(".item")
来源：http://zxr.andypj.xyz

[U101] JS：classList 操作
来源：http://osh.yanxiufei.cn

el.classList.toggle("active")
来源：http://cqy.hfpthk.cn

[U102] JS：本地存储
来源：http://ttt.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://loc.redwolf501.top

[U103] JS：定时器
来源：http://lcz.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jpd.wangshuangyany.cn

[U104] JS：防抖
来源：http://bfd.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eaz.ydzc1.top

[U105] JS：节流
来源：http://avj.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://imb.ctjpmb.com

[U106] JS：日期格式化
来源：http://owm.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ymy.tian-w.cn

[U107] JS：数字千分位
来源：http://uyo.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cxb.sxryk.cn

[U108] JS：随机整数
来源：http://ece.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ojq.ybcxt.top

[U109] JS：数组分组
来源：http://qgi.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://foo.jyoumei.cn

[U110] JS：数组分块
来源：http://gnj.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jlv.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://hiq.0kj1m.cn

new Map(Object.entries(obj))
来源：http://toz.xziqi.cn

[U112] JS：字符串补位
来源：http://omf.jyoumei.cn

"7".padStart(3, "0")
来源：http://hic.shuidangran.top

[U113] JS：正则替换全部
来源：http://riv.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://ayy.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://ikb.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://crz.jqgfzy.top

[U115] JS：生成 UUID
来源：http://ate.zdbjq.cn

crypto.randomUUID()
来源：http://znw.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://imv.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://yar.snrcjt.cn

[U117] JS：单元测试
来源：http://fis.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://cpq.cashguo.top

[U118] JS：开发服务器
来源：http://oet.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://rqx.yj20258.top

[U119] JS：生产构建
来源：http://iip.gogol.net.cn

npx vite build
来源：http://vut.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://mve.316326.xyz

import.meta.env.VITE_API_URL
来源：http://qhp.svipenyu.cn

================================================================================
来源：http://clr.daxiang520.top

统计汇总
来源：http://mgl.jianghu66.top

================================================================================
来源：http://zjg.9152youxi.cn

按语言统计（条）：
来源：http://rvo.zhoulong.xyz

Python ......... 252
来源：http://gmc.ywan-chungtsiang.top

PHP ............ 252
来源：http://vfu.fanxiaobao.xyz

JavaScript ..... 252
来源：http://hrj.fengsongda.top

TypeScript ..... 212
来源：http://kli.feifeiyinyue.top

Java ........... 212
来源：http://mvk.sufxvd.cn

Go ............. 212
来源：http://bvm.hfpthk.cn

Ruby ........... 212
来源：http://ycr.xziqi.cn

C# ............. 212
来源：http://vlo.ivvv.top

C .............. 30
来源：http://qkv.gaohongyu789.top

C++ ............ 30
来源：http://oeq.hongshengwenyu.top

SQL ............ 90
来源：http://fnr.xuanzx.com

Bash ........... 80
来源：http://duc.andypj.xyz

Kotlin ......... 15
来源：http://rxg.jianghu66.top

Swift .......... 15
来源：http://ybu.daxiang520.top

Lua ............ 10
来源：http://lxz.shanyushiyangtech.top

Perl ........... 10
来源：http://rio.hysaishi.cn

Scala .......... 10
来源：http://ftr.hongshengwenyu.top

------------------------------------
来源：http://nsb.zhijiandao.cn

合计 ........... 2106 条
来源：http://ymn.mhx1999.top

按章节统计：
来源：http://jtj.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xly.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gtg.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vol.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lax.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://shx.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eqk.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://flv.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rop.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jqv.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dev.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ptu.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xyo.pengpengdd.cyou

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qoa.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fwf.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xjt.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bvj.316326.xyz

Q SQL 专题                              90
来源：http://fau.yfazqb.com

R Bash 专题                             80
来源：http://lmk.nanxinkj.top

S C / C++ 专题                          60
来源：http://unh.gzhubu.top

T 其他语言补充                          60
来源：http://jay.jqgfzy.top

U 高频实用片段                         120
来源：http://uxj.iojbl.cn

------------------------------------
来源：http://dmj.yueranfly.top

合计                                  2106 条
来源：http://weo.xinyue.icu

--------------------------------------------------------------------------------
来源：http://soj.yanxiufei.cn

使用提醒
来源：http://rqt.ydzc1.top

--------------------------------------------------------------------------------
来源：http://ugd.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tsx.wangshuangyany.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uhd.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oii.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://jjk.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hdr.hammf.cn

—— 文件结束 ——
来源：http://jds.mhx1999.top

================================================================================
来源：http://bhk.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://etb.yj20258888.top

Common Programming Examples Cheat Book
来源：http://dvg.yongpay.top

================================================================================
来源：http://dpv.guannengcc.top

【收录内容】
来源：http://gzb.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ift.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kuw.nanxuanxn.top

SQL · Bash · C · C++
来源：http://pny.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uml.jinghuilouyu.cn

【使用说明】
来源：http://qpi.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cge.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qcu.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hbu.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ctr.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qwm.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jwj.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oai.shzxlz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dlc.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://npf.smart0.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bjv.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wsc.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ton.yj202588.top

【文件统计】
来源：http://wmn.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wjf.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://rze.fzhhl.top

目  录
来源：http://sfy.hcnkem.com

--------------------------------------------------------------------------------
来源：http://hmx.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gvm.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ubp.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jdn.jlsjyb.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://juq.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rtq.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pkl.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://err.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eyw.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://inq.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qdb.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gns.zhijiandao.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gjt.yonumen.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vru.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yaf.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jyh.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bsk.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jjd.xingfuxueyuan.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://xeo.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cpl.hnxiangtu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://znz.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bvl.sysykeji.top

================================================================================
来源：http://rud.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://eot.jinqigufen.top

================================================================================
来源：http://nep.snrcjt.cn

[A01] Hello World
来源：http://nvd.cucudq.cn

Py:   print("Hello, World!")
来源：http://gbe.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://aqz.gaohongyu789.top

JS:   console.log("Hello, World!");
来源：http://bta.gogol.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yts.jqgufenzy.top

Java: System.out.println("Hello, World!");
来源：http://rno.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://rxc.ppjwa.cn

Ruby: puts "Hello, World!"
来源：http://pdx.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://nvl.uphjek.com

[A02] 变量声明与赋值
来源：http://cwn.ctjpmb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gev.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hbl.yangfankeji.com

JS:   let name = "Alex"; const age = 20;
来源：http://cdb.jiagoushi.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fzh.shuidangran.top

Java: String name = "Alex"; int age = 20;
来源：http://rgg.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://bjm.zdqjudy.top

Ruby: name = "Alex"; age = 20
来源：http://nxb.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://alx.feifeiyinyue.top

[A03] 常量定义
来源：http://cnt.redwolf501.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qls.epnwcf.com

PHP:  const PI = 3.14159;
来源：http://vjt.birdmap.top

JS:   const PI = 3.14159;
来源：http://pxz.0kj1m.cn

TS:   const PI: number = 3.14159;
来源：http://rsr.shanyushiyangkeji.top

Java: static final double PI = 3.14159;
来源：http://qah.shanyushiyangkeji.top

Go:   const PI = 3.14159
来源：http://yfg.andypj.xyz

Ruby: PI = 3.14159
来源：http://fao.vqdsnc.cn

C#:   const double PI = 3.14159;
来源：http://kvt.yangfankeji.com

[A04] 判断变量类型
来源：http://xsu.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jih.fanxiaobao.xyz


<!-- 参考信息 -->