代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://dmr.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yop.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://erl.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xlu.jianghu66.top

[U43] PHP：声明命名空间
来源：http://pzw.cheryme.top

namespace App\Http;
来源：http://xae.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://akw.jianghu66.top

declare(strict_types=1);
来源：http://cqh.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://jjb.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rri.sjlbkw.cn

[U46] PHP：可空类型
来源：http://ypm.fanxiaobao.xyz

?string $name = null
来源：http://uoy.quarkkingdee.top

[U47] PHP：联合类型
来源：http://bbv.feifeiyinyue.top

int|string $id
来源：http://oxy.sxryk.cn

[U48] PHP：纯枚举
来源：http://qwa.yuxming.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dth.xinyue.icu

[U49] PHP：只读属性
来源：http://cxh.dashuyun.cn

public readonly string $name
来源：http://kbu.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://spl.yuanzhike.top

public function __construct(private int $id) {}
来源：http://ncd.meibo888.top

[U51] PHP：数组解构
来源：http://lng.guowangkeji.top

[$a, $b] = $arr;
来源：http://vik.gotoacloud.top

[U52] PHP：箭头函数
来源：http://apc.yj20258.top

$double = fn($x) => $x * 2;
来源：http://bjk.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://ndi.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://inn.jiagoushi.top

[U54] PHP：空安全调用
来源：http://jan.zdbjq.cn

$obj?->method()
来源：http://tdi.nanxinkj.top

[U55] PHP：match 表达式
来源：http://pyd.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ofn.sjlbkw.cn

[U56] PHP：命名参数
来源：http://cwk.shzxlz.cn

f(a: 1, b: 2)
来源：http://mor.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://fwe.daxiang520.top

"值: {$a}"
来源：http://spl.cqqwz.cn

[U58] PHP：数组三件套
来源：http://tnt.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nxg.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://bkv.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pcv.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://ybw.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ezk.gzhubu.top

[U61] PHP：正则
来源：http://rwk.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qec.hammf.cn

[U62] PHP：日期对象
来源：http://uhc.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vat.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://zmp.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pym.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://azj.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://oec.hammf.cn

[U65] PHP：会话
来源：http://lof.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iej.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://qii.yuxming.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wzx.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://veo.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cgh.andypj.xyz

[U68] PHP：PDO 连接
来源：http://srm.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://axv.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://bck.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kcl.sweek.top

[U70] PHP：PDO 事务
来源：http://cgs.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fid.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://bgl.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://ned.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://ghc.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://lke.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://ftk.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://ylq.yj20258.top

[U74] PHP：读取环境变量
来源：http://xcz.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://wbz.meibo888.top

[U75] PHP：依赖注入
来源：http://uao.jinghuilouyu.cn

composer require psr/container
来源：http://yez.yuanzhike.top

[U76] PHP：简单路由
来源：http://nba.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://udj.yangfankeji.com

[U77] PHP：模板渲染
来源：http://qjf.jinyuanbaomall.cn

composer require twig/twig
来源：http://drq.xinyue.icu

[U78] PHP：单元测试
来源：http://ktr.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://ffl.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://aqy.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://llq.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://mrn.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ryo.9152youxi.cn

[U81] JS：初始化项目
来源：http://xni.jianghu66.top

npm init -y;  npm i express
来源：http://gsn.wangdashe.top

[U82] JS：package.json 脚本
来源：http://oxu.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mps.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://qgo.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tlz.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://pvj.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://sby.dashuyun.cn

[U85] JS：可选链
来源：http://sux.ppjwa.cn

a?.b?.c
来源：http://rdw.aizwys.cn

[U86] JS：空值合并
来源：http://zcr.pycfn.com

a ?? b
来源：http://jji.fktsv.cn

[U87] JS：解构默认值
来源：http://hju.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://rvm.guannengcc.top

[U88] JS：对象展开合并
来源：http://twl.fanxiaobao.xyz

{ ...a, ...b }
来源：http://twf.andypj.xyz

[U89] JS：数组去重
来源：http://pwx.pycfn.com

[...new Set(arr)]
来源：http://ncj.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://ytb.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://lhr.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://sjg.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://spr.52xcode.cn

[U92] JS：深拷贝
来源：http://zjr.xinyue.icu

structuredClone(obj)
来源：http://tct.gzhubu.top

[U93] JS：模板字符串
来源：http://dvf.ybcxt.top

`共 ${n} 条`
来源：http://xzl.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://nvc.jyoumei.cn

const double = x => x * 2;
来源：http://enx.yfazqb.com

[U95] JS：Promise 包装
来源：http://xxu.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://egc.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://fmd.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pri.gaohongyu789.top

[U97] JS：并发请求
来源：http://dia.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://moc.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://nhk.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ycl.smart0.xyz

[U99] JS：事件监听
来源：http://xzb.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://fgl.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://nfl.redwolf501.top

document.querySelector(".item")
来源：http://gft.fktsv.cn

[U101] JS：classList 操作
来源：http://ypg.yj20258.top

el.classList.toggle("active")
来源：http://nwx.epnwcf.com

[U102] JS：本地存储
来源：http://xez.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ceo.shangyingyoupin.top

[U103] JS：定时器
来源：http://ftg.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cxz.daxiang520.top

[U104] JS：防抖
来源：http://udy.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzz.svipenyu.cn

[U105] JS：节流
来源：http://pvm.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://afo.redwolf501.top

[U106] JS：日期格式化
来源：http://tjj.cucudq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vcb.jqgufenzy.top

[U107] JS：数字千分位
来源：http://ukg.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yua.cqqwz.cn

[U108] JS：随机整数
来源：http://xmt.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ooz.bbcook.cn

[U109] JS：数组分组
来源：http://yrr.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://jpf.bbcook.cn

[U110] JS：数组分块
来源：http://oxn.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ewz.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://mec.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://ysw.ehwqpu.com

[U112] JS：字符串补位
来源：http://jsf.gaohongyu789.top

"7".padStart(3, "0")
来源：http://szd.havefunace.top

[U113] JS：正则替换全部
来源：http://zfm.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://tek.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://hcx.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bnx.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://wwf.tarul.cn

crypto.randomUUID()
来源：http://azl.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://jah.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://whl.hammf.cn

[U117] JS：单元测试
来源：http://ima.zhixingplan.top

npm i -D vitest;  npx vitest
来源：http://jxq.jqgfzy.top

[U118] JS：开发服务器
来源：http://lka.cashguo.top

npm i -D vite;  npx vite
来源：http://css.tian-w.cn

[U119] JS：生产构建
来源：http://kqi.dashuyun.cn

npx vite build
来源：http://fpg.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://alk.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://izh.guannengcc.top

================================================================================
来源：http://cyh.hnqzz.top

统计汇总
来源：http://vyk.yonumen.top

================================================================================
来源：http://bhf.birdmap.top

按语言统计（条）：
来源：http://yax.hongshengwenyu.top

Python ......... 252
来源：http://zbv.chenjidiqi.icu

PHP ............ 252
来源：http://jxx.tianlin.xyz

JavaScript ..... 252
来源：http://zry.daxiang520.top

TypeScript ..... 212
来源：http://dyn.bjfxy.top

Java ........... 212
来源：http://ewv.jinyuanbaomall.cn

Go ............. 212
来源：http://msh.birdmap.top

Ruby ........... 212
来源：http://zch.gotoacloud.top

C# ............. 212
来源：http://wuo.hammf.cn

C .............. 30
来源：http://hfv.cheryme.top

C++ ............ 30
来源：http://cpc.chenlongwang.top

SQL ............ 90
来源：http://ngr.zdbjq.cn

Bash ........... 80
来源：http://fso.fktsv.cn

Kotlin ......... 15
来源：http://pln.shanyushiyangkeji.top

Swift .......... 15
来源：http://qcz.jinyuanbaomall.cn

Lua ............ 10
来源：http://hjk.shanyushiyangkeji.top

Perl ........... 10
来源：http://aen.xingfuxueyuan.xyz

Scala .......... 10
来源：http://qlc.zhoulong.xyz

------------------------------------
来源：http://luh.jiagoushi.top

合计 ........... 2106 条
来源：http://szf.zhongyouzk.top

按章节统计：
来源：http://ybo.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hfd.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zxs.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pmj.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://axg.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://czv.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mrq.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pib.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ury.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://crq.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tdc.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://elc.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dig.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nye.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://twh.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://buy.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cxl.haohaochexian.top

Q SQL 专题                              90
来源：http://mfv.jiagoushi.top

R Bash 专题                             80
来源：http://ifm.ydjk.org.cn

S C / C++ 专题                          60
来源：http://pdv.zdqjudy.top

T 其他语言补充                          60
来源：http://nwr.jqgufenzy.top

U 高频实用片段                         120
来源：http://jzc.zhaomingkeji.xyz

------------------------------------
来源：http://sid.hnqzz.top

合计                                  2106 条
来源：http://xeu.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://vmh.yfazqb.com

使用提醒
来源：http://ixu.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://wxp.redwolf501.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://axc.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fis.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://prr.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oqb.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gev.tanke756.top

—— 文件结束 ——
来源：http://gjg.zhixingplan.top

================================================================================
来源：http://nqp.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://ccz.birdmap.top

Common Programming Examples Cheat Book
来源：http://zqw.daxiang520.top

================================================================================
来源：http://eou.bbcook.cn

【收录内容】
来源：http://fao.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nvf.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jhd.aizwys.cn

SQL · Bash · C · C++
来源：http://crt.redwolf501.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://psj.yvedp.cn

【使用说明】
来源：http://zcr.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nzt.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aye.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gvq.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gih.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://giq.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://snp.hysaishi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hpx.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mrf.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://psg.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hcs.tanke756.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gyh.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nsi.sxryk.cn

【文件统计】
来源：http://iya.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uvt.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://cap.fanxiaobao.xyz

目  录
来源：http://duq.c1oappe.top

--------------------------------------------------------------------------------
来源：http://ywo.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hrv.hcnkem.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gjg.aibaodan.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mtc.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xko.guowangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tos.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://oee.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ucw.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gsg.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lpu.nanxuanxn.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cix.hongshengwenyu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kfg.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yls.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://puf.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iab.xuetiantiany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cas.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lpd.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ysg.birdmap.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ivb.svipenyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iun.yanxiufei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://elz.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fgu.dianchejie.cn

================================================================================
来源：http://uea.sweek.top

A. 基础语法与类型
来源：http://fkd.shuidangran.top

================================================================================
来源：http://koz.yj20258888.top

[A01] Hello World
来源：http://azz.sjlbkw.cn

Py:   print("Hello, World!")
来源：http://shm.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://ckp.ydzc1.top

JS:   console.log("Hello, World!");
来源：http://kww.shanyushiyangtech.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pcd.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://ucn.xziqi.cn

Go:   fmt.Println("Hello, World!")
来源：http://neq.hongshengwenyu.top

Ruby: puts "Hello, World!"
来源：http://ebs.shangyingyoupin.top

C#:   Console.WriteLine("Hello, World!");
来源：http://uqm.haohaochexian.top

[A02] 变量声明与赋值
来源：http://lfh.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hvx.ivvv.top

PHP:  $name = "Alex"; $age = 20;
来源：http://hus.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://axa.0kj1m.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fja.jiagoushi.top

Java: String name = "Alex"; int age = 20;
来源：http://wyd.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://bgq.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://atu.yueranfly.top

C#:   string name = "Alex"; int age = 20;
来源：http://maw.zhengqikj.top

[A03] 常量定义
来源：http://ucv.sjlbkw.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ksc.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://nyf.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://soz.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://qnl.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://jte.haohaochexian.top

Go:   const PI = 3.14159
来源：http://gxf.nanxinkj.top

Ruby: PI = 3.14159
来源：http://jdc.jianghu66.top

C#:   const double PI = 3.14159;
来源：http://qmj.snrcjt.cn

[A04] 判断变量类型
来源：http://vha.c1oappe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://omt.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://phm.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gqx.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://kqh.sjlbkw.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hff.dianchejie.cn


<!-- 参考信息 -->