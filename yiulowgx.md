代发 wailian999

[U25] Py：CSV 按字典读
来源：http://mep.redwolf501.top

csv.DictReader(f)
来源：http://rgc.bbcook.cn

[U26] Py：并发下载
来源：http://iyl.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://odi.bbcook.cn

[U27] Py：异步 HTTP
来源：http://bhk.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://vvk.sjlbkw.cn

[U28] Py：类型别名
来源：http://qmr.epnwcf.com

UserId = int
来源：http://cdq.tian-w.cn

[U29] Py：属性校验
来源：http://uzo.fzhhl.top

@property 与 @x.setter 配合
来源：http://pde.sjlbkw.cn

[U30] Py：数据类
来源：http://ytq.yj20258.top

@dataclass(slots=True)
来源：http://qre.iojbl.cn

[U31] Py：单测
来源：http://qnm.wangshuangyany.cn

python -m pytest -q
来源：http://bbw.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://wbk.epnwcf.com

ruff format . && ruff check --fix .
来源：http://nkx.cqqwz.cn

[U33] Py：打包发布
来源：http://bnh.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://pbm.xylfe.cn

[U34] Py：判断编码
来源：http://vpz.havefunace.top

chardet.detect(raw)
来源：http://rsz.gzhubu.top

[U35] Py：发送邮件
来源：http://ofp.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://get.nanxinkj.top

[U36] Py：定时任务
来源：http://ewk.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://wkj.cqqwz.cn

[U37] Py：读写 Excel
来源：http://vbr.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tzr.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://nxt.chenzaomai.com

Path(__file__).resolve().parent
来源：http://ttk.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://joe.jiagoushi.top

sys.stdout.isatty()
来源：http://eqy.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://fbe.vehdjk.com

print("err", file=sys.stderr)
来源：http://taj.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ytr.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zsy.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ubu.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rjt.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://pkq.jlsjyb.cn

namespace App\Http;
来源：http://jxm.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://fzx.hammf.cn

declare(strict_types=1);
来源：http://hqv.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://xto.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hdc.hfpthk.cn

[U46] PHP：可空类型
来源：http://mie.quarkkingdee.top

?string $name = null
来源：http://rwr.sysykeji.top

[U47] PHP：联合类型
来源：http://jqq.jinyuanbaomall.cn

int|string $id
来源：http://ggu.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://dmk.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zco.fehbvm.com

[U49] PHP：只读属性
来源：http://rii.ehwqpu.com

public readonly string $name
来源：http://mmv.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://nlx.xuanzx.com

public function __construct(private int $id) {}
来源：http://kkx.gzhubu.top

[U51] PHP：数组解构
来源：http://efb.yfazqb.com

[$a, $b] = $arr;
来源：http://zvf.bjfxy.top

[U52] PHP：箭头函数
来源：http://mvh.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://nwh.iojbl.cn

[U53] PHP：空合并运算符
来源：http://lum.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://ebj.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://zup.gaohongyu789.top

$obj?->method()
来源：http://spt.mhx1999.top

[U55] PHP：match 表达式
来源：http://azc.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ybp.mhx1999.top

[U56] PHP：命名参数
来源：http://vjx.ctjpmb.com

f(a: 1, b: 2)
来源：http://bxn.nanxinkj.top

[U57] PHP：字符串插值
来源：http://iac.zhixingplan.top

"值: {$a}"
来源：http://hom.dianchejie.cn

[U58] PHP：数组三件套
来源：http://zon.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xdy.9152youxi.cn

[U59] PHP：自定义排序
来源：http://wox.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://weu.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://dum.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nea.tarul.cn

[U61] PHP：正则
来源：http://luv.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://axw.316326.xyz

[U62] PHP：日期对象
来源：http://dps.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gxu.gogol.net.cn

[U63] PHP：文件读写
来源：http://zcr.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hvw.0kj1m.cn

[U64] PHP：目录遍历
来源：http://hrp.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://lhs.hnqzz.top

[U65] PHP：会话
来源：http://xor.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://lbg.yonumen.top

[U66] PHP：设置 Cookie
来源：http://xqp.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wkd.316326.xyz

[U67] PHP：处理文件上传
来源：http://ytf.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://loe.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://rky.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iuj.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://ooh.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lsk.yj20258888.top

[U70] PHP：PDO 事务
来源：http://wrf.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bnn.9152youxi.cn

[U71] PHP：抛出异常
来源：http://clk.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://twl.andypj.xyz

[U72] PHP：写错误日志
来源：http://ijf.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://mbl.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://mzi.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://sgm.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://wsh.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://hgw.jinqigufen.top

[U75] PHP：依赖注入
来源：http://wkd.zdbjq.cn

composer require psr/container
来源：http://lfl.jiagoushi.top

[U76] PHP：简单路由
来源：http://irc.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ojo.jinyuanbaomall.cn

[U77] PHP：模板渲染
来源：http://bov.hongshengwenyu.top

composer require twig/twig
来源：http://jdw.havefunace.top

[U78] PHP：单元测试
来源：http://lav.zhongyouzk.top

composer require --dev phpunit/phpunit
来源：http://ffp.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://yuy.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://lcf.xuanzx.com

[U80] PHP：代码规范修复
来源：http://vyd.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://aga.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://lfn.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://grd.yj202588.top

[U82] JS：package.json 脚本
来源：http://cqw.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nov.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://ljh.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://iyj.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://ljh.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://mwe.bbcook.cn

[U85] JS：可选链
来源：http://azt.sxryk.cn

a?.b?.c
来源：http://tme.ppjwa.cn

[U86] JS：空值合并
来源：http://tha.chenzaomai.com

a ?? b
来源：http://vca.ydjk.org.cn

[U87] JS：解构默认值
来源：http://xon.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://aeb.fehbvm.com

[U88] JS：对象展开合并
来源：http://tjx.zdqjudy.top

{ ...a, ...b }
来源：http://eej.epnwcf.com

[U89] JS：数组去重
来源：http://ctx.yangfankeji.com

[...new Set(arr)]
来源：http://qfy.redwolf501.top

[U90] JS：数字数组排序
来源：http://iud.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://udf.tianlin.xyz

[U91] JS：对象键值遍历
来源：http://pfa.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://duf.vqdsnc.cn

[U92] JS：深拷贝
来源：http://joo.andypj.xyz

structuredClone(obj)
来源：http://bqs.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://pnn.fzhhl.top

`共 ${n} 条`
来源：http://fxs.fktsv.cn

[U94] JS：箭头函数
来源：http://kku.yuxming.cn

const double = x => x * 2;
来源：http://fdr.316326.xyz

[U95] JS：Promise 包装
来源：http://szb.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://cvu.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://fba.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jhp.jinqigufen.top

[U97] JS：并发请求
来源：http://fpn.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://wzm.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://hbr.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://srg.pycfn.com

[U99] JS：事件监听
来源：http://wmh.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://axt.ehwqpu.com

[U100] JS：DOM 查询
来源：http://byl.cashguo.top

document.querySelector(".item")
来源：http://rmf.bbcook.cn

[U101] JS：classList 操作
来源：http://fsd.hysaishi.cn

el.classList.toggle("active")
来源：http://qbc.jinqigufen.top

[U102] JS：本地存储
来源：http://gbb.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ujv.cdnleiting.top

[U103] JS：定时器
来源：http://hbh.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iyk.ctjpmb.com

[U104] JS：防抖
来源：http://ptr.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xgc.dashuyun.cn

[U105] JS：节流
来源：http://nsp.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jda.wangdashe.top

[U106] JS：日期格式化
来源：http://yjo.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yoj.cashguo.top

[U107] JS：数字千分位
来源：http://dky.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mgq.daxiang520.top

[U108] JS：随机整数
来源：http://cok.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nyc.havefunace.top

[U109] JS：数组分组
来源：http://tzs.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://ypr.jianghu66.top

[U110] JS：数组分块
来源：http://yug.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kyk.hfpthk.cn

[U111] JS：对象转 Map
来源：http://vbh.svipenyu.cn

new Map(Object.entries(obj))
来源：http://fuh.yuxming.cn

[U112] JS：字符串补位
来源：http://tve.bbcook.cn

"7".padStart(3, "0")
来源：http://ynb.gotoacloud.top

[U113] JS：正则替换全部
来源：http://dza.jiagoushi.top

s.replaceAll("a", "b")
来源：http://exi.c1oappe.top

[U114] JS：JSON 深比较
来源：http://ezs.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ctv.xylfe.cn

[U115] JS：生成 UUID
来源：http://nfw.yvedp.cn

crypto.randomUUID()
来源：http://bfs.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://kod.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://vjp.aizwys.cn

[U117] JS：单元测试
来源：http://onc.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://dhj.yuanzhike.top

[U118] JS：开发服务器
来源：http://ckj.yfazqb.com

npm i -D vite;  npx vite
来源：http://yqu.hysaishi.cn

[U119] JS：生产构建
来源：http://wyp.hnqzz.top

npx vite build
来源：http://zva.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://vmf.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://yxk.jianghu66.top

================================================================================
来源：http://bem.yj202588.top

统计汇总
来源：http://kge.nanxinkj.top

================================================================================
来源：http://dej.sjlbkw.cn

按语言统计（条）：
来源：http://bjj.zhoulong.xyz

Python ......... 252
来源：http://qyy.hysaishi.cn

PHP ............ 252
来源：http://lyz.hcnkem.com

JavaScript ..... 252
来源：http://ckn.hammf.cn

TypeScript ..... 212
来源：http://iec.yonumen.top

Java ........... 212
来源：http://ltl.gogol.net.cn

Go ............. 212
来源：http://kpj.jqgfzy.top

Ruby ........... 212
来源：http://hbt.yonumen.top

C# ............. 212
来源：http://mzi.zhaomingkeji.xyz

C .............. 30
来源：http://utt.gzhubu.top

C++ ............ 30
来源：http://zwn.jiagoushi.top

SQL ............ 90
来源：http://mku.yfazqb.com

Bash ........... 80
来源：http://glc.havefunace.top

Kotlin ......... 15
来源：http://laz.jinyuanbaomall.cn

Swift .......... 15
来源：http://rcc.yangfankeji.com

Lua ............ 10
来源：http://lst.wangdashe.top

Perl ........... 10
来源：http://gij.gaohongyu789.top

Scala .......... 10
来源：http://kud.yongpay.top

------------------------------------
来源：http://scm.meibo888.top

合计 ........... 2106 条
来源：http://hhe.sxryk.cn

按章节统计：
来源：http://qql.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eyc.jianghu66.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dpd.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cdn.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sjg.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jaf.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://euu.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wtv.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://joh.ydzc1.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kkb.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gmu.tian-w.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ipj.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zjb.ydjk.org.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://orx.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fwe.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ata.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gch.gotoacloud.top

Q SQL 专题                              90
来源：http://vfc.jinghuilouyu.cn

R Bash 专题                             80
来源：http://etz.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://geb.yfazqb.com

T 其他语言补充                          60
来源：http://edu.hywenlv.cn

U 高频实用片段                         120
来源：http://izx.zhengqikj.top

------------------------------------
来源：http://pwg.hcnkem.com

合计                                  2106 条
来源：http://ouc.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://tgn.wangdashe.top

使用提醒
来源：http://nug.epnwcf.com

--------------------------------------------------------------------------------
来源：http://sqs.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mfl.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dut.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fen.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://msi.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://juf.zhoulong.xyz

—— 文件结束 ——
来源：http://dvu.meibo888.top

================================================================================
来源：http://ebh.yj20258888.top

程序语言常见例子速查手册（2024 版）
来源：http://qae.sxryk.cn

Common Programming Examples Cheat Book
来源：http://bcy.fzhhl.top

================================================================================
来源：http://gur.316326.xyz

【收录内容】
来源：http://lrk.tian-w.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ibc.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wbp.haohaochexian.top

SQL · Bash · C · C++
来源：http://hvb.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ahd.hammf.cn

【使用说明】
来源：http://aap.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gpr.redwolf501.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dxv.aizwys.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://atp.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gru.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gcs.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://btm.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://axm.bjfxy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pfz.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ccp.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://znb.zhengqikj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xsf.ybcxt.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kuk.yueranfly.top

【文件统计】
来源：http://wqt.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ikb.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://dmt.hongshengwenyu.top

目  录
来源：http://dqp.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://ojw.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hai.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mpm.zhoulong.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://upl.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zov.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wmn.ppjwa.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mmp.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dpr.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ydt.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vit.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ffi.sjlbkw.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nzm.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qly.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yqt.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cyh.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ppg.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nvx.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://evh.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fcm.zycfv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qne.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzg.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gig.ydzc1.top

================================================================================
来源：http://cfi.cashguo.top

A. 基础语法与类型
来源：http://qzy.smart0.xyz

================================================================================
来源：http://jhq.316326.xyz

[A01] Hello World
来源：http://evo.jianghu66.top


<!-- 参考信息 -->