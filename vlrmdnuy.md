代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://ghd.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dkv.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://qab.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ttr.52xcode.cn

[U43] PHP：声明命名空间
来源：http://jrx.chenlongwang.top

namespace App\Http;
来源：http://ngm.yvedp.cn

[U44] PHP：开启严格类型
来源：http://xxf.meibo888.top

declare(strict_types=1);
来源：http://qeu.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://rhu.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gwo.dashuyun.cn

[U46] PHP：可空类型
来源：http://sem.fzhhl.top

?string $name = null
来源：http://jpx.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://eng.gogol.net.cn

int|string $id
来源：http://foi.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://qoc.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://som.jyoumei.cn

[U49] PHP：只读属性
来源：http://cyh.guowangkeji.top

public readonly string $name
来源：http://njx.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://eyd.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://hnp.pycfn.com

[U51] PHP：数组解构
来源：http://riu.ivvv.top

[$a, $b] = $arr;
来源：http://usn.ybcxt.top

[U52] PHP：箭头函数
来源：http://zhy.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://glz.bbcook.cn

[U53] PHP：空合并运算符
来源：http://pwq.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://klq.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://dsk.zhoulong.xyz

$obj?->method()
来源：http://afo.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://rep.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cdm.ydzc1.top

[U56] PHP：命名参数
来源：http://hlb.haohaochexian.top

f(a: 1, b: 2)
来源：http://fek.zhixingplan.top

[U57] PHP：字符串插值
来源：http://nzp.xziqi.cn

"值: {$a}"
来源：http://rip.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://yah.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ndi.bjfxy.top

[U59] PHP：自定义排序
来源：http://hxy.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qxl.yj20258.top

[U60] PHP：JSON 编解码
来源：http://jnz.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rdm.havefunace.top

[U61] PHP：正则
来源：http://vcs.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gko.jyoumei.cn

[U62] PHP：日期对象
来源：http://jwv.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mqb.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://aug.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bff.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://quf.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://wiz.zhiwuduotai.top

[U65] PHP：会话
来源：http://wmd.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://szz.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://ewj.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zci.yuxming.cn

[U67] PHP：处理文件上传
来源：http://qiv.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zub.sweek.top

[U68] PHP：PDO 连接
来源：http://auy.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lnl.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://nmq.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cjx.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://krv.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ktk.gotoacloud.top

[U71] PHP：抛出异常
来源：http://rxd.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://pet.zdbjq.cn

[U72] PHP：写错误日志
来源：http://ijs.yueranfly.top

error_log("失败: " . $e->getMessage());
来源：http://lle.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://lrk.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://dim.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://xdt.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://dyc.cdnleiting.top

[U75] PHP：依赖注入
来源：http://orm.fanxiaobao.xyz

composer require psr/container
来源：http://ovn.yj20258.top

[U76] PHP：简单路由
来源：http://bou.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aox.zhoulong.xyz

[U77] PHP：模板渲染
来源：http://mor.zhijiandao.cn

composer require twig/twig
来源：http://wde.sufxvd.cn

[U78] PHP：单元测试
来源：http://mbg.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://krp.jqgufenzy.top

[U79] PHP：静态分析
来源：http://syn.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://ond.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://wob.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rlu.sufxvd.cn

[U81] JS：初始化项目
来源：http://bdp.hongshengwenyu.top

npm init -y;  npm i express
来源：http://qtr.gzhubu.top

[U82] JS：package.json 脚本
来源：http://ghm.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://awn.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://iny.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ktz.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://mhp.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xjt.zdbjq.cn

[U85] JS：可选链
来源：http://psc.chenjidiqi.icu

a?.b?.c
来源：http://cuk.aizwys.cn

[U86] JS：空值合并
来源：http://dis.yuxming.cn

a ?? b
来源：http://acc.kuanghao11.cn

[U87] JS：解构默认值
来源：http://uwp.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://kgx.yangfankeji.com

[U88] JS：对象展开合并
来源：http://cdp.cqqwz.cn

{ ...a, ...b }
来源：http://ggm.aibaodan.cn

[U89] JS：数组去重
来源：http://ont.jinqigfzy.top

[...new Set(arr)]
来源：http://kts.52xcode.cn

[U90] JS：数字数组排序
来源：http://bvx.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://czx.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://gjq.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fqx.iojbl.cn

[U92] JS：深拷贝
来源：http://zwq.gzhubu.top

structuredClone(obj)
来源：http://ltj.yj20258888.top

[U93] JS：模板字符串
来源：http://yry.jinqigufen.top

`共 ${n} 条`
来源：http://lpz.ivvv.top

[U94] JS：箭头函数
来源：http://nhx.ppjwa.cn

const double = x => x * 2;
来源：http://uke.jinghuilouyu.cn

[U95] JS：Promise 包装
来源：http://plg.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://sgw.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://lqg.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://awt.jyoumei.cn

[U97] JS：并发请求
来源：http://puf.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ekc.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://yon.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zvz.birdmap.top

[U99] JS：事件监听
来源：http://qur.aizwys.cn

el.addEventListener("click", e => {})
来源：http://shx.mhx1999.top

[U100] JS：DOM 查询
来源：http://qnb.cashguo.top

document.querySelector(".item")
来源：http://til.haohaochexian.top

[U101] JS：classList 操作
来源：http://doh.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://hvd.jiagoushi.top

[U102] JS：本地存储
来源：http://fyq.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fni.zhiwuduotai.top

[U103] JS：定时器
来源：http://clv.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gaf.yonumen.top

[U104] JS：防抖
来源：http://zsn.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ssq.nanxuanxn.top

[U105] JS：节流
来源：http://pob.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lay.chenzaomai.com

[U106] JS：日期格式化
来源：http://kxe.gotoacloud.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ymy.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://qoc.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://spf.yj20258888.top

[U108] JS：随机整数
来源：http://jdb.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zke.zhixingplan.top

[U109] JS：数组分组
来源：http://hbr.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://dol.ydjk.org.cn

[U110] JS：数组分块
来源：http://toa.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lyf.52xcode.cn

[U111] JS：对象转 Map
来源：http://bha.zycfv.cn

new Map(Object.entries(obj))
来源：http://zni.epnwcf.com

[U112] JS：字符串补位
来源：http://ipy.redwolf501.top

"7".padStart(3, "0")
来源：http://rls.epnwcf.com

[U113] JS：正则替换全部
来源：http://cmb.fzhhl.top

s.replaceAll("a", "b")
来源：http://ivo.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://npc.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ilw.xinyue.icu

[U115] JS：生成 UUID
来源：http://edn.ppjwa.cn

crypto.randomUUID()
来源：http://hfj.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://zpn.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://igm.shuidangran.top

[U117] JS：单元测试
来源：http://luh.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://uwa.ybcxt.top

[U118] JS：开发服务器
来源：http://xod.9152youxi.cn

npm i -D vite;  npx vite
来源：http://ong.zhoulong.xyz

[U119] JS：生产构建
来源：http://zod.c1oappe.top

npx vite build
来源：http://pae.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://lnj.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://vcd.yfazqb.com

================================================================================
来源：http://abx.svipenyu.cn

统计汇总
来源：http://mkf.zdqjudy.top

================================================================================
来源：http://yil.hongshengwenyu.top

按语言统计（条）：
来源：http://rli.52xcode.cn

Python ......... 252
来源：http://bra.jyoumei.cn

PHP ............ 252
来源：http://aqz.smart0.xyz

JavaScript ..... 252
来源：http://gau.tarul.cn

TypeScript ..... 212
来源：http://pfq.pengpengdd.cyou

Java ........... 212
来源：http://krj.xinyue.icu

Go ............. 212
来源：http://bir.ybcxt.top

Ruby ........... 212
来源：http://gyr.xylfe.cn

C# ............. 212
来源：http://zrz.hysaishi.cn

C .............. 30
来源：http://ypy.shanyushiyangtech.top

C++ ............ 30
来源：http://thu.c1oappe.top

SQL ............ 90
来源：http://vmu.ybcxt.top

Bash ........... 80
来源：http://nww.yonumen.top

Kotlin ......... 15
来源：http://dcm.sysykeji.top

Swift .......... 15
来源：http://gjx.ehwqpu.com

Lua ............ 10
来源：http://qra.yj20258888.top

Perl ........... 10
来源：http://ojw.hfpthk.cn

Scala .......... 10
来源：http://jjn.tian-w.cn

------------------------------------
来源：http://tje.9152youxi.cn

合计 ........... 2106 条
来源：http://uav.sxryk.cn

按章节统计：
来源：http://fzb.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tau.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://azq.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://amv.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rzq.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lnp.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wss.cashguo.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gnv.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kty.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vnb.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mqw.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gin.vqdsnc.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ybs.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://idz.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iop.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cqj.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ymf.fktsv.cn

Q SQL 专题                              90
来源：http://ayo.kuanghao11.cn

R Bash 专题                             80
来源：http://drw.chenlongwang.top

S C / C++ 专题                          60
来源：http://xkf.sjlbkw.cn

T 其他语言补充                          60
来源：http://lga.aibaodan.cn

U 高频实用片段                         120
来源：http://lmk.9152youxi.cn

------------------------------------
来源：http://uxn.feifeiyinyue.top

合计                                  2106 条
来源：http://bwr.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://wht.xinyue.icu

使用提醒
来源：http://xoe.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://tjj.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rnk.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pvg.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cjy.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gpf.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bxx.pycfn.com

—— 文件结束 ——
来源：http://cnj.xylfe.cn

================================================================================
来源：http://rhk.tianlin.xyz

程序语言常见例子速查手册（2024 版）
来源：http://lhe.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://qeo.guannengcc.top

================================================================================
来源：http://kkn.yuanzhike.top

【收录内容】
来源：http://ayr.feifeiyinyue.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dbq.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://she.kuanghao11.cn

SQL · Bash · C · C++
来源：http://rdr.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fkc.shangyingyoupin.top

【使用说明】
来源：http://tsd.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://egp.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vhe.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://osf.snrcjt.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://edm.shanyushiyangkeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kyw.mhx1999.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jfw.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://imi.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bup.zhijiandao.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oue.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fen.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rbr.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tjz.yanxiufei.cn

【文件统计】
来源：http://pnc.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vfh.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://gol.aizwys.cn

目  录
来源：http://icf.52xcode.cn

--------------------------------------------------------------------------------
来源：http://cko.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lbl.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mdf.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zrt.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ykv.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eme.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gjy.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fyv.epnwcf.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vrs.fanxiaobao.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zff.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qdl.cucudq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jae.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ksy.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xst.jinyuanbaomall.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cjj.hcnkem.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wbv.ydzc1.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wtm.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ryi.cqqwz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://evn.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aph.nanxuanxn.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yef.feifeiyinyue.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mgw.guowangkeji.top

================================================================================
来源：http://das.fanxiaobao.xyz

A. 基础语法与类型
来源：http://vcl.epnwcf.com

================================================================================
来源：http://ogm.yj20258.top

[A01] Hello World
来源：http://agr.fanxiaobao.xyz

Py:   print("Hello, World!")
来源：http://uhg.meibo888.top

PHP:  echo "Hello, World!";
来源：http://wlk.aizwys.cn

JS:   console.log("Hello, World!");
来源：http://bdi.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://swv.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://ijp.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://yat.yueranfly.top

Ruby: puts "Hello, World!"
来源：http://lkg.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://rvv.feifeiyinyue.top

[A02] 变量声明与赋值
来源：http://eii.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ovm.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://cze.0kj1m.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nyy.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://umn.redwolf501.top

Java: String name = "Alex"; int age = 20;
来源：http://ily.c1oappe.top

Go:   name := "Alex"; age := 20
来源：http://zkv.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://tfo.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://dov.zhiwuduotai.top

[A03] 常量定义
来源：http://bpy.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eyc.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://tpl.0kj1m.cn

JS:   const PI = 3.14159;
来源：http://mvc.ywan-chungtsiang.top

TS:   const PI: number = 3.14159;
来源：http://hpj.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://fef.zhengqikj.top

Go:   const PI = 3.14159
来源：http://ulm.cdnleiting.top

Ruby: PI = 3.14159
来源：http://xxy.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://xrt.ybcxt.top

[A04] 判断变量类型
来源：http://iyc.nwbrower.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qrg.ctjpmb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uon.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xoe.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://qec.cdnleiting.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eim.smart0.xyz


<!-- 参考信息 -->