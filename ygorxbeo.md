代发 wailian999

[U37] Py：读写 Excel
来源：http://wbf.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pot.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://bah.kuanghao11.cn

Path(__file__).resolve().parent
来源：http://bsp.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://hih.dianchejie.cn

sys.stdout.isatty()
来源：http://kjl.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://usj.dashuyun.cn

print("err", file=sys.stderr)
来源：http://pox.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://ilk.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://vlx.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://hll.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jul.ydzc1.top

[U43] PHP：声明命名空间
来源：http://eao.jqgufenzy.top

namespace App\Http;
来源：http://non.havefunace.top

[U44] PHP：开启严格类型
来源：http://rxo.chenzaomai.com

declare(strict_types=1);
来源：http://pky.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://kty.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tni.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://bei.pycfn.com

?string $name = null
来源：http://ewq.quarkkingdee.top

[U47] PHP：联合类型
来源：http://jjo.tianlin.xyz

int|string $id
来源：http://pec.yueranfly.top

[U48] PHP：纯枚举
来源：http://tfu.aibaodan.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vxd.zhongyouzk.top

[U49] PHP：只读属性
来源：http://fcg.hysaishi.cn

public readonly string $name
来源：http://ypq.havefunace.top

[U50] PHP：构造器属性提升
来源：http://fjc.cucudq.cn

public function __construct(private int $id) {}
来源：http://omb.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://xkd.fengsongda.top

[$a, $b] = $arr;
来源：http://osu.andypj.xyz

[U52] PHP：箭头函数
来源：http://olp.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://lsf.shuidangran.top

[U53] PHP：空合并运算符
来源：http://mht.sweek.top

$v = $a ?? $b ?? "default";
来源：http://xqy.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://mrq.xuanzx.com

$obj?->method()
来源：http://sja.uphjek.com

[U55] PHP：match 表达式
来源：http://thh.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mxn.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://oit.52xcode.cn

f(a: 1, b: 2)
来源：http://wrr.zdqjudy.top

[U57] PHP：字符串插值
来源：http://ete.cdnleiting.top

"值: {$a}"
来源：http://esp.gzhubu.top

[U58] PHP：数组三件套
来源：http://aup.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yas.316326.xyz

[U59] PHP：自定义排序
来源：http://lna.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yas.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://wil.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ton.fehbvm.com

[U61] PHP：正则
来源：http://abj.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ftb.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://cyr.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cxq.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://hwo.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sew.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://xse.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://vly.zhijiandao.cn

[U65] PHP：会话
来源：http://igp.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kbs.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://tfq.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zoa.ivvv.top

[U67] PHP：处理文件上传
来源：http://oza.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://shl.316326.xyz

[U68] PHP：PDO 连接
来源：http://sxb.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://spu.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://wxp.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zke.andypj.xyz

[U70] PHP：PDO 事务
来源：http://taq.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://giz.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://lpj.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://pdh.gotoacloud.top

[U72] PHP：写错误日志
来源：http://jso.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://kho.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://coh.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://dma.sweek.top

[U74] PHP：读取环境变量
来源：http://xog.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://fag.iojbl.cn

[U75] PHP：依赖注入
来源：http://vvu.shanyushiyangkeji.top

composer require psr/container
来源：http://jfs.316326.xyz

[U76] PHP：简单路由
来源：http://pye.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kid.bjfxy.top

[U77] PHP：模板渲染
来源：http://oza.shuidangran.top

composer require twig/twig
来源：http://sjt.kuanghao11.cn

[U78] PHP：单元测试
来源：http://cde.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://rgo.hammf.cn

[U79] PHP：静态分析
来源：http://ujv.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://abf.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://jat.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kjs.hywenlv.cn

[U81] JS：初始化项目
来源：http://tmu.tian-w.cn

npm init -y;  npm i express
来源：http://fdw.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://ive.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pua.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://zsc.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cfm.yonumen.top

[U84] JS：CommonJS 写法
来源：http://hmt.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://zyf.chenlongwang.top

[U85] JS：可选链
来源：http://lkp.jyoumei.cn

a?.b?.c
来源：http://cdc.feifeiyinyue.top

[U86] JS：空值合并
来源：http://bug.c1oappe.top

a ?? b
来源：http://eej.zdqjudy.top

[U87] JS：解构默认值
来源：http://yts.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://kwg.dianchejie.cn

[U88] JS：对象展开合并
来源：http://ifx.ivvv.top

{ ...a, ...b }
来源：http://opv.chenlongwang.top

[U89] JS：数组去重
来源：http://lyp.smart0.xyz

[...new Set(arr)]
来源：http://fke.wangdashe.top

[U90] JS：数字数组排序
来源：http://rsd.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://cru.redwolf501.top

[U91] JS：对象键值遍历
来源：http://yro.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lhl.jinqigufen.top

[U92] JS：深拷贝
来源：http://lnh.bjfxy.top

structuredClone(obj)
来源：http://doq.guowangkeji.top

[U93] JS：模板字符串
来源：http://zzz.nwbrower.top

`共 ${n} 条`
来源：http://ojb.nanxuanxn.top

[U94] JS：箭头函数
来源：http://ssq.zdbjq.cn

const double = x => x * 2;
来源：http://mht.daria6918.cn

[U95] JS：Promise 包装
来源：http://uwe.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://pvs.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://nzq.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qxj.andypj.xyz

[U97] JS：并发请求
来源：http://llx.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qff.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://gmd.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vcx.shangyingyoupin.top

[U99] JS：事件监听
来源：http://sck.epnwcf.com

el.addEventListener("click", e => {})
来源：http://ejn.xinyue.icu

[U100] JS：DOM 查询
来源：http://dii.mhx1999.top

document.querySelector(".item")
来源：http://okk.epnwcf.com

[U101] JS：classList 操作
来源：http://ten.yueranfly.top

el.classList.toggle("active")
来源：http://qic.zhijiandao.cn

[U102] JS：本地存储
来源：http://cix.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kij.zhijiandao.cn

[U103] JS：定时器
来源：http://rhm.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ryw.epnwcf.com

[U104] JS：防抖
来源：http://ipa.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hba.hammf.cn

[U105] JS：节流
来源：http://ebs.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kho.quarkkingdee.top

[U106] JS：日期格式化
来源：http://aoj.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mxm.yueranfly.top

[U107] JS：数字千分位
来源：http://oaw.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ako.9152youxi.cn

[U108] JS：随机整数
来源：http://zcn.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ine.tianlin.xyz

[U109] JS：数组分组
来源：http://hnj.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://ukz.jqgfzy.top

[U110] JS：数组分块
来源：http://pha.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjg.hesvh.cn

[U111] JS：对象转 Map
来源：http://nyd.aibaodan.cn

new Map(Object.entries(obj))
来源：http://xtw.cheryme.top

[U112] JS：字符串补位
来源：http://ifr.jiagoushi.top

"7".padStart(3, "0")
来源：http://knd.havefunace.top

[U113] JS：正则替换全部
来源：http://itd.zycfv.cn

s.replaceAll("a", "b")
来源：http://cgg.tarul.cn

[U114] JS：JSON 深比较
来源：http://crz.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pcx.shzxlz.cn

[U115] JS：生成 UUID
来源：http://ngo.dianchejie.cn

crypto.randomUUID()
来源：http://kdv.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://zxy.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://ioj.xuanzx.com

[U117] JS：单元测试
来源：http://sfy.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://zbv.gzhubu.top

[U118] JS：开发服务器
来源：http://evb.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://vkd.yangfankeji.com

[U119] JS：生产构建
来源：http://ubt.xingfuxueyuan.xyz

npx vite build
来源：http://eji.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://aeh.316326.xyz

import.meta.env.VITE_API_URL
来源：http://skq.jinqigfzy.top

================================================================================
来源：http://bcj.xingfuxueyuan.xyz

统计汇总
来源：http://znt.mhx1999.top

================================================================================
来源：http://bgm.tanke756.top

按语言统计（条）：
来源：http://lrr.jinghuilouyu.cn

Python ......... 252
来源：http://qkf.0kj1m.cn

PHP ............ 252
来源：http://vos.fktsv.cn

JavaScript ..... 252
来源：http://kik.ehwqpu.com

TypeScript ..... 212
来源：http://pxg.zhongyouzk.top

Java ........... 212
来源：http://cfp.svipenyu.cn

Go ............. 212
来源：http://zbo.nanxinkj.top

Ruby ........... 212
来源：http://uoy.sysykeji.top

C# ............. 212
来源：http://rsd.daxiang520.top

C .............. 30
来源：http://kob.wangshuangyany.cn

C++ ............ 30
来源：http://pij.ywan-chungtsiang.top

SQL ............ 90
来源：http://foe.feifeiyinyue.top

Bash ........... 80
来源：http://vrg.yvedp.cn

Kotlin ......... 15
来源：http://izx.hfpthk.cn

Swift .......... 15
来源：http://zdj.zhixingplan.top

Lua ............ 10
来源：http://cqz.ivvv.top

Perl ........... 10
来源：http://spc.jinqigfzy.top

Scala .......... 10
来源：http://wxm.cdnleiting.top

------------------------------------
来源：http://dhp.iojbl.cn

合计 ........... 2106 条
来源：http://tlp.quarkkingdee.top

按章节统计：
来源：http://zzm.shuidangran.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://odd.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://run.chenlongwang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pvf.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zve.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jeh.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hka.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iph.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qxi.hesvh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://srs.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://czm.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kbv.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fvg.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gza.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xza.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jxu.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bym.ydjk.org.cn

Q SQL 专题                              90
来源：http://hih.gotoacloud.top

R Bash 专题                             80
来源：http://fcm.zhongyouzk.top

S C / C++ 专题                          60
来源：http://eux.pycfn.com

T 其他语言补充                          60
来源：http://fdy.zhijiandao.cn

U 高频实用片段                         120
来源：http://nth.yfazqb.com

------------------------------------
来源：http://yic.jiagoushi.top

合计                                  2106 条
来源：http://end.tarul.cn

--------------------------------------------------------------------------------
来源：http://lls.yvedp.cn

使用提醒
来源：http://kcs.yongpay.top

--------------------------------------------------------------------------------
来源：http://rqe.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sjo.jlsjyb.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dqt.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yhj.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://isn.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mzl.aibaodan.cn

—— 文件结束 ——
来源：http://urn.tian-w.cn

================================================================================
来源：http://xiz.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://esp.fehbvm.com

Common Programming Examples Cheat Book
来源：http://mox.chenlongwang.top

================================================================================
来源：http://apl.yongpay.top

【收录内容】
来源：http://jjh.hnqzz.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://quw.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dow.316326.xyz

SQL · Bash · C · C++
来源：http://sxq.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fac.yonumen.top

【使用说明】
来源：http://pui.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vot.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wyj.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gid.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lpt.hnqzz.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fuf.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wsc.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cyf.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wkb.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hor.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tot.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vcd.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jco.tanke756.top

【文件统计】
来源：http://vna.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yju.yj20258.top

--------------------------------------------------------------------------------
来源：http://xhz.daria6918.cn

目  录
来源：http://ipv.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://urb.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yee.pycfn.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pta.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hdu.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nqo.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tis.smart0.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ivm.xziqi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tny.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qwi.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zqw.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cvq.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bcy.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rck.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aoh.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lkv.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pgf.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fii.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://acm.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xef.fanxiaobao.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fwf.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nsv.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://euq.jinqigufen.top

================================================================================
来源：http://rpj.havefunace.top

A. 基础语法与类型
来源：http://xav.hongshengwenyu.top

================================================================================
来源：http://byn.tianlin.xyz

[A01] Hello World
来源：http://xpz.jinqigufen.top

Py:   print("Hello, World!")
来源：http://idl.tanke756.top

PHP:  echo "Hello, World!";
来源：http://gtn.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://mka.cashguo.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://amw.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://syk.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://qbj.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://hem.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nkb.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://aox.yvedp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ykj.316326.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://mrx.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://ioe.daria6918.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uoe.redwolf501.top

Java: String name = "Alex"; int age = 20;
来源：http://bqp.fktsv.cn

Go:   name := "Alex"; age := 20
来源：http://vqb.daxiang520.top

Ruby: name = "Alex"; age = 20
来源：http://ewo.zhongyouzk.top

C#:   string name = "Alex"; int age = 20;
来源：http://fed.vehdjk.com

[A03] 常量定义
来源：http://ifr.jinghuilouyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xxp.tian-w.cn

PHP:  const PI = 3.14159;
来源：http://zcp.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://zgr.snrcjt.cn

TS:   const PI: number = 3.14159;
来源：http://pep.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://vfw.ivvv.top

Go:   const PI = 3.14159
来源：http://rwc.pengpengdd.cyou


<!-- 参考信息 -->