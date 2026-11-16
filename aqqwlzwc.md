代发 wailian999

[U27] Py：异步 HTTP
来源：http://ufq.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://exl.gogol.net.cn

[U28] Py：类型别名
来源：http://yuu.sufxvd.cn

UserId = int
来源：http://vmd.xylfe.cn

[U29] Py：属性校验
来源：http://qfp.sxryk.cn

@property 与 @x.setter 配合
来源：http://cin.zdbjq.cn

[U30] Py：数据类
来源：http://gsi.chenzaomai.com

@dataclass(slots=True)
来源：http://xpn.zhengqikj.top

[U31] Py：单测
来源：http://zik.bjfxy.top

python -m pytest -q
来源：http://fdn.shuidangran.top

[U32] Py：代码格式化
来源：http://pci.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://aaq.cqqwz.cn

[U33] Py：打包发布
来源：http://ifr.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://psh.yangfankeji.com

[U34] Py：判断编码
来源：http://tha.ydjk.org.cn

chardet.detect(raw)
来源：http://por.yongpay.top

[U35] Py：发送邮件
来源：http://lnn.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ivy.nanxinkj.top

[U36] Py：定时任务
来源：http://qyj.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://iey.yangfankeji.com

[U37] Py：读写 Excel
来源：http://zys.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tii.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://duc.hesvh.cn

Path(__file__).resolve().parent
来源：http://dtc.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://uss.wangdashe.top

sys.stdout.isatty()
来源：http://biu.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://hjr.yonumen.top

print("err", file=sys.stderr)
来源：http://psu.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://jte.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uwa.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://ozf.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fhc.cashguo.top

[U43] PHP：声明命名空间
来源：http://fub.yj20258.top

namespace App\Http;
来源：http://oqd.yj20258888.top

[U44] PHP：开启严格类型
来源：http://adq.ybcxt.top

declare(strict_types=1);
来源：http://myf.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://hem.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zyr.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://yjs.pengpengdd.cyou

?string $name = null
来源：http://zqc.pycfn.com

[U47] PHP：联合类型
来源：http://xnr.sufxvd.cn

int|string $id
来源：http://fyc.ehwqpu.com

[U48] PHP：纯枚举
来源：http://fyx.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ckh.yuxming.cn

[U49] PHP：只读属性
来源：http://pud.ppjwa.cn

public readonly string $name
来源：http://eha.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://che.tarul.cn

public function __construct(private int $id) {}
来源：http://ojb.gaohongyu789.top

[U51] PHP：数组解构
来源：http://evl.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://xoo.havefunace.top

[U52] PHP：箭头函数
来源：http://ggl.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://cgi.uphjek.com

[U53] PHP：空合并运算符
来源：http://dpr.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://pps.xuanzx.com

[U54] PHP：空安全调用
来源：http://erp.bjfxy.top

$obj?->method()
来源：http://okh.sweek.top

[U55] PHP：match 表达式
来源：http://xgm.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://efd.tian-w.cn

[U56] PHP：命名参数
来源：http://tjp.yuxming.cn

f(a: 1, b: 2)
来源：http://kbp.nanxuanxn.top

[U57] PHP：字符串插值
来源：http://ahf.andypj.xyz

"值: {$a}"
来源：http://iky.zdbjq.cn

[U58] PHP：数组三件套
来源：http://rcx.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ytq.fengsongda.top

[U59] PHP：自定义排序
来源：http://tpq.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqf.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://mbp.tarul.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vsk.hfpthk.cn

[U61] PHP：正则
来源：http://ibo.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hrl.uphjek.com

[U62] PHP：日期对象
来源：http://ftd.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qgv.gotoacloud.top

[U63] PHP：文件读写
来源：http://mst.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qmk.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://cmw.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://vcb.pycfn.com

[U65] PHP：会话
来源：http://vsj.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://maz.uphjek.com

[U66] PHP：设置 Cookie
来源：http://qyc.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jzk.mhx1999.top

[U67] PHP：处理文件上传
来源：http://wvd.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mlt.fzhhl.top

[U68] PHP：PDO 连接
来源：http://wga.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://veu.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://zcj.yongpay.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zac.yongpay.top

[U70] PHP：PDO 事务
来源：http://xbn.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vwq.yonumen.top

[U71] PHP：抛出异常
来源：http://niw.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://ysi.haohaochexian.top

[U72] PHP：写错误日志
来源：http://djt.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://vmb.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://jnw.yj20258.top

parse_ini_file("config.ini", true)
来源：http://syo.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://hoh.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://baj.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://hzp.haohaochexian.top

composer require psr/container
来源：http://qup.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://ysg.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xbp.birdmap.top

[U77] PHP：模板渲染
来源：http://dqh.jqgfzy.top

composer require twig/twig
来源：http://vnj.pycfn.com

[U78] PHP：单元测试
来源：http://qtn.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://xsu.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://ucv.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://szf.tian-w.cn

[U80] PHP：代码规范修复
来源：http://pwo.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://cdt.kuanghao11.cn

[U81] JS：初始化项目
来源：http://hzb.wangdashe.top

npm init -y;  npm i express
来源：http://idu.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://qpr.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rum.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://hqb.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://cnc.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://mae.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://kbc.sxryk.cn

[U85] JS：可选链
来源：http://gtg.0kj1m.cn

a?.b?.c
来源：http://dha.tian-w.cn

[U86] JS：空值合并
来源：http://gpk.zdbjq.cn

a ?? b
来源：http://eyt.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://myx.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://gok.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://gyl.wangdashe.top

{ ...a, ...b }
来源：http://faf.zhixingplan.top

[U89] JS：数组去重
来源：http://pqr.sysykeji.top

[...new Set(arr)]
来源：http://meo.cqqwz.cn

[U90] JS：数字数组排序
来源：http://dnp.daria6918.cn

[...arr].sort((a, b) => a - b)
来源：http://xvc.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://wtn.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pfk.sjlbkw.cn

[U92] JS：深拷贝
来源：http://lwb.gzhubu.top

structuredClone(obj)
来源：http://auk.hfpthk.cn

[U93] JS：模板字符串
来源：http://akf.yuanzhike.top

`共 ${n} 条`
来源：http://hwx.cdnleiting.top

[U94] JS：箭头函数
来源：http://qof.sjlbkw.cn

const double = x => x * 2;
来源：http://rbi.tanke756.top

[U95] JS：Promise 包装
来源：http://pmy.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://uhe.ydzc1.top

[U96] JS：async/await 与异常
来源：http://egf.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jco.chenjidiqi.icu

[U97] JS：并发请求
来源：http://jcr.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qwa.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://atn.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uro.kuanghao11.cn

[U99] JS：事件监听
来源：http://azz.hnqzz.top

el.addEventListener("click", e => {})
来源：http://zlr.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://sjd.svipenyu.cn

document.querySelector(".item")
来源：http://crj.ppjwa.cn

[U101] JS：classList 操作
来源：http://xed.uphjek.com

el.classList.toggle("active")
来源：http://kfe.jyoumei.cn

[U102] JS：本地存储
来源：http://njf.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rsh.zhongyouzk.top

[U103] JS：定时器
来源：http://hcb.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tpc.haohaochexian.top

[U104] JS：防抖
来源：http://khr.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fti.gogol.net.cn

[U105] JS：节流
来源：http://tis.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bqc.zhoulong.xyz

[U106] JS：日期格式化
来源：http://nlp.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dpv.jinqigfzy.top

[U107] JS：数字千分位
来源：http://vwu.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://acb.birdmap.top

[U108] JS：随机整数
来源：http://vrs.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rbj.zhijiandao.cn

[U109] JS：数组分组
来源：http://kip.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://wfs.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://eoy.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://erz.meibo888.top

[U111] JS：对象转 Map
来源：http://hay.tianlin.xyz

new Map(Object.entries(obj))
来源：http://bxz.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://rml.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://wvf.gotoacloud.top

[U113] JS：正则替换全部
来源：http://ggo.vehdjk.com

s.replaceAll("a", "b")
来源：http://gyx.yuxming.cn

[U114] JS：JSON 深比较
来源：http://sqb.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tfk.pycfn.com

[U115] JS：生成 UUID
来源：http://wik.shzxlz.cn

crypto.randomUUID()
来源：http://jbj.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://gif.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://vco.52xcode.cn

[U117] JS：单元测试
来源：http://bhv.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://elh.hfpthk.cn

[U118] JS：开发服务器
来源：http://xya.gzhubu.top

npm i -D vite;  npx vite
来源：http://dgb.jianghu66.top

[U119] JS：生产构建
来源：http://ncx.jiagoushi.top

npx vite build
来源：http://vbo.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://lnq.hywenlv.cn

import.meta.env.VITE_API_URL
来源：http://vzj.gaohongyu789.top

================================================================================
来源：http://kax.haohaochexian.top

统计汇总
来源：http://xde.jqgufenzy.top

================================================================================
来源：http://eqr.yj20258.top

按语言统计（条）：
来源：http://wiw.dashuyun.cn

Python ......... 252
来源：http://unv.tianlin.xyz

PHP ............ 252
来源：http://obp.tianlin.xyz

JavaScript ..... 252
来源：http://xam.zdbjq.cn

TypeScript ..... 212
来源：http://ywy.zhengqikj.top

Java ........... 212
来源：http://hya.bbcook.cn

Go ............. 212
来源：http://lgs.ydjk.org.cn

Ruby ........... 212
来源：http://lyp.jlsjyb.cn

C# ............. 212
来源：http://izp.tian-w.cn

C .............. 30
来源：http://gcu.ydzc1.top

C++ ............ 30
来源：http://old.zhijiandao.cn

SQL ............ 90
来源：http://nwh.zdbjq.cn

Bash ........... 80
来源：http://olm.zhoulong.xyz

Kotlin ......... 15
来源：http://cvk.zhijiandao.cn

Swift .......... 15
来源：http://tfz.chenjidiqi.icu

Lua ............ 10
来源：http://zeg.aizwys.cn

Perl ........... 10
来源：http://xmr.fzhhl.top

Scala .......... 10
来源：http://awb.shanyushiyangtech.top

------------------------------------
来源：http://fzo.guowangkeji.top

合计 ........... 2106 条
来源：http://elv.bjfxy.top

按章节统计：
来源：http://ctc.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zhk.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nwa.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wye.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rbm.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bro.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://abi.tianlin.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://muh.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yjo.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://imb.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://thk.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ggr.pengpengdd.cyou

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wme.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qlz.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wwr.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pqf.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ags.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://jcn.hywenlv.cn

R Bash 专题                             80
来源：http://dnv.redwolf501.top

S C / C++ 专题                          60
来源：http://foc.xylfe.cn

T 其他语言补充                          60
来源：http://wja.haohaochexian.top

U 高频实用片段                         120
来源：http://llc.gaohongyu789.top

------------------------------------
来源：http://vcj.yonumen.top

合计                                  2106 条
来源：http://hra.daxiang520.top

--------------------------------------------------------------------------------
来源：http://bpk.zhoulong.xyz

使用提醒
来源：http://usp.havefunace.top

--------------------------------------------------------------------------------
来源：http://nde.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jfw.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bfn.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ukl.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gdo.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fbp.hfpthk.cn

—— 文件结束 ——
来源：http://sxy.ybcxt.top

================================================================================
来源：http://rft.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://rxt.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://mke.ydzc1.top

================================================================================
来源：http://qii.cucudq.cn

【收录内容】
来源：http://zjb.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://svv.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oev.sweek.top

SQL · Bash · C · C++
来源：http://ypi.yj20258.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uoh.vehdjk.com

【使用说明】
来源：http://mrd.shanyushiyangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://djz.hysaishi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xvn.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pvn.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://exq.bbcook.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nzn.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://inx.bbcook.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pja.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ntb.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tcu.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xdv.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wui.ydzc1.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dmo.tanke756.top

【文件统计】
来源：http://olu.pengpengdd.cyou

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bsx.yongpay.top

--------------------------------------------------------------------------------
来源：http://ljw.fehbvm.com

目  录
来源：http://dny.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://ekf.tianlin.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rbs.mhx1999.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mvj.tanke756.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hxx.cucudq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nju.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gfw.c1oappe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ucr.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://myo.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uaf.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lpw.vehdjk.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iou.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sli.havefunace.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gcn.cqqwz.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xud.yfazqb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sbq.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://laj.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://smn.svipenyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ong.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eot.daxiang520.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://exn.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bzr.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://abc.gogol.net.cn

================================================================================
来源：http://mxx.zhoulong.xyz

A. 基础语法与类型
来源：http://ovk.sweek.top

================================================================================
来源：http://yfs.tarul.cn

[A01] Hello World
来源：http://vgn.jinyuanbaomall.cn

Py:   print("Hello, World!")
来源：http://yne.pycfn.com

PHP:  echo "Hello, World!";
来源：http://sci.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://gsl.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ozr.wangshuangyany.cn


<!-- 参考信息 -->