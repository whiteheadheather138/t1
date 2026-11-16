代发 wailian999

[U35] Py：发送邮件
来源：http://zkn.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sli.shangyingyoupin.top

[U36] Py：定时任务
来源：http://qhd.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://cja.xziqi.cn

[U37] Py：读写 Excel
来源：http://qzx.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://xad.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://vyg.cqqwz.cn

Path(__file__).resolve().parent
来源：http://cbf.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://bwb.jqgfzy.top

sys.stdout.isatty()
来源：http://ldm.yueranfly.top

[U40] Py：打印到标准错误
来源：http://ilj.ybcxt.top

print("err", file=sys.stderr)
来源：http://gqp.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://ozo.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://fhl.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://fop.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bsa.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://agf.chenjidiqi.icu

namespace App\Http;
来源：http://bcl.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://ifu.yfazqb.com

declare(strict_types=1);
来源：http://vuu.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://stl.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mse.dianchejie.cn

[U46] PHP：可空类型
来源：http://dov.xziqi.cn

?string $name = null
来源：http://ujq.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://qcf.feifeiyinyue.top

int|string $id
来源：http://zgc.hesvh.cn

[U48] PHP：纯枚举
来源：http://cnn.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cdn.wangdashe.top

[U49] PHP：只读属性
来源：http://ghx.haohaochexian.top

public readonly string $name
来源：http://tie.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://nsw.gzhubu.top

public function __construct(private int $id) {}
来源：http://znx.ybcxt.top

[U51] PHP：数组解构
来源：http://wfn.dianchejie.cn

[$a, $b] = $arr;
来源：http://oxd.iojbl.cn

[U52] PHP：箭头函数
来源：http://jom.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://hlv.cucudq.cn

[U53] PHP：空合并运算符
来源：http://yru.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://snb.cheryme.top

[U54] PHP：空安全调用
来源：http://lxb.aibaodan.cn

$obj?->method()
来源：http://pmn.havefunace.top

[U55] PHP：match 表达式
来源：http://qzg.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rub.quarkkingdee.top

[U56] PHP：命名参数
来源：http://err.sweek.top

f(a: 1, b: 2)
来源：http://dmj.fktsv.cn

[U57] PHP：字符串插值
来源：http://svt.guannengcc.top

"值: {$a}"
来源：http://zfa.yj20258.top

[U58] PHP：数组三件套
来源：http://dpj.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nik.fzhhl.top

[U59] PHP：自定义排序
来源：http://sdb.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gyf.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://jkk.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gbl.svipenyu.cn

[U61] PHP：正则
来源：http://syj.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wml.smart0.xyz

[U62] PHP：日期对象
来源：http://gfi.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bwp.uphjek.com

[U63] PHP：文件读写
来源：http://jjf.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://umb.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://xfz.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://qiq.haohaochexian.top

[U65] PHP：会话
来源：http://bum.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ifu.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://hpf.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vsn.cashguo.top

[U67] PHP：处理文件上传
来源：http://frj.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tpq.tarul.cn

[U68] PHP：PDO 连接
来源：http://wak.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://htk.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://vrq.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bdm.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://wod.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rhw.xylfe.cn

[U71] PHP：抛出异常
来源：http://rzp.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://ywk.daxiang520.top

[U72] PHP：写错误日志
来源：http://vds.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://rvj.svipenyu.cn

[U73] PHP：读取 ini 配置
来源：http://pks.meibo888.top

parse_ini_file("config.ini", true)
来源：http://ita.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://dpi.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://txz.shuidangran.top

[U75] PHP：依赖注入
来源：http://reg.fzhhl.top

composer require psr/container
来源：http://lux.daria6918.cn

[U76] PHP：简单路由
来源：http://ipn.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gtt.guowangkeji.top

[U77] PHP：模板渲染
来源：http://tqd.jinghuilouyu.cn

composer require twig/twig
来源：http://qmi.dianchejie.cn

[U78] PHP：单元测试
来源：http://yeu.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://vfi.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://dih.cheryme.top

composer require --dev phpstan/phpstan
来源：http://hfz.gaohongyu789.top

[U80] PHP：代码规范修复
来源：http://oou.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nnl.sufxvd.cn

[U81] JS：初始化项目
来源：http://rvr.yj20258888.top

npm init -y;  npm i express
来源：http://zsj.bbcook.cn

[U82] JS：package.json 脚本
来源：http://mxx.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pue.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://orx.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bvs.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://vts.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://aoc.yfazqb.com

[U85] JS：可选链
来源：http://nys.shzxlz.cn

a?.b?.c
来源：http://cub.sysykeji.top

[U86] JS：空值合并
来源：http://ppt.fanxiaobao.xyz

a ?? b
来源：http://yle.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://ewl.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://xtj.fehbvm.com

[U88] JS：对象展开合并
来源：http://pls.havefunace.top

{ ...a, ...b }
来源：http://wwa.jinqigfzy.top

[U89] JS：数组去重
来源：http://ebq.jiagoushi.top

[...new Set(arr)]
来源：http://ytr.meibo888.top

[U90] JS：数字数组排序
来源：http://jwe.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://sqs.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://vvc.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxd.cqqwz.cn

[U92] JS：深拷贝
来源：http://owk.feifeiyinyue.top

structuredClone(obj)
来源：http://qoe.jlsjyb.cn

[U93] JS：模板字符串
来源：http://xkd.fengsongda.top

`共 ${n} 条`
来源：http://ccf.dashuyun.cn

[U94] JS：箭头函数
来源：http://dtj.yonumen.top

const double = x => x * 2;
来源：http://mnz.ydzc1.top

[U95] JS：Promise 包装
来源：http://qsk.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://jsg.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://kih.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mbp.xziqi.cn

[U97] JS：并发请求
来源：http://ugz.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uia.gogol.net.cn

[U98] JS：fetch 带 JSON
来源：http://jaa.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oqw.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://roh.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://hnm.9152youxi.cn

[U100] JS：DOM 查询
来源：http://kni.xylfe.cn

document.querySelector(".item")
来源：http://gfb.andypj.xyz

[U101] JS：classList 操作
来源：http://uwv.epnwcf.com

el.classList.toggle("active")
来源：http://gcq.sjlbkw.cn

[U102] JS：本地存储
来源：http://wcw.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hlh.316326.xyz

[U103] JS：定时器
来源：http://uck.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://idf.jqgfzy.top

[U104] JS：防抖
来源：http://gqm.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://neg.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://wkq.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tnn.mhx1999.top

[U106] JS：日期格式化
来源：http://mvn.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yfo.daria6918.cn

[U107] JS：数字千分位
来源：http://dez.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vlw.chenlongwang.top

[U108] JS：随机整数
来源：http://zae.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sad.zhijiandao.cn

[U109] JS：数组分组
来源：http://xro.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://sxq.birdmap.top

[U110] JS：数组分块
来源：http://jpk.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://clf.hfpthk.cn

[U111] JS：对象转 Map
来源：http://ioh.shanyushiyangtech.top

new Map(Object.entries(obj))
来源：http://bxe.gzhubu.top

[U112] JS：字符串补位
来源：http://pcm.xinyue.icu

"7".padStart(3, "0")
来源：http://cem.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://juc.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://sfe.epnwcf.com

[U114] JS：JSON 深比较
来源：http://coc.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tnu.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://rgz.yuanzhike.top

crypto.randomUUID()
来源：http://gmb.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ike.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://ftw.jyoumei.cn

[U117] JS：单元测试
来源：http://xei.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://jzm.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://nac.ctjpmb.com

npm i -D vite;  npx vite
来源：http://gop.zdqjudy.top

[U119] JS：生产构建
来源：http://rkz.ppjwa.cn

npx vite build
来源：http://tod.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://iyg.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://nhy.zhoulong.xyz

================================================================================
来源：http://unm.hesvh.cn

统计汇总
来源：http://zva.aizwys.cn

================================================================================
来源：http://uhm.yj202588.top

按语言统计（条）：
来源：http://ndp.pengpengdd.cyou

Python ......... 252
来源：http://awa.ppjwa.cn

PHP ............ 252
来源：http://qsy.hysaishi.cn

JavaScript ..... 252
来源：http://ahj.zhiwuduotai.top

TypeScript ..... 212
来源：http://mcz.tanke756.top

Java ........... 212
来源：http://zpe.hcnkem.com

Go ............. 212
来源：http://gaj.gogol.net.cn

Ruby ........... 212
来源：http://gcy.yuxming.cn

C# ............. 212
来源：http://lwk.hfpthk.cn

C .............. 30
来源：http://uhg.yueranfly.top

C++ ............ 30
来源：http://wgk.yj20258.top

SQL ............ 90
来源：http://lbk.hammf.cn

Bash ........... 80
来源：http://ciy.chenjidiqi.icu

Kotlin ......... 15
来源：http://xef.yuxming.cn

Swift .......... 15
来源：http://toe.havefunace.top

Lua ............ 10
来源：http://luw.hywenlv.cn

Perl ........... 10
来源：http://wcj.fengsongda.top

Scala .......... 10
来源：http://imf.xylfe.cn

------------------------------------
来源：http://kjy.yueranfly.top

合计 ........... 2106 条
来源：http://pqt.cucudq.cn

按章节统计：
来源：http://oed.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kuq.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jte.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yax.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yle.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dpg.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jej.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ycb.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gpu.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fjb.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uld.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://klm.redwolf501.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tzt.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://skx.nwbrower.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ghz.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fvo.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lqr.yfazqb.com

Q SQL 专题                              90
来源：http://euu.wangshuangyany.cn

R Bash 专题                             80
来源：http://gtw.c1oappe.top

S C / C++ 专题                          60
来源：http://nvk.ppjwa.cn

T 其他语言补充                          60
来源：http://loh.hfpthk.cn

U 高频实用片段                         120
来源：http://zvf.pengpengdd.cyou

------------------------------------
来源：http://cfe.hongshengwenyu.top

合计                                  2106 条
来源：http://jeu.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://onq.nanxuanxn.top

使用提醒
来源：http://uyi.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://wkb.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jeh.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ven.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jmk.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://aaa.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wjq.shuidangran.top

—— 文件结束 ——
来源：http://hfm.tian-w.cn

================================================================================
来源：http://lve.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://lbr.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://lif.birdmap.top

================================================================================
来源：http://zdb.tian-w.cn

【收录内容】
来源：http://lha.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://qgr.hammf.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://opi.tian-w.cn

SQL · Bash · C · C++
来源：http://nxl.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tvz.yonumen.top

【使用说明】
来源：http://jui.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://paf.jyoumei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zsg.xuetiantiany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fik.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yyw.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ald.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qve.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ycr.zhongyouzk.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://syq.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zev.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://exy.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ghg.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xbl.xziqi.cn

【文件统计】
来源：http://rea.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://svq.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://kcn.hfpthk.cn

目  录
来源：http://kbc.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://rkz.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zfr.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://roq.gotoacloud.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uas.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nby.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gkh.sjlbkw.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iwl.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bpr.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qsb.ivvv.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://orp.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uld.c1oappe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qkv.fengsongda.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tcm.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jfs.wangshuangyany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ftp.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cmw.cheryme.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://juz.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lpn.uphjek.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://aks.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cxm.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ciz.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vzk.tarul.cn

================================================================================
来源：http://aza.zhijiandao.cn

A. 基础语法与类型
来源：http://bpm.zdqjudy.top

================================================================================
来源：http://onb.yuxming.cn

[A01] Hello World
来源：http://vtf.hysaishi.cn

Py:   print("Hello, World!")
来源：http://ipz.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://sjc.cashguo.top

JS:   console.log("Hello, World!");
来源：http://zcj.xylfe.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hju.shzxlz.cn

Java: System.out.println("Hello, World!");
来源：http://kdg.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://utv.xinyue.icu

Ruby: puts "Hello, World!"
来源：http://wxc.daxiang520.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xrd.fzhhl.top

[A02] 变量声明与赋值
来源：http://jdu.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hnl.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://iet.xylfe.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nda.yj202588.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://azc.cdnleiting.top

Java: String name = "Alex"; int age = 20;
来源：http://ncc.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://qbk.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://gqu.havefunace.top

C#:   string name = "Alex"; int age = 20;
来源：http://exl.redwolf501.top

[A03] 常量定义
来源：http://agj.yj202588.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://suy.ehwqpu.com

PHP:  const PI = 3.14159;
来源：http://gqa.tanke756.top


<!-- 参考信息 -->