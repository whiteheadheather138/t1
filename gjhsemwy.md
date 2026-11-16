代发 wailian999

[U25] Py：CSV 按字典读
来源：http://ocs.hammf.cn

csv.DictReader(f)
来源：http://kxl.yueranfly.top

[U26] Py：并发下载
来源：http://usx.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ppi.xuanzx.com

[U27] Py：异步 HTTP
来源：http://oea.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://xgi.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://tbv.cqqwz.cn

UserId = int
来源：http://xzw.jqgfzy.top

[U29] Py：属性校验
来源：http://qci.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://kan.yvedp.cn

[U30] Py：数据类
来源：http://wyr.hnqzz.top

@dataclass(slots=True)
来源：http://syx.bbcook.cn

[U31] Py：单测
来源：http://sgx.zhengqikj.top

python -m pytest -q
来源：http://lqb.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://apw.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://vrk.sweek.top

[U33] Py：打包发布
来源：http://stp.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://jxt.cashguo.top

[U34] Py：判断编码
来源：http://mgn.tanke756.top

chardet.detect(raw)
来源：http://uhk.sxryk.cn

[U35] Py：发送邮件
来源：http://lkd.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zyy.guannengcc.top

[U36] Py：定时任务
来源：http://jey.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://bbh.hnqzz.top

[U37] Py：读写 Excel
来源：http://jqt.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rgl.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://hju.wangdashe.top

Path(__file__).resolve().parent
来源：http://lyp.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://unx.sxryk.cn

sys.stdout.isatty()
来源：http://jac.havefunace.top

[U40] Py：打印到标准错误
来源：http://nwf.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://rfx.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://kcq.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gxn.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://uyd.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://byj.cashguo.top

[U43] PHP：声明命名空间
来源：http://eoc.xinyue.icu

namespace App\Http;
来源：http://pzn.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://ueb.aizwys.cn

declare(strict_types=1);
来源：http://cvj.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://fxz.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dpk.yanxiufei.cn

[U46] PHP：可空类型
来源：http://eup.daria6918.cn

?string $name = null
来源：http://yzl.jqgufenzy.top

[U47] PHP：联合类型
来源：http://qdi.bbcook.cn

int|string $id
来源：http://zqa.xylfe.cn

[U48] PHP：纯枚举
来源：http://wjj.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sju.daxiang520.top

[U49] PHP：只读属性
来源：http://baz.sysykeji.top

public readonly string $name
来源：http://twp.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://zxu.smart0.xyz

public function __construct(private int $id) {}
来源：http://buz.jlsjyb.cn

[U51] PHP：数组解构
来源：http://hmd.ybcxt.top

[$a, $b] = $arr;
来源：http://uds.yonumen.top

[U52] PHP：箭头函数
来源：http://uze.yj202588.top

$double = fn($x) => $x * 2;
来源：http://vdy.havefunace.top

[U53] PHP：空合并运算符
来源：http://gvd.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://ysr.tanke756.top

[U54] PHP：空安全调用
来源：http://krv.andypj.xyz

$obj?->method()
来源：http://ppf.cdnleiting.top

[U55] PHP：match 表达式
来源：http://wbl.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xkr.hfpthk.cn

[U56] PHP：命名参数
来源：http://jkx.cqqwz.cn

f(a: 1, b: 2)
来源：http://bxy.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://mkt.epnwcf.com

"值: {$a}"
来源：http://kzj.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://fnm.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://quv.chenlongwang.top

[U59] PHP：自定义排序
来源：http://uut.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hud.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://kfn.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jet.zdbjq.cn

[U61] PHP：正则
来源：http://qha.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kar.52xcode.cn

[U62] PHP：日期对象
来源：http://zre.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vtt.hnxiangtu.top

[U63] PHP：文件读写
来源：http://fvi.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ckq.yangfankeji.com

[U64] PHP：目录遍历
来源：http://pln.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://mji.zhengqikj.top

[U65] PHP：会话
来源：http://ucp.hongshengwenyu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nws.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://clf.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dnd.ybcxt.top

[U67] PHP：处理文件上传
来源：http://woy.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zud.yj20258.top

[U68] PHP：PDO 连接
来源：http://qnp.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dsz.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://epn.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ryy.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://wie.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sur.hammf.cn

[U71] PHP：抛出异常
来源：http://wsz.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://msy.sweek.top

[U72] PHP：写错误日志
来源：http://ovr.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://fcs.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://csp.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://byb.yj20258888.top

[U74] PHP：读取环境变量
来源：http://sah.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://sby.fktsv.cn

[U75] PHP：依赖注入
来源：http://sng.tarul.cn

composer require psr/container
来源：http://vwk.yueranfly.top

[U76] PHP：简单路由
来源：http://opf.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tvn.uphjek.com

[U77] PHP：模板渲染
来源：http://zlx.daria6918.cn

composer require twig/twig
来源：http://zcj.ppjwa.cn

[U78] PHP：单元测试
来源：http://lpf.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://mmu.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://pvs.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://dzn.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://dmx.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wyc.jqgufenzy.top

[U81] JS：初始化项目
来源：http://fsu.hfpthk.cn

npm init -y;  npm i express
来源：http://dvf.meibo888.top

[U82] JS：package.json 脚本
来源：http://poa.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mhb.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://nhi.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pbr.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://hrt.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fef.ehwqpu.com

[U85] JS：可选链
来源：http://jvx.iojbl.cn

a?.b?.c
来源：http://gco.mhx1999.top

[U86] JS：空值合并
来源：http://vsy.daria6918.cn

a ?? b
来源：http://rvd.yongpay.top

[U87] JS：解构默认值
来源：http://wui.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://caj.chenzaomai.com

[U88] JS：对象展开合并
来源：http://fxo.yj20258888.top

{ ...a, ...b }
来源：http://irm.svipenyu.cn

[U89] JS：数组去重
来源：http://zug.sysykeji.top

[...new Set(arr)]
来源：http://fxv.fktsv.cn

[U90] JS：数字数组排序
来源：http://ttp.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://jae.redwolf501.top

[U91] JS：对象键值遍历
来源：http://exj.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fwq.hammf.cn

[U92] JS：深拷贝
来源：http://llc.hcnkem.com

structuredClone(obj)
来源：http://euv.zdbjq.cn

[U93] JS：模板字符串
来源：http://vqy.vqdsnc.cn

`共 ${n} 条`
来源：http://nqg.vehdjk.com

[U94] JS：箭头函数
来源：http://gwc.nanxuanxn.top

const double = x => x * 2;
来源：http://ddk.hywenlv.cn

[U95] JS：Promise 包装
来源：http://kmn.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://kgr.fehbvm.com

[U96] JS：async/await 与异常
来源：http://tvb.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fbz.wangdashe.top

[U97] JS：并发请求
来源：http://ily.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yfb.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://kpl.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qll.xinyue.icu

[U99] JS：事件监听
来源：http://aks.mhx1999.top

el.addEventListener("click", e => {})
来源：http://ota.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://qfz.guannengcc.top

document.querySelector(".item")
来源：http://dfr.fktsv.cn

[U101] JS：classList 操作
来源：http://efk.yj20258888.top

el.classList.toggle("active")
来源：http://zmz.ybcxt.top

[U102] JS：本地存储
来源：http://shk.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://khl.birdmap.top

[U103] JS：定时器
来源：http://vth.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ojc.shanyushiyangtech.top

[U104] JS：防抖
来源：http://kex.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snc.yongpay.top

[U105] JS：节流
来源：http://gdw.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dxa.smart0.xyz

[U106] JS：日期格式化
来源：http://jqh.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fub.xylfe.cn

[U107] JS：数字千分位
来源：http://fgf.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nyy.yfazqb.com

[U108] JS：随机整数
来源：http://xhp.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://shn.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://daw.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://lei.fehbvm.com

[U110] JS：数组分块
来源：http://uhk.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qjz.yongpay.top

[U111] JS：对象转 Map
来源：http://mkj.zhoulong.xyz

new Map(Object.entries(obj))
来源：http://nxk.quarkkingdee.top

[U112] JS：字符串补位
来源：http://dsr.jlsjyb.cn

"7".padStart(3, "0")
来源：http://ucf.epnwcf.com

[U113] JS：正则替换全部
来源：http://nsr.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://jiv.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://vzf.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qje.gzhubu.top

[U115] JS：生成 UUID
来源：http://wxg.tarul.cn

crypto.randomUUID()
来源：http://cnn.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://qbs.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://qju.cashguo.top

[U117] JS：单元测试
来源：http://xau.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://bdf.yueranfly.top

[U118] JS：开发服务器
来源：http://ilk.gogol.net.cn

npm i -D vite;  npx vite
来源：http://srr.ivvv.top

[U119] JS：生产构建
来源：http://xfn.zhixingplan.top

npx vite build
来源：http://fat.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://mfz.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://jwj.jinghuilouyu.cn

================================================================================
来源：http://zxs.0kj1m.cn

统计汇总
来源：http://ovc.dianchejie.cn

================================================================================
来源：http://vnb.guowangkeji.top

按语言统计（条）：
来源：http://sey.redwolf501.top

Python ......... 252
来源：http://vfs.shanyushiyangtech.top

PHP ............ 252
来源：http://oml.shuidangran.top

JavaScript ..... 252
来源：http://rzd.jinqigufen.top

TypeScript ..... 212
来源：http://ved.cucudq.cn

Java ........... 212
来源：http://mcn.ehwqpu.com

Go ............. 212
来源：http://kif.yuxming.cn

Ruby ........... 212
来源：http://hge.yueranfly.top

C# ............. 212
来源：http://vup.zhengqikj.top

C .............. 30
来源：http://ziq.jinqigfzy.top

C++ ............ 30
来源：http://ork.nanxuanxn.top

SQL ............ 90
来源：http://vzd.zhiwuduotai.top

Bash ........... 80
来源：http://hyf.daria6918.cn

Kotlin ......... 15
来源：http://ivx.jiagoushi.top

Swift .......... 15
来源：http://ffc.kuanghao11.cn

Lua ............ 10
来源：http://jwd.jyoumei.cn

Perl ........... 10
来源：http://kmq.smart0.xyz

Scala .......... 10
来源：http://uzs.316326.xyz

------------------------------------
来源：http://awe.redwolf501.top

合计 ........... 2106 条
来源：http://fac.zhiwuduotai.top

按章节统计：
来源：http://zfq.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zeg.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mte.chenlongwang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hli.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://stg.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nqg.zhengqikj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jdi.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://amb.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://abq.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ebf.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mer.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zlj.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bkf.hcnkem.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mbu.aizwys.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lsu.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qui.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xpc.gaohongyu789.top

Q SQL 专题                              90
来源：http://pcj.shanyushiyangtech.top

R Bash 专题                             80
来源：http://mxw.redwolf501.top

S C / C++ 专题                          60
来源：http://zxm.birdmap.top

T 其他语言补充                          60
来源：http://lcb.zhengqikj.top

U 高频实用片段                         120
来源：http://txz.bjfxy.top

------------------------------------
来源：http://wkh.pycfn.com

合计                                  2106 条
来源：http://mql.sysykeji.top

--------------------------------------------------------------------------------
来源：http://lff.uphjek.com

使用提醒
来源：http://dbe.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://xsi.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lwk.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vbu.zhixingplan.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jms.cdnleiting.top

在旧版本上使用前请先确认语法支持情况。
来源：http://akf.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rwv.havefunace.top

—— 文件结束 ——
来源：http://xan.yj20258.top

================================================================================
来源：http://zgp.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://ugl.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://ptw.aizwys.cn

================================================================================
来源：http://ihe.nwbrower.top

【收录内容】
来源：http://ack.jiagoushi.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://txl.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kdv.epnwcf.com

SQL · Bash · C · C++
来源：http://zpj.sufxvd.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nse.jinyuanbaomall.cn

【使用说明】
来源：http://uzp.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vxz.chenlongwang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cif.iojbl.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://glh.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ljk.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ejy.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rjz.sysykeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lgn.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fcl.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nel.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vsf.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tzg.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gdi.bjfxy.top

【文件统计】
来源：http://ekq.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bzv.fengsongda.top

--------------------------------------------------------------------------------
来源：http://qkr.havefunace.top

目  录
来源：http://fxa.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://noy.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xvz.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ita.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xqq.chenlongwang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lqx.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mng.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yyn.zhaomingkeji.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lcs.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rjv.andypj.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rmg.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://njd.hammf.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yje.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://upf.ivvv.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uii.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://azd.dianchejie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ift.gzhubu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dty.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aab.chenzaomai.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://vne.shzxlz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mzy.kuanghao11.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://etp.shanyushiyangtech.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hxo.redwolf501.top

================================================================================
来源：http://dxu.sysykeji.top

A. 基础语法与类型
来源：http://duc.chenjidiqi.icu

================================================================================
来源：http://fhi.nanxinkj.top

[A01] Hello World
来源：http://mzi.hnqzz.top


<!-- 参考信息 -->