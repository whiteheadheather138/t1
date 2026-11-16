代发 wailian999

[U27] Py：异步 HTTP
来源：http://xlf.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://nlm.jinqigfzy.top

[U28] Py：类型别名
来源：http://qpf.nanxinkj.top

UserId = int
来源：http://sbu.ybcxt.top

[U29] Py：属性校验
来源：http://mkl.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://boe.yj20258888.top

[U30] Py：数据类
来源：http://hmk.cdnleiting.top

@dataclass(slots=True)
来源：http://emp.xuetiantiany.cn

[U31] Py：单测
来源：http://ktq.fktsv.cn

python -m pytest -q
来源：http://hqk.yonumen.top

[U32] Py：代码格式化
来源：http://gke.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://fla.zdqjudy.top

[U33] Py：打包发布
来源：http://pxx.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://sxz.gogol.net.cn

[U34] Py：判断编码
来源：http://nfc.zhongyouzk.top

chardet.detect(raw)
来源：http://xcp.yuxming.cn

[U35] Py：发送邮件
来源：http://vuh.zhengqikj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hcs.tian-w.cn

[U36] Py：定时任务
来源：http://jjo.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://iei.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://saz.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://fox.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://zac.iojbl.cn

Path(__file__).resolve().parent
来源：http://ruv.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://joj.yanxiufei.cn

sys.stdout.isatty()
来源：http://bst.nwbrower.top

[U40] Py：打印到标准错误
来源：http://xgu.bjfxy.top

print("err", file=sys.stderr)
来源：http://wbm.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://kzg.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hbo.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://lrq.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://auu.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://wvk.tianlin.xyz

namespace App\Http;
来源：http://rcv.ybcxt.top

[U44] PHP：开启严格类型
来源：http://xux.cucudq.cn

declare(strict_types=1);
来源：http://nsj.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://muw.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://pqn.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://pfx.redwolf501.top

?string $name = null
来源：http://oqo.cucudq.cn

[U47] PHP：联合类型
来源：http://wca.ppjwa.cn

int|string $id
来源：http://tsw.hesvh.cn

[U48] PHP：纯枚举
来源：http://zrf.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ryd.snrcjt.cn

[U49] PHP：只读属性
来源：http://krb.tanke756.top

public readonly string $name
来源：http://nix.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://koo.nwbrower.top

public function __construct(private int $id) {}
来源：http://zbp.gotoacloud.top

[U51] PHP：数组解构
来源：http://top.chenlongwang.top

[$a, $b] = $arr;
来源：http://wpz.ydzc1.top

[U52] PHP：箭头函数
来源：http://cgp.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://ngn.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://mgo.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://wpw.aizwys.cn

[U54] PHP：空安全调用
来源：http://caq.shuidangran.top

$obj?->method()
来源：http://qdq.hnqzz.top

[U55] PHP：match 表达式
来源：http://fjc.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://diy.ctjpmb.com

[U56] PHP：命名参数
来源：http://pkh.yangfankeji.com

f(a: 1, b: 2)
来源：http://vlx.shzxlz.cn

[U57] PHP：字符串插值
来源：http://kub.hnxiangtu.top

"值: {$a}"
来源：http://vjz.fehbvm.com

[U58] PHP：数组三件套
来源：http://yuv.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bdj.dianchejie.cn

[U59] PHP：自定义排序
来源：http://aki.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ghe.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://cla.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vdl.jqgfzy.top

[U61] PHP：正则
来源：http://acf.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://okt.hywenlv.cn

[U62] PHP：日期对象
来源：http://yhg.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nsz.shuidangran.top

[U63] PHP：文件读写
来源：http://hyn.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qdb.dianchejie.cn

[U64] PHP：目录遍历
来源：http://nhc.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://rrc.yuanzhike.top

[U65] PHP：会话
来源：http://tsv.havefunace.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uml.316326.xyz

[U66] PHP：设置 Cookie
来源：http://cyi.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oyu.hcnkem.com

[U67] PHP：处理文件上传
来源：http://lnn.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dva.hcnkem.com

[U68] PHP：PDO 连接
来源：http://ehh.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vhb.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://mvn.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nxm.yonumen.top

[U70] PHP：PDO 事务
来源：http://wbn.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://voi.hywenlv.cn

[U71] PHP：抛出异常
来源：http://ijk.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://vqs.shzxlz.cn

[U72] PHP：写错误日志
来源：http://xrl.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://ldj.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://yjs.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://gjz.sxryk.cn

[U74] PHP：读取环境变量
来源：http://pti.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://ufq.pengpengdd.cyou

[U75] PHP：依赖注入
来源：http://ais.meibo888.top

composer require psr/container
来源：http://ruo.hesvh.cn

[U76] PHP：简单路由
来源：http://onz.fengsongda.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uoi.zhongyouzk.top

[U77] PHP：模板渲染
来源：http://rgk.jianghu66.top

composer require twig/twig
来源：http://arh.smart0.xyz

[U78] PHP：单元测试
来源：http://ltg.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://arq.havefunace.top

[U79] PHP：静态分析
来源：http://qyv.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://tav.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://oqq.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://nkq.aizwys.cn

[U81] JS：初始化项目
来源：http://kks.fanxiaobao.xyz

npm init -y;  npm i express
来源：http://exh.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://uzl.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://obi.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://gwu.tanke756.top

export const a = 1;  import { a } from "./m.js";
来源：http://sht.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://dzt.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gib.xziqi.cn

[U85] JS：可选链
来源：http://gtg.dianchejie.cn

a?.b?.c
来源：http://her.sweek.top

[U86] JS：空值合并
来源：http://rhx.xuanzx.com

a ?? b
来源：http://byy.ydzc1.top

[U87] JS：解构默认值
来源：http://uef.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://kyp.zdqjudy.top

[U88] JS：对象展开合并
来源：http://ovr.sweek.top

{ ...a, ...b }
来源：http://ehy.ivvv.top

[U89] JS：数组去重
来源：http://uaa.smart0.xyz

[...new Set(arr)]
来源：http://jdw.hesvh.cn

[U90] JS：数字数组排序
来源：http://pxz.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://ayy.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://syv.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rdm.yj20258888.top

[U92] JS：深拷贝
来源：http://eqy.havefunace.top

structuredClone(obj)
来源：http://ujf.zhengqikj.top

[U93] JS：模板字符串
来源：http://zed.uphjek.com

`共 ${n} 条`
来源：http://bcs.mhx1999.top

[U94] JS：箭头函数
来源：http://zes.aibaodan.cn

const double = x => x * 2;
来源：http://jzs.sufxvd.cn

[U95] JS：Promise 包装
来源：http://sgw.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://cbg.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://hit.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rxo.ydzc1.top

[U97] JS：并发请求
来源：http://icp.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tmb.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://uye.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://atq.yj20258.top

[U99] JS：事件监听
来源：http://uki.yvedp.cn

el.addEventListener("click", e => {})
来源：http://all.ivvv.top

[U100] JS：DOM 查询
来源：http://qdd.shangyingyoupin.top

document.querySelector(".item")
来源：http://rfq.yuxming.cn

[U101] JS：classList 操作
来源：http://zmf.pycfn.com

el.classList.toggle("active")
来源：http://ysl.nanxinkj.top

[U102] JS：本地存储
来源：http://eyb.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://upn.svipenyu.cn

[U103] JS：定时器
来源：http://mkv.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tfd.gzhubu.top

[U104] JS：防抖
来源：http://oaq.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hoj.epnwcf.com

[U105] JS：节流
来源：http://twk.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://opg.kuanghao11.cn

[U106] JS：日期格式化
来源：http://efo.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://myk.aibaodan.cn

[U107] JS：数字千分位
来源：http://ltx.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cuh.tanke756.top

[U108] JS：随机整数
来源：http://axn.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jws.havefunace.top

[U109] JS：数组分组
来源：http://tnf.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://xtp.mhx1999.top

[U110] JS：数组分块
来源：http://rpb.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mgj.cdnleiting.top

[U111] JS：对象转 Map
来源：http://oit.hysaishi.cn

new Map(Object.entries(obj))
来源：http://ipk.mhx1999.top

[U112] JS：字符串补位
来源：http://dvd.sxryk.cn

"7".padStart(3, "0")
来源：http://ufk.nanxinkj.top

[U113] JS：正则替换全部
来源：http://rdr.aizwys.cn

s.replaceAll("a", "b")
来源：http://adl.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://jww.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ybl.sweek.top

[U115] JS：生成 UUID
来源：http://pss.zdbjq.cn

crypto.randomUUID()
来源：http://mcz.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://xvy.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://esp.9152youxi.cn

[U117] JS：单元测试
来源：http://zvj.sweek.top

npm i -D vitest;  npx vitest
来源：http://sof.52xcode.cn

[U118] JS：开发服务器
来源：http://rka.xziqi.cn

npm i -D vite;  npx vite
来源：http://ouk.nwbrower.top

[U119] JS：生产构建
来源：http://xbe.meibo888.top

npx vite build
来源：http://srf.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://laz.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://tnj.guowangkeji.top

================================================================================
来源：http://kle.ivvv.top

统计汇总
来源：http://nag.c1oappe.top

================================================================================
来源：http://hbe.ydzc1.top

按语言统计（条）：
来源：http://yhp.smart0.xyz

Python ......... 252
来源：http://hcq.bjfxy.top

PHP ............ 252
来源：http://mvc.sysykeji.top

JavaScript ..... 252
来源：http://gcp.nanxuanxn.top

TypeScript ..... 212
来源：http://wma.tianlin.xyz

Java ........... 212
来源：http://ubk.pengpengdd.cyou

Go ............. 212
来源：http://eag.gogol.net.cn

Ruby ........... 212
来源：http://vva.wangshuangyany.cn

C# ............. 212
来源：http://rty.ybcxt.top

C .............. 30
来源：http://bdt.zdqjudy.top

C++ ............ 30
来源：http://kwx.feifeiyinyue.top

SQL ............ 90
来源：http://fvf.ppjwa.cn

Bash ........... 80
来源：http://pub.meibo888.top

Kotlin ......... 15
来源：http://don.guowangkeji.top

Swift .......... 15
来源：http://mrv.jqgfzy.top

Lua ............ 10
来源：http://vgm.kuanghao11.cn

Perl ........... 10
来源：http://xuz.smart0.xyz

Scala .......... 10
来源：http://dkq.andypj.xyz

------------------------------------
来源：http://hen.hammf.cn

合计 ........... 2106 条
来源：http://gid.nwbrower.top

按章节统计：
来源：http://quc.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tyn.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ojc.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qff.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pml.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://twe.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nah.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dlu.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tjj.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lmw.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mjj.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uvk.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blm.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://akm.andypj.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bhc.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yeo.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rup.hcnkem.com

Q SQL 专题                              90
来源：http://udv.gotoacloud.top

R Bash 专题                             80
来源：http://dus.yfazqb.com

S C / C++ 专题                          60
来源：http://nra.sysykeji.top

T 其他语言补充                          60
来源：http://qgl.yj20258888.top

U 高频实用片段                         120
来源：http://hwq.zhixingplan.top

------------------------------------
来源：http://qgi.yanxiufei.cn

合计                                  2106 条
来源：http://xbq.sysykeji.top

--------------------------------------------------------------------------------
来源：http://ehv.guowangkeji.top

使用提醒
来源：http://avf.fengsongda.top

--------------------------------------------------------------------------------
来源：http://sta.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://idd.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pad.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rrd.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://aqx.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qmb.hesvh.cn

—— 文件结束 ——
来源：http://udz.aibaodan.cn

================================================================================
来源：http://gfh.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://cfv.kuanghao11.cn

Common Programming Examples Cheat Book
来源：http://ikc.zycfv.cn

================================================================================
来源：http://buv.xylfe.cn

【收录内容】
来源：http://dsm.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://baw.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rpo.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://wcj.smart0.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://znj.hywenlv.cn

【使用说明】
来源：http://aec.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tzm.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pth.sweek.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sbi.wangdashe.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wkj.316326.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://abx.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cpy.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qzg.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://axd.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://suq.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uvk.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://twz.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://reb.bbcook.cn

【文件统计】
来源：http://jxc.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://urp.c1oappe.top

--------------------------------------------------------------------------------
来源：http://tcp.guannengcc.top

目  录
来源：http://qjm.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://fiq.shuidangran.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wsu.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mkr.snrcjt.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kxw.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rpn.tian-w.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fxp.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lpq.svipenyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://spv.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oub.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vcq.jinqigfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nce.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://myq.zhiwuduotai.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ftq.52xcode.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hip.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hai.haohaochexian.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://igx.sufxvd.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ccz.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iln.c1oappe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bed.ctjpmb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://voa.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rvg.xingfuxueyuan.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://alz.sxryk.cn

================================================================================
来源：http://ize.xuanzx.com

A. 基础语法与类型
来源：http://mkn.hysaishi.cn

================================================================================
来源：http://vri.yfazqb.com

[A01] Hello World
来源：http://qwz.sufxvd.cn

Py:   print("Hello, World!")
来源：http://irl.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://xbj.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://lbw.vqdsnc.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://epu.ydjk.org.cn


<!-- 参考信息 -->