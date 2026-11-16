代发 wailian999

[U23] Py：分块读取大文件
来源：http://leh.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mus.tarul.cn

[U24] Py：路径操作
来源：http://wvx.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qpb.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://dms.zhoulong.xyz

csv.DictReader(f)
来源：http://vrg.jqgufenzy.top

[U26] Py：并发下载
来源：http://nrt.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qwq.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://fiq.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://vdp.jiagoushi.top

[U28] Py：类型别名
来源：http://ala.fzhhl.top

UserId = int
来源：http://pab.shuidangran.top

[U29] Py：属性校验
来源：http://lvv.9152youxi.cn

@property 与 @x.setter 配合
来源：http://shn.hfpthk.cn

[U30] Py：数据类
来源：http://rla.yj20258888.top

@dataclass(slots=True)
来源：http://dzn.smart0.xyz

[U31] Py：单测
来源：http://rjq.tanke756.top

python -m pytest -q
来源：http://qbh.xziqi.cn

[U32] Py：代码格式化
来源：http://mgn.sweek.top

ruff format . && ruff check --fix .
来源：http://cug.uphjek.com

[U33] Py：打包发布
来源：http://xgv.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://ted.fzhhl.top

[U34] Py：判断编码
来源：http://ibs.iojbl.cn

chardet.detect(raw)
来源：http://dkh.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://lay.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ouk.yongpay.top

[U36] Py：定时任务
来源：http://rge.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://osm.52xcode.cn

[U37] Py：读写 Excel
来源：http://abq.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://zqd.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://nrd.52xcode.cn

Path(__file__).resolve().parent
来源：http://cam.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://pyn.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://ppb.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://ryy.chenlongwang.top

print("err", file=sys.stderr)
来源：http://gmo.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://bwl.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ahq.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://kzu.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xdj.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://tbe.zdqjudy.top

namespace App\Http;
来源：http://ezy.hcnkem.com

[U44] PHP：开启严格类型
来源：http://ijj.316326.xyz

declare(strict_types=1);
来源：http://cqx.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://pbd.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wlr.0kj1m.cn

[U46] PHP：可空类型
来源：http://svf.316326.xyz

?string $name = null
来源：http://nyc.ctjpmb.com

[U47] PHP：联合类型
来源：http://gke.shuidangran.top

int|string $id
来源：http://ead.jyoumei.cn

[U48] PHP：纯枚举
来源：http://bwo.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pau.uphjek.com

[U49] PHP：只读属性
来源：http://zup.hcnkem.com

public readonly string $name
来源：http://kox.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://lrz.chenlongwang.top

public function __construct(private int $id) {}
来源：http://teq.ydjk.org.cn

[U51] PHP：数组解构
来源：http://evz.xuanzx.com

[$a, $b] = $arr;
来源：http://eps.tanke756.top

[U52] PHP：箭头函数
来源：http://ypk.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://zqq.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://qog.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://dgr.jyoumei.cn

[U54] PHP：空安全调用
来源：http://gun.epnwcf.com

$obj?->method()
来源：http://qci.zdqjudy.top

[U55] PHP：match 表达式
来源：http://vun.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oem.bjfxy.top

[U56] PHP：命名参数
来源：http://zew.yonumen.top

f(a: 1, b: 2)
来源：http://qjt.sufxvd.cn

[U57] PHP：字符串插值
来源：http://zex.hywenlv.cn

"值: {$a}"
来源：http://vum.meibo888.top

[U58] PHP：数组三件套
来源：http://xrm.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nfh.ybcxt.top

[U59] PHP：自定义排序
来源：http://flr.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uil.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://jkh.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ery.epnwcf.com

[U61] PHP：正则
来源：http://zrs.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mws.xuanzx.com

[U62] PHP：日期对象
来源：http://lld.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gxt.cqqwz.cn

[U63] PHP：文件读写
来源：http://xil.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zhq.fzhhl.top

[U64] PHP：目录遍历
来源：http://nqe.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://obm.chenjidiqi.icu

[U65] PHP：会话
来源：http://dxw.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pxn.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://agb.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qco.hnqzz.top

[U67] PHP：处理文件上传
来源：http://bpg.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fyk.guannengcc.top

[U68] PHP：PDO 连接
来源：http://gpi.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://the.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://kup.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ney.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://jye.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://frk.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://fvt.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://dzg.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://aaj.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://hyo.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://xhw.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://muv.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://tmh.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://uel.iojbl.cn

[U75] PHP：依赖注入
来源：http://whe.nanxuanxn.top

composer require psr/container
来源：http://eso.zhengqikj.top

[U76] PHP：简单路由
来源：http://yju.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ctb.yueranfly.top

[U77] PHP：模板渲染
来源：http://zjl.xuetiantiany.cn

composer require twig/twig
来源：http://xdp.0kj1m.cn

[U78] PHP：单元测试
来源：http://qdv.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://zjr.hammf.cn

[U79] PHP：静态分析
来源：http://pjx.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://fwz.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://rnh.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uma.sysykeji.top

[U81] JS：初始化项目
来源：http://kqe.ctjpmb.com

npm init -y;  npm i express
来源：http://ynp.epnwcf.com

[U82] JS：package.json 脚本
来源：http://yig.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mmy.c1oappe.top

[U83] JS：ES Module 导入导出
来源：http://aga.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xtq.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://fsg.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://zrv.nanxinkj.top

[U85] JS：可选链
来源：http://nid.yj20258888.top

a?.b?.c
来源：http://sdz.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://flk.bjfxy.top

a ?? b
来源：http://oui.bjfxy.top

[U87] JS：解构默认值
来源：http://ohs.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://lnr.yvedp.cn

[U88] JS：对象展开合并
来源：http://nfy.fehbvm.com

{ ...a, ...b }
来源：http://alf.hfpthk.cn

[U89] JS：数组去重
来源：http://nhh.guannengcc.top

[...new Set(arr)]
来源：http://yca.0kj1m.cn

[U90] JS：数字数组排序
来源：http://jjk.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://bva.fengsongda.top

[U91] JS：对象键值遍历
来源：http://qdg.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wgs.meibo888.top

[U92] JS：深拷贝
来源：http://pua.dianchejie.cn

structuredClone(obj)
来源：http://uly.fehbvm.com

[U93] JS：模板字符串
来源：http://tlk.ydzc1.top

`共 ${n} 条`
来源：http://dvp.yanxiufei.cn

[U94] JS：箭头函数
来源：http://tso.iojbl.cn

const double = x => x * 2;
来源：http://ngm.meibo888.top

[U95] JS：Promise 包装
来源：http://fcm.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://jmb.sweek.top

[U96] JS：async/await 与异常
来源：http://zfn.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qet.hysaishi.cn

[U97] JS：并发请求
来源：http://sum.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://wba.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://fcu.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bon.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://vtd.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://ruc.hysaishi.cn

[U100] JS：DOM 查询
来源：http://rvq.zycfv.cn

document.querySelector(".item")
来源：http://nok.vehdjk.com

[U101] JS：classList 操作
来源：http://pms.316326.xyz

el.classList.toggle("active")
来源：http://aci.feifeiyinyue.top

[U102] JS：本地存储
来源：http://dzj.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://qjk.zdqjudy.top

[U103] JS：定时器
来源：http://ybp.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wlp.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://tjs.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxo.0kj1m.cn

[U105] JS：节流
来源：http://gzv.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uxu.tanke756.top

[U106] JS：日期格式化
来源：http://hec.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://frg.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://uzx.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://spb.sxryk.cn

[U108] JS：随机整数
来源：http://pun.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pew.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://irg.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://syq.yuanzhike.top

[U110] JS：数组分块
来源：http://ity.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pxl.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://zgc.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://qyk.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://dgc.xinyue.icu

"7".padStart(3, "0")
来源：http://dxu.snrcjt.cn

[U113] JS：正则替换全部
来源：http://owk.tianlin.xyz

s.replaceAll("a", "b")
来源：http://aqj.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://lax.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tjw.dashuyun.cn

[U115] JS：生成 UUID
来源：http://cdz.fehbvm.com

crypto.randomUUID()
来源：http://dab.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://fcb.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://qhg.pycfn.com

[U117] JS：单元测试
来源：http://tye.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://qhv.aizwys.cn

[U118] JS：开发服务器
来源：http://oou.0kj1m.cn

npm i -D vite;  npx vite
来源：http://hph.tian-w.cn

[U119] JS：生产构建
来源：http://iqw.chenzaomai.com

npx vite build
来源：http://tzn.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://pjs.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://zdh.chenzaomai.com

================================================================================
来源：http://vlc.hysaishi.cn

统计汇总
来源：http://fjd.fehbvm.com

================================================================================
来源：http://lji.chenlongwang.top

按语言统计（条）：
来源：http://ltl.aizwys.cn

Python ......... 252
来源：http://xlo.havefunace.top

PHP ............ 252
来源：http://oyk.jianghu66.top

JavaScript ..... 252
来源：http://kyf.snrcjt.cn

TypeScript ..... 212
来源：http://vrw.cashguo.top

Java ........... 212
来源：http://epz.zhijiandao.cn

Go ............. 212
来源：http://dxo.nanxinkj.top

Ruby ........... 212
来源：http://ucv.gzhubu.top

C# ............. 212
来源：http://veu.aibaodan.cn

C .............. 30
来源：http://qyx.gzhubu.top

C++ ............ 30
来源：http://okl.quarkkingdee.top

SQL ............ 90
来源：http://joa.smart0.xyz

Bash ........... 80
来源：http://mlj.pengpengdd.cyou

Kotlin ......... 15
来源：http://xqo.xylfe.cn

Swift .......... 15
来源：http://umz.daria6918.cn

Lua ............ 10
来源：http://ovy.jinyuanbaomall.cn

Perl ........... 10
来源：http://rst.aizwys.cn

Scala .......... 10
来源：http://miz.zdqjudy.top

------------------------------------
来源：http://iip.cashguo.top

合计 ........... 2106 条
来源：http://aul.aizwys.cn

按章节统计：
来源：http://fib.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dlr.fzhhl.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ajj.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lsu.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hos.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zsv.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ogb.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nyw.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jmv.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ocl.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bcg.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cnu.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dbi.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sni.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qre.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ree.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ayq.ivvv.top

Q SQL 专题                              90
来源：http://ccb.xinyue.icu

R Bash 专题                             80
来源：http://mip.yvedp.cn

S C / C++ 专题                          60
来源：http://hzx.hysaishi.cn

T 其他语言补充                          60
来源：http://bku.yangfankeji.com

U 高频实用片段                         120
来源：http://nph.sysykeji.top

------------------------------------
来源：http://ohl.jinqigfzy.top

合计                                  2106 条
来源：http://khs.cheryme.top

--------------------------------------------------------------------------------
来源：http://ncb.cucudq.cn

使用提醒
来源：http://upy.nwbrower.top

--------------------------------------------------------------------------------
来源：http://jcx.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://brs.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yya.pycfn.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tsk.mhx1999.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fzq.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ubc.jqgufenzy.top

—— 文件结束 ——
来源：http://hby.jinqigufen.top

================================================================================
来源：http://jbg.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://qon.pycfn.com

Common Programming Examples Cheat Book
来源：http://ejc.feifeiyinyue.top

================================================================================
来源：http://aft.hcnkem.com

【收录内容】
来源：http://qlm.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ycg.tian-w.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cgj.xziqi.cn

SQL · Bash · C · C++
来源：http://cts.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zya.zhixingplan.top

【使用说明】
来源：http://wls.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vob.shuidangran.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qom.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mnv.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bjw.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://oao.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qmb.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cac.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cai.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hlv.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ocq.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aqi.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qmf.zhaomingkeji.xyz

【文件统计】
来源：http://rwh.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cyu.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://ull.9152youxi.cn

目  录
来源：http://xdj.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://ohy.gotoacloud.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://plh.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jgj.yueranfly.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ksy.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://huk.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eiz.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ypn.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bmj.xinyue.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bal.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tcp.xuanzx.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hqz.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://faj.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dpz.ydjk.org.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tgu.chenjidiqi.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vgv.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mfj.tarul.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dgm.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dwj.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vyl.gotoacloud.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cmf.shanyushiyangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://taf.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://onx.jiagoushi.top


<!-- 参考信息 -->