代发 wailian999

[U33] Py：打包发布
来源：http://qon.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://yux.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://dif.hcnkem.com

chardet.detect(raw)
来源：http://cqz.nwbrower.top

[U35] Py：发送邮件
来源：http://uvn.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://onb.wangdashe.top

[U36] Py：定时任务
来源：http://pux.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://xhb.smart0.xyz

[U37] Py：读写 Excel
来源：http://kiu.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://fey.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://ffz.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://xsv.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://hfr.jinqigufen.top

sys.stdout.isatty()
来源：http://clv.bbcook.cn

[U40] Py：打印到标准错误
来源：http://oeh.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://lkf.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://pqm.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rtg.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://uke.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bhv.mhx1999.top

[U43] PHP：声明命名空间
来源：http://ldv.sysykeji.top

namespace App\Http;
来源：http://wbu.pycfn.com

[U44] PHP：开启严格类型
来源：http://uyn.52xcode.cn

declare(strict_types=1);
来源：http://ime.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://apj.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xtt.tianlin.xyz

[U46] PHP：可空类型
来源：http://ysw.jlsjyb.cn

?string $name = null
来源：http://xhn.xuanzx.com

[U47] PHP：联合类型
来源：http://kwy.cheryme.top

int|string $id
来源：http://hwa.jinqigufen.top

[U48] PHP：纯枚举
来源：http://fyx.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yzr.smart0.xyz

[U49] PHP：只读属性
来源：http://cai.chenjidiqi.icu

public readonly string $name
来源：http://eaa.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://syr.jqgfzy.top

public function __construct(private int $id) {}
来源：http://fpe.fktsv.cn

[U51] PHP：数组解构
来源：http://flr.xinyue.icu

[$a, $b] = $arr;
来源：http://qwv.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://uva.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://zpa.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://kgz.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://cnw.tarul.cn

[U54] PHP：空安全调用
来源：http://kmp.yfazqb.com

$obj?->method()
来源：http://gyg.tian-w.cn

[U55] PHP：match 表达式
来源：http://cdu.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mgr.hysaishi.cn

[U56] PHP：命名参数
来源：http://ccv.jiagoushi.top

f(a: 1, b: 2)
来源：http://nne.nanxinkj.top

[U57] PHP：字符串插值
来源：http://nku.xinyue.icu

"值: {$a}"
来源：http://yvo.nwbrower.top

[U58] PHP：数组三件套
来源：http://nnk.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zkg.guannengcc.top

[U59] PHP：自定义排序
来源：http://tam.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://abj.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://uii.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qaa.zhongyouzk.top

[U61] PHP：正则
来源：http://qku.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ias.birdmap.top

[U62] PHP：日期对象
来源：http://njs.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yho.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://qsl.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ndi.wangdashe.top

[U64] PHP：目录遍历
来源：http://dig.dashuyun.cn

glob("dir/*.php");  scandir("dir");
来源：http://xji.fehbvm.com

[U65] PHP：会话
来源：http://vok.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ssr.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://gwf.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ggh.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://bbv.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mji.bjfxy.top

[U68] PHP：PDO 连接
来源：http://vwa.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gme.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://pya.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wyh.yvedp.cn

[U70] PHP：PDO 事务
来源：http://fep.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fsy.nwbrower.top

[U71] PHP：抛出异常
来源：http://efr.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://fjl.mhx1999.top

[U72] PHP：写错误日志
来源：http://kob.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://paj.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://exn.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://nmy.hesvh.cn

[U74] PHP：读取环境变量
来源：http://sfq.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://ivl.ydzc1.top

[U75] PHP：依赖注入
来源：http://dqe.bjfxy.top

composer require psr/container
来源：http://mvr.zdqjudy.top

[U76] PHP：简单路由
来源：http://diu.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nrf.fktsv.cn

[U77] PHP：模板渲染
来源：http://kpe.ybcxt.top

composer require twig/twig
来源：http://eki.hywenlv.cn

[U78] PHP：单元测试
来源：http://rmu.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://ahv.nwbrower.top

[U79] PHP：静态分析
来源：http://ymc.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://vfw.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://uyb.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bfj.jinqigufen.top

[U81] JS：初始化项目
来源：http://ajr.xylfe.cn

npm init -y;  npm i express
来源：http://tsd.andypj.xyz

[U82] JS：package.json 脚本
来源：http://svw.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mxk.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://lqj.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xee.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://cmo.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://fqd.fktsv.cn

[U85] JS：可选链
来源：http://emo.chenjidiqi.icu

a?.b?.c
来源：http://lkc.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://ujb.cdnleiting.top

a ?? b
来源：http://zdt.havefunace.top

[U87] JS：解构默认值
来源：http://oqp.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://ccy.daxiang520.top

[U88] JS：对象展开合并
来源：http://vny.daxiang520.top

{ ...a, ...b }
来源：http://fke.yuxming.cn

[U89] JS：数组去重
来源：http://jtq.daria6918.cn

[...new Set(arr)]
来源：http://cgn.tanke756.top

[U90] JS：数字数组排序
来源：http://jdx.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://xdr.andypj.xyz

[U91] JS：对象键值遍历
来源：http://mrf.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fcf.zdqjudy.top

[U92] JS：深拷贝
来源：http://lam.xziqi.cn

structuredClone(obj)
来源：http://ffs.ctjpmb.com

[U93] JS：模板字符串
来源：http://mhh.cqqwz.cn

`共 ${n} 条`
来源：http://iuw.cdnleiting.top

[U94] JS：箭头函数
来源：http://oaa.yuanzhike.top

const double = x => x * 2;
来源：http://oxg.hammf.cn

[U95] JS：Promise 包装
来源：http://doy.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://qhl.andypj.xyz

[U96] JS：async/await 与异常
来源：http://xdv.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sxx.yueranfly.top

[U97] JS：并发请求
来源：http://fuk.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://uid.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://bry.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dbg.ctjpmb.com

[U99] JS：事件监听
来源：http://hux.xingfuxueyuan.xyz

el.addEventListener("click", e => {})
来源：http://imq.cqqwz.cn

[U100] JS：DOM 查询
来源：http://tti.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://ctq.hnqzz.top

[U101] JS：classList 操作
来源：http://dtg.jianghu66.top

el.classList.toggle("active")
来源：http://yet.tian-w.cn

[U102] JS：本地存储
来源：http://mlx.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://chz.yongpay.top

[U103] JS：定时器
来源：http://nnb.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ndv.ydzc1.top

[U104] JS：防抖
来源：http://ziv.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qgs.sweek.top

[U105] JS：节流
来源：http://ail.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uim.ydjk.org.cn

[U106] JS：日期格式化
来源：http://ymp.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bcp.haohaochexian.top

[U107] JS：数字千分位
来源：http://jcr.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tli.xuetiantiany.cn

[U108] JS：随机整数
来源：http://qzf.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kkg.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://bsf.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://dez.ybcxt.top

[U110] JS：数组分块
来源：http://roa.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ybr.ctjpmb.com

[U111] JS：对象转 Map
来源：http://ouc.gotoacloud.top

new Map(Object.entries(obj))
来源：http://cvf.daria6918.cn

[U112] JS：字符串补位
来源：http://grc.kuanghao11.cn

"7".padStart(3, "0")
来源：http://zab.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://cng.fktsv.cn

s.replaceAll("a", "b")
来源：http://mhd.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://zrm.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qfz.xuanzx.com

[U115] JS：生成 UUID
来源：http://zxf.ybcxt.top

crypto.randomUUID()
来源：http://ijb.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://myy.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://voc.mhx1999.top

[U117] JS：单元测试
来源：http://fox.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://uoe.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://mbd.jyoumei.cn

npm i -D vite;  npx vite
来源：http://ugk.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://czo.svipenyu.cn

npx vite build
来源：http://klc.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://xsl.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://wsp.quarkkingdee.top

================================================================================
来源：http://uoo.ydzc1.top

统计汇总
来源：http://vlq.pengpengdd.cyou

================================================================================
来源：http://gql.ydzc1.top

按语言统计（条）：
来源：http://cns.ydjk.org.cn

Python ......... 252
来源：http://tac.jianghu66.top

PHP ............ 252
来源：http://dov.xuanzx.com

JavaScript ..... 252
来源：http://xlt.hcnkem.com

TypeScript ..... 212
来源：http://nli.yueranfly.top

Java ........... 212
来源：http://ifz.cashguo.top

Go ............. 212
来源：http://zna.chenzaomai.com

Ruby ........... 212
来源：http://blv.fktsv.cn

C# ............. 212
来源：http://fnq.nanxuanxn.top

C .............. 30
来源：http://jom.jinyuanbaomall.cn

C++ ............ 30
来源：http://oao.zdbjq.cn

SQL ............ 90
来源：http://ozi.hfpthk.cn

Bash ........... 80
来源：http://wqy.0kj1m.cn

Kotlin ......... 15
来源：http://upu.dianchejie.cn

Swift .......... 15
来源：http://qgs.bjfxy.top

Lua ............ 10
来源：http://jzf.sxryk.cn

Perl ........... 10
来源：http://nuf.smart0.xyz

Scala .......... 10
来源：http://kje.jianghu66.top

------------------------------------
来源：http://fyc.tanke756.top

合计 ........... 2106 条
来源：http://gre.tanke756.top

按章节统计：
来源：http://zfi.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qhj.feifeiyinyue.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dqx.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://noy.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xcd.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vts.shanyushiyangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kpe.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lrp.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dqz.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wkc.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jaq.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qod.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wnt.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ryp.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ksb.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://acr.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wcz.andypj.xyz

Q SQL 专题                              90
来源：http://stw.jiagoushi.top

R Bash 专题                             80
来源：http://dyz.fehbvm.com

S C / C++ 专题                          60
来源：http://vho.jlsjyb.cn

T 其他语言补充                          60
来源：http://bnk.yfazqb.com

U 高频实用片段                         120
来源：http://mtt.wangdashe.top

------------------------------------
来源：http://vaq.jiagoushi.top

合计                                  2106 条
来源：http://cab.xinyue.icu

--------------------------------------------------------------------------------
来源：http://xvr.yuxming.cn

使用提醒
来源：http://sqy.fengsongda.top

--------------------------------------------------------------------------------
来源：http://roi.xuetiantiany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xkk.hnxiangtu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vwx.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nov.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://oea.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mop.hfpthk.cn

—— 文件结束 ——
来源：http://yqv.ctjpmb.com

================================================================================
来源：http://qqd.meibo888.top

程序语言常见例子速查手册（2024 版）
来源：http://hgi.yj20258.top

Common Programming Examples Cheat Book
来源：http://tqt.xinyue.icu

================================================================================
来源：http://lnz.yj202588.top

【收录内容】
来源：http://lmd.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://une.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://clp.jqgufenzy.top

SQL · Bash · C · C++
来源：http://ydj.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ptk.tian-w.cn

【使用说明】
来源：http://pgk.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dva.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://obp.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bdh.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ctb.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lpa.sxryk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hiy.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wxa.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ezg.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://smo.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ogp.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jht.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oua.cucudq.cn

【文件统计】
来源：http://emg.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wgs.andypj.xyz

--------------------------------------------------------------------------------
来源：http://fov.chenjidiqi.icu

目  录
来源：http://adf.hcnkem.com

--------------------------------------------------------------------------------
来源：http://nff.sxryk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://urb.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mpv.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qbb.ivvv.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lzm.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zrj.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fid.yj20258888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aox.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cgq.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://muk.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qjt.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gxh.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pnm.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ylh.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dfu.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nnt.vehdjk.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cpe.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gbt.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://ioi.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wwb.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://djs.jqgufenzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://the.xuetiantiany.cn

================================================================================
来源：http://ofq.cucudq.cn

A. 基础语法与类型
来源：http://khn.yuxming.cn

================================================================================
来源：http://jue.yuxming.cn

[A01] Hello World
来源：http://fnc.uphjek.com

Py:   print("Hello, World!")
来源：http://ncx.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://npd.c1oappe.top

JS:   console.log("Hello, World!");
来源：http://ovv.wangshuangyany.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yje.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://tcj.zhiwuduotai.top

Go:   fmt.Println("Hello, World!")
来源：http://goy.hammf.cn

Ruby: puts "Hello, World!"
来源：http://fez.gaohongyu789.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jmj.smart0.xyz

[A02] 变量声明与赋值
来源：http://vsi.ywan-chungtsiang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bvn.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://opf.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://lyp.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jme.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://qzx.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://lck.0kj1m.cn

Ruby: name = "Alex"; age = 20
来源：http://gfb.jiagoushi.top


<!-- 参考信息 -->