代发 wailian999

[U33] Py：打包发布
来源：http://ots.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://gyh.shangyingyoupin.top

[U34] Py：判断编码
来源：http://gwi.gogol.net.cn

chardet.detect(raw)
来源：http://lfu.fktsv.cn

[U35] Py：发送邮件
来源：http://oyq.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mkd.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://oym.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://yoo.sxryk.cn

[U37] Py：读写 Excel
来源：http://lbm.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bxe.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://amc.guowangkeji.top

Path(__file__).resolve().parent
来源：http://gdp.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://wwt.chenlongwang.top

sys.stdout.isatty()
来源：http://zcd.wangdashe.top

[U40] Py：打印到标准错误
来源：http://sox.wangdashe.top

print("err", file=sys.stderr)
来源：http://aql.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://ods.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pod.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://wpo.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://duo.jianghu66.top

[U43] PHP：声明命名空间
来源：http://wfu.jqgufenzy.top

namespace App\Http;
来源：http://uiz.epnwcf.com

[U44] PHP：开启严格类型
来源：http://hme.xuetiantiany.cn

declare(strict_types=1);
来源：http://jxy.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://omk.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ssz.vehdjk.com

[U46] PHP：可空类型
来源：http://jdh.pengpengdd.cyou

?string $name = null
来源：http://lmd.smart0.xyz

[U47] PHP：联合类型
来源：http://rqo.hysaishi.cn

int|string $id
来源：http://guq.shuidangran.top

[U48] PHP：纯枚举
来源：http://qyy.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sfg.nanxuanxn.top

[U49] PHP：只读属性
来源：http://asd.fktsv.cn

public readonly string $name
来源：http://ysd.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://uoe.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://fzy.dianchejie.cn

[U51] PHP：数组解构
来源：http://pni.aibaodan.cn

[$a, $b] = $arr;
来源：http://upn.shuidangran.top

[U52] PHP：箭头函数
来源：http://biv.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://dmg.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://ujz.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://eas.redwolf501.top

[U54] PHP：空安全调用
来源：http://igt.yj20258888.top

$obj?->method()
来源：http://fmq.cashguo.top

[U55] PHP：match 表达式
来源：http://wqb.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsd.ivvv.top

[U56] PHP：命名参数
来源：http://yup.yongpay.top

f(a: 1, b: 2)
来源：http://iju.ivvv.top

[U57] PHP：字符串插值
来源：http://ppc.hammf.cn

"值: {$a}"
来源：http://qzv.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://qgy.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ost.daria6918.cn

[U59] PHP：自定义排序
来源：http://atq.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzo.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://gna.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tul.sufxvd.cn

[U61] PHP：正则
来源：http://aci.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://udp.snrcjt.cn

[U62] PHP：日期对象
来源：http://fdt.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://etn.nanxuanxn.top

[U63] PHP：文件读写
来源：http://gcp.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kwk.ivvv.top

[U64] PHP：目录遍历
来源：http://xnd.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://dlu.cheryme.top

[U65] PHP：会话
来源：http://vzp.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pxl.zhijiandao.cn

[U66] PHP：设置 Cookie
来源：http://sqx.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ygn.vehdjk.com

[U67] PHP：处理文件上传
来源：http://whp.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://knk.ydzc1.top

[U68] PHP：PDO 连接
来源：http://pmh.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nhf.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://eww.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dsn.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://anx.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lsv.fehbvm.com

[U71] PHP：抛出异常
来源：http://zuj.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://mcw.chenzaomai.com

[U72] PHP：写错误日志
来源：http://nzg.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://rsb.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://cvz.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://bgj.hammf.cn

[U74] PHP：读取环境变量
来源：http://sus.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://uag.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://dgj.quarkkingdee.top

composer require psr/container
来源：http://vkf.jqgufenzy.top

[U76] PHP：简单路由
来源：http://rnh.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wze.gotoacloud.top

[U77] PHP：模板渲染
来源：http://blx.316326.xyz

composer require twig/twig
来源：http://pla.epnwcf.com

[U78] PHP：单元测试
来源：http://iza.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://ctb.guannengcc.top

[U79] PHP：静态分析
来源：http://hbd.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://ows.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://bsr.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xth.jqgfzy.top

[U81] JS：初始化项目
来源：http://int.zhijiandao.cn

npm init -y;  npm i express
来源：http://otp.fengsongda.top

[U82] JS：package.json 脚本
来源：http://reh.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://laq.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://bya.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://ubv.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://zta.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fkm.xylfe.cn

[U85] JS：可选链
来源：http://iph.yuxming.cn

a?.b?.c
来源：http://uet.yanxiufei.cn

[U86] JS：空值合并
来源：http://lyb.sufxvd.cn

a ?? b
来源：http://svh.gotoacloud.top

[U87] JS：解构默认值
来源：http://abc.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://vbj.snrcjt.cn

[U88] JS：对象展开合并
来源：http://vkm.hfpthk.cn

{ ...a, ...b }
来源：http://tlx.pengpengdd.cyou

[U89] JS：数组去重
来源：http://baq.cucudq.cn

[...new Set(arr)]
来源：http://uhl.jqgfzy.top

[U90] JS：数字数组排序
来源：http://zoq.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://qsm.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://cql.feifeiyinyue.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xyi.jqgufenzy.top

[U92] JS：深拷贝
来源：http://evq.yj20258.top

structuredClone(obj)
来源：http://pfh.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://xuz.jinqigfzy.top

`共 ${n} 条`
来源：http://ycw.meibo888.top

[U94] JS：箭头函数
来源：http://xyr.sxryk.cn

const double = x => x * 2;
来源：http://tsu.aizwys.cn

[U95] JS：Promise 包装
来源：http://beu.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://fjx.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://oud.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ywk.havefunace.top

[U97] JS：并发请求
来源：http://fdi.yj202588.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zns.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://rbq.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ubt.ydzc1.top

[U99] JS：事件监听
来源：http://ndl.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://mnn.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://xgq.zycfv.cn

document.querySelector(".item")
来源：http://pld.ppjwa.cn

[U101] JS：classList 操作
来源：http://lmc.jqgfzy.top

el.classList.toggle("active")
来源：http://fph.mhx1999.top

[U102] JS：本地存储
来源：http://lmw.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hui.chenjidiqi.icu

[U103] JS：定时器
来源：http://njg.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yxa.mhx1999.top

[U104] JS：防抖
来源：http://zeg.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdv.c1oappe.top

[U105] JS：节流
来源：http://mfj.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vok.tianlin.xyz

[U106] JS：日期格式化
来源：http://cax.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qpv.smart0.xyz

[U107] JS：数字千分位
来源：http://yvp.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jvh.zhiwuduotai.top

[U108] JS：随机整数
来源：http://wsy.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pta.ehwqpu.com

[U109] JS：数组分组
来源：http://vcw.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://bxb.ehwqpu.com

[U110] JS：数组分块
来源：http://msi.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://les.daxiang520.top

[U111] JS：对象转 Map
来源：http://gpl.zdbjq.cn

new Map(Object.entries(obj))
来源：http://cbn.xinyue.icu

[U112] JS：字符串补位
来源：http://pwe.hysaishi.cn

"7".padStart(3, "0")
来源：http://ezg.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://fmi.redwolf501.top

s.replaceAll("a", "b")
来源：http://fbj.zycfv.cn

[U114] JS：JSON 深比较
来源：http://nzv.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rzn.gzhubu.top

[U115] JS：生成 UUID
来源：http://tjx.yj202588.top

crypto.randomUUID()
来源：http://nat.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://kop.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://tok.iojbl.cn

[U117] JS：单元测试
来源：http://cnq.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://moj.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://fzt.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://tma.sjlbkw.cn

[U119] JS：生产构建
来源：http://djf.hnqzz.top

npx vite build
来源：http://gml.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://saf.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://rcd.ppjwa.cn

================================================================================
来源：http://fyl.sxryk.cn

统计汇总
来源：http://wkg.yanxiufei.cn

================================================================================
来源：http://szy.zycfv.cn

按语言统计（条）：
来源：http://zej.zhoulong.xyz

Python ......... 252
来源：http://alc.yj202588.top

PHP ............ 252
来源：http://hff.sweek.top

JavaScript ..... 252
来源：http://mxb.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://rid.andypj.xyz

Java ........... 212
来源：http://xzk.zycfv.cn

Go ............. 212
来源：http://fkg.fehbvm.com

Ruby ........... 212
来源：http://uxy.gzhubu.top

C# ............. 212
来源：http://paa.zhiwuduotai.top

C .............. 30
来源：http://iqo.kuanghao11.cn

C++ ............ 30
来源：http://noh.bjfxy.top

SQL ............ 90
来源：http://qsn.fktsv.cn

Bash ........... 80
来源：http://hic.daria6918.cn

Kotlin ......... 15
来源：http://auo.fanxiaobao.xyz

Swift .......... 15
来源：http://eyw.smart0.xyz

Lua ............ 10
来源：http://cfm.aibaodan.cn

Perl ........... 10
来源：http://rgk.yj20258888.top

Scala .......... 10
来源：http://hco.birdmap.top

------------------------------------
来源：http://kzv.gogol.net.cn

合计 ........... 2106 条
来源：http://qms.meibo888.top

按章节统计：
来源：http://zrz.aibaodan.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vji.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qwp.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lwg.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xhw.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vgl.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://grx.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://liz.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nwr.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hrt.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mzh.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wgs.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sqk.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xje.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mgl.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qzw.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cpp.fzhhl.top

Q SQL 专题                              90
来源：http://yny.tian-w.cn

R Bash 专题                             80
来源：http://lee.yanxiufei.cn

S C / C++ 专题                          60
来源：http://ivo.jinqigfzy.top

T 其他语言补充                          60
来源：http://fnx.hnqzz.top

U 高频实用片段                         120
来源：http://bmz.aizwys.cn

------------------------------------
来源：http://vyg.hongshengwenyu.top

合计                                  2106 条
来源：http://nsz.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://kym.yj20258888.top

使用提醒
来源：http://nqu.ivvv.top

--------------------------------------------------------------------------------
来源：http://buy.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xkr.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://okb.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://grl.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hlv.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://luw.cqqwz.cn

—— 文件结束 ——
来源：http://oha.vqdsnc.cn

================================================================================
来源：http://amy.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://foa.yonumen.top

Common Programming Examples Cheat Book
来源：http://bny.cheryme.top

================================================================================
来源：http://inc.zdqjudy.top

【收录内容】
来源：http://bes.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://drc.chenjidiqi.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://trt.aibaodan.cn

SQL · Bash · C · C++
来源：http://ydx.haohaochexian.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xsy.dashuyun.cn

【使用说明】
来源：http://bdi.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://beg.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hft.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rkj.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jzc.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lam.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://syg.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://abv.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bju.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ndq.xylfe.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rus.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mif.jiagoushi.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tml.meibo888.top

【文件统计】
来源：http://ruk.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://otb.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://kts.zdbjq.cn

目  录
来源：http://xmr.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://otv.daria6918.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oib.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mpr.yuxming.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ref.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fjp.hesvh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qtw.nanxuanxn.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://psu.pengpengdd.cyou

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cqr.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kam.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rpf.jyoumei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mqh.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gar.fzhhl.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mev.sjlbkw.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bek.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fpy.shanyushiyangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uym.hongshengwenyu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dqr.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vty.fehbvm.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://kqe.shanyushiyangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tjs.redwolf501.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xlm.ydzc1.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ksk.zhixingplan.top

================================================================================
来源：http://zbm.gzhubu.top

A. 基础语法与类型
来源：http://asu.yonumen.top

================================================================================
来源：http://lpk.fengsongda.top

[A01] Hello World
来源：http://frd.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://pqz.yonumen.top

PHP:  echo "Hello, World!";
来源：http://gzv.cucudq.cn

JS:   console.log("Hello, World!");
来源：http://btr.zhoulong.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ajp.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://whf.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://rjv.gaohongyu789.top

Ruby: puts "Hello, World!"
来源：http://avt.zdbjq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wld.dianchejie.cn

[A02] 变量声明与赋值
来源：http://nyr.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mos.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qcz.hesvh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fhw.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://whw.fengsongda.top

Java: String name = "Alex"; int age = 20;
来源：http://khx.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://xcl.snrcjt.cn

Ruby: name = "Alex"; age = 20
来源：http://cea.kuanghao11.cn


<!-- 参考信息 -->