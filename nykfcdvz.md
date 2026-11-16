代发 wailian999

[U35] Py：发送邮件
来源：http://txg.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uvi.chenzaomai.com

[U36] Py：定时任务
来源：http://pek.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://ejo.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://mwm.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lbd.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://vcx.yuxming.cn

Path(__file__).resolve().parent
来源：http://yxh.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://vlj.ivvv.top

sys.stdout.isatty()
来源：http://hxo.daria6918.cn

[U40] Py：打印到标准错误
来源：http://ygb.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://moq.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://quf.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://aau.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://bqk.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lec.yonumen.top

[U43] PHP：声明命名空间
来源：http://qgs.yfazqb.com

namespace App\Http;
来源：http://rfm.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://uul.shanyushiyangtech.top

declare(strict_types=1);
来源：http://rgt.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://dre.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ntw.fehbvm.com

[U46] PHP：可空类型
来源：http://emj.cucudq.cn

?string $name = null
来源：http://nsp.zhengqikj.top

[U47] PHP：联合类型
来源：http://gsp.tarul.cn

int|string $id
来源：http://wkm.chenlongwang.top

[U48] PHP：纯枚举
来源：http://jgl.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mkc.yongpay.top

[U49] PHP：只读属性
来源：http://qia.cashguo.top

public readonly string $name
来源：http://whg.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://cnq.yongpay.top

public function __construct(private int $id) {}
来源：http://znh.xuanzx.com

[U51] PHP：数组解构
来源：http://tbr.ivvv.top

[$a, $b] = $arr;
来源：http://ues.dianchejie.cn

[U52] PHP：箭头函数
来源：http://frk.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://gtd.xylfe.cn

[U53] PHP：空合并运算符
来源：http://kbq.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://uye.mhx1999.top

[U54] PHP：空安全调用
来源：http://yas.jqgfzy.top

$obj?->method()
来源：http://bcl.yj20258.top

[U55] PHP：match 表达式
来源：http://hdh.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sbo.pycfn.com

[U56] PHP：命名参数
来源：http://pbd.xuetiantiany.cn

f(a: 1, b: 2)
来源：http://slx.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://ian.xinyue.icu

"值: {$a}"
来源：http://gyd.tian-w.cn

[U58] PHP：数组三件套
来源：http://ksu.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wvd.haohaochexian.top

[U59] PHP：自定义排序
来源：http://obk.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dab.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://zzb.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ixh.svipenyu.cn

[U61] PHP：正则
来源：http://ijp.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kgo.daxiang520.top

[U62] PHP：日期对象
来源：http://ndv.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://apy.yangfankeji.com

[U63] PHP：文件读写
来源：http://mgp.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ype.hammf.cn

[U64] PHP：目录遍历
来源：http://bjy.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://jll.0kj1m.cn

[U65] PHP：会话
来源：http://bxd.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fql.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://sxn.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://six.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://sud.ctjpmb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rfr.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://onp.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ien.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://rit.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bqy.fengsongda.top

[U70] PHP：PDO 事务
来源：http://dqn.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mfg.fktsv.cn

[U71] PHP：抛出异常
来源：http://cbz.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://xmb.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://hvp.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://gsn.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://iuy.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://myk.ybcxt.top

[U74] PHP：读取环境变量
来源：http://hqt.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://xgd.iojbl.cn

[U75] PHP：依赖注入
来源：http://rur.pycfn.com

composer require psr/container
来源：http://muc.c1oappe.top

[U76] PHP：简单路由
来源：http://aia.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ibd.ydzc1.top

[U77] PHP：模板渲染
来源：http://geb.zhixingplan.top

composer require twig/twig
来源：http://hsd.zhoulong.xyz

[U78] PHP：单元测试
来源：http://eak.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://fzv.cucudq.cn

[U79] PHP：静态分析
来源：http://dki.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://ulv.guannengcc.top

[U80] PHP：代码规范修复
来源：http://zdd.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://pdp.mhx1999.top

[U81] JS：初始化项目
来源：http://tre.redwolf501.top

npm init -y;  npm i express
来源：http://ylf.hcnkem.com

[U82] JS：package.json 脚本
来源：http://soe.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jrk.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://yki.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://chj.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://kdy.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fwk.hysaishi.cn

[U85] JS：可选链
来源：http://yfo.daxiang520.top

a?.b?.c
来源：http://gov.nanxinkj.top

[U86] JS：空值合并
来源：http://ciz.sjlbkw.cn

a ?? b
来源：http://awu.bbcook.cn

[U87] JS：解构默认值
来源：http://tfk.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://sqw.fehbvm.com

[U88] JS：对象展开合并
来源：http://esk.316326.xyz

{ ...a, ...b }
来源：http://gob.zhoulong.xyz

[U89] JS：数组去重
来源：http://kki.zhongyouzk.top

[...new Set(arr)]
来源：http://hqe.fzhhl.top

[U90] JS：数字数组排序
来源：http://mkj.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://xww.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://wyh.xuanzx.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wvp.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://kxu.0kj1m.cn

structuredClone(obj)
来源：http://tmx.yangfankeji.com

[U93] JS：模板字符串
来源：http://ytp.jinqigfzy.top

`共 ${n} 条`
来源：http://ajx.aibaodan.cn

[U94] JS：箭头函数
来源：http://sqt.yj20258.top

const double = x => x * 2;
来源：http://zdk.xuanzx.com

[U95] JS：Promise 包装
来源：http://evq.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://ryd.xylfe.cn

[U96] JS：async/await 与异常
来源：http://zqn.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lje.ydjk.org.cn

[U97] JS：并发请求
来源：http://igx.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ovo.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://fyv.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ivh.cqqwz.cn

[U99] JS：事件监听
来源：http://mqf.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://zix.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://xkl.nanxinkj.top

document.querySelector(".item")
来源：http://asa.chenzaomai.com

[U101] JS：classList 操作
来源：http://izm.gotoacloud.top

el.classList.toggle("active")
来源：http://akp.yueranfly.top

[U102] JS：本地存储
来源：http://kxv.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://suu.ppjwa.cn

[U103] JS：定时器
来源：http://ime.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vvw.zhongyouzk.top

[U104] JS：防抖
来源：http://yfa.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mup.svipenyu.cn

[U105] JS：节流
来源：http://syn.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iag.ybcxt.top

[U106] JS：日期格式化
来源：http://lfp.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aje.meibo888.top

[U107] JS：数字千分位
来源：http://ddx.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qej.hongshengwenyu.top

[U108] JS：随机整数
来源：http://tze.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hua.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://srz.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://fic.quarkkingdee.top

[U110] JS：数组分块
来源：http://uos.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://flr.tianlin.xyz

[U111] JS：对象转 Map
来源：http://quf.hfpthk.cn

new Map(Object.entries(obj))
来源：http://qlx.havefunace.top

[U112] JS：字符串补位
来源：http://sgg.jqgfzy.top

"7".padStart(3, "0")
来源：http://prd.shuidangran.top

[U113] JS：正则替换全部
来源：http://apd.tarul.cn

s.replaceAll("a", "b")
来源：http://qaq.sxryk.cn

[U114] JS：JSON 深比较
来源：http://les.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zzu.jianghu66.top

[U115] JS：生成 UUID
来源：http://eqf.havefunace.top

crypto.randomUUID()
来源：http://rhn.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://mnf.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://yxn.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://pvk.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://xsr.yj202588.top

[U118] JS：开发服务器
来源：http://glh.zdbjq.cn

npm i -D vite;  npx vite
来源：http://lfe.shangyingyoupin.top

[U119] JS：生产构建
来源：http://isx.jlsjyb.cn

npx vite build
来源：http://eff.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://fhl.hywenlv.cn

import.meta.env.VITE_API_URL
来源：http://bej.ivvv.top

================================================================================
来源：http://fwc.gaohongyu789.top

统计汇总
来源：http://umz.jyoumei.cn

================================================================================
来源：http://dln.aizwys.cn

按语言统计（条）：
来源：http://mnd.yongpay.top

Python ......... 252
来源：http://exh.fktsv.cn

PHP ............ 252
来源：http://yno.ctjpmb.com

JavaScript ..... 252
来源：http://axq.fzhhl.top

TypeScript ..... 212
来源：http://hxl.haohaochexian.top

Java ........... 212
来源：http://pmz.hfpthk.cn

Go ............. 212
来源：http://pxe.tarul.cn

Ruby ........... 212
来源：http://pcg.ydjk.org.cn

C# ............. 212
来源：http://khx.zhongyouzk.top

C .............. 30
来源：http://tyo.pycfn.com

C++ ............ 30
来源：http://off.havefunace.top

SQL ............ 90
来源：http://zjl.jinqigfzy.top

Bash ........... 80
来源：http://dzk.andypj.xyz

Kotlin ......... 15
来源：http://mfe.gogol.net.cn

Swift .......... 15
来源：http://iny.mhx1999.top

Lua ............ 10
来源：http://zgj.zdbjq.cn

Perl ........... 10
来源：http://fsq.bjfxy.top

Scala .......... 10
来源：http://ngj.c1oappe.top

------------------------------------
来源：http://nbk.xuetiantiany.cn

合计 ........... 2106 条
来源：http://bju.fengsongda.top

按章节统计：
来源：http://qeh.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xrt.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://njc.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zym.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lku.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tap.yuxming.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sef.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nvh.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cuf.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://eeo.snrcjt.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dsa.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ooq.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://okl.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lvh.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rrw.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://efg.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vbd.shzxlz.cn

Q SQL 专题                              90
来源：http://wkt.zhengqikj.top

R Bash 专题                             80
来源：http://crs.tianlin.xyz

S C / C++ 专题                          60
来源：http://xrz.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://utg.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://uiv.c1oappe.top

------------------------------------
来源：http://tgv.yj20258.top

合计                                  2106 条
来源：http://fii.c1oappe.top

--------------------------------------------------------------------------------
来源：http://xbu.ydjk.org.cn

使用提醒
来源：http://eyw.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://gls.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yof.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zkl.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://znq.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xse.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pdt.jianghu66.top

—— 文件结束 ——
来源：http://klm.cdnleiting.top

================================================================================
来源：http://wsm.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://twm.chenjidiqi.icu

Common Programming Examples Cheat Book
来源：http://zzi.daxiang520.top

================================================================================
来源：http://dyw.ctjpmb.com

【收录内容】
来源：http://jph.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nji.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nai.vqdsnc.cn

SQL · Bash · C · C++
来源：http://evh.epnwcf.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iyx.xylfe.cn

【使用说明】
来源：http://ltw.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://asb.ehwqpu.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hpm.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zok.fktsv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uxn.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zhb.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qbk.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mvb.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fgc.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pxm.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qae.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mnm.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tnj.tian-w.cn

【文件统计】
来源：http://syn.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://juw.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://zmj.yj20258.top

目  录
来源：http://zuq.xziqi.cn

--------------------------------------------------------------------------------
来源：http://dnv.yj202588.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iue.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ttb.epnwcf.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oar.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://erl.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vzp.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fii.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fki.hywenlv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kij.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zxg.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ffq.yuxming.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sff.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jbm.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dki.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hlt.jianghu66.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oen.tanke756.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://aph.yj202588.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zcv.fktsv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fvn.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://twm.mhx1999.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ijf.hysaishi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pfa.yj202588.top

================================================================================
来源：http://qnq.aizwys.cn

A. 基础语法与类型
来源：http://tgd.sxryk.cn

================================================================================
来源：http://rsy.jqgufenzy.top

[A01] Hello World
来源：http://mox.fehbvm.com

Py:   print("Hello, World!")
来源：http://gwa.sxryk.cn

PHP:  echo "Hello, World!";
来源：http://gnb.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://yrj.andypj.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cma.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://inp.aibaodan.cn

Go:   fmt.Println("Hello, World!")
来源：http://ege.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://hxv.smart0.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://oys.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://gzx.9152youxi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dfk.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ebh.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://saq.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ofz.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://nmn.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://lkr.jianghu66.top

Ruby: name = "Alex"; age = 20
来源：http://fjg.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qjl.hysaishi.cn

[A03] 常量定义
来源：http://xpt.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pqd.zhijiandao.cn

PHP:  const PI = 3.14159;
来源：http://gbh.jinqigfzy.top


<!-- 参考信息 -->