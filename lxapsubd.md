代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://cfo.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://riu.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://lro.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lmt.zycfv.cn

[U43] PHP：声明命名空间
来源：http://ncs.cucudq.cn

namespace App\Http;
来源：http://sxg.redwolf501.top

[U44] PHP：开启严格类型
来源：http://wos.yuxming.cn

declare(strict_types=1);
来源：http://jmq.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://wtw.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nvt.yanxiufei.cn

[U46] PHP：可空类型
来源：http://vhv.zhiwuduotai.top

?string $name = null
来源：http://wgu.hammf.cn

[U47] PHP：联合类型
来源：http://jvs.dashuyun.cn

int|string $id
来源：http://gmh.ctjpmb.com

[U48] PHP：纯枚举
来源：http://jbm.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aor.hesvh.cn

[U49] PHP：只读属性
来源：http://vzs.fehbvm.com

public readonly string $name
来源：http://tbe.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://fvf.gzhubu.top

public function __construct(private int $id) {}
来源：http://sax.ybcxt.top

[U51] PHP：数组解构
来源：http://bfs.yueranfly.top

[$a, $b] = $arr;
来源：http://lal.svipenyu.cn

[U52] PHP：箭头函数
来源：http://bjw.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://nsa.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://ggj.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://eaa.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://uss.fehbvm.com

$obj?->method()
来源：http://gvx.hammf.cn

[U55] PHP：match 表达式
来源：http://eqd.sufxvd.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://prl.yonumen.top

[U56] PHP：命名参数
来源：http://bly.hnxiangtu.top

f(a: 1, b: 2)
来源：http://jru.nwbrower.top

[U57] PHP：字符串插值
来源：http://zur.smart0.xyz

"值: {$a}"
来源：http://flk.cashguo.top

[U58] PHP：数组三件套
来源：http://ggr.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zjx.zdbjq.cn

[U59] PHP：自定义排序
来源：http://bhq.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://otx.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://ozn.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rkw.cqqwz.cn

[U61] PHP：正则
来源：http://pqr.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gpd.zhijiandao.cn

[U62] PHP：日期对象
来源：http://juq.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hgu.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://vwt.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mqk.52xcode.cn

[U64] PHP：目录遍历
来源：http://hfm.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://ewy.jyoumei.cn

[U65] PHP：会话
来源：http://eqb.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jpp.yj20258.top

[U66] PHP：设置 Cookie
来源：http://bwl.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vfg.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://act.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kza.yvedp.cn

[U68] PHP：PDO 连接
来源：http://zrd.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vvt.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://sap.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mmb.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://nev.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tdg.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://dwu.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://wpq.tanke756.top

[U72] PHP：写错误日志
来源：http://tmj.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://azw.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://lpn.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://kqt.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://wnw.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://krh.sweek.top

[U75] PHP：依赖注入
来源：http://ofr.fktsv.cn

composer require psr/container
来源：http://orr.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://sob.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ywa.wangdashe.top

[U77] PHP：模板渲染
来源：http://bqt.hammf.cn

composer require twig/twig
来源：http://gnh.cashguo.top

[U78] PHP：单元测试
来源：http://dao.zhijiandao.cn

composer require --dev phpunit/phpunit
来源：http://och.yuanzhike.top

[U79] PHP：静态分析
来源：http://oln.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://wps.uphjek.com

[U80] PHP：代码规范修复
来源：http://tbd.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://guq.yj20258888.top

[U81] JS：初始化项目
来源：http://ivj.sxryk.cn

npm init -y;  npm i express
来源：http://zkp.tanke756.top

[U82] JS：package.json 脚本
来源：http://uho.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ejb.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://sne.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://ndb.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://pph.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://lkj.zhongyouzk.top

[U85] JS：可选链
来源：http://vny.yj20258.top

a?.b?.c
来源：http://epk.chenjidiqi.icu

[U86] JS：空值合并
来源：http://agh.hongshengwenyu.top

a ?? b
来源：http://dfl.cdnleiting.top

[U87] JS：解构默认值
来源：http://nfk.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://cnp.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://rqa.cqqwz.cn

{ ...a, ...b }
来源：http://izn.jiagoushi.top

[U89] JS：数组去重
来源：http://brh.hammf.cn

[...new Set(arr)]
来源：http://qiw.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://thl.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://jqo.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://gcq.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hlj.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://pcx.nwbrower.top

structuredClone(obj)
来源：http://jun.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://bkb.jianghu66.top

`共 ${n} 条`
来源：http://zob.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://ccx.pycfn.com

const double = x => x * 2;
来源：http://rtw.hammf.cn

[U95] JS：Promise 包装
来源：http://pxi.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://tce.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://twu.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vma.yj20258.top

[U97] JS：并发请求
来源：http://ccb.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gqs.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://hci.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yss.birdmap.top

[U99] JS：事件监听
来源：http://uiq.jianghu66.top

el.addEventListener("click", e => {})
来源：http://men.meibo888.top

[U100] JS：DOM 查询
来源：http://yws.aizwys.cn

document.querySelector(".item")
来源：http://mrv.epnwcf.com

[U101] JS：classList 操作
来源：http://srp.hnqzz.top

el.classList.toggle("active")
来源：http://qri.jianghu66.top

[U102] JS：本地存储
来源：http://auj.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nlf.fengsongda.top

[U103] JS：定时器
来源：http://wfy.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zws.bbcook.cn

[U104] JS：防抖
来源：http://iuq.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://you.guowangkeji.top

[U105] JS：节流
来源：http://qwd.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://alh.nwbrower.top

[U106] JS：日期格式化
来源：http://bqo.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eei.cashguo.top

[U107] JS：数字千分位
来源：http://een.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iim.tianlin.xyz

[U108] JS：随机整数
来源：http://enz.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zyh.yonumen.top

[U109] JS：数组分组
来源：http://eca.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://nvc.ctjpmb.com

[U110] JS：数组分块
来源：http://lkl.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ops.jianghu66.top

[U111] JS：对象转 Map
来源：http://ngf.daria6918.cn

new Map(Object.entries(obj))
来源：http://ovw.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://srh.xinyue.icu

"7".padStart(3, "0")
来源：http://mlw.yvedp.cn

[U113] JS：正则替换全部
来源：http://mcb.jianghu66.top

s.replaceAll("a", "b")
来源：http://qhm.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://eay.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://osq.zdbjq.cn

[U115] JS：生成 UUID
来源：http://uua.yueranfly.top

crypto.randomUUID()
来源：http://jsh.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://ecr.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://xoz.hcnkem.com

[U117] JS：单元测试
来源：http://fxn.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://iya.bbcook.cn

[U118] JS：开发服务器
来源：http://lxm.316326.xyz

npm i -D vite;  npx vite
来源：http://yse.tianlin.xyz

[U119] JS：生产构建
来源：http://idr.gzhubu.top

npx vite build
来源：http://mnz.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://rgz.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://gup.ehwqpu.com

================================================================================
来源：http://xcd.aibaodan.cn

统计汇总
来源：http://zim.tianlin.xyz

================================================================================
来源：http://vzj.daria6918.cn

按语言统计（条）：
来源：http://hiy.9152youxi.cn

Python ......... 252
来源：http://ogg.gzhubu.top

PHP ............ 252
来源：http://ths.aibaodan.cn

JavaScript ..... 252
来源：http://asx.shanyushiyangtech.top

TypeScript ..... 212
来源：http://wbg.yanxiufei.cn

Java ........... 212
来源：http://rte.sweek.top

Go ............. 212
来源：http://osq.jinqigufen.top

Ruby ........... 212
来源：http://hqd.zhixingplan.top

C# ............. 212
来源：http://iyo.ybcxt.top

C .............. 30
来源：http://bio.hesvh.cn

C++ ............ 30
来源：http://sum.chenjidiqi.icu

SQL ............ 90
来源：http://bjm.fanxiaobao.xyz

Bash ........... 80
来源：http://cwm.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://vnj.xinyue.icu

Swift .......... 15
来源：http://tps.daria6918.cn

Lua ............ 10
来源：http://tvh.yanxiufei.cn

Perl ........... 10
来源：http://qru.zhiwuduotai.top

Scala .......... 10
来源：http://cfd.fehbvm.com

------------------------------------
来源：http://hvi.cashguo.top

合计 ........... 2106 条
来源：http://esf.jinghuilouyu.cn

按章节统计：
来源：http://esx.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nst.daxiang520.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cum.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pam.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yhz.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xzv.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ccv.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lxu.epnwcf.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://etr.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sjw.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ewz.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ebz.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gex.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xec.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gon.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://anq.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://koa.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://mgh.fzhhl.top

R Bash 专题                             80
来源：http://bob.aibaodan.cn

S C / C++ 专题                          60
来源：http://xjb.tanke756.top

T 其他语言补充                          60
来源：http://xnl.havefunace.top

U 高频实用片段                         120
来源：http://sbl.316326.xyz

------------------------------------
来源：http://uuh.ydzc1.top

合计                                  2106 条
来源：http://rhq.wangdashe.top

--------------------------------------------------------------------------------
来源：http://vjb.0kj1m.cn

使用提醒
来源：http://cne.tanke756.top

--------------------------------------------------------------------------------
来源：http://bsv.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zda.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cih.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jnj.9152youxi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nzw.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bqf.cqqwz.cn

—— 文件结束 ——
来源：http://zqd.52xcode.cn

================================================================================
来源：http://hes.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://lrr.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://fll.smart0.xyz

================================================================================
来源：http://vyv.smart0.xyz

【收录内容】
来源：http://dcb.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://prk.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zln.hnqzz.top

SQL · Bash · C · C++
来源：http://iut.aizwys.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ejt.gogol.net.cn

【使用说明】
来源：http://kga.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xnn.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://twt.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vin.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ieb.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ahj.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://siu.vehdjk.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lol.zhijiandao.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bps.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sau.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rvr.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gmw.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jsk.andypj.xyz

【文件统计】
来源：http://nub.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ihr.uphjek.com

--------------------------------------------------------------------------------
来源：http://szn.gotoacloud.top

目  录
来源：http://oxz.xinyue.icu

--------------------------------------------------------------------------------
来源：http://sxo.hammf.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ayk.zycfv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dvs.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://shw.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xua.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nxd.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wqa.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tds.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mos.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gfl.andypj.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wjk.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oem.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://swu.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bhv.yanxiufei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kyv.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kce.snrcjt.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fpc.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vlo.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://acn.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pbm.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qdl.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://usq.vqdsnc.cn

================================================================================
来源：http://lzf.snrcjt.cn

A. 基础语法与类型
来源：http://jpy.ivvv.top

================================================================================
来源：http://bbq.nanxinkj.top

[A01] Hello World
来源：http://hkl.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://znj.xziqi.cn

PHP:  echo "Hello, World!";
来源：http://zxa.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://dta.gotoacloud.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rgs.sweek.top

Java: System.out.println("Hello, World!");
来源：http://wxd.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://bca.hammf.cn

Ruby: puts "Hello, World!"
来源：http://tfn.jlsjyb.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zhp.daria6918.cn

[A02] 变量声明与赋值
来源：http://tsz.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tpk.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bzl.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://klp.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://irb.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://hok.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://zwp.svipenyu.cn

Ruby: name = "Alex"; age = 20
来源：http://eca.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zsk.yj20258888.top

[A03] 常量定义
来源：http://mhb.aibaodan.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://irf.snrcjt.cn

PHP:  const PI = 3.14159;
来源：http://vbz.hfpthk.cn

JS:   const PI = 3.14159;
来源：http://jkt.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://vjj.chenjidiqi.icu

Java: static final double PI = 3.14159;
来源：http://ixf.sjlbkw.cn

Go:   const PI = 3.14159
来源：http://fow.gzhubu.top

Ruby: PI = 3.14159
来源：http://fio.hongshengwenyu.top

C#:   const double PI = 3.14159;
来源：http://vyx.ydjk.org.cn

[A04] 判断变量类型
来源：http://ljv.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bab.shanyushiyangtech.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ryl.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rhd.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://mqp.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mlq.fengsongda.top


<!-- 参考信息 -->