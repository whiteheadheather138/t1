代发 wailian999

[U35] Py：发送邮件
来源：http://vic.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qhj.sysykeji.top

[U36] Py：定时任务
来源：http://axs.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://ycd.cucudq.cn

[U37] Py：读写 Excel
来源：http://irj.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://iof.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://nbb.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://vgu.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://aoi.iojbl.cn

sys.stdout.isatty()
来源：http://vvt.yvedp.cn

[U40] Py：打印到标准错误
来源：http://vne.guowangkeji.top

print("err", file=sys.stderr)
来源：http://ugf.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://ers.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eio.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://xog.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nvf.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://qtl.chenjidiqi.icu

namespace App\Http;
来源：http://hwj.feifeiyinyue.top

[U44] PHP：开启严格类型
来源：http://rmm.xinyue.icu

declare(strict_types=1);
来源：http://cee.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://kam.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ziw.cheryme.top

[U46] PHP：可空类型
来源：http://vly.daxiang520.top

?string $name = null
来源：http://wut.9152youxi.cn

[U47] PHP：联合类型
来源：http://wpm.jinqigfzy.top

int|string $id
来源：http://bro.tianlin.xyz

[U48] PHP：纯枚举
来源：http://fpz.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qta.52xcode.cn

[U49] PHP：只读属性
来源：http://wze.tian-w.cn

public readonly string $name
来源：http://evk.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://sgh.haohaochexian.top

public function __construct(private int $id) {}
来源：http://pzm.cashguo.top

[U51] PHP：数组解构
来源：http://xcc.tarul.cn

[$a, $b] = $arr;
来源：http://mto.bjfxy.top

[U52] PHP：箭头函数
来源：http://oxm.yj202588.top

$double = fn($x) => $x * 2;
来源：http://pud.xinyue.icu

[U53] PHP：空合并运算符
来源：http://eyd.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://ndw.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://ydb.gzhubu.top

$obj?->method()
来源：http://sff.fktsv.cn

[U55] PHP：match 表达式
来源：http://oja.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jix.andypj.xyz

[U56] PHP：命名参数
来源：http://bae.zhixingplan.top

f(a: 1, b: 2)
来源：http://wxu.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://pod.cqqwz.cn

"值: {$a}"
来源：http://ikh.uphjek.com

[U58] PHP：数组三件套
来源：http://fzz.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nhr.yangfankeji.com

[U59] PHP：自定义排序
来源：http://mbp.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://szj.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://czw.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xmf.nanxinkj.top

[U61] PHP：正则
来源：http://oiw.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wtd.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://cvs.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vcp.fengsongda.top

[U63] PHP：文件读写
来源：http://eeo.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ihg.xuanzx.com

[U64] PHP：目录遍历
来源：http://wax.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://aaw.meibo888.top

[U65] PHP：会话
来源：http://oss.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qss.tanke756.top

[U66] PHP：设置 Cookie
来源：http://rzf.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://smb.cucudq.cn

[U67] PHP：处理文件上传
来源：http://qlh.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dvn.yonumen.top

[U68] PHP：PDO 连接
来源：http://xwx.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fbl.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://ibt.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://roo.daria6918.cn

[U70] PHP：PDO 事务
来源：http://yhm.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cyr.tian-w.cn

[U71] PHP：抛出异常
来源：http://hdd.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://xdw.cheryme.top

[U72] PHP：写错误日志
来源：http://okx.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://pwu.chenzaomai.com

[U73] PHP：读取 ini 配置
来源：http://evv.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://jvt.hnqzz.top

[U74] PHP：读取环境变量
来源：http://ivu.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://fde.dashuyun.cn

[U75] PHP：依赖注入
来源：http://oei.shuidangran.top

composer require psr/container
来源：http://yhs.epnwcf.com

[U76] PHP：简单路由
来源：http://zhs.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xhh.jiagoushi.top

[U77] PHP：模板渲染
来源：http://rpu.shzxlz.cn

composer require twig/twig
来源：http://xts.zhixingplan.top

[U78] PHP：单元测试
来源：http://mjf.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://pnd.cucudq.cn

[U79] PHP：静态分析
来源：http://szc.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://fgj.wangdashe.top

[U80] PHP：代码规范修复
来源：http://lul.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yum.jiagoushi.top

[U81] JS：初始化项目
来源：http://cwc.gogol.net.cn

npm init -y;  npm i express
来源：http://vvk.yvedp.cn

[U82] JS：package.json 脚本
来源：http://fed.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tbk.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://kfl.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hix.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://tbg.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://xdm.tanke756.top

[U85] JS：可选链
来源：http://fqj.gaohongyu789.top

a?.b?.c
来源：http://tzs.shuidangran.top

[U86] JS：空值合并
来源：http://gts.hongshengwenyu.top

a ?? b
来源：http://ilx.zhengqikj.top

[U87] JS：解构默认值
来源：http://ell.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://cxs.316326.xyz

[U88] JS：对象展开合并
来源：http://czx.fanxiaobao.xyz

{ ...a, ...b }
来源：http://btz.jinqigfzy.top

[U89] JS：数组去重
来源：http://nqq.jlsjyb.cn

[...new Set(arr)]
来源：http://swn.guowangkeji.top

[U90] JS：数字数组排序
来源：http://sbp.chenjidiqi.icu

[...arr].sort((a, b) => a - b)
来源：http://bov.vehdjk.com

[U91] JS：对象键值遍历
来源：http://gbo.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zfd.yuanzhike.top

[U92] JS：深拷贝
来源：http://mxo.cucudq.cn

structuredClone(obj)
来源：http://nrd.wangdashe.top

[U93] JS：模板字符串
来源：http://ybs.jqgufenzy.top

`共 ${n} 条`
来源：http://nsi.yueranfly.top

[U94] JS：箭头函数
来源：http://dvk.gaohongyu789.top

const double = x => x * 2;
来源：http://pla.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://jtf.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://mla.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://nvn.zdqjudy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ksx.pycfn.com

[U97] JS：并发请求
来源：http://vaz.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zta.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://roh.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ckk.ivvv.top

[U99] JS：事件监听
来源：http://nic.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://zun.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://zjk.chenlongwang.top

document.querySelector(".item")
来源：http://ckc.svipenyu.cn

[U101] JS：classList 操作
来源：http://okm.svipenyu.cn

el.classList.toggle("active")
来源：http://ecn.sysykeji.top

[U102] JS：本地存储
来源：http://qgj.xinyue.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://iii.jqgufenzy.top

[U103] JS：定时器
来源：http://tyn.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ekv.hywenlv.cn

[U104] JS：防抖
来源：http://dxz.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lip.jinqigfzy.top

[U105] JS：节流
来源：http://cks.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hry.316326.xyz

[U106] JS：日期格式化
来源：http://wdd.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gmy.shzxlz.cn

[U107] JS：数字千分位
来源：http://mlw.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jdc.epnwcf.com

[U108] JS：随机整数
来源：http://ktj.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tma.hongshengwenyu.top

[U109] JS：数组分组
来源：http://erf.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://ind.feifeiyinyue.top

[U110] JS：数组分块
来源：http://lax.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://euz.zhixingplan.top

[U111] JS：对象转 Map
来源：http://ypt.yvedp.cn

new Map(Object.entries(obj))
来源：http://cwe.jianghu66.top

[U112] JS：字符串补位
来源：http://sox.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://nsq.52xcode.cn

[U113] JS：正则替换全部
来源：http://khx.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://ufi.xylfe.cn

[U114] JS：JSON 深比较
来源：http://tgk.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vto.cdnleiting.top

[U115] JS：生成 UUID
来源：http://pom.jqgfzy.top

crypto.randomUUID()
来源：http://vpr.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://oio.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://pgz.meibo888.top

[U117] JS：单元测试
来源：http://evw.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://lao.bjfxy.top

[U118] JS：开发服务器
来源：http://adl.daria6918.cn

npm i -D vite;  npx vite
来源：http://hpa.feifeiyinyue.top

[U119] JS：生产构建
来源：http://jsp.andypj.xyz

npx vite build
来源：http://szw.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://wcl.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://tdv.shanyushiyangkeji.top

================================================================================
来源：http://ysw.fehbvm.com

统计汇总
来源：http://zbh.0kj1m.cn

================================================================================
来源：http://xsu.jiagoushi.top

按语言统计（条）：
来源：http://tiv.fehbvm.com

Python ......... 252
来源：http://tnx.hysaishi.cn

PHP ............ 252
来源：http://epw.uphjek.com

JavaScript ..... 252
来源：http://gbj.sjlbkw.cn

TypeScript ..... 212
来源：http://saz.yj202588.top

Java ........... 212
来源：http://fsa.9152youxi.cn

Go ............. 212
来源：http://ced.epnwcf.com

Ruby ........... 212
来源：http://mta.jqgufenzy.top

C# ............. 212
来源：http://qcu.shangyingyoupin.top

C .............. 30
来源：http://iya.ehwqpu.com

C++ ............ 30
来源：http://dcy.zhaomingkeji.xyz

SQL ............ 90
来源：http://zbx.chenjidiqi.icu

Bash ........... 80
来源：http://vuw.sxryk.cn

Kotlin ......... 15
来源：http://yti.feifeiyinyue.top

Swift .......... 15
来源：http://txh.aibaodan.cn

Lua ............ 10
来源：http://eax.sysykeji.top

Perl ........... 10
来源：http://fwz.cheryme.top

Scala .......... 10
来源：http://odg.daxiang520.top

------------------------------------
来源：http://lxh.jyoumei.cn

合计 ........... 2106 条
来源：http://bnn.aibaodan.cn

按章节统计：
来源：http://edx.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yna.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mxx.zhixingplan.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nnm.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kgp.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jhn.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fml.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zrh.hysaishi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fqu.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fnb.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hef.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qul.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pgm.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://asq.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://glp.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yhm.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fmw.aibaodan.cn

Q SQL 专题                              90
来源：http://wmx.hnxiangtu.top

R Bash 专题                             80
来源：http://esr.cdnleiting.top

S C / C++ 专题                          60
来源：http://eut.gogol.net.cn

T 其他语言补充                          60
来源：http://oxm.daxiang520.top

U 高频实用片段                         120
来源：http://efy.jyoumei.cn

------------------------------------
来源：http://lla.yj20258888.top

合计                                  2106 条
来源：http://nyz.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://dio.ydjk.org.cn

使用提醒
来源：http://czj.tarul.cn

--------------------------------------------------------------------------------
来源：http://kym.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zwp.yj20258888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pmp.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://flh.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ioe.ppjwa.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zbi.sxryk.cn

—— 文件结束 ——
来源：http://gtk.jinqigfzy.top

================================================================================
来源：http://dzj.xinyue.icu

程序语言常见例子速查手册（2024 版）
来源：http://ota.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://fxj.zhiwuduotai.top

================================================================================
来源：http://obe.gogol.net.cn

【收录内容】
来源：http://zwb.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mvx.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zli.zhixingplan.top

SQL · Bash · C · C++
来源：http://cfz.pengpengdd.cyou

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uzv.cashguo.top

【使用说明】
来源：http://pxr.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jcp.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fos.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yhi.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dxx.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://sej.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rqx.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hzn.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bii.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pbc.fzhhl.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aaa.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://svf.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wuc.fengsongda.top

【文件统计】
来源：http://vlt.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dsy.xinyue.icu

--------------------------------------------------------------------------------
来源：http://vji.tian-w.cn

目  录
来源：http://jeg.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://gaz.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lwu.andypj.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jtc.yj20258888.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bvs.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cjp.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qif.zhixingplan.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zuw.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ims.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rzu.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kjy.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jzg.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nuu.tianlin.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xmi.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rta.cdnleiting.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wyg.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vlf.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dfv.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pnr.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://woe.hfpthk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uxm.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lnj.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uun.gzhubu.top

================================================================================
来源：http://poy.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://lfx.pycfn.com

================================================================================
来源：http://wuu.fengsongda.top

[A01] Hello World
来源：http://kxh.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://pdw.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://qql.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://hoy.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dvk.hywenlv.cn

Java: System.out.println("Hello, World!");
来源：http://rdd.ywan-chungtsiang.top

Go:   fmt.Println("Hello, World!")
来源：http://hxe.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://hmv.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dcq.gaohongyu789.top

[A02] 变量声明与赋值
来源：http://vne.zhongyouzk.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fjd.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vha.vqdsnc.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vnj.zhaomingkeji.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nhb.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://huo.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://wpa.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://lrp.snrcjt.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tzc.hnxiangtu.top

[A03] 常量定义
来源：http://prz.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://idr.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://krd.ydjk.org.cn


<!-- 参考信息 -->