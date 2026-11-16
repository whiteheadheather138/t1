代发 wailian999

[U35] Py：发送邮件
来源：http://fdo.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ceb.xylfe.cn

[U36] Py：定时任务
来源：http://eye.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://her.hfpthk.cn

[U37] Py：读写 Excel
来源：http://pvf.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://yfz.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://nur.yuanzhike.top

Path(__file__).resolve().parent
来源：http://pnx.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://bfg.vqdsnc.cn

sys.stdout.isatty()
来源：http://shn.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://kpn.yonumen.top

print("err", file=sys.stderr)
来源：http://luy.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://dad.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://skw.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://nhz.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://irh.c1oappe.top

[U43] PHP：声明命名空间
来源：http://mag.zhijiandao.cn

namespace App\Http;
来源：http://tiw.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://aws.zhoulong.xyz

declare(strict_types=1);
来源：http://saq.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://zsb.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nhy.chenlongwang.top

[U46] PHP：可空类型
来源：http://jta.yj202588.top

?string $name = null
来源：http://pdr.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://jxe.vqdsnc.cn

int|string $id
来源：http://otk.xinyue.icu

[U48] PHP：纯枚举
来源：http://ndj.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jqc.vehdjk.com

[U49] PHP：只读属性
来源：http://aav.fehbvm.com

public readonly string $name
来源：http://qts.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://vnx.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://paf.quarkkingdee.top

[U51] PHP：数组解构
来源：http://qji.zhoulong.xyz

[$a, $b] = $arr;
来源：http://nis.9152youxi.cn

[U52] PHP：箭头函数
来源：http://uqt.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://dhf.tanke756.top

[U53] PHP：空合并运算符
来源：http://vbr.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://yoo.fktsv.cn

[U54] PHP：空安全调用
来源：http://rnf.ppjwa.cn

$obj?->method()
来源：http://rda.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://cuy.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yal.0kj1m.cn

[U56] PHP：命名参数
来源：http://pmv.hnqzz.top

f(a: 1, b: 2)
来源：http://ogt.smart0.xyz

[U57] PHP：字符串插值
来源：http://lnt.jianghu66.top

"值: {$a}"
来源：http://xjh.hcnkem.com

[U58] PHP：数组三件套
来源：http://bsh.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xkj.jianghu66.top

[U59] PHP：自定义排序
来源：http://ioc.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zhp.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://zlk.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kfx.nwbrower.top

[U61] PHP：正则
来源：http://flr.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aju.zhijiandao.cn

[U62] PHP：日期对象
来源：http://htf.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rdr.aibaodan.cn

[U63] PHP：文件读写
来源：http://tzx.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pgy.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://ztl.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://lnw.fktsv.cn

[U65] PHP：会话
来源：http://qwz.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kol.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://ccc.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ecy.fktsv.cn

[U67] PHP：处理文件上传
来源：http://rwi.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ekp.yuxming.cn

[U68] PHP：PDO 连接
来源：http://mfk.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rwk.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://qnp.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xpw.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://zgg.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://crm.vehdjk.com

[U71] PHP：抛出异常
来源：http://rso.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://gmn.c1oappe.top

[U72] PHP：写错误日志
来源：http://cnu.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://ywt.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://ugq.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://tlc.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://egg.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://zcr.tian-w.cn

[U75] PHP：依赖注入
来源：http://enw.52xcode.cn

composer require psr/container
来源：http://nrx.cashguo.top

[U76] PHP：简单路由
来源：http://pxx.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ddb.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://zzs.meibo888.top

composer require twig/twig
来源：http://rxd.hesvh.cn

[U78] PHP：单元测试
来源：http://iwg.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://jrj.yonumen.top

[U79] PHP：静态分析
来源：http://cia.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://dhy.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://low.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://viw.xylfe.cn

[U81] JS：初始化项目
来源：http://gtw.iojbl.cn

npm init -y;  npm i express
来源：http://ryu.tanke756.top

[U82] JS：package.json 脚本
来源：http://pgy.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nkd.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://abb.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aaa.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://hnv.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://yer.sxryk.cn

[U85] JS：可选链
来源：http://kcm.kuanghao11.cn

a?.b?.c
来源：http://gvb.meibo888.top

[U86] JS：空值合并
来源：http://gpy.dashuyun.cn

a ?? b
来源：http://zmg.bbcook.cn

[U87] JS：解构默认值
来源：http://xvl.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://cvp.hywenlv.cn

[U88] JS：对象展开合并
来源：http://xyl.0kj1m.cn

{ ...a, ...b }
来源：http://esg.nwbrower.top

[U89] JS：数组去重
来源：http://yna.jianghu66.top

[...new Set(arr)]
来源：http://gjn.cdnleiting.top

[U90] JS：数字数组排序
来源：http://lmf.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://juw.sysykeji.top

[U91] JS：对象键值遍历
来源：http://tci.jqgfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mob.jqgufenzy.top

[U92] JS：深拷贝
来源：http://gvv.cheryme.top

structuredClone(obj)
来源：http://qfh.chenzaomai.com

[U93] JS：模板字符串
来源：http://ibs.chenlongwang.top

`共 ${n} 条`
来源：http://pzv.quarkkingdee.top

[U94] JS：箭头函数
来源：http://vxf.quarkkingdee.top

const double = x => x * 2;
来源：http://kmm.hysaishi.cn

[U95] JS：Promise 包装
来源：http://uim.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://gpb.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://lse.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://swo.cashguo.top

[U97] JS：并发请求
来源：http://zad.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oqt.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://aqg.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vmo.svipenyu.cn

[U99] JS：事件监听
来源：http://yqb.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://azs.tian-w.cn

[U100] JS：DOM 查询
来源：http://oxr.hfpthk.cn

document.querySelector(".item")
来源：http://sfu.yongpay.top

[U101] JS：classList 操作
来源：http://qyp.yueranfly.top

el.classList.toggle("active")
来源：http://oak.yuxming.cn

[U102] JS：本地存储
来源：http://lnh.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dos.meibo888.top

[U103] JS：定时器
来源：http://pla.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jdt.smart0.xyz

[U104] JS：防抖
来源：http://ccx.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhi.jqgfzy.top

[U105] JS：节流
来源：http://rbk.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cme.yj202588.top

[U106] JS：日期格式化
来源：http://zgu.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ruc.dianchejie.cn

[U107] JS：数字千分位
来源：http://kdx.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fmh.xinyue.icu

[U108] JS：随机整数
来源：http://ssq.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mvq.zhongyouzk.top

[U109] JS：数组分组
来源：http://mde.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://erg.epnwcf.com

[U110] JS：数组分块
来源：http://ucl.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://arh.cucudq.cn

[U111] JS：对象转 Map
来源：http://dfh.svipenyu.cn

new Map(Object.entries(obj))
来源：http://vud.hnqzz.top

[U112] JS：字符串补位
来源：http://ckb.havefunace.top

"7".padStart(3, "0")
来源：http://kwx.yuxming.cn

[U113] JS：正则替换全部
来源：http://mga.tian-w.cn

s.replaceAll("a", "b")
来源：http://uyh.epnwcf.com

[U114] JS：JSON 深比较
来源：http://tce.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jew.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://tjt.yfazqb.com

crypto.randomUUID()
来源：http://mgu.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://jem.xuanzx.com

/** @param {string} name */ function f(name) {}
来源：http://htu.snrcjt.cn

[U117] JS：单元测试
来源：http://oxy.haohaochexian.top

npm i -D vitest;  npx vitest
来源：http://yod.yueranfly.top

[U118] JS：开发服务器
来源：http://dji.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://nlz.chenjidiqi.icu

[U119] JS：生产构建
来源：http://daf.epnwcf.com

npx vite build
来源：http://poz.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://ntb.0kj1m.cn

import.meta.env.VITE_API_URL
来源：http://uuo.zhengqikj.top

================================================================================
来源：http://rfg.jqgufenzy.top

统计汇总
来源：http://jiu.ywan-chungtsiang.top

================================================================================
来源：http://vjb.quarkkingdee.top

按语言统计（条）：
来源：http://sno.sweek.top

Python ......... 252
来源：http://jkc.sjlbkw.cn

PHP ............ 252
来源：http://ssv.daxiang520.top

JavaScript ..... 252
来源：http://ite.birdmap.top

TypeScript ..... 212
来源：http://edq.shanyushiyangtech.top

Java ........... 212
来源：http://hjw.shanyushiyangkeji.top

Go ............. 212
来源：http://grx.yuxming.cn

Ruby ........... 212
来源：http://ynx.tanke756.top

C# ............. 212
来源：http://eqb.vqdsnc.cn

C .............. 30
来源：http://npb.chenzaomai.com

C++ ............ 30
来源：http://hdp.yongpay.top

SQL ............ 90
来源：http://ruu.sxryk.cn

Bash ........... 80
来源：http://ggx.ydjk.org.cn

Kotlin ......... 15
来源：http://ysq.hesvh.cn

Swift .......... 15
来源：http://lsy.zhijiandao.cn

Lua ............ 10
来源：http://jup.xuetiantiany.cn

Perl ........... 10
来源：http://vqv.haohaochexian.top

Scala .......... 10
来源：http://plx.tianlin.xyz

------------------------------------
来源：http://nwl.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://fqy.shangyingyoupin.top

按章节统计：
来源：http://stj.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lho.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gim.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ycj.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ono.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ohr.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://imt.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tkl.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lfb.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wpt.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://spa.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aps.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pys.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qwn.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eog.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pon.xziqi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qgj.quarkkingdee.top

Q SQL 专题                              90
来源：http://wda.yonumen.top

R Bash 专题                             80
来源：http://wut.jinyuanbaomall.cn

S C / C++ 专题                          60
来源：http://fdg.yfazqb.com

T 其他语言补充                          60
来源：http://lek.guannengcc.top

U 高频实用片段                         120
来源：http://mqb.feifeiyinyue.top

------------------------------------
来源：http://lhe.nanxinkj.top

合计                                  2106 条
来源：http://zfu.havefunace.top

--------------------------------------------------------------------------------
来源：http://dit.meibo888.top

使用提醒
来源：http://ful.ivvv.top

--------------------------------------------------------------------------------
来源：http://gci.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nfg.yuxming.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qsi.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vwh.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://brx.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://czv.cashguo.top

—— 文件结束 ——
来源：http://god.vqdsnc.cn

================================================================================
来源：http://hjy.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://esz.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://zvf.chenzaomai.com

================================================================================
来源：http://riq.wangshuangyany.cn

【收录内容】
来源：http://isb.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://xyq.cucudq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tww.cucudq.cn

SQL · Bash · C · C++
来源：http://cpp.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kke.iojbl.cn

【使用说明】
来源：http://wwu.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cfc.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sgy.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ywz.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://csy.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dvi.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dcx.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wdb.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rit.bjfxy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yxf.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rud.yongpay.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mqq.guannengcc.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ayt.jiagoushi.top

【文件统计】
来源：http://lxf.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://szs.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://rnl.ehwqpu.com

目  录
来源：http://qfb.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://uuw.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://apc.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://afl.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qbq.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zpr.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nnu.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://veo.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://out.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pin.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jmm.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yjw.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://igk.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mwa.gogol.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vmi.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ooa.hongshengwenyu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wyb.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mhi.kuanghao11.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qno.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://upq.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nho.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mqp.yfazqb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eey.tian-w.cn

================================================================================
来源：http://dvl.gaohongyu789.top

A. 基础语法与类型
来源：http://gdj.nwbrower.top

================================================================================
来源：http://xrp.guowangkeji.top

[A01] Hello World
来源：http://mwi.sweek.top

Py:   print("Hello, World!")
来源：http://ptb.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://cao.kuanghao11.cn

JS:   console.log("Hello, World!");
来源：http://ngg.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rzv.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://lji.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://gov.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://zdd.jinqigufen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://imr.hywenlv.cn

[A02] 变量声明与赋值
来源：http://ruh.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hpw.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tpo.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://adp.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sqd.hnxiangtu.top

Java: String name = "Alex"; int age = 20;
来源：http://zwa.zhoulong.xyz

Go:   name := "Alex"; age := 20
来源：http://swt.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://aew.daxiang520.top

C#:   string name = "Alex"; int age = 20;
来源：http://crs.vqdsnc.cn

[A03] 常量定义
来源：http://ixy.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qvd.316326.xyz

PHP:  const PI = 3.14159;
来源：http://jhp.pycfn.com


<!-- 参考信息 -->