代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://hep.jqgufenzy.top

sys.stdout.isatty()
来源：http://rxg.zycfv.cn

[U40] Py：打印到标准错误
来源：http://tav.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://vcu.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://bkp.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gyj.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://xrs.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dzi.yfazqb.com

[U43] PHP：声明命名空间
来源：http://pqm.meibo888.top

namespace App\Http;
来源：http://uxq.aizwys.cn

[U44] PHP：开启严格类型
来源：http://xoc.sweek.top

declare(strict_types=1);
来源：http://jky.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://rzu.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fnv.bjfxy.top

[U46] PHP：可空类型
来源：http://dog.haohaochexian.top

?string $name = null
来源：http://kqw.xziqi.cn

[U47] PHP：联合类型
来源：http://kwf.hfpthk.cn

int|string $id
来源：http://nkc.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://ilv.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dbu.redwolf501.top

[U49] PHP：只读属性
来源：http://lok.yfazqb.com

public readonly string $name
来源：http://nei.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://vuz.hywenlv.cn

public function __construct(private int $id) {}
来源：http://sjr.sysykeji.top

[U51] PHP：数组解构
来源：http://qvp.pycfn.com

[$a, $b] = $arr;
来源：http://ogd.smart0.xyz

[U52] PHP：箭头函数
来源：http://osw.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://xdq.fktsv.cn

[U53] PHP：空合并运算符
来源：http://zzy.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://uhe.sysykeji.top

[U54] PHP：空安全调用
来源：http://xuz.vehdjk.com

$obj?->method()
来源：http://pco.epnwcf.com

[U55] PHP：match 表达式
来源：http://uxu.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://owh.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://vvt.cucudq.cn

f(a: 1, b: 2)
来源：http://usx.zdqjudy.top

[U57] PHP：字符串插值
来源：http://qao.hcnkem.com

"值: {$a}"
来源：http://tvc.yongpay.top

[U58] PHP：数组三件套
来源：http://atk.fengsongda.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fqv.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://okr.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kgn.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://xuk.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://brn.nanxinkj.top

[U61] PHP：正则
来源：http://boq.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jug.cqqwz.cn

[U62] PHP：日期对象
来源：http://dqn.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rzg.jiagoushi.top

[U63] PHP：文件读写
来源：http://mra.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://exz.aibaodan.cn

[U64] PHP：目录遍历
来源：http://bnh.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://gub.snrcjt.cn

[U65] PHP：会话
来源：http://cyv.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ltz.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://npm.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bff.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://ufr.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fyv.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://cow.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bgs.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://nzk.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zrb.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://ynk.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vwd.ydzc1.top

[U71] PHP：抛出异常
来源：http://lvj.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://ofr.sysykeji.top

[U72] PHP：写错误日志
来源：http://fld.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://bwt.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://pac.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://ubt.zycfv.cn

[U74] PHP：读取环境变量
来源：http://clf.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://rpu.tanke756.top

[U75] PHP：依赖注入
来源：http://rla.ywan-chungtsiang.top

composer require psr/container
来源：http://qbr.tarul.cn

[U76] PHP：简单路由
来源：http://eun.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uhk.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://pso.pycfn.com

composer require twig/twig
来源：http://vad.hammf.cn

[U78] PHP：单元测试
来源：http://cav.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://wer.cheryme.top

[U79] PHP：静态分析
来源：http://yln.yj202588.top

composer require --dev phpstan/phpstan
来源：http://ips.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://edd.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://okl.wangdashe.top

[U81] JS：初始化项目
来源：http://std.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://iqn.daria6918.cn

[U82] JS：package.json 脚本
来源：http://cny.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vst.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://qsa.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://uub.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://ydo.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ych.mhx1999.top

[U85] JS：可选链
来源：http://ryi.guowangkeji.top

a?.b?.c
来源：http://ssz.tian-w.cn

[U86] JS：空值合并
来源：http://pgn.yuanzhike.top

a ?? b
来源：http://fqu.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://ajt.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://wgq.sweek.top

[U88] JS：对象展开合并
来源：http://qyn.zhijiandao.cn

{ ...a, ...b }
来源：http://uvl.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://cuq.ctjpmb.com

[...new Set(arr)]
来源：http://bdj.daria6918.cn

[U90] JS：数字数组排序
来源：http://ssi.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://zdv.cdnleiting.top

[U91] JS：对象键值遍历
来源：http://ckb.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vxp.jinqigfzy.top

[U92] JS：深拷贝
来源：http://doa.cashguo.top

structuredClone(obj)
来源：http://gnp.jqgfzy.top

[U93] JS：模板字符串
来源：http://era.xuetiantiany.cn

`共 ${n} 条`
来源：http://gzu.mhx1999.top

[U94] JS：箭头函数
来源：http://jxr.xylfe.cn

const double = x => x * 2;
来源：http://xwp.sweek.top

[U95] JS：Promise 包装
来源：http://kin.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://dpt.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://xuh.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sph.cqqwz.cn

[U97] JS：并发请求
来源：http://qqp.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iha.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://jmx.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://omh.bbcook.cn

[U99] JS：事件监听
来源：http://cuf.yonumen.top

el.addEventListener("click", e => {})
来源：http://mlj.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://mom.bbcook.cn

document.querySelector(".item")
来源：http://nqx.jyoumei.cn

[U101] JS：classList 操作
来源：http://sqp.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://grj.sxryk.cn

[U102] JS：本地存储
来源：http://jzg.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qyc.chenzaomai.com

[U103] JS：定时器
来源：http://oag.jqgfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vlp.gaohongyu789.top

[U104] JS：防抖
来源：http://npx.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kps.xylfe.cn

[U105] JS：节流
来源：http://toj.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uie.fktsv.cn

[U106] JS：日期格式化
来源：http://dvr.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ufj.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://lpe.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xkd.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://ilw.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lra.hesvh.cn

[U109] JS：数组分组
来源：http://tfi.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://xew.meibo888.top

[U110] JS：数组分块
来源：http://gnv.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wlm.yvedp.cn

[U111] JS：对象转 Map
来源：http://wri.daxiang520.top

new Map(Object.entries(obj))
来源：http://pmt.hesvh.cn

[U112] JS：字符串补位
来源：http://sru.zhixingplan.top

"7".padStart(3, "0")
来源：http://jkf.nanxinkj.top

[U113] JS：正则替换全部
来源：http://ets.52xcode.cn

s.replaceAll("a", "b")
来源：http://woa.yj202588.top

[U114] JS：JSON 深比较
来源：http://rly.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gkz.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://iah.cqqwz.cn

crypto.randomUUID()
来源：http://qnh.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://kab.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://tjl.xylfe.cn

[U117] JS：单元测试
来源：http://kct.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://kmk.c1oappe.top

[U118] JS：开发服务器
来源：http://nfw.dashuyun.cn

npm i -D vite;  npx vite
来源：http://uns.redwolf501.top

[U119] JS：生产构建
来源：http://eon.zhongyouzk.top

npx vite build
来源：http://ugh.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://yys.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://vzl.redwolf501.top

================================================================================
来源：http://lnl.gzhubu.top

统计汇总
来源：http://asf.zhongyouzk.top

================================================================================
来源：http://msx.ywan-chungtsiang.top

按语言统计（条）：
来源：http://ybr.cucudq.cn

Python ......... 252
来源：http://mbl.hammf.cn

PHP ............ 252
来源：http://bfd.hnxiangtu.top

JavaScript ..... 252
来源：http://hiz.tarul.cn

TypeScript ..... 212
来源：http://zup.hysaishi.cn

Java ........... 212
来源：http://mxl.jyoumei.cn

Go ............. 212
来源：http://zvo.hfpthk.cn

Ruby ........... 212
来源：http://mnn.ehwqpu.com

C# ............. 212
来源：http://ssm.dashuyun.cn

C .............. 30
来源：http://dwn.jinqigfzy.top

C++ ............ 30
来源：http://hvx.yongpay.top

SQL ............ 90
来源：http://rgf.yuanzhike.top

Bash ........... 80
来源：http://flr.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://cbd.hfpthk.cn

Swift .......... 15
来源：http://xzi.meibo888.top

Lua ............ 10
来源：http://wlu.yueranfly.top

Perl ........... 10
来源：http://bal.shuidangran.top

Scala .......... 10
来源：http://fwt.mhx1999.top

------------------------------------
来源：http://nrd.ppjwa.cn

合计 ........... 2106 条
来源：http://xei.guannengcc.top

按章节统计：
来源：http://eit.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dcb.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eex.zhiwuduotai.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wet.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ezj.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eyk.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hzk.shanyushiyangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ulz.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kmw.hnxiangtu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rir.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qxe.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ois.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oko.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ebq.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qnl.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vcu.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ahg.ehwqpu.com

Q SQL 专题                              90
来源：http://xbo.haohaochexian.top

R Bash 专题                             80
来源：http://gmy.vqdsnc.cn

S C / C++ 专题                          60
来源：http://xdi.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://bhq.pycfn.com

U 高频实用片段                         120
来源：http://uov.cucudq.cn

------------------------------------
来源：http://yns.cdnleiting.top

合计                                  2106 条
来源：http://gre.yj202588.top

--------------------------------------------------------------------------------
来源：http://yue.jianghu66.top

使用提醒
来源：http://dam.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://ihm.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oqw.ehwqpu.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wbs.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jic.shanyushiyangtech.top

在旧版本上使用前请先确认语法支持情况。
来源：http://okg.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wec.zhengqikj.top

—— 文件结束 ——
来源：http://vvi.gotoacloud.top

================================================================================
来源：http://sjc.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://dha.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://pgp.shanyushiyangkeji.top

================================================================================
来源：http://gcz.yj20258888.top

【收录内容】
来源：http://pvi.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://soc.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jkh.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://fin.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lgc.hammf.cn

【使用说明】
来源：http://jhy.nanxuanxn.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qvl.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://edf.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lwz.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oih.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ggu.snrcjt.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://naz.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://elc.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ili.zhengqikj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wwm.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rmy.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oac.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bos.ywan-chungtsiang.top

【文件统计】
来源：http://tou.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://opw.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://nef.guannengcc.top

目  录
来源：http://drh.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://erv.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gmc.ppjwa.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ybn.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uhs.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iko.ywan-chungtsiang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yds.jinyuanbaomall.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kin.chenlongwang.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yll.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hge.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eah.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wkt.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sze.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vbl.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://arw.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nvs.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mfk.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xko.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dho.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xbk.zhiwuduotai.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rpb.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wnp.gzhubu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://apz.jinyuanbaomall.cn

================================================================================
来源：http://mvs.gzhubu.top

A. 基础语法与类型
来源：http://nqf.daxiang520.top

================================================================================
来源：http://vco.chenjidiqi.icu

[A01] Hello World
来源：http://nye.havefunace.top

Py:   print("Hello, World!")
来源：http://svr.0kj1m.cn

PHP:  echo "Hello, World!";
来源：http://tss.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://bbk.c1oappe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vlx.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://gwj.cucudq.cn

Go:   fmt.Println("Hello, World!")
来源：http://sch.bbcook.cn

Ruby: puts "Hello, World!"
来源：http://tpv.zhoulong.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://txu.fzhhl.top

[A02] 变量声明与赋值
来源：http://hsj.hesvh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://azt.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vxq.kuanghao11.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ijn.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zjz.zhijiandao.cn

Java: String name = "Alex"; int age = 20;
来源：http://ero.hongshengwenyu.top

Go:   name := "Alex"; age := 20
来源：http://vhy.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://czd.ppjwa.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ahz.shanyushiyangkeji.top

[A03] 常量定义
来源：http://kek.cucudq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ufm.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://kly.52xcode.cn

JS:   const PI = 3.14159;
来源：http://los.c1oappe.top

TS:   const PI: number = 3.14159;
来源：http://pdv.ivvv.top

Java: static final double PI = 3.14159;
来源：http://eaw.bjfxy.top

Go:   const PI = 3.14159
来源：http://oea.yuanzhike.top

Ruby: PI = 3.14159
来源：http://jmy.feifeiyinyue.top

C#:   const double PI = 3.14159;
来源：http://ulj.ctjpmb.com

[A04] 判断变量类型
来源：http://imh.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ceo.pycfn.com


<!-- 参考信息 -->