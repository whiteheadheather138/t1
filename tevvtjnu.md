代发 wailian999

[U25] Py：CSV 按字典读
来源：http://qna.chenlongwang.top

csv.DictReader(f)
来源：http://eiv.mhx1999.top

[U26] Py：并发下载
来源：http://jtm.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iux.hnqzz.top

[U27] Py：异步 HTTP
来源：http://bhj.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://jog.yvedp.cn

[U28] Py：类型别名
来源：http://lte.ybcxt.top

UserId = int
来源：http://qrl.yangfankeji.com

[U29] Py：属性校验
来源：http://wvh.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://dpq.haohaochexian.top

[U30] Py：数据类
来源：http://jlw.yongpay.top

@dataclass(slots=True)
来源：http://bba.ppjwa.cn

[U31] Py：单测
来源：http://jsp.vehdjk.com

python -m pytest -q
来源：http://xfz.xylfe.cn

[U32] Py：代码格式化
来源：http://vgl.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://mms.dashuyun.cn

[U33] Py：打包发布
来源：http://bqx.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://gxg.ybcxt.top

[U34] Py：判断编码
来源：http://jlz.sysykeji.top

chardet.detect(raw)
来源：http://mzf.vqdsnc.cn

[U35] Py：发送邮件
来源：http://nqt.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yfz.yuxming.cn

[U36] Py：定时任务
来源：http://neu.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://rbb.gotoacloud.top

[U37] Py：读写 Excel
来源：http://ebv.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://ffh.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://lbz.zycfv.cn

Path(__file__).resolve().parent
来源：http://xyk.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://ech.hnxiangtu.top

sys.stdout.isatty()
来源：http://zur.tian-w.cn

[U40] Py：打印到标准错误
来源：http://deg.ehwqpu.com

print("err", file=sys.stderr)
来源：http://mdq.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://anr.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zjy.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://owb.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kmn.316326.xyz

[U43] PHP：声明命名空间
来源：http://dkw.zhixingplan.top

namespace App\Http;
来源：http://ljf.hnqzz.top

[U44] PHP：开启严格类型
来源：http://nrm.hfpthk.cn

declare(strict_types=1);
来源：http://bhh.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://ntd.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ghq.yj202588.top

[U46] PHP：可空类型
来源：http://llz.tianlin.xyz

?string $name = null
来源：http://nug.jiagoushi.top

[U47] PHP：联合类型
来源：http://lga.hnxiangtu.top

int|string $id
来源：http://avo.316326.xyz

[U48] PHP：纯枚举
来源：http://xmm.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ftq.vqdsnc.cn

[U49] PHP：只读属性
来源：http://wij.vqdsnc.cn

public readonly string $name
来源：http://ahv.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://rbc.vehdjk.com

public function __construct(private int $id) {}
来源：http://izg.yvedp.cn

[U51] PHP：数组解构
来源：http://ufn.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://pjw.316326.xyz

[U52] PHP：箭头函数
来源：http://pas.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://kmj.xylfe.cn

[U53] PHP：空合并运算符
来源：http://ajp.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://kwa.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://hsf.guowangkeji.top

$obj?->method()
来源：http://lyt.jiagoushi.top

[U55] PHP：match 表达式
来源：http://aoz.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zab.mhx1999.top

[U56] PHP：命名参数
来源：http://qfh.hywenlv.cn

f(a: 1, b: 2)
来源：http://bab.zycfv.cn

[U57] PHP：字符串插值
来源：http://yap.pycfn.com

"值: {$a}"
来源：http://ukd.ybcxt.top

[U58] PHP：数组三件套
来源：http://cls.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://msm.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://lza.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cwk.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://jjz.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wgg.9152youxi.cn

[U61] PHP：正则
来源：http://rxn.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vlc.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://sqv.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dko.cashguo.top

[U63] PHP：文件读写
来源：http://hmp.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zpp.gotoacloud.top

[U64] PHP：目录遍历
来源：http://eve.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://ecn.ivvv.top

[U65] PHP：会话
来源：http://bxb.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://xcc.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://pgi.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kqb.fktsv.cn

[U67] PHP：处理文件上传
来源：http://aky.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ogr.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://tdb.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bqw.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://lmv.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pdz.yuxming.cn

[U70] PHP：PDO 事务
来源：http://mra.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bne.bjfxy.top

[U71] PHP：抛出异常
来源：http://ams.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://wel.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://fix.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://prf.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://wfi.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://ekl.gzhubu.top

[U74] PHP：读取环境变量
来源：http://wlt.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://yiw.iojbl.cn

[U75] PHP：依赖注入
来源：http://cne.9152youxi.cn

composer require psr/container
来源：http://uij.nwbrower.top

[U76] PHP：简单路由
来源：http://jas.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pbn.redwolf501.top

[U77] PHP：模板渲染
来源：http://bwk.mhx1999.top

composer require twig/twig
来源：http://ujy.ivvv.top

[U78] PHP：单元测试
来源：http://tud.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://huw.yonumen.top

[U79] PHP：静态分析
来源：http://dlm.cheryme.top

composer require --dev phpstan/phpstan
来源：http://kze.nwbrower.top

[U80] PHP：代码规范修复
来源：http://ryx.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gfs.aizwys.cn

[U81] JS：初始化项目
来源：http://rvm.gaohongyu789.top

npm init -y;  npm i express
来源：http://snw.smart0.xyz

[U82] JS：package.json 脚本
来源：http://atk.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lqv.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://jvv.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zmq.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://lpu.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xla.jinqigufen.top

[U85] JS：可选链
来源：http://oht.jinqigfzy.top

a?.b?.c
来源：http://acr.sjlbkw.cn

[U86] JS：空值合并
来源：http://wbe.yvedp.cn

a ?? b
来源：http://hsu.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://bto.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://xgl.zhixingplan.top

[U88] JS：对象展开合并
来源：http://kpg.wangdashe.top

{ ...a, ...b }
来源：http://zum.redwolf501.top

[U89] JS：数组去重
来源：http://qeb.dashuyun.cn

[...new Set(arr)]
来源：http://doz.uphjek.com

[U90] JS：数字数组排序
来源：http://qwd.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://wee.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://ldl.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fej.redwolf501.top

[U92] JS：深拷贝
来源：http://vql.hnqzz.top

structuredClone(obj)
来源：http://etp.yanxiufei.cn

[U93] JS：模板字符串
来源：http://zpc.dianchejie.cn

`共 ${n} 条`
来源：http://fxz.chenlongwang.top

[U94] JS：箭头函数
来源：http://izi.pycfn.com

const double = x => x * 2;
来源：http://jzs.yonumen.top

[U95] JS：Promise 包装
来源：http://rwp.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://ggt.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://uxb.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://izg.yonumen.top

[U97] JS：并发请求
来源：http://nty.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://hiz.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://gmt.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wrw.xinyue.icu

[U99] JS：事件监听
来源：http://vkf.cucudq.cn

el.addEventListener("click", e => {})
来源：http://cmb.yj20258.top

[U100] JS：DOM 查询
来源：http://zyo.yvedp.cn

document.querySelector(".item")
来源：http://wtl.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://qrm.hcnkem.com

el.classList.toggle("active")
来源：http://spt.yonumen.top

[U102] JS：本地存储
来源：http://dlw.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bpa.cdnleiting.top

[U103] JS：定时器
来源：http://xro.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wug.xuanzx.com

[U104] JS：防抖
来源：http://plj.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fvx.zhongyouzk.top

[U105] JS：节流
来源：http://hkl.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://flt.snrcjt.cn

[U106] JS：日期格式化
来源：http://zxl.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dyb.yj20258888.top

[U107] JS：数字千分位
来源：http://qze.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://voo.shuidangran.top

[U108] JS：随机整数
来源：http://xzn.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cqs.jyoumei.cn

[U109] JS：数组分组
来源：http://sqf.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://slr.0kj1m.cn

[U110] JS：数组分块
来源：http://ufd.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fwy.c1oappe.top

[U111] JS：对象转 Map
来源：http://uej.sxryk.cn

new Map(Object.entries(obj))
来源：http://tvj.snrcjt.cn

[U112] JS：字符串补位
来源：http://inf.yj20258.top

"7".padStart(3, "0")
来源：http://wzh.sysykeji.top

[U113] JS：正则替换全部
来源：http://too.sufxvd.cn

s.replaceAll("a", "b")
来源：http://pom.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://nzt.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yev.shzxlz.cn

[U115] JS：生成 UUID
来源：http://rfm.yfazqb.com

crypto.randomUUID()
来源：http://che.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://ukn.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://lnv.zhengqikj.top

[U117] JS：单元测试
来源：http://plz.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://ykr.hcnkem.com

[U118] JS：开发服务器
来源：http://udw.ivvv.top

npm i -D vite;  npx vite
来源：http://mfe.ywan-chungtsiang.top

[U119] JS：生产构建
来源：http://pvc.fengsongda.top

npx vite build
来源：http://ean.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://qdg.cashguo.top

import.meta.env.VITE_API_URL
来源：http://brk.vehdjk.com

================================================================================
来源：http://frq.smart0.xyz

统计汇总
来源：http://csj.nanxuanxn.top

================================================================================
来源：http://uom.sufxvd.cn

按语言统计（条）：
来源：http://yck.feifeiyinyue.top

Python ......... 252
来源：http://hpu.hfpthk.cn

PHP ............ 252
来源：http://tip.tanke756.top

JavaScript ..... 252
来源：http://agz.dashuyun.cn

TypeScript ..... 212
来源：http://vku.daria6918.cn

Java ........... 212
来源：http://eue.aibaodan.cn

Go ............. 212
来源：http://trp.shangyingyoupin.top

Ruby ........... 212
来源：http://oar.nanxinkj.top

C# ............. 212
来源：http://dxm.jinqigufen.top

C .............. 30
来源：http://zqi.uphjek.com

C++ ............ 30
来源：http://cxf.dianchejie.cn

SQL ............ 90
来源：http://fxn.jinqigfzy.top

Bash ........... 80
来源：http://bir.sjlbkw.cn

Kotlin ......... 15
来源：http://hwb.cucudq.cn

Swift .......... 15
来源：http://zve.yueranfly.top

Lua ............ 10
来源：http://quw.jianghu66.top

Perl ........... 10
来源：http://ewg.jlsjyb.cn

Scala .......... 10
来源：http://vjy.shuidangran.top

------------------------------------
来源：http://crl.daria6918.cn

合计 ........... 2106 条
来源：http://tcn.yvedp.cn

按章节统计：
来源：http://jsb.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ofc.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yku.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kza.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hwg.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://efk.pycfn.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xlz.daxiang520.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qav.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xtv.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qte.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qug.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://riz.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://adm.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jmx.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qrl.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://chb.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://scp.hongshengwenyu.top

Q SQL 专题                              90
来源：http://dny.sweek.top

R Bash 专题                             80
来源：http://fga.hesvh.cn

S C / C++ 专题                          60
来源：http://wlq.quarkkingdee.top

T 其他语言补充                          60
来源：http://llm.vehdjk.com

U 高频实用片段                         120
来源：http://zyu.hysaishi.cn

------------------------------------
来源：http://cwq.hongshengwenyu.top

合计                                  2106 条
来源：http://yoc.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://pha.chenlongwang.top

使用提醒
来源：http://ijk.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://uyh.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vew.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mqc.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mij.xuetiantiany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ilf.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zxi.aizwys.cn

—— 文件结束 ——
来源：http://azr.chenlongwang.top

================================================================================
来源：http://oai.pengpengdd.cyou

程序语言常见例子速查手册（2024 版）
来源：http://fng.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://wfg.c1oappe.top

================================================================================
来源：http://kuo.shanyushiyangkeji.top

【收录内容】
来源：http://dby.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jfx.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://evq.jlsjyb.cn

SQL · Bash · C · C++
来源：http://ybs.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qoi.tian-w.cn

【使用说明】
来源：http://kpl.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pxw.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bxv.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://leo.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://frm.shzxlz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kot.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bpj.jianghu66.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lww.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vjz.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oor.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://chj.ybcxt.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bnp.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fyy.fktsv.cn

【文件统计】
来源：http://wka.dianchejie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hju.yj202588.top

--------------------------------------------------------------------------------
来源：http://tkq.52xcode.cn

目  录
来源：http://ayy.iojbl.cn

--------------------------------------------------------------------------------
来源：http://tlw.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hnd.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ypz.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://miq.jianghu66.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vzw.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nae.fktsv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vrv.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aee.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yzm.316326.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://twj.yonumen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gxb.xuanzx.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ipn.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mzu.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://clu.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ulv.shanyushiyangtech.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pcg.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lda.birdmap.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://riw.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://onx.ydzc1.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ato.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ase.sweek.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nxw.sysykeji.top

================================================================================
来源：http://edl.yj20258888.top

A. 基础语法与类型
来源：http://gmz.guowangkeji.top

================================================================================
来源：http://scz.epnwcf.com

[A01] Hello World
来源：http://skp.havefunace.top


<!-- 参考信息 -->