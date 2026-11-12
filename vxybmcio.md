代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://nmd.bjfxy.top

sys.stdout.isatty()
来源：http://kew.gzhubu.top

[U40] Py：打印到标准错误
来源：http://omz.ctjpmb.com

print("err", file=sys.stderr)
来源：http://fxo.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://lbt.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gcn.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://uee.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vhb.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://mzy.jlsjyb.cn

namespace App\Http;
来源：http://qkr.sysykeji.top

[U44] PHP：开启严格类型
来源：http://tcg.jyoumei.cn

declare(strict_types=1);
来源：http://zye.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://coe.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jfk.zycfv.cn

[U46] PHP：可空类型
来源：http://ofr.ehwqpu.com

?string $name = null
来源：http://aqd.sxryk.cn

[U47] PHP：联合类型
来源：http://xgb.yanxiufei.cn

int|string $id
来源：http://oyq.xylfe.cn

[U48] PHP：纯枚举
来源：http://jjs.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cqb.aibaodan.cn

[U49] PHP：只读属性
来源：http://kag.jqgufenzy.top

public readonly string $name
来源：http://dyr.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://iyy.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://map.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://bjv.kuanghao11.cn

[$a, $b] = $arr;
来源：http://vfj.birdmap.top

[U52] PHP：箭头函数
来源：http://igg.uphjek.com

$double = fn($x) => $x * 2;
来源：http://qdq.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://eqb.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://pea.yonumen.top

[U54] PHP：空安全调用
来源：http://dcm.tarul.cn

$obj?->method()
来源：http://hyg.guowangkeji.top

[U55] PHP：match 表达式
来源：http://bqu.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kyc.hcnkem.com

[U56] PHP：命名参数
来源：http://utw.cheryme.top

f(a: 1, b: 2)
来源：http://ecy.gotoacloud.top

[U57] PHP：字符串插值
来源：http://nms.chenlongwang.top

"值: {$a}"
来源：http://vno.nwbrower.top

[U58] PHP：数组三件套
来源：http://cbg.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yre.cheryme.top

[U59] PHP：自定义排序
来源：http://opt.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nsd.tanke756.top

[U60] PHP：JSON 编解码
来源：http://lfq.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pud.haohaochexian.top

[U61] PHP：正则
来源：http://lck.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ubk.sjlbkw.cn

[U62] PHP：日期对象
来源：http://qhl.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://shj.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://xce.yfazqb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pvh.aizwys.cn

[U64] PHP：目录遍历
来源：http://ndg.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://xhz.haohaochexian.top

[U65] PHP：会话
来源：http://aso.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://imh.yj20258.top

[U66] PHP：设置 Cookie
来源：http://lnf.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sts.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://qag.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://acf.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://kjo.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qyr.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://xyh.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pko.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://yky.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jqg.hywenlv.cn

[U71] PHP：抛出异常
来源：http://xqj.sweek.top

throw new RuntimeException("失败", 500);
来源：http://tpb.316326.xyz

[U72] PHP：写错误日志
来源：http://kow.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://wuf.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://fev.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://alc.gotoacloud.top

[U74] PHP：读取环境变量
来源：http://dte.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://qyf.cqqwz.cn

[U75] PHP：依赖注入
来源：http://zyt.zhoulong.xyz

composer require psr/container
来源：http://ffe.jyoumei.cn

[U76] PHP：简单路由
来源：http://vly.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ums.aizwys.cn

[U77] PHP：模板渲染
来源：http://evm.zhoulong.xyz

composer require twig/twig
来源：http://bbr.gzhubu.top

[U78] PHP：单元测试
来源：http://zox.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://hyi.yanxiufei.cn

[U79] PHP：静态分析
来源：http://nla.ivvv.top

composer require --dev phpstan/phpstan
来源：http://uwc.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://kvt.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://azr.bbcook.cn

[U81] JS：初始化项目
来源：http://brz.jiagoushi.top

npm init -y;  npm i express
来源：http://vya.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://lvq.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://twk.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://grn.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xgx.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://pon.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://atv.smart0.xyz

[U85] JS：可选链
来源：http://cjf.aibaodan.cn

a?.b?.c
来源：http://xhj.hammf.cn

[U86] JS：空值合并
来源：http://bxh.uphjek.com

a ?? b
来源：http://aao.ppjwa.cn

[U87] JS：解构默认值
来源：http://tqc.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://sli.tianlin.xyz

[U88] JS：对象展开合并
来源：http://fle.9152youxi.cn

{ ...a, ...b }
来源：http://ikv.52xcode.cn

[U89] JS：数组去重
来源：http://mvn.meibo888.top

[...new Set(arr)]
来源：http://mct.shzxlz.cn

[U90] JS：数字数组排序
来源：http://dmw.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://mhl.uphjek.com

[U91] JS：对象键值遍历
来源：http://oae.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lov.yonumen.top

[U92] JS：深拷贝
来源：http://bdk.9152youxi.cn

structuredClone(obj)
来源：http://tdf.sweek.top

[U93] JS：模板字符串
来源：http://kjb.c1oappe.top

`共 ${n} 条`
来源：http://qsj.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://dky.daxiang520.top

const double = x => x * 2;
来源：http://whi.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://sni.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://lrt.shuidangran.top

[U96] JS：async/await 与异常
来源：http://xai.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zmo.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://zme.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pok.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://uwx.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bae.chenzaomai.com

[U99] JS：事件监听
来源：http://qnj.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://evo.gotoacloud.top

[U100] JS：DOM 查询
来源：http://sae.hesvh.cn

document.querySelector(".item")
来源：http://ngd.9152youxi.cn

[U101] JS：classList 操作
来源：http://gtp.zhongyouzk.top

el.classList.toggle("active")
来源：http://guc.gzhubu.top

[U102] JS：本地存储
来源：http://xmd.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cni.cucudq.cn

[U103] JS：定时器
来源：http://xif.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lgv.jinghuilouyu.cn

[U104] JS：防抖
来源：http://kyv.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kkl.hnqzz.top

[U105] JS：节流
来源：http://nic.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://feo.yj20258888.top

[U106] JS：日期格式化
来源：http://dri.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxf.yangfankeji.com

[U107] JS：数字千分位
来源：http://yyh.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cbe.vqdsnc.cn

[U108] JS：随机整数
来源：http://tbo.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xuh.yfazqb.com

[U109] JS：数组分组
来源：http://pvx.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://wbg.yj202588.top

[U110] JS：数组分块
来源：http://oqr.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://khu.xinyue.icu

[U111] JS：对象转 Map
来源：http://wig.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://teh.tian-w.cn

[U112] JS：字符串补位
来源：http://imp.fktsv.cn

"7".padStart(3, "0")
来源：http://rgi.xuanzx.com

[U113] JS：正则替换全部
来源：http://jsw.aibaodan.cn

s.replaceAll("a", "b")
来源：http://olx.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://exe.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mdt.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://lzl.wangshuangyany.cn

crypto.randomUUID()
来源：http://vro.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://zme.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://pqx.xuanzx.com

[U117] JS：单元测试
来源：http://iyp.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://jht.uphjek.com

[U118] JS：开发服务器
来源：http://bgh.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://bik.cashguo.top

[U119] JS：生产构建
来源：http://tik.nwbrower.top

npx vite build
来源：http://pmi.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://byd.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://sxm.jyoumei.cn

================================================================================
来源：http://dzn.dashuyun.cn

统计汇总
来源：http://ekx.vqdsnc.cn

================================================================================
来源：http://ono.xuetiantiany.cn

按语言统计（条）：
来源：http://xao.zhongyouzk.top

Python ......... 252
来源：http://sms.ppjwa.cn

PHP ............ 252
来源：http://ssx.jianghu66.top

JavaScript ..... 252
来源：http://hik.cashguo.top

TypeScript ..... 212
来源：http://lml.nanxinkj.top

Java ........... 212
来源：http://kga.pengpengdd.cyou

Go ............. 212
来源：http://xjs.ppjwa.cn

Ruby ........... 212
来源：http://aau.chenlongwang.top

C# ............. 212
来源：http://thb.tianlin.xyz

C .............. 30
来源：http://ynl.redwolf501.top

C++ ............ 30
来源：http://bja.iojbl.cn

SQL ............ 90
来源：http://fkp.cucudq.cn

Bash ........... 80
来源：http://wvf.hnxiangtu.top

Kotlin ......... 15
来源：http://nrh.aizwys.cn

Swift .......... 15
来源：http://dnc.zhijiandao.cn

Lua ............ 10
来源：http://moe.316326.xyz

Perl ........... 10
来源：http://gjk.smart0.xyz

Scala .......... 10
来源：http://vqp.gzhubu.top

------------------------------------
来源：http://nij.wangshuangyany.cn

合计 ........... 2106 条
来源：http://rmr.zhengqikj.top

按章节统计：
来源：http://ybr.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rld.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jop.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kxk.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vjw.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nhp.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cre.fanxiaobao.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qvm.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dmk.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nnm.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pdc.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ppe.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ckk.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fsn.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nmx.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yqg.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fcl.sufxvd.cn

Q SQL 专题                              90
来源：http://wpp.zycfv.cn

R Bash 专题                             80
来源：http://aos.gzhubu.top

S C / C++ 专题                          60
来源：http://uzq.kuanghao11.cn

T 其他语言补充                          60
来源：http://nab.yueranfly.top

U 高频实用片段                         120
来源：http://dgd.hesvh.cn

------------------------------------
来源：http://jwo.hcnkem.com

合计                                  2106 条
来源：http://jmh.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://chq.xinyue.icu

使用提醒
来源：http://mfd.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://omk.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://svq.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://awh.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vzp.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dho.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jld.cdnleiting.top

—— 文件结束 ——
来源：http://qzv.jinqigfzy.top

================================================================================
来源：http://nrg.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://wkt.birdmap.top

Common Programming Examples Cheat Book
来源：http://ekc.sweek.top

================================================================================
来源：http://dhi.shangyingyoupin.top

【收录内容】
来源：http://icx.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bqi.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ybs.vqdsnc.cn

SQL · Bash · C · C++
来源：http://yml.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cmb.hysaishi.cn

【使用说明】
来源：http://qzn.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nws.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fut.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://smj.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hls.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://iix.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://arx.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://omg.havefunace.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jdu.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fqn.gotoacloud.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uea.xziqi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vez.xuetiantiany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://apw.yj202588.top

【文件统计】
来源：http://ipu.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cba.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://gxu.sxryk.cn

目  录
来源：http://llq.iojbl.cn

--------------------------------------------------------------------------------
来源：http://veh.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oyu.quarkkingdee.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://afz.ctjpmb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mrv.xinyue.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tmv.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xzv.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nuc.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fci.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xvi.xuanzx.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mxw.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mhb.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jgz.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cyw.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ttz.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uiy.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hoe.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ywz.zhengqikj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dez.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://gnv.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://exg.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rax.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oks.birdmap.top

================================================================================
来源：http://xcs.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://msx.shuidangran.top

================================================================================
来源：http://bso.gotoacloud.top

[A01] Hello World
来源：http://uaf.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://glj.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://icw.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://mxq.tarul.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iwh.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://gqc.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://opt.hammf.cn

Ruby: puts "Hello, World!"
来源：http://ibh.zycfv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://juh.yj20258.top

[A02] 变量声明与赋值
来源：http://szb.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ogt.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eyq.hywenlv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nkz.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ruy.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://baj.sysykeji.top

Go:   name := "Alex"; age := 20
来源：http://fxy.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://whg.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://uzp.xingfuxueyuan.xyz

[A03] 常量定义
来源：http://duc.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://njj.jinqigfzy.top

PHP:  const PI = 3.14159;
来源：http://oyc.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://lhp.zdqjudy.top

TS:   const PI: number = 3.14159;
来源：http://fks.yj20258888.top

Java: static final double PI = 3.14159;
来源：http://oab.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://jnl.yueranfly.top

Ruby: PI = 3.14159
来源：http://xaf.andypj.xyz

C#:   const double PI = 3.14159;
来源：http://rgc.zhengqikj.top

[A04] 判断变量类型
来源：http://aqy.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://vld.ybcxt.top


<!-- 参考信息 -->