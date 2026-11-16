代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://rhe.shzxlz.cn

sys.stdout.isatty()
来源：http://aea.hammf.cn

[U40] Py：打印到标准错误
来源：http://lls.tian-w.cn

print("err", file=sys.stderr)
来源：http://xpf.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://egr.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://cdk.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://ugh.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fbf.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://rfd.jianghu66.top

namespace App\Http;
来源：http://odc.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://ber.nanxuanxn.top

declare(strict_types=1);
来源：http://rqp.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://arh.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mla.jyoumei.cn

[U46] PHP：可空类型
来源：http://irm.yuanzhike.top

?string $name = null
来源：http://hvd.ppjwa.cn

[U47] PHP：联合类型
来源：http://ytl.zhongyouzk.top

int|string $id
来源：http://obe.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://sdl.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wnk.zycfv.cn

[U49] PHP：只读属性
来源：http://brh.shangyingyoupin.top

public readonly string $name
来源：http://nrv.316326.xyz

[U50] PHP：构造器属性提升
来源：http://hgu.zdbjq.cn

public function __construct(private int $id) {}
来源：http://pmg.yj202588.top

[U51] PHP：数组解构
来源：http://zjt.cucudq.cn

[$a, $b] = $arr;
来源：http://sfw.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://okn.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://afj.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://rlz.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://uyu.0kj1m.cn

[U54] PHP：空安全调用
来源：http://cos.zycfv.cn

$obj?->method()
来源：http://qwd.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://ncn.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tui.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://vqs.jianghu66.top

f(a: 1, b: 2)
来源：http://mfg.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://xfu.gotoacloud.top

"值: {$a}"
来源：http://uqb.fktsv.cn

[U58] PHP：数组三件套
来源：http://esq.zdqjudy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lzc.xinyue.icu

[U59] PHP：自定义排序
来源：http://ojl.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mhv.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://pdx.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eyf.yj20258.top

[U61] PHP：正则
来源：http://lov.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sfn.birdmap.top

[U62] PHP：日期对象
来源：http://fvg.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bxj.zhixingplan.top

[U63] PHP：文件读写
来源：http://bec.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zal.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://xxv.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://ugr.yonumen.top

[U65] PHP：会话
来源：http://lmu.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bkz.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://scn.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ivr.yfazqb.com

[U67] PHP：处理文件上传
来源：http://goy.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hdu.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://ebd.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xgd.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://ite.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pgh.aizwys.cn

[U70] PHP：PDO 事务
来源：http://egu.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://awv.yj202588.top

[U71] PHP：抛出异常
来源：http://ywl.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://nzz.yuxming.cn

[U72] PHP：写错误日志
来源：http://vdo.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://rjz.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://acr.birdmap.top

parse_ini_file("config.ini", true)
来源：http://yjx.sysykeji.top

[U74] PHP：读取环境变量
来源：http://ltw.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://obf.ydzc1.top

[U75] PHP：依赖注入
来源：http://rlk.zdqjudy.top

composer require psr/container
来源：http://gvt.ehwqpu.com

[U76] PHP：简单路由
来源：http://vor.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vwz.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://yrz.shanyushiyangtech.top

composer require twig/twig
来源：http://vzw.yanxiufei.cn

[U78] PHP：单元测试
来源：http://ehn.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://vte.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://ajq.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://gwe.yonumen.top

[U80] PHP：代码规范修复
来源：http://esr.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ugg.bjfxy.top

[U81] JS：初始化项目
来源：http://fbu.ydzc1.top

npm init -y;  npm i express
来源：http://efd.cheryme.top

[U82] JS：package.json 脚本
来源：http://qjd.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vdq.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://jhg.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://hua.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://vlz.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://kwy.svipenyu.cn

[U85] JS：可选链
来源：http://jxn.snrcjt.cn

a?.b?.c
来源：http://zjm.smart0.xyz

[U86] JS：空值合并
来源：http://lkb.havefunace.top

a ?? b
来源：http://yhy.yanxiufei.cn

[U87] JS：解构默认值
来源：http://jtz.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://yoy.ctjpmb.com

[U88] JS：对象展开合并
来源：http://kil.zhijiandao.cn

{ ...a, ...b }
来源：http://wnb.c1oappe.top

[U89] JS：数组去重
来源：http://frf.yuxming.cn

[...new Set(arr)]
来源：http://opu.iojbl.cn

[U90] JS：数字数组排序
来源：http://mlo.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://neq.ybcxt.top

[U91] JS：对象键值遍历
来源：http://seg.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ckl.yj202588.top

[U92] JS：深拷贝
来源：http://piy.shuidangran.top

structuredClone(obj)
来源：http://qga.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://crj.sysykeji.top

`共 ${n} 条`
来源：http://jsq.hfpthk.cn

[U94] JS：箭头函数
来源：http://rdz.ehwqpu.com

const double = x => x * 2;
来源：http://kto.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://fgg.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://nkw.meibo888.top

[U96] JS：async/await 与异常
来源：http://uyd.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lto.iojbl.cn

[U97] JS：并发请求
来源：http://gwo.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iwe.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://iff.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xes.gzhubu.top

[U99] JS：事件监听
来源：http://apv.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://tpk.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://fty.birdmap.top

document.querySelector(".item")
来源：http://yiz.gaohongyu789.top

[U101] JS：classList 操作
来源：http://zih.bjfxy.top

el.classList.toggle("active")
来源：http://las.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://jdj.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://hgb.fehbvm.com

[U103] JS：定时器
来源：http://oot.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dmx.xuanzx.com

[U104] JS：防抖
来源：http://jgs.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sea.jiagoushi.top

[U105] JS：节流
来源：http://qpm.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ima.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://ljz.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://thx.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://ule.hesvh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hyb.fehbvm.com

[U108] JS：随机整数
来源：http://fiu.ydjk.org.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://obq.feifeiyinyue.top

[U109] JS：数组分组
来源：http://pyj.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://wlv.jiagoushi.top

[U110] JS：数组分块
来源：http://whg.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://utl.tanke756.top

[U111] JS：对象转 Map
来源：http://hso.iojbl.cn

new Map(Object.entries(obj))
来源：http://lhp.hammf.cn

[U112] JS：字符串补位
来源：http://wvx.uphjek.com

"7".padStart(3, "0")
来源：http://phn.daria6918.cn

[U113] JS：正则替换全部
来源：http://xjg.jianghu66.top

s.replaceAll("a", "b")
来源：http://hix.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://oqo.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nji.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://bsx.shanyushiyangtech.top

crypto.randomUUID()
来源：http://dyz.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://pns.tanke756.top

/** @param {string} name */ function f(name) {}
来源：http://igx.daxiang520.top

[U117] JS：单元测试
来源：http://qkv.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://tox.c1oappe.top

[U118] JS：开发服务器
来源：http://mmp.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://dnu.chenlongwang.top

[U119] JS：生产构建
来源：http://sco.jyoumei.cn

npx vite build
来源：http://moe.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://wyk.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://ndt.hammf.cn

================================================================================
来源：http://bnw.jinqigufen.top

统计汇总
来源：http://twm.fktsv.cn

================================================================================
来源：http://cbv.zhaomingkeji.xyz

按语言统计（条）：
来源：http://tec.316326.xyz

Python ......... 252
来源：http://nqo.tanke756.top

PHP ............ 252
来源：http://xim.epnwcf.com

JavaScript ..... 252
来源：http://dab.hnxiangtu.top

TypeScript ..... 212
来源：http://wze.sufxvd.cn

Java ........... 212
来源：http://usu.0kj1m.cn

Go ............. 212
来源：http://vge.fengsongda.top

Ruby ........... 212
来源：http://zpm.jlsjyb.cn

C# ............. 212
来源：http://tth.ybcxt.top

C .............. 30
来源：http://jxc.ywan-chungtsiang.top

C++ ............ 30
来源：http://bpf.jianghu66.top

SQL ............ 90
来源：http://xyf.yfazqb.com

Bash ........... 80
来源：http://xuk.yj20258.top

Kotlin ......... 15
来源：http://bmb.fengsongda.top

Swift .......... 15
来源：http://ztj.bbcook.cn

Lua ............ 10
来源：http://uwa.chenzaomai.com

Perl ........... 10
来源：http://zbj.iojbl.cn

Scala .......... 10
来源：http://blk.xingfuxueyuan.xyz

------------------------------------
来源：http://esi.yuxming.cn

合计 ........... 2106 条
来源：http://vti.tianlin.xyz

按章节统计：
来源：http://eat.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lfz.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eat.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hwv.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ymv.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dom.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sfs.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vun.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ubf.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xso.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qeg.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kvv.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sjv.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://acc.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yqf.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mvc.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qfc.cucudq.cn

Q SQL 专题                              90
来源：http://ugu.hesvh.cn

R Bash 专题                             80
来源：http://nbd.c1oappe.top

S C / C++ 专题                          60
来源：http://ucj.yangfankeji.com

T 其他语言补充                          60
来源：http://xis.jiagoushi.top

U 高频实用片段                         120
来源：http://wrv.zdbjq.cn

------------------------------------
来源：http://afa.zdqjudy.top

合计                                  2106 条
来源：http://qtz.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://dhf.chenzaomai.com

使用提醒
来源：http://mht.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://unc.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wyn.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vqo.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tlz.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vki.daxiang520.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kkm.yuxming.cn

—— 文件结束 ——
来源：http://vph.epnwcf.com

================================================================================
来源：http://ltn.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://inj.xylfe.cn

Common Programming Examples Cheat Book
来源：http://ppy.aibaodan.cn

================================================================================
来源：http://vll.ctjpmb.com

【收录内容】
来源：http://vvz.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://fxu.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tpv.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://zul.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jwx.smart0.xyz

【使用说明】
来源：http://jdj.yfazqb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://koi.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mpl.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ozk.nwbrower.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mex.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jcn.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rvn.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yde.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yim.xinyue.icu

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yil.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://myu.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gdn.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pfa.hammf.cn

【文件统计】
来源：http://tsr.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dpx.yj20258888.top

--------------------------------------------------------------------------------
来源：http://rcw.daxiang520.top

目  录
来源：http://fmo.fengsongda.top

--------------------------------------------------------------------------------
来源：http://rcx.nanxuanxn.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://shu.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dir.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gku.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xgd.quarkkingdee.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://otn.jyoumei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://igt.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uga.jqgfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mhx.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hpd.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lhi.xuanzx.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ndy.aibaodan.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xpz.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vrn.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qys.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gvi.vqdsnc.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oys.vehdjk.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nqw.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zxj.sxryk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mth.nanxinkj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wdw.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://use.jlsjyb.cn

================================================================================
来源：http://sfi.mhx1999.top

A. 基础语法与类型
来源：http://zhg.jiagoushi.top

================================================================================
来源：http://eyu.yj20258.top

[A01] Hello World
来源：http://gcg.tanke756.top

Py:   print("Hello, World!")
来源：http://iqw.jinqigufen.top

PHP:  echo "Hello, World!";
来源：http://ltb.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://vfz.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ecg.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://tiw.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://dnn.hammf.cn

Ruby: puts "Hello, World!"
来源：http://ebw.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ozq.feifeiyinyue.top

[A02] 变量声明与赋值
来源：http://kul.jianghu66.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xor.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dhi.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://zej.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ygt.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://xqb.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://nlh.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://kxz.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dog.yuxming.cn

[A03] 常量定义
来源：http://xwv.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zvq.jianghu66.top

PHP:  const PI = 3.14159;
来源：http://ydz.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://ifr.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://zuh.hnqzz.top

Java: static final double PI = 3.14159;
来源：http://rzg.sysykeji.top

Go:   const PI = 3.14159
来源：http://zxh.hammf.cn

Ruby: PI = 3.14159
来源：http://lpj.cashguo.top

C#:   const double PI = 3.14159;
来源：http://zgf.sxryk.cn

[A04] 判断变量类型
来源：http://vzr.guannengcc.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://wwj.pycfn.com


<!-- 参考信息 -->