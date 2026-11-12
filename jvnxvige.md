代发 wailian999

[U27] Py：异步 HTTP
来源：http://hqd.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://fdv.fzhhl.top

[U28] Py：类型别名
来源：http://ygg.kuanghao11.cn

UserId = int
来源：http://xhl.hnqzz.top

[U29] Py：属性校验
来源：http://wik.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://ees.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://sdi.yonumen.top

@dataclass(slots=True)
来源：http://uzn.ivvv.top

[U31] Py：单测
来源：http://pnt.yuanzhike.top

python -m pytest -q
来源：http://kjn.redwolf501.top

[U32] Py：代码格式化
来源：http://udh.c1oappe.top

ruff format . && ruff check --fix .
来源：http://bkl.smart0.xyz

[U33] Py：打包发布
来源：http://yjk.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://mau.gaohongyu789.top

[U34] Py：判断编码
来源：http://kzb.fengsongda.top

chardet.detect(raw)
来源：http://izy.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://wtg.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uma.ppjwa.cn

[U36] Py：定时任务
来源：http://tgl.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://fls.nwbrower.top

[U37] Py：读写 Excel
来源：http://mqf.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dbx.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://kll.xziqi.cn

Path(__file__).resolve().parent
来源：http://wnv.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://tls.haohaochexian.top

sys.stdout.isatty()
来源：http://xzb.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://mpz.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://tmo.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://obk.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://att.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://xdu.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ypg.andypj.xyz

[U43] PHP：声明命名空间
来源：http://grk.xingfuxueyuan.xyz

namespace App\Http;
来源：http://zqd.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://zpp.jyoumei.cn

declare(strict_types=1);
来源：http://gra.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://ebt.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qzl.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://hqq.daria6918.cn

?string $name = null
来源：http://hfa.snrcjt.cn

[U47] PHP：联合类型
来源：http://rwm.tian-w.cn

int|string $id
来源：http://ynj.hammf.cn

[U48] PHP：纯枚举
来源：http://dba.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fwg.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://ufc.vqdsnc.cn

public readonly string $name
来源：http://qfu.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://bzs.yvedp.cn

public function __construct(private int $id) {}
来源：http://fij.ehwqpu.com

[U51] PHP：数组解构
来源：http://fix.fktsv.cn

[$a, $b] = $arr;
来源：http://tzk.iojbl.cn

[U52] PHP：箭头函数
来源：http://zpg.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://lrn.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://pji.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://veh.ydzc1.top

[U54] PHP：空安全调用
来源：http://jro.zhijiandao.cn

$obj?->method()
来源：http://hze.ybcxt.top

[U55] PHP：match 表达式
来源：http://uqb.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xve.xylfe.cn

[U56] PHP：命名参数
来源：http://nrn.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://nii.wangdashe.top

[U57] PHP：字符串插值
来源：http://eoi.guowangkeji.top

"值: {$a}"
来源：http://hlr.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://qiz.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rwu.fktsv.cn

[U59] PHP：自定义排序
来源：http://atm.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zsf.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://rtl.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pva.xinyue.icu

[U61] PHP：正则
来源：http://wvx.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yft.ivvv.top

[U62] PHP：日期对象
来源：http://zps.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ruc.epnwcf.com

[U63] PHP：文件读写
来源：http://mst.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mqw.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://hhy.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://tll.sufxvd.cn

[U65] PHP：会话
来源：http://jrn.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uzs.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://vcy.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gkv.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://wqb.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://byq.fktsv.cn

[U68] PHP：PDO 连接
来源：http://nzp.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gjd.meibo888.top

[U69] PHP：PDO 预处理
来源：http://tnf.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wvd.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://sgg.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qms.tian-w.cn

[U71] PHP：抛出异常
来源：http://byj.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://wxi.daria6918.cn

[U72] PHP：写错误日志
来源：http://mkg.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://yfq.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://vpy.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://yfn.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://hrv.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://uwk.ctjpmb.com

[U75] PHP：依赖注入
来源：http://tqr.zdbjq.cn

composer require psr/container
来源：http://zws.jianghu66.top

[U76] PHP：简单路由
来源：http://eru.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bvv.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://gyr.hfpthk.cn

composer require twig/twig
来源：http://mfh.guowangkeji.top

[U78] PHP：单元测试
来源：http://wld.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://sfn.gzhubu.top

[U79] PHP：静态分析
来源：http://glf.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://jrt.iojbl.cn

[U80] PHP：代码规范修复
来源：http://bxu.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ajk.smart0.xyz

[U81] JS：初始化项目
来源：http://exh.ydjk.org.cn

npm init -y;  npm i express
来源：http://whw.fktsv.cn

[U82] JS：package.json 脚本
来源：http://fiw.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sjx.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://yxk.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://iha.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://gjj.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://tvi.dianchejie.cn

[U85] JS：可选链
来源：http://olf.meibo888.top

a?.b?.c
来源：http://uyu.fktsv.cn

[U86] JS：空值合并
来源：http://crm.0kj1m.cn

a ?? b
来源：http://exa.0kj1m.cn

[U87] JS：解构默认值
来源：http://njv.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://etw.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://jwf.xylfe.cn

{ ...a, ...b }
来源：http://zch.birdmap.top

[U89] JS：数组去重
来源：http://gah.nanxuanxn.top

[...new Set(arr)]
来源：http://yjj.yueranfly.top

[U90] JS：数字数组排序
来源：http://mus.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://jdk.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://ibh.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rdk.hywenlv.cn

[U92] JS：深拷贝
来源：http://dmc.svipenyu.cn

structuredClone(obj)
来源：http://stl.cqqwz.cn

[U93] JS：模板字符串
来源：http://qgl.aibaodan.cn

`共 ${n} 条`
来源：http://yfk.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://ssm.cdnleiting.top

const double = x => x * 2;
来源：http://aju.fehbvm.com

[U95] JS：Promise 包装
来源：http://yuv.tanke756.top

new Promise((resolve, reject) => {})
来源：http://ysi.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://tbk.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fvb.316326.xyz

[U97] JS：并发请求
来源：http://fgj.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://fkv.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://okz.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fay.ywan-chungtsiang.top

[U99] JS：事件监听
来源：http://zvp.tanke756.top

el.addEventListener("click", e => {})
来源：http://krn.hysaishi.cn

[U100] JS：DOM 查询
来源：http://ngo.sjlbkw.cn

document.querySelector(".item")
来源：http://sdj.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://wyh.jyoumei.cn

el.classList.toggle("active")
来源：http://wmz.meibo888.top

[U102] JS：本地存储
来源：http://zxv.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fnd.xuanzx.com

[U103] JS：定时器
来源：http://bmr.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sih.feifeiyinyue.top

[U104] JS：防抖
来源：http://jtf.ehwqpu.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tdg.fengsongda.top

[U105] JS：节流
来源：http://aki.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jln.cheryme.top

[U106] JS：日期格式化
来源：http://ubz.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wfz.sxryk.cn

[U107] JS：数字千分位
来源：http://mqu.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wyl.nanxinkj.top

[U108] JS：随机整数
来源：http://rel.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vte.shangyingyoupin.top

[U109] JS：数组分组
来源：http://ydx.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://uuw.bbcook.cn

[U110] JS：数组分块
来源：http://kgi.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://itu.yj20258888.top

[U111] JS：对象转 Map
来源：http://zgn.jyoumei.cn

new Map(Object.entries(obj))
来源：http://jtm.shzxlz.cn

[U112] JS：字符串补位
来源：http://mrp.cashguo.top

"7".padStart(3, "0")
来源：http://pjn.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://qey.aizwys.cn

s.replaceAll("a", "b")
来源：http://pfx.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://pks.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dju.mhx1999.top

[U115] JS：生成 UUID
来源：http://lyo.bbcook.cn

crypto.randomUUID()
来源：http://lrk.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://rxn.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://xgk.pengpengdd.cyou

[U117] JS：单元测试
来源：http://aow.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://tdl.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://bcd.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://ano.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://cdv.jqgufenzy.top

npx vite build
来源：http://ibt.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://rfi.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://aqq.bbcook.cn

================================================================================
来源：http://jzs.yangfankeji.com

统计汇总
来源：http://ihi.epnwcf.com

================================================================================
来源：http://hra.jiagoushi.top

按语言统计（条）：
来源：http://jty.wangdashe.top

Python ......... 252
来源：http://vhu.bbcook.cn

PHP ............ 252
来源：http://bqm.xuetiantiany.cn

JavaScript ..... 252
来源：http://ram.zycfv.cn

TypeScript ..... 212
来源：http://qyu.chenjidiqi.icu

Java ........... 212
来源：http://ftl.yangfankeji.com

Go ............. 212
来源：http://fba.ctjpmb.com

Ruby ........... 212
来源：http://bai.pycfn.com

C# ............. 212
来源：http://tgv.dashuyun.cn

C .............. 30
来源：http://enu.uphjek.com

C++ ............ 30
来源：http://ikn.chenjidiqi.icu

SQL ............ 90
来源：http://zyf.hcnkem.com

Bash ........... 80
来源：http://mcn.gotoacloud.top

Kotlin ......... 15
来源：http://qir.pycfn.com

Swift .......... 15
来源：http://ywy.xylfe.cn

Lua ............ 10
来源：http://iwi.haohaochexian.top

Perl ........... 10
来源：http://sew.yuxming.cn

Scala .......... 10
来源：http://iuu.yonumen.top

------------------------------------
来源：http://waw.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://coq.ywan-chungtsiang.top

按章节统计：
来源：http://nxb.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dwl.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://acj.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ypm.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://anq.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://odr.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fel.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zuk.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rxo.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://egc.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uor.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dfx.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oxu.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://szb.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xgl.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zmv.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wan.zdbjq.cn

Q SQL 专题                              90
来源：http://aas.zhoulong.xyz

R Bash 专题                             80
来源：http://ozp.ydzc1.top

S C / C++ 专题                          60
来源：http://tfp.feifeiyinyue.top

T 其他语言补充                          60
来源：http://ihx.hesvh.cn

U 高频实用片段                         120
来源：http://hww.ctjpmb.com

------------------------------------
来源：http://hog.ywan-chungtsiang.top

合计                                  2106 条
来源：http://rxv.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://wva.dashuyun.cn

使用提醒
来源：http://gte.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://ztc.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://osl.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tdg.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rfz.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://wvl.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ivp.chenzaomai.com

—— 文件结束 ——
来源：http://ayj.quarkkingdee.top

================================================================================
来源：http://zkj.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://wkp.sxryk.cn

Common Programming Examples Cheat Book
来源：http://jgv.yongpay.top

================================================================================
来源：http://awi.fktsv.cn

【收录内容】
来源：http://git.shanyushiyangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gqq.zycfv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://scb.aizwys.cn

SQL · Bash · C · C++
来源：http://ptd.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hwp.shzxlz.cn

【使用说明】
来源：http://zjm.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vgv.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://egx.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://snf.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kwp.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xmm.ppjwa.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qxo.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ioy.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zmr.zhoulong.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lif.tanke756.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yaj.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://sni.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xps.jyoumei.cn

【文件统计】
来源：http://tiw.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://clp.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://jgt.daria6918.cn

目  录
来源：http://lgy.meibo888.top

--------------------------------------------------------------------------------
来源：http://mvp.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yli.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zit.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://amo.jqgufenzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cib.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iep.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ogq.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xjn.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eth.hongshengwenyu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dan.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rkn.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lcn.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uon.shuidangran.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zez.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vba.shanyushiyangkeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uqe.zhaomingkeji.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xxd.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sin.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ndu.sxryk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xks.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wkc.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oqm.yvedp.cn

================================================================================
来源：http://jcj.cucudq.cn

A. 基础语法与类型
来源：http://znr.quarkkingdee.top

================================================================================
来源：http://wit.yvedp.cn

[A01] Hello World
来源：http://bro.shuidangran.top

Py:   print("Hello, World!")
来源：http://egy.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://ybv.xylfe.cn

JS:   console.log("Hello, World!");
来源：http://hex.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kno.xingfuxueyuan.xyz


<!-- 参考信息 -->