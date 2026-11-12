代发 wailian999

[U35] Py：发送邮件
来源：http://qxn.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nqw.xuanzx.com

[U36] Py：定时任务
来源：http://sjz.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://brz.jyoumei.cn

[U37] Py：读写 Excel
来源：http://ezc.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rgy.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://zgk.iojbl.cn

Path(__file__).resolve().parent
来源：http://nhy.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://sar.yonumen.top

sys.stdout.isatty()
来源：http://fpl.zycfv.cn

[U40] Py：打印到标准错误
来源：http://iud.c1oappe.top

print("err", file=sys.stderr)
来源：http://imt.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://kdv.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://php.kuanghao11.cn

[U42] PHP：PSR-4 自动加载
来源：http://fnr.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nlj.vehdjk.com

[U43] PHP：声明命名空间
来源：http://grr.yonumen.top

namespace App\Http;
来源：http://khk.pycfn.com

[U44] PHP：开启严格类型
来源：http://hni.zhijiandao.cn

declare(strict_types=1);
来源：http://exs.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://gvj.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rii.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://chc.zhixingplan.top

?string $name = null
来源：http://yke.zdqjudy.top

[U47] PHP：联合类型
来源：http://wrz.shanyushiyangkeji.top

int|string $id
来源：http://tbf.yongpay.top

[U48] PHP：纯枚举
来源：http://dxl.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uef.ppjwa.cn

[U49] PHP：只读属性
来源：http://dop.guowangkeji.top

public readonly string $name
来源：http://jcb.nanxinkj.top

[U50] PHP：构造器属性提升
来源：http://tfz.xinyue.icu

public function __construct(private int $id) {}
来源：http://rzh.zycfv.cn

[U51] PHP：数组解构
来源：http://auf.chenzaomai.com

[$a, $b] = $arr;
来源：http://uwj.zdqjudy.top

[U52] PHP：箭头函数
来源：http://txd.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://qmx.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://not.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://xzf.fktsv.cn

[U54] PHP：空安全调用
来源：http://tkk.tian-w.cn

$obj?->method()
来源：http://ssg.daria6918.cn

[U55] PHP：match 表达式
来源：http://opp.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vlz.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://ewa.sxryk.cn

f(a: 1, b: 2)
来源：http://pvb.sysykeji.top

[U57] PHP：字符串插值
来源：http://qdw.yangfankeji.com

"值: {$a}"
来源：http://lgt.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://gmd.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://huy.zdbjq.cn

[U59] PHP：自定义排序
来源：http://uab.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hto.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://gjl.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ldw.chenjidiqi.icu

[U61] PHP：正则
来源：http://enk.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hij.daria6918.cn

[U62] PHP：日期对象
来源：http://bim.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xdk.bjfxy.top

[U63] PHP：文件读写
来源：http://mbe.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bpq.hysaishi.cn

[U64] PHP：目录遍历
来源：http://tlm.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://pwo.shangyingyoupin.top

[U65] PHP：会话
来源：http://byn.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xlg.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://gsh.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oii.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://oqy.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://flt.hammf.cn

[U68] PHP：PDO 连接
来源：http://cgc.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xpp.316326.xyz

[U69] PHP：PDO 预处理
来源：http://wju.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://die.smart0.xyz

[U70] PHP：PDO 事务
来源：http://pbp.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bux.haohaochexian.top

[U71] PHP：抛出异常
来源：http://efy.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://dmv.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://lkw.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://smh.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://qkw.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://gwp.meibo888.top

[U74] PHP：读取环境变量
来源：http://svv.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://raz.cheryme.top

[U75] PHP：依赖注入
来源：http://onp.kuanghao11.cn

composer require psr/container
来源：http://urr.hfpthk.cn

[U76] PHP：简单路由
来源：http://jnb.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ydl.meibo888.top

[U77] PHP：模板渲染
来源：http://iai.zhengqikj.top

composer require twig/twig
来源：http://ynn.dashuyun.cn

[U78] PHP：单元测试
来源：http://xqg.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://lel.sufxvd.cn

[U79] PHP：静态分析
来源：http://mco.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://vgh.yongpay.top

[U80] PHP：代码规范修复
来源：http://eqm.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qzr.yvedp.cn

[U81] JS：初始化项目
来源：http://mqo.c1oappe.top

npm init -y;  npm i express
来源：http://ros.aizwys.cn

[U82] JS：package.json 脚本
来源：http://ceo.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://buh.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://pup.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://qaz.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://itw.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://soz.shanyushiyangkeji.top

[U85] JS：可选链
来源：http://ppm.haohaochexian.top

a?.b?.c
来源：http://ujx.smart0.xyz

[U86] JS：空值合并
来源：http://ipz.zdqjudy.top

a ?? b
来源：http://lvn.daxiang520.top

[U87] JS：解构默认值
来源：http://muy.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://dgm.jyoumei.cn

[U88] JS：对象展开合并
来源：http://rln.jqgfzy.top

{ ...a, ...b }
来源：http://abj.jqgfzy.top

[U89] JS：数组去重
来源：http://zjv.yuxming.cn

[...new Set(arr)]
来源：http://nfm.guannengcc.top

[U90] JS：数字数组排序
来源：http://xjx.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://mur.havefunace.top

[U91] JS：对象键值遍历
来源：http://zja.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fxq.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://tru.snrcjt.cn

structuredClone(obj)
来源：http://fel.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://opm.xuanzx.com

`共 ${n} 条`
来源：http://egu.ydjk.org.cn

[U94] JS：箭头函数
来源：http://mnw.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://cxs.yj20258888.top

[U95] JS：Promise 包装
来源：http://dza.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://tda.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://oqj.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eub.zdbjq.cn

[U97] JS：并发请求
来源：http://jjv.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://evq.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://dil.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ues.aizwys.cn

[U99] JS：事件监听
来源：http://zgb.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://usn.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://zjd.gaohongyu789.top

document.querySelector(".item")
来源：http://zgl.ywan-chungtsiang.top

[U101] JS：classList 操作
来源：http://gqn.gzhubu.top

el.classList.toggle("active")
来源：http://zpw.yuxming.cn

[U102] JS：本地存储
来源：http://hxg.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://aax.pycfn.com

[U103] JS：定时器
来源：http://dbx.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xfx.chenlongwang.top

[U104] JS：防抖
来源：http://gil.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhf.bjfxy.top

[U105] JS：节流
来源：http://jnr.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uzp.gogol.net.cn

[U106] JS：日期格式化
来源：http://rid.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://swf.xuanzx.com

[U107] JS：数字千分位
来源：http://oqg.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nlf.shzxlz.cn

[U108] JS：随机整数
来源：http://cpu.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vyw.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://shu.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://nqq.xinyue.icu

[U110] JS：数组分块
来源：http://cvo.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://obd.ybcxt.top

[U111] JS：对象转 Map
来源：http://pgg.guowangkeji.top

new Map(Object.entries(obj))
来源：http://lyx.zdqjudy.top

[U112] JS：字符串补位
来源：http://yzk.jlsjyb.cn

"7".padStart(3, "0")
来源：http://vkk.hesvh.cn

[U113] JS：正则替换全部
来源：http://vmo.ydzc1.top

s.replaceAll("a", "b")
来源：http://efy.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://bgx.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lcv.tian-w.cn

[U115] JS：生成 UUID
来源：http://jie.chenzaomai.com

crypto.randomUUID()
来源：http://nln.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ixf.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://bpj.xziqi.cn

[U117] JS：单元测试
来源：http://xsx.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://gbu.daria6918.cn

[U118] JS：开发服务器
来源：http://rhh.yj20258888.top

npm i -D vite;  npx vite
来源：http://xhq.chenjidiqi.icu

[U119] JS：生产构建
来源：http://cna.vehdjk.com

npx vite build
来源：http://ddt.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://txs.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://ktu.tianlin.xyz

================================================================================
来源：http://fwv.havefunace.top

统计汇总
来源：http://bjb.wangdashe.top

================================================================================
来源：http://rbu.meibo888.top

按语言统计（条）：
来源：http://xdr.smart0.xyz

Python ......... 252
来源：http://fpx.jinqigfzy.top

PHP ............ 252
来源：http://pat.xuanzx.com

JavaScript ..... 252
来源：http://lwo.cdnleiting.top

TypeScript ..... 212
来源：http://gwr.nwbrower.top

Java ........... 212
来源：http://eif.sweek.top

Go ............. 212
来源：http://gzr.jinyuanbaomall.cn

Ruby ........... 212
来源：http://hoi.pycfn.com

C# ............. 212
来源：http://lcd.shuidangran.top

C .............. 30
来源：http://kqd.tanke756.top

C++ ............ 30
来源：http://zbe.shuidangran.top

SQL ............ 90
来源：http://pft.dashuyun.cn

Bash ........... 80
来源：http://dvb.yj202588.top

Kotlin ......... 15
来源：http://dpc.sufxvd.cn

Swift .......... 15
来源：http://vvq.ctjpmb.com

Lua ............ 10
来源：http://ycu.tarul.cn

Perl ........... 10
来源：http://iuq.nwbrower.top

Scala .......... 10
来源：http://vui.jqgufenzy.top

------------------------------------
来源：http://znl.shuidangran.top

合计 ........... 2106 条
来源：http://xlr.yfazqb.com

按章节统计：
来源：http://vhb.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kit.bbcook.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bhi.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hvs.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nky.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ymn.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wfr.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lzu.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tas.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ajc.kuanghao11.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://olg.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xew.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uvd.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bnm.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fuf.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vbf.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vwj.yj202588.top

Q SQL 专题                              90
来源：http://ouu.wangdashe.top

R Bash 专题                             80
来源：http://wus.aibaodan.cn

S C / C++ 专题                          60
来源：http://edn.xinyue.icu

T 其他语言补充                          60
来源：http://fda.jinqigfzy.top

U 高频实用片段                         120
来源：http://bux.svipenyu.cn

------------------------------------
来源：http://lwz.ydzc1.top

合计                                  2106 条
来源：http://tae.gzhubu.top

--------------------------------------------------------------------------------
来源：http://wia.cashguo.top

使用提醒
来源：http://icd.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://odg.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://owe.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bky.wangshuangyany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jvf.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fzz.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kgr.uphjek.com

—— 文件结束 ——
来源：http://yrl.yanxiufei.cn

================================================================================
来源：http://rqm.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://irl.zhixingplan.top

Common Programming Examples Cheat Book
来源：http://ykp.sysykeji.top

================================================================================
来源：http://vyj.sxryk.cn

【收录内容】
来源：http://wdu.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://pcw.fehbvm.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://khk.pycfn.com

SQL · Bash · C · C++
来源：http://bmx.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ezk.fanxiaobao.xyz

【使用说明】
来源：http://vfd.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dmc.pycfn.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cgy.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wjv.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qcu.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://euq.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lha.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bfj.zhengqikj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jlu.zdbjq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://foe.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uum.svipenyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aba.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oys.zdqjudy.top

【文件统计】
来源：http://cfi.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qoe.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://obq.epnwcf.com

目  录
来源：http://jix.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://pzm.daria6918.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tvy.jqgfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dxh.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://piw.52xcode.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rmj.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mtj.fengsongda.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ijk.cashguo.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bfo.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wgu.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hzq.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wuf.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mzy.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xqz.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lin.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://weq.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ljp.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yxf.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lxv.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rke.xuetiantiany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bsl.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mvx.yj202588.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://azm.52xcode.cn

================================================================================
来源：http://phr.shangyingyoupin.top

A. 基础语法与类型
来源：http://ylr.sysykeji.top

================================================================================
来源：http://aar.jyoumei.cn

[A01] Hello World
来源：http://rog.birdmap.top

Py:   print("Hello, World!")
来源：http://whd.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://mxr.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://upk.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kcy.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://ukq.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://dcp.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://ujg.shuidangran.top

C#:   Console.WriteLine("Hello, World!");
来源：http://xvu.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://jum.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cpu.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://frz.smart0.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://lgl.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oma.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://vhx.nwbrower.top

Go:   name := "Alex"; age := 20
来源：http://dte.hysaishi.cn

Ruby: name = "Alex"; age = 20
来源：http://suu.jinghuilouyu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cuy.hesvh.cn

[A03] 常量定义
来源：http://wro.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nph.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://lht.yonumen.top


<!-- 参考信息 -->