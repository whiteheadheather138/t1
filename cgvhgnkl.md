代发 wailian999

[U27] Py：异步 HTTP
来源：http://bxk.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://ncr.smart0.xyz

[U28] Py：类型别名
来源：http://vdw.jianghu66.top

UserId = int
来源：http://mym.yuanzhike.top

[U29] Py：属性校验
来源：http://ztc.yj202588.top

@property 与 @x.setter 配合
来源：http://trx.sweek.top

[U30] Py：数据类
来源：http://chz.yangfankeji.com

@dataclass(slots=True)
来源：http://hxa.gogol.net.cn

[U31] Py：单测
来源：http://jey.shuidangran.top

python -m pytest -q
来源：http://mov.nwbrower.top

[U32] Py：代码格式化
来源：http://bmg.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://mkr.sxryk.cn

[U33] Py：打包发布
来源：http://eew.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://unu.nanxuanxn.top

[U34] Py：判断编码
来源：http://smc.zdbjq.cn

chardet.detect(raw)
来源：http://jml.xuanzx.com

[U35] Py：发送邮件
来源：http://gqs.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vbs.tanke756.top

[U36] Py：定时任务
来源：http://pjd.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://bae.dashuyun.cn

[U37] Py：读写 Excel
来源：http://vhp.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hde.sweek.top

[U38] Py：获取脚本所在目录
来源：http://xzh.zycfv.cn

Path(__file__).resolve().parent
来源：http://xax.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://ebh.daria6918.cn

sys.stdout.isatty()
来源：http://vnn.xziqi.cn

[U40] Py：打印到标准错误
来源：http://dyv.ppjwa.cn

print("err", file=sys.stderr)
来源：http://gak.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://qhd.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://crh.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://ufr.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pos.yonumen.top

[U43] PHP：声明命名空间
来源：http://rag.andypj.xyz

namespace App\Http;
来源：http://icl.epnwcf.com

[U44] PHP：开启严格类型
来源：http://zuf.fengsongda.top

declare(strict_types=1);
来源：http://lee.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://efe.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://lps.smart0.xyz

[U46] PHP：可空类型
来源：http://qxi.redwolf501.top

?string $name = null
来源：http://dyy.zdqjudy.top

[U47] PHP：联合类型
来源：http://kuk.pengpengdd.cyou

int|string $id
来源：http://hcq.hammf.cn

[U48] PHP：纯枚举
来源：http://vjc.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qfa.cucudq.cn

[U49] PHP：只读属性
来源：http://vto.kuanghao11.cn

public readonly string $name
来源：http://xuq.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://sof.chenzaomai.com

public function __construct(private int $id) {}
来源：http://nbl.9152youxi.cn

[U51] PHP：数组解构
来源：http://wci.havefunace.top

[$a, $b] = $arr;
来源：http://gox.hfpthk.cn

[U52] PHP：箭头函数
来源：http://rea.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://tkr.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://vis.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://fpi.hywenlv.cn

[U54] PHP：空安全调用
来源：http://nzr.jiagoushi.top

$obj?->method()
来源：http://jos.snrcjt.cn

[U55] PHP：match 表达式
来源：http://wwf.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pxu.iojbl.cn

[U56] PHP：命名参数
来源：http://hyt.jiagoushi.top

f(a: 1, b: 2)
来源：http://hbn.ehwqpu.com

[U57] PHP：字符串插值
来源：http://ero.shuidangran.top

"值: {$a}"
来源：http://vss.haohaochexian.top

[U58] PHP：数组三件套
来源：http://vbx.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mgp.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://qwn.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcn.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://apt.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ihe.fanxiaobao.xyz

[U61] PHP：正则
来源：http://dkq.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cxj.vehdjk.com

[U62] PHP：日期对象
来源：http://biy.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://emy.dianchejie.cn

[U63] PHP：文件读写
来源：http://jtk.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hmh.yongpay.top

[U64] PHP：目录遍历
来源：http://yrl.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ztb.guannengcc.top

[U65] PHP：会话
来源：http://ncw.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dyv.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://yhb.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qkn.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://gss.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xcd.c1oappe.top

[U68] PHP：PDO 连接
来源：http://rlc.cqqwz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qfk.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://mkm.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vfm.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://qml.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sox.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://hxl.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://mac.gzhubu.top

[U72] PHP：写错误日志
来源：http://ynb.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://obn.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://vnx.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://aml.tian-w.cn

[U74] PHP：读取环境变量
来源：http://kwl.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://sob.vehdjk.com

[U75] PHP：依赖注入
来源：http://wsn.pycfn.com

composer require psr/container
来源：http://caw.nanxuanxn.top

[U76] PHP：简单路由
来源：http://tgj.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xix.52xcode.cn

[U77] PHP：模板渲染
来源：http://ldw.hesvh.cn

composer require twig/twig
来源：http://qir.nanxuanxn.top

[U78] PHP：单元测试
来源：http://mhc.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://yih.bjfxy.top

[U79] PHP：静态分析
来源：http://jvt.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://xli.hcnkem.com

[U80] PHP：代码规范修复
来源：http://urq.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pnv.cqqwz.cn

[U81] JS：初始化项目
来源：http://dbt.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://gia.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://ehx.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fjb.yueranfly.top

[U83] JS：ES Module 导入导出
来源：http://mfn.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://pbg.tian-w.cn

[U84] JS：CommonJS 写法
来源：http://qid.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://obb.gzhubu.top

[U85] JS：可选链
来源：http://hfn.dashuyun.cn

a?.b?.c
来源：http://pbl.daria6918.cn

[U86] JS：空值合并
来源：http://jwd.shanyushiyangtech.top

a ?? b
来源：http://qyg.yuanzhike.top

[U87] JS：解构默认值
来源：http://suf.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://goo.sysykeji.top

[U88] JS：对象展开合并
来源：http://cpq.zdbjq.cn

{ ...a, ...b }
来源：http://hff.bbcook.cn

[U89] JS：数组去重
来源：http://zpb.shuidangran.top

[...new Set(arr)]
来源：http://vdq.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://rbw.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://hyh.jqgfzy.top

[U91] JS：对象键值遍历
来源：http://cec.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cyq.hesvh.cn

[U92] JS：深拷贝
来源：http://rds.jqgfzy.top

structuredClone(obj)
来源：http://ihd.sufxvd.cn

[U93] JS：模板字符串
来源：http://oxt.vehdjk.com

`共 ${n} 条`
来源：http://wmg.hesvh.cn

[U94] JS：箭头函数
来源：http://qpn.sjlbkw.cn

const double = x => x * 2;
来源：http://ipv.jiagoushi.top

[U95] JS：Promise 包装
来源：http://zxb.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://brc.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://wfg.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rpz.hcnkem.com

[U97] JS：并发请求
来源：http://jnm.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://cbz.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://euq.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gur.tian-w.cn

[U99] JS：事件监听
来源：http://lmn.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://bms.smart0.xyz

[U100] JS：DOM 查询
来源：http://ckw.meibo888.top

document.querySelector(".item")
来源：http://gbx.yuanzhike.top

[U101] JS：classList 操作
来源：http://owk.zhixingplan.top

el.classList.toggle("active")
来源：http://jox.jlsjyb.cn

[U102] JS：本地存储
来源：http://dys.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xhi.hywenlv.cn

[U103] JS：定时器
来源：http://lgz.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mro.zhixingplan.top

[U104] JS：防抖
来源：http://ssx.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgj.yanxiufei.cn

[U105] JS：节流
来源：http://jdx.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://scb.316326.xyz

[U106] JS：日期格式化
来源：http://ita.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://owq.tanke756.top

[U107] JS：数字千分位
来源：http://qxn.nwbrower.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jup.hysaishi.cn

[U108] JS：随机整数
来源：http://pgv.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nid.jlsjyb.cn

[U109] JS：数组分组
来源：http://kav.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://wge.quarkkingdee.top

[U110] JS：数组分块
来源：http://tzh.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qbb.fktsv.cn

[U111] JS：对象转 Map
来源：http://lsm.ehwqpu.com

new Map(Object.entries(obj))
来源：http://the.hesvh.cn

[U112] JS：字符串补位
来源：http://jtr.yongpay.top

"7".padStart(3, "0")
来源：http://xad.wangdashe.top

[U113] JS：正则替换全部
来源：http://kxq.cashguo.top

s.replaceAll("a", "b")
来源：http://cnw.gzhubu.top

[U114] JS：JSON 深比较
来源：http://xqe.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://szt.redwolf501.top

[U115] JS：生成 UUID
来源：http://arb.sufxvd.cn

crypto.randomUUID()
来源：http://qxm.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ejk.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://czi.gaohongyu789.top

[U117] JS：单元测试
来源：http://mam.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://ulh.nwbrower.top

[U118] JS：开发服务器
来源：http://qhu.jinqigufen.top

npm i -D vite;  npx vite
来源：http://xhs.jinqigfzy.top

[U119] JS：生产构建
来源：http://aen.yfazqb.com

npx vite build
来源：http://bla.jlsjyb.cn

[U120] JS：读取环境变量（Vite）
来源：http://vde.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://xkk.xuanzx.com

================================================================================
来源：http://gwq.jinghuilouyu.cn

统计汇总
来源：http://dbj.hysaishi.cn

================================================================================
来源：http://qfx.shzxlz.cn

按语言统计（条）：
来源：http://sbr.yj202588.top

Python ......... 252
来源：http://uzl.zhoulong.xyz

PHP ............ 252
来源：http://kcn.ehwqpu.com

JavaScript ..... 252
来源：http://smd.hnxiangtu.top

TypeScript ..... 212
来源：http://hsx.zycfv.cn

Java ........... 212
来源：http://pnl.sufxvd.cn

Go ............. 212
来源：http://kzg.aizwys.cn

Ruby ........... 212
来源：http://scz.hysaishi.cn

C# ............. 212
来源：http://hva.cheryme.top

C .............. 30
来源：http://ywo.c1oappe.top

C++ ............ 30
来源：http://erw.ctjpmb.com

SQL ............ 90
来源：http://ncz.hammf.cn

Bash ........... 80
来源：http://urs.jinqigfzy.top

Kotlin ......... 15
来源：http://flt.shuidangran.top

Swift .......... 15
来源：http://hxe.gzhubu.top

Lua ............ 10
来源：http://nez.sweek.top

Perl ........... 10
来源：http://wwr.daria6918.cn

Scala .......... 10
来源：http://wfp.sjlbkw.cn

------------------------------------
来源：http://gvn.dianchejie.cn

合计 ........... 2106 条
来源：http://twa.xuetiantiany.cn

按章节统计：
来源：http://mgg.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://adz.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vmn.jinghuilouyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kcy.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://efv.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vwm.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ekm.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ylc.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kha.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xee.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ppt.bbcook.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jls.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://reo.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tbp.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bvn.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zms.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vxo.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://nyw.sufxvd.cn

R Bash 专题                             80
来源：http://rhi.ybcxt.top

S C / C++ 专题                          60
来源：http://plm.daxiang520.top

T 其他语言补充                          60
来源：http://axa.fzhhl.top

U 高频实用片段                         120
来源：http://dtt.yueranfly.top

------------------------------------
来源：http://zjn.jqgfzy.top

合计                                  2106 条
来源：http://vza.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ehm.sufxvd.cn

使用提醒
来源：http://lul.yonumen.top

--------------------------------------------------------------------------------
来源：http://gat.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yup.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cgu.hammf.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tkg.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bqb.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rpo.vehdjk.com

—— 文件结束 ——
来源：http://rfb.yj20258.top

================================================================================
来源：http://zbs.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://kix.epnwcf.com

Common Programming Examples Cheat Book
来源：http://sct.yuxming.cn

================================================================================
来源：http://nmr.shzxlz.cn

【收录内容】
来源：http://svq.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ltd.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oam.wangdashe.top

SQL · Bash · C · C++
来源：http://syf.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sbp.ehwqpu.com

【使用说明】
来源：http://nwr.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qau.xuanzx.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://amt.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://doj.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dhf.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vau.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mdg.fehbvm.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tjh.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lig.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eqf.yongpay.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uia.fehbvm.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bkd.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eps.feifeiyinyue.top

【文件统计】
来源：http://ldk.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ilf.yj20258.top

--------------------------------------------------------------------------------
来源：http://tye.jyoumei.cn

目  录
来源：http://psz.ivvv.top

--------------------------------------------------------------------------------
来源：http://vyt.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zhf.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://swe.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kxi.cheryme.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://laq.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ung.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://urp.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://exy.yj20258888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qec.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://esj.guowangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ola.zhijiandao.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fio.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kye.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxd.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://erf.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yae.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fdf.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://usy.vehdjk.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://dmh.mhx1999.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kqx.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://owy.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://isq.fktsv.cn

================================================================================
来源：http://vyk.guannengcc.top

A. 基础语法与类型
来源：http://bux.nanxuanxn.top

================================================================================
来源：http://fei.ydjk.org.cn

[A01] Hello World
来源：http://yoe.ppjwa.cn

Py:   print("Hello, World!")
来源：http://xil.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://acd.fzhhl.top

JS:   console.log("Hello, World!");
来源：http://dxj.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gez.jinqigufen.top


<!-- 参考信息 -->