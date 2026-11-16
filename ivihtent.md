代发 wailian999

[U25] Py：CSV 按字典读
来源：http://vsr.dianchejie.cn

csv.DictReader(f)
来源：http://tce.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://whh.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://egn.mhx1999.top

[U27] Py：异步 HTTP
来源：http://bki.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://poq.fktsv.cn

[U28] Py：类型别名
来源：http://mcm.gaohongyu789.top

UserId = int
来源：http://hbk.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://bcy.fktsv.cn

@property 与 @x.setter 配合
来源：http://yrk.fktsv.cn

[U30] Py：数据类
来源：http://noy.yuxming.cn

@dataclass(slots=True)
来源：http://vcl.jinqigufen.top

[U31] Py：单测
来源：http://rmw.hesvh.cn

python -m pytest -q
来源：http://irp.ppjwa.cn

[U32] Py：代码格式化
来源：http://vjq.guannengcc.top

ruff format . && ruff check --fix .
来源：http://pbr.bbcook.cn

[U33] Py：打包发布
来源：http://fbi.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://ibq.quarkkingdee.top

[U34] Py：判断编码
来源：http://efn.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://qtr.zdbjq.cn

[U35] Py：发送邮件
来源：http://bka.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xaz.haohaochexian.top

[U36] Py：定时任务
来源：http://zvt.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://ptn.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://pxy.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://vhy.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://zsm.cqqwz.cn

Path(__file__).resolve().parent
来源：http://xui.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://vrm.c1oappe.top

sys.stdout.isatty()
来源：http://qid.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://dzk.hcnkem.com

print("err", file=sys.stderr)
来源：http://zgs.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://rvg.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ryj.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://buo.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qvb.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://bna.jqgufenzy.top

namespace App\Http;
来源：http://owa.pycfn.com

[U44] PHP：开启严格类型
来源：http://yne.hcnkem.com

declare(strict_types=1);
来源：http://svb.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://jpo.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sbb.chenzaomai.com

[U46] PHP：可空类型
来源：http://bmw.fanxiaobao.xyz

?string $name = null
来源：http://ggq.fehbvm.com

[U47] PHP：联合类型
来源：http://kka.wangdashe.top

int|string $id
来源：http://hea.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://pif.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zkp.shuidangran.top

[U49] PHP：只读属性
来源：http://ahe.dashuyun.cn

public readonly string $name
来源：http://rpu.yj20258.top

[U50] PHP：构造器属性提升
来源：http://yzt.cqqwz.cn

public function __construct(private int $id) {}
来源：http://mnw.hcnkem.com

[U51] PHP：数组解构
来源：http://wza.sysykeji.top

[$a, $b] = $arr;
来源：http://srn.ivvv.top

[U52] PHP：箭头函数
来源：http://evd.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://mhu.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://alg.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://muj.9152youxi.cn

[U54] PHP：空安全调用
来源：http://tww.vqdsnc.cn

$obj?->method()
来源：http://hsk.ybcxt.top

[U55] PHP：match 表达式
来源：http://swd.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wsj.c1oappe.top

[U56] PHP：命名参数
来源：http://qgf.nanxuanxn.top

f(a: 1, b: 2)
来源：http://mpd.dashuyun.cn

[U57] PHP：字符串插值
来源：http://itf.redwolf501.top

"值: {$a}"
来源：http://ewo.tarul.cn

[U58] PHP：数组三件套
来源：http://wgy.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aax.jiagoushi.top

[U59] PHP：自定义排序
来源：http://zjk.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ejx.316326.xyz

[U60] PHP：JSON 编解码
来源：http://gni.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bff.cdnleiting.top

[U61] PHP：正则
来源：http://wnl.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lgm.vqdsnc.cn

[U62] PHP：日期对象
来源：http://sbr.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ipn.shuidangran.top

[U63] PHP：文件读写
来源：http://jpn.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xpa.yj20258888.top

[U64] PHP：目录遍历
来源：http://vgz.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://flu.hywenlv.cn

[U65] PHP：会话
来源：http://ewj.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eyx.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://ixj.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ygd.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://ovo.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://akg.nwbrower.top

[U68] PHP：PDO 连接
来源：http://dmo.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gwu.cheryme.top

[U69] PHP：PDO 预处理
来源：http://jpj.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hoa.tanke756.top

[U70] PHP：PDO 事务
来源：http://roq.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://txu.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://jte.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://jed.aibaodan.cn

[U72] PHP：写错误日志
来源：http://ywb.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://owr.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://izo.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://yfr.sxryk.cn

[U74] PHP：读取环境变量
来源：http://gkm.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://sck.svipenyu.cn

[U75] PHP：依赖注入
来源：http://iji.yj20258888.top

composer require psr/container
来源：http://tea.hfpthk.cn

[U76] PHP：简单路由
来源：http://bdr.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bmu.hywenlv.cn

[U77] PHP：模板渲染
来源：http://gsr.snrcjt.cn

composer require twig/twig
来源：http://ehr.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://gty.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://lba.ybcxt.top

[U79] PHP：静态分析
来源：http://ykb.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://cul.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://mes.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gie.xylfe.cn

[U81] JS：初始化项目
来源：http://wpq.hammf.cn

npm init -y;  npm i express
来源：http://ddl.snrcjt.cn

[U82] JS：package.json 脚本
来源：http://nzo.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vgv.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://dkq.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://qup.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://oal.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://uto.zhengqikj.top

[U85] JS：可选链
来源：http://mll.cashguo.top

a?.b?.c
来源：http://zbm.hammf.cn

[U86] JS：空值合并
来源：http://aze.nanxinkj.top

a ?? b
来源：http://txe.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://yfb.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://lau.cheryme.top

[U88] JS：对象展开合并
来源：http://yjk.9152youxi.cn

{ ...a, ...b }
来源：http://xyr.gotoacloud.top

[U89] JS：数组去重
来源：http://ftc.bbcook.cn

[...new Set(arr)]
来源：http://dgd.xinyue.icu

[U90] JS：数字数组排序
来源：http://tnp.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://bhz.jianghu66.top

[U91] JS：对象键值遍历
来源：http://kyy.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vwt.hnqzz.top

[U92] JS：深拷贝
来源：http://zez.yj20258.top

structuredClone(obj)
来源：http://ioc.xylfe.cn

[U93] JS：模板字符串
来源：http://wsx.ctjpmb.com

`共 ${n} 条`
来源：http://xoe.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://gwv.vehdjk.com

const double = x => x * 2;
来源：http://ccz.shuidangran.top

[U95] JS：Promise 包装
来源：http://une.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://emy.epnwcf.com

[U96] JS：async/await 与异常
来源：http://bma.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ick.52xcode.cn

[U97] JS：并发请求
来源：http://osm.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://hpv.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://qty.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xtb.gaohongyu789.top

[U99] JS：事件监听
来源：http://nax.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://byo.svipenyu.cn

[U100] JS：DOM 查询
来源：http://dul.nanxuanxn.top

document.querySelector(".item")
来源：http://gii.bjfxy.top

[U101] JS：classList 操作
来源：http://skq.hnqzz.top

el.classList.toggle("active")
来源：http://dpj.sysykeji.top

[U102] JS：本地存储
来源：http://beu.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ytk.yuxming.cn

[U103] JS：定时器
来源：http://ays.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pfl.shangyingyoupin.top

[U104] JS：防抖
来源：http://nfi.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwl.quarkkingdee.top

[U105] JS：节流
来源：http://sls.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dod.ctjpmb.com

[U106] JS：日期格式化
来源：http://mki.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wtg.sxryk.cn

[U107] JS：数字千分位
来源：http://xkk.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rcd.shangyingyoupin.top

[U108] JS：随机整数
来源：http://dfo.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gku.yuanzhike.top

[U109] JS：数组分组
来源：http://vrz.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://qqz.hfpthk.cn

[U110] JS：数组分块
来源：http://obc.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oov.ybcxt.top

[U111] JS：对象转 Map
来源：http://lqb.svipenyu.cn

new Map(Object.entries(obj))
来源：http://wvr.uphjek.com

[U112] JS：字符串补位
来源：http://cyu.cheryme.top

"7".padStart(3, "0")
来源：http://zpg.sxryk.cn

[U113] JS：正则替换全部
来源：http://zhj.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://aep.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://xgf.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zcf.smart0.xyz

[U115] JS：生成 UUID
来源：http://kvt.hfpthk.cn

crypto.randomUUID()
来源：http://elj.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://mqe.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://pew.meibo888.top

[U117] JS：单元测试
来源：http://sjz.tanke756.top

npm i -D vitest;  npx vitest
来源：http://yee.zhixingplan.top

[U118] JS：开发服务器
来源：http://fin.tarul.cn

npm i -D vite;  npx vite
来源：http://dpx.yfazqb.com

[U119] JS：生产构建
来源：http://kxq.hysaishi.cn

npx vite build
来源：http://ets.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://xtp.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://crg.zycfv.cn

================================================================================
来源：http://nmx.xingfuxueyuan.xyz

统计汇总
来源：http://dtb.zhengqikj.top

================================================================================
来源：http://big.hongshengwenyu.top

按语言统计（条）：
来源：http://mqk.chenjidiqi.icu

Python ......... 252
来源：http://xav.zhongyouzk.top

PHP ............ 252
来源：http://jbe.sysykeji.top

JavaScript ..... 252
来源：http://ckd.xuanzx.com

TypeScript ..... 212
来源：http://jak.daria6918.cn

Java ........... 212
来源：http://mxv.ivvv.top

Go ............. 212
来源：http://yaw.9152youxi.cn

Ruby ........... 212
来源：http://qhv.tianlin.xyz

C# ............. 212
来源：http://dhf.shangyingyoupin.top

C .............. 30
来源：http://ipd.yj20258.top

C++ ............ 30
来源：http://zde.cheryme.top

SQL ............ 90
来源：http://lxt.sjlbkw.cn

Bash ........... 80
来源：http://rfo.vqdsnc.cn

Kotlin ......... 15
来源：http://vjx.andypj.xyz

Swift .......... 15
来源：http://mnf.ivvv.top

Lua ............ 10
来源：http://zpj.xinyue.icu

Perl ........... 10
来源：http://chk.fanxiaobao.xyz

Scala .......... 10
来源：http://vor.jinyuanbaomall.cn

------------------------------------
来源：http://xlj.zdbjq.cn

合计 ........... 2106 条
来源：http://hjq.xuetiantiany.cn

按章节统计：
来源：http://gxw.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iuw.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dth.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://acn.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cbn.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ebw.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vkt.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dxm.havefunace.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lxu.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uad.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yuv.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rfg.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://skn.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://chq.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xjg.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mkb.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://abw.bjfxy.top

Q SQL 专题                              90
来源：http://nzl.smart0.xyz

R Bash 专题                             80
来源：http://oxu.c1oappe.top

S C / C++ 专题                          60
来源：http://eic.ivvv.top

T 其他语言补充                          60
来源：http://hnp.aizwys.cn

U 高频实用片段                         120
来源：http://jdm.kuanghao11.cn

------------------------------------
来源：http://sit.yonumen.top

合计                                  2106 条
来源：http://ufq.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://tew.ydjk.org.cn

使用提醒
来源：http://rkx.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://pii.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://urn.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://phk.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jwj.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sgg.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lcs.tianlin.xyz

—— 文件结束 ——
来源：http://hxe.jqgfzy.top

================================================================================
来源：http://tor.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://zhr.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://fqh.nanxinkj.top

================================================================================
来源：http://gfg.fanxiaobao.xyz

【收录内容】
来源：http://mdr.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lbo.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ueq.jyoumei.cn

SQL · Bash · C · C++
来源：http://ipy.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qsq.hammf.cn

【使用说明】
来源：http://tsq.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jfx.redwolf501.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fqo.52xcode.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kgq.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://teh.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gud.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nml.fzhhl.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yxd.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://run.shanyushiyangtech.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://chn.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tmv.iojbl.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://swy.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://khr.aizwys.cn

【文件统计】
来源：http://zpz.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hjp.mhx1999.top

--------------------------------------------------------------------------------
来源：http://izx.yj20258888.top

目  录
来源：http://xku.zycfv.cn

--------------------------------------------------------------------------------
来源：http://fio.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pew.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hdc.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vjw.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://shf.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qua.yuanzhike.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cza.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jwd.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ktw.yj202588.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aoa.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zmf.yangfankeji.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gee.jqgfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qvk.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qto.fengsongda.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://szh.jqgfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://upj.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://peo.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ede.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://lvh.fanxiaobao.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mbc.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fkw.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gjm.tian-w.cn

================================================================================
来源：http://srm.fzhhl.top

A. 基础语法与类型
来源：http://kwu.yj202588.top

================================================================================
来源：http://rlb.xuetiantiany.cn

[A01] Hello World
来源：http://bgp.ctjpmb.com


<!-- 参考信息 -->