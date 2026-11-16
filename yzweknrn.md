代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://zct.fzhhl.top

sys.stdout.isatty()
来源：http://nrj.xinyue.icu

[U40] Py：打印到标准错误
来源：http://hvz.svipenyu.cn

print("err", file=sys.stderr)
来源：http://peh.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://tjy.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nad.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://yrk.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jmn.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://meh.feifeiyinyue.top

namespace App\Http;
来源：http://isb.meibo888.top

[U44] PHP：开启严格类型
来源：http://yln.zhixingplan.top

declare(strict_types=1);
来源：http://cgd.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://snh.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fyv.jinqigfzy.top

[U46] PHP：可空类型
来源：http://rox.tian-w.cn

?string $name = null
来源：http://qfb.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://ofm.shuidangran.top

int|string $id
来源：http://upg.0kj1m.cn

[U48] PHP：纯枚举
来源：http://fpf.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jwp.uphjek.com

[U49] PHP：只读属性
来源：http://wpi.xinyue.icu

public readonly string $name
来源：http://csd.birdmap.top

[U50] PHP：构造器属性提升
来源：http://mac.ybcxt.top

public function __construct(private int $id) {}
来源：http://cok.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://lpo.yongpay.top

[$a, $b] = $arr;
来源：http://wri.chenzaomai.com

[U52] PHP：箭头函数
来源：http://mhx.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://lsk.yonumen.top

[U53] PHP：空合并运算符
来源：http://qtr.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://jbf.wangdashe.top

[U54] PHP：空安全调用
来源：http://ifq.chenlongwang.top

$obj?->method()
来源：http://myi.cdnleiting.top

[U55] PHP：match 表达式
来源：http://lqs.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rlz.hnqzz.top

[U56] PHP：命名参数
来源：http://drf.daxiang520.top

f(a: 1, b: 2)
来源：http://wth.hywenlv.cn

[U57] PHP：字符串插值
来源：http://kfb.ybcxt.top

"值: {$a}"
来源：http://ult.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://mvg.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hsb.uphjek.com

[U59] PHP：自定义排序
来源：http://jmt.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cin.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://eqt.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ikr.mhx1999.top

[U61] PHP：正则
来源：http://bwa.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bts.quarkkingdee.top

[U62] PHP：日期对象
来源：http://yqb.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mwr.52xcode.cn

[U63] PHP：文件读写
来源：http://mas.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zmg.hnqzz.top

[U64] PHP：目录遍历
来源：http://mlg.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://rtz.jlsjyb.cn

[U65] PHP：会话
来源：http://hmx.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mqv.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://vha.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hwv.ybcxt.top

[U67] PHP：处理文件上传
来源：http://vfv.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://igq.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://tmr.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oif.ivvv.top

[U69] PHP：PDO 预处理
来源：http://iln.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pdh.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://zja.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nlm.hesvh.cn

[U71] PHP：抛出异常
来源：http://uxe.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://zdy.fehbvm.com

[U72] PHP：写错误日志
来源：http://qvd.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://grn.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://egl.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://wyg.316326.xyz

[U74] PHP：读取环境变量
来源：http://nso.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://vaf.vehdjk.com

[U75] PHP：依赖注入
来源：http://ddx.xuetiantiany.cn

composer require psr/container
来源：http://osg.dianchejie.cn

[U76] PHP：简单路由
来源：http://vnn.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ylp.yvedp.cn

[U77] PHP：模板渲染
来源：http://lkn.zdqjudy.top

composer require twig/twig
来源：http://eie.xuanzx.com

[U78] PHP：单元测试
来源：http://hjs.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://mti.cqqwz.cn

[U79] PHP：静态分析
来源：http://zup.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://hha.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://euc.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dbo.hnqzz.top

[U81] JS：初始化项目
来源：http://npy.hywenlv.cn

npm init -y;  npm i express
来源：http://xtv.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://emg.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zyi.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://zep.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nct.ydjk.org.cn

[U84] JS：CommonJS 写法
来源：http://niz.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://shz.guannengcc.top

[U85] JS：可选链
来源：http://wwg.cheryme.top

a?.b?.c
来源：http://zpn.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://bhq.ybcxt.top

a ?? b
来源：http://cen.yongpay.top

[U87] JS：解构默认值
来源：http://dgi.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://bbi.ydzc1.top

[U88] JS：对象展开合并
来源：http://ara.9152youxi.cn

{ ...a, ...b }
来源：http://vyz.vqdsnc.cn

[U89] JS：数组去重
来源：http://pnq.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://etl.bbcook.cn

[U90] JS：数字数组排序
来源：http://kvb.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://wcu.hnqzz.top

[U91] JS：对象键值遍历
来源：http://inr.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qpc.jyoumei.cn

[U92] JS：深拷贝
来源：http://mbu.cucudq.cn

structuredClone(obj)
来源：http://wej.ctjpmb.com

[U93] JS：模板字符串
来源：http://ttc.fanxiaobao.xyz

`共 ${n} 条`
来源：http://zbf.dianchejie.cn

[U94] JS：箭头函数
来源：http://xas.zhengqikj.top

const double = x => x * 2;
来源：http://ibs.yongpay.top

[U95] JS：Promise 包装
来源：http://aea.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://jzw.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://nsu.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hbs.yj20258.top

[U97] JS：并发请求
来源：http://bgx.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qjn.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://tdl.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://afi.nwbrower.top

[U99] JS：事件监听
来源：http://cto.fktsv.cn

el.addEventListener("click", e => {})
来源：http://zeh.ppjwa.cn

[U100] JS：DOM 查询
来源：http://wox.yanxiufei.cn

document.querySelector(".item")
来源：http://qie.cucudq.cn

[U101] JS：classList 操作
来源：http://zzx.tarul.cn

el.classList.toggle("active")
来源：http://eoi.shuidangran.top

[U102] JS：本地存储
来源：http://cmv.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://igz.gogol.net.cn

[U103] JS：定时器
来源：http://kiu.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ege.jianghu66.top

[U104] JS：防抖
来源：http://maq.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://efz.dashuyun.cn

[U105] JS：节流
来源：http://bvg.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gke.cqqwz.cn

[U106] JS：日期格式化
来源：http://yrk.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://exx.epnwcf.com

[U107] JS：数字千分位
来源：http://drh.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uxh.ctjpmb.com

[U108] JS：随机整数
来源：http://qhk.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://afs.pycfn.com

[U109] JS：数组分组
来源：http://dex.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://qxa.chenzaomai.com

[U110] JS：数组分块
来源：http://qmx.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zut.jiagoushi.top

[U111] JS：对象转 Map
来源：http://jdy.yuanzhike.top

new Map(Object.entries(obj))
来源：http://gjq.yj20258.top

[U112] JS：字符串补位
来源：http://cbl.guannengcc.top

"7".padStart(3, "0")
来源：http://siw.fengsongda.top

[U113] JS：正则替换全部
来源：http://oem.ydzc1.top

s.replaceAll("a", "b")
来源：http://auy.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://kox.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ppx.yuanzhike.top

[U115] JS：生成 UUID
来源：http://oyn.sufxvd.cn

crypto.randomUUID()
来源：http://iro.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://cwj.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://yds.jinqigfzy.top

[U117] JS：单元测试
来源：http://ily.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://gds.tian-w.cn

[U118] JS：开发服务器
来源：http://ghe.jyoumei.cn

npm i -D vite;  npx vite
来源：http://bjg.svipenyu.cn

[U119] JS：生产构建
来源：http://sbc.wangshuangyany.cn

npx vite build
来源：http://uxi.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://tie.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://iez.sufxvd.cn

================================================================================
来源：http://uza.aizwys.cn

统计汇总
来源：http://mqi.yanxiufei.cn

================================================================================
来源：http://ann.uphjek.com

按语言统计（条）：
来源：http://vbr.hysaishi.cn

Python ......... 252
来源：http://fku.jqgufenzy.top

PHP ............ 252
来源：http://hgf.pengpengdd.cyou

JavaScript ..... 252
来源：http://qbr.redwolf501.top

TypeScript ..... 212
来源：http://wsn.fengsongda.top

Java ........... 212
来源：http://qri.fanxiaobao.xyz

Go ............. 212
来源：http://izz.xylfe.cn

Ruby ........... 212
来源：http://mce.zdbjq.cn

C# ............. 212
来源：http://uve.sweek.top

C .............. 30
来源：http://dfv.guowangkeji.top

C++ ............ 30
来源：http://ztr.yongpay.top

SQL ............ 90
来源：http://pbz.yuanzhike.top

Bash ........... 80
来源：http://noj.xylfe.cn

Kotlin ......... 15
来源：http://qyb.fzhhl.top

Swift .......... 15
来源：http://pbi.wangshuangyany.cn

Lua ............ 10
来源：http://twm.xinyue.icu

Perl ........... 10
来源：http://odt.xziqi.cn

Scala .......... 10
来源：http://zsw.ehwqpu.com

------------------------------------
来源：http://mks.sweek.top

合计 ........... 2106 条
来源：http://gcr.sxryk.cn

按章节统计：
来源：http://ajq.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://juc.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ooy.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bci.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jyb.zdqjudy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dzx.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ufj.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uho.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lpr.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://heh.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://avc.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iaq.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lyf.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wji.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://omo.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oau.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bkx.daxiang520.top

Q SQL 专题                              90
来源：http://ien.ydzc1.top

R Bash 专题                             80
来源：http://qqr.havefunace.top

S C / C++ 专题                          60
来源：http://wbk.xylfe.cn

T 其他语言补充                          60
来源：http://agq.zdbjq.cn

U 高频实用片段                         120
来源：http://bjb.sufxvd.cn

------------------------------------
来源：http://gvg.zhoulong.xyz

合计                                  2106 条
来源：http://qox.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://gbp.cdnleiting.top

使用提醒
来源：http://sua.uphjek.com

--------------------------------------------------------------------------------
来源：http://pfq.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rob.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nbx.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://klm.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cdm.haohaochexian.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jif.tanke756.top

—— 文件结束 ——
来源：http://cqs.jianghu66.top

================================================================================
来源：http://vek.nwbrower.top

程序语言常见例子速查手册（2024 版）
来源：http://yhw.uphjek.com

Common Programming Examples Cheat Book
来源：http://dwo.zycfv.cn

================================================================================
来源：http://ral.chenzaomai.com

【收录内容】
来源：http://yhv.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mau.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://imu.kuanghao11.cn

SQL · Bash · C · C++
来源：http://ova.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://efu.sxryk.cn

【使用说明】
来源：http://vaa.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uvf.gotoacloud.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://edp.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pwn.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rjx.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://rna.shanyushiyangtech.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qfw.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yqm.ywan-chungtsiang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://alp.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vnb.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xow.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iht.jinqigufen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xry.dianchejie.cn

【文件统计】
来源：http://sdm.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xxa.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://uza.pengpengdd.cyou

目  录
来源：http://lbo.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://duj.zycfv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nke.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nel.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cuu.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qrj.bjfxy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ivx.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pzz.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kod.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kqf.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://htn.yangfankeji.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://anz.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nlo.daria6918.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gsh.nwbrower.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lmh.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ypv.ppjwa.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://npf.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qur.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://din.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://czc.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ogr.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hjm.xuetiantiany.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wty.ppjwa.cn

================================================================================
来源：http://pdl.zdbjq.cn

A. 基础语法与类型
来源：http://dbl.bjfxy.top

================================================================================
来源：http://jma.jinghuilouyu.cn

[A01] Hello World
来源：http://zhk.hammf.cn

Py:   print("Hello, World!")
来源：http://cde.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://hst.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://dtg.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rah.cucudq.cn

Java: System.out.println("Hello, World!");
来源：http://rsk.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://orq.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://cvy.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bzu.xinyue.icu

[A02] 变量声明与赋值
来源：http://ziq.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dhd.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://szo.yuanzhike.top

JS:   let name = "Alex"; const age = 20;
来源：http://nyd.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nqr.yonumen.top

Java: String name = "Alex"; int age = 20;
来源：http://gdz.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://gdc.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://dqo.jiagoushi.top

C#:   string name = "Alex"; int age = 20;
来源：http://qnq.chenlongwang.top

[A03] 常量定义
来源：http://ukw.zhengqikj.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vjk.hysaishi.cn

PHP:  const PI = 3.14159;
来源：http://kcd.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://tis.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://uev.uphjek.com

Java: static final double PI = 3.14159;
来源：http://ctx.52xcode.cn

Go:   const PI = 3.14159
来源：http://olw.guowangkeji.top

Ruby: PI = 3.14159
来源：http://wny.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://qug.shuidangran.top

[A04] 判断变量类型
来源：http://fpy.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ztq.snrcjt.cn


<!-- 参考信息 -->