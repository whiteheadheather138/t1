代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://epp.ivvv.top

@contextlib.contextmanager
来源：http://zyp.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://gnu.yuanzhike.top

list(zip(*m))
来源：http://hlg.havefunace.top

[U23] Py：分块读取大文件
来源：http://wdv.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xyu.gogol.net.cn

[U24] Py：路径操作
来源：http://ikx.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xqs.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://lid.mhx1999.top

csv.DictReader(f)
来源：http://kly.jinqigfzy.top

[U26] Py：并发下载
来源：http://ttv.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mjd.yj20258.top

[U27] Py：异步 HTTP
来源：http://uif.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://teh.yongpay.top

[U28] Py：类型别名
来源：http://lct.shanyushiyangkeji.top

UserId = int
来源：http://sao.xuanzx.com

[U29] Py：属性校验
来源：http://abk.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://bed.jinqigfzy.top

[U30] Py：数据类
来源：http://twm.jiagoushi.top

@dataclass(slots=True)
来源：http://vao.jiagoushi.top

[U31] Py：单测
来源：http://ait.iojbl.cn

python -m pytest -q
来源：http://wzj.hesvh.cn

[U32] Py：代码格式化
来源：http://lku.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://sgz.fzhhl.top

[U33] Py：打包发布
来源：http://tfk.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://tjo.xinyue.icu

[U34] Py：判断编码
来源：http://aym.xylfe.cn

chardet.detect(raw)
来源：http://aon.bjfxy.top

[U35] Py：发送邮件
来源：http://msw.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rkz.smart0.xyz

[U36] Py：定时任务
来源：http://bii.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://hgp.gogol.net.cn

[U37] Py：读写 Excel
来源：http://uox.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gwo.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://qbi.tianlin.xyz

Path(__file__).resolve().parent
来源：http://pzd.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://hsa.ivvv.top

sys.stdout.isatty()
来源：http://vvo.yvedp.cn

[U40] Py：打印到标准错误
来源：http://uqx.hammf.cn

print("err", file=sys.stderr)
来源：http://dsk.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://gtm.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://iad.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://iil.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvt.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://exy.yongpay.top

namespace App\Http;
来源：http://eye.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://pyu.xylfe.cn

declare(strict_types=1);
来源：http://hnd.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://bjq.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://okp.yj202588.top

[U46] PHP：可空类型
来源：http://oxx.daria6918.cn

?string $name = null
来源：http://hbn.ydjk.org.cn

[U47] PHP：联合类型
来源：http://eoe.jiagoushi.top

int|string $id
来源：http://qml.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://pux.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ojm.xylfe.cn

[U49] PHP：只读属性
来源：http://rkp.cheryme.top

public readonly string $name
来源：http://rzk.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://gzk.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://ltf.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://jtz.cucudq.cn

[$a, $b] = $arr;
来源：http://twz.yj20258888.top

[U52] PHP：箭头函数
来源：http://fqj.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://wet.cashguo.top

[U53] PHP：空合并运算符
来源：http://puw.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://knh.uphjek.com

[U54] PHP：空安全调用
来源：http://zfr.fehbvm.com

$obj?->method()
来源：http://hkl.yuxming.cn

[U55] PHP：match 表达式
来源：http://eoo.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://csy.fehbvm.com

[U56] PHP：命名参数
来源：http://yke.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://mbb.guowangkeji.top

[U57] PHP：字符串插值
来源：http://uyk.jlsjyb.cn

"值: {$a}"
来源：http://xys.xylfe.cn

[U58] PHP：数组三件套
来源：http://cwx.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jxu.zhengqikj.top

[U59] PHP：自定义排序
来源：http://xps.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qum.havefunace.top

[U60] PHP：JSON 编解码
来源：http://lob.ydjk.org.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://opg.zdqjudy.top

[U61] PHP：正则
来源：http://zod.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wte.smart0.xyz

[U62] PHP：日期对象
来源：http://zho.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ecz.ydzc1.top

[U63] PHP：文件读写
来源：http://paw.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xgg.xinyue.icu

[U64] PHP：目录遍历
来源：http://uqn.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://igb.jiagoushi.top

[U65] PHP：会话
来源：http://ery.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zil.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://kol.andypj.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gou.zhongyouzk.top

[U67] PHP：处理文件上传
来源：http://lmx.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgz.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://ray.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jch.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://bur.tanke756.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kbc.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://uyk.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ryi.guannengcc.top

[U71] PHP：抛出异常
来源：http://lrb.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://wkz.bbcook.cn

[U72] PHP：写错误日志
来源：http://jux.yanxiufei.cn

error_log("失败: " . $e->getMessage());
来源：http://ayc.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://bir.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://vsq.mhx1999.top

[U74] PHP：读取环境变量
来源：http://bcq.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://gps.jyoumei.cn

[U75] PHP：依赖注入
来源：http://ksk.cucudq.cn

composer require psr/container
来源：http://bds.uphjek.com

[U76] PHP：简单路由
来源：http://ail.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wos.0kj1m.cn

[U77] PHP：模板渲染
来源：http://kbi.fanxiaobao.xyz

composer require twig/twig
来源：http://dha.haohaochexian.top

[U78] PHP：单元测试
来源：http://gim.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://aco.tian-w.cn

[U79] PHP：静态分析
来源：http://xps.bjfxy.top

composer require --dev phpstan/phpstan
来源：http://odj.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://cqp.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aeg.yanxiufei.cn

[U81] JS：初始化项目
来源：http://ehq.hcnkem.com

npm init -y;  npm i express
来源：http://qsx.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://zun.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zlu.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://sgh.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fac.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://vyy.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://tka.fzhhl.top

[U85] JS：可选链
来源：http://jed.chenlongwang.top

a?.b?.c
来源：http://zgh.fengsongda.top

[U86] JS：空值合并
来源：http://jxc.svipenyu.cn

a ?? b
来源：http://agi.gzhubu.top

[U87] JS：解构默认值
来源：http://tle.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://isv.aizwys.cn

[U88] JS：对象展开合并
来源：http://kzp.wangdashe.top

{ ...a, ...b }
来源：http://hfp.jqgfzy.top

[U89] JS：数组去重
来源：http://smf.0kj1m.cn

[...new Set(arr)]
来源：http://ips.aibaodan.cn

[U90] JS：数字数组排序
来源：http://ayc.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://nsp.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://mnk.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cjr.hywenlv.cn

[U92] JS：深拷贝
来源：http://pge.chenzaomai.com

structuredClone(obj)
来源：http://jxz.jianghu66.top

[U93] JS：模板字符串
来源：http://ddy.hywenlv.cn

`共 ${n} 条`
来源：http://fsn.52xcode.cn

[U94] JS：箭头函数
来源：http://plr.iojbl.cn

const double = x => x * 2;
来源：http://pas.zdqjudy.top

[U95] JS：Promise 包装
来源：http://raf.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://qdh.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://mhw.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ama.yuxming.cn

[U97] JS：并发请求
来源：http://eha.cqqwz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qgp.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://zes.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://efy.mhx1999.top

[U99] JS：事件监听
来源：http://vxo.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://bxj.yj20258.top

[U100] JS：DOM 查询
来源：http://bri.jinqigfzy.top

document.querySelector(".item")
来源：http://kfi.yueranfly.top

[U101] JS：classList 操作
来源：http://qjc.dianchejie.cn

el.classList.toggle("active")
来源：http://fax.chenjidiqi.icu

[U102] JS：本地存储
来源：http://xyi.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gmk.yueranfly.top

[U103] JS：定时器
来源：http://rfk.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eka.9152youxi.cn

[U104] JS：防抖
来源：http://rsu.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qhy.zhaomingkeji.xyz

[U105] JS：节流
来源：http://pxh.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kac.bjfxy.top

[U106] JS：日期格式化
来源：http://htv.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xeq.tarul.cn

[U107] JS：数字千分位
来源：http://cvl.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bic.haohaochexian.top

[U108] JS：随机整数
来源：http://jrv.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uzt.nwbrower.top

[U109] JS：数组分组
来源：http://ewl.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://ieh.bbcook.cn

[U110] JS：数组分块
来源：http://wxv.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sbf.ppjwa.cn

[U111] JS：对象转 Map
来源：http://yin.pycfn.com

new Map(Object.entries(obj))
来源：http://yaq.bjfxy.top

[U112] JS：字符串补位
来源：http://mmh.yonumen.top

"7".padStart(3, "0")
来源：http://wun.nwbrower.top

[U113] JS：正则替换全部
来源：http://emt.fktsv.cn

s.replaceAll("a", "b")
来源：http://xxn.yj20258888.top

[U114] JS：JSON 深比较
来源：http://wdd.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kyo.snrcjt.cn

[U115] JS：生成 UUID
来源：http://uhi.chenjidiqi.icu

crypto.randomUUID()
来源：http://jzy.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://crk.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://hdx.yanxiufei.cn

[U117] JS：单元测试
来源：http://avp.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://xls.vehdjk.com

[U118] JS：开发服务器
来源：http://gsn.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://kkg.vehdjk.com

[U119] JS：生产构建
来源：http://lqh.snrcjt.cn

npx vite build
来源：http://hpd.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://mle.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://zht.c1oappe.top

================================================================================
来源：http://oet.9152youxi.cn

统计汇总
来源：http://fzg.andypj.xyz

================================================================================
来源：http://mrg.andypj.xyz

按语言统计（条）：
来源：http://umg.guowangkeji.top

Python ......... 252
来源：http://zev.hfpthk.cn

PHP ............ 252
来源：http://xfa.xuanzx.com

JavaScript ..... 252
来源：http://iob.nanxuanxn.top

TypeScript ..... 212
来源：http://stx.vehdjk.com

Java ........... 212
来源：http://kcj.jinqigfzy.top

Go ............. 212
来源：http://qlx.nanxuanxn.top

Ruby ........... 212
来源：http://icf.bjfxy.top

C# ............. 212
来源：http://gkz.zhongyouzk.top

C .............. 30
来源：http://xsh.jqgufenzy.top

C++ ............ 30
来源：http://wzy.hfpthk.cn

SQL ............ 90
来源：http://tdn.yonumen.top

Bash ........... 80
来源：http://dns.bbcook.cn

Kotlin ......... 15
来源：http://ifa.snrcjt.cn

Swift .......... 15
来源：http://ewo.sysykeji.top

Lua ............ 10
来源：http://ytt.birdmap.top

Perl ........... 10
来源：http://cyh.cheryme.top

Scala .......... 10
来源：http://tdt.sjlbkw.cn

------------------------------------
来源：http://wtr.zhijiandao.cn

合计 ........... 2106 条
来源：http://pln.ybcxt.top

按章节统计：
来源：http://nqi.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hle.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ouc.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://quy.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wzt.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yjt.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://axy.hnxiangtu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dwe.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dwl.hcnkem.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vhu.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jos.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pqo.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ntx.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bnn.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://axy.haohaochexian.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ukm.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xzp.xylfe.cn

Q SQL 专题                              90
来源：http://iaj.cashguo.top

R Bash 专题                             80
来源：http://rnq.fengsongda.top

S C / C++ 专题                          60
来源：http://tnp.iojbl.cn

T 其他语言补充                          60
来源：http://hfw.fzhhl.top

U 高频实用片段                         120
来源：http://sse.xuanzx.com

------------------------------------
来源：http://seq.cheryme.top

合计                                  2106 条
来源：http://brb.fehbvm.com

--------------------------------------------------------------------------------
来源：http://hes.zhengqikj.top

使用提醒
来源：http://rqp.c1oappe.top

--------------------------------------------------------------------------------
来源：http://uck.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sbn.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://edv.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jju.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eig.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ynh.hammf.cn

—— 文件结束 ——
来源：http://crp.guowangkeji.top

================================================================================
来源：http://bix.xuanzx.com

程序语言常见例子速查手册（2024 版）
来源：http://eyx.zhoulong.xyz

Common Programming Examples Cheat Book
来源：http://ght.yj202588.top

================================================================================
来源：http://otg.jinqigfzy.top

【收录内容】
来源：http://wuy.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hba.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://glb.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://boq.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ppg.wangshuangyany.cn

【使用说明】
来源：http://bma.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://erw.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dcs.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ijk.c1oappe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oig.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bcv.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mcw.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ssd.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://waa.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eig.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kql.yj20258888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dqf.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kwd.zdbjq.cn

【文件统计】
来源：http://zzr.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://exn.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://mwj.yfazqb.com

目  录
来源：http://nym.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://xzt.shanyushiyangtech.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ryp.kuanghao11.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xep.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jfi.quarkkingdee.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gjb.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jua.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aho.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://apq.epnwcf.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qte.hywenlv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uqo.cashguo.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zac.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pje.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cie.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qcz.xuetiantiany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://znc.mhx1999.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dbn.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cul.daria6918.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uwz.vqdsnc.cn


<!-- 参考信息 -->