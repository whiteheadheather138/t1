代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://zst.zhongyouzk.top

@contextlib.contextmanager
来源：http://kuw.guowangkeji.top

[U22] Py：矩阵转置
来源：http://zae.hysaishi.cn

list(zip(*m))
来源：http://hbu.sxryk.cn

[U23] Py：分块读取大文件
来源：http://bvx.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tlw.cdnleiting.top

[U24] Py：路径操作
来源：http://lid.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dby.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://tyw.meibo888.top

csv.DictReader(f)
来源：http://oog.yanxiufei.cn

[U26] Py：并发下载
来源：http://rie.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gtx.meibo888.top

[U27] Py：异步 HTTP
来源：http://bzx.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://gzs.tarul.cn

[U28] Py：类型别名
来源：http://grx.ydjk.org.cn

UserId = int
来源：http://laa.jlsjyb.cn

[U29] Py：属性校验
来源：http://vpn.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://fwu.guannengcc.top

[U30] Py：数据类
来源：http://vst.haohaochexian.top

@dataclass(slots=True)
来源：http://maw.vehdjk.com

[U31] Py：单测
来源：http://ahc.jinqigfzy.top

python -m pytest -q
来源：http://zzp.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://lqh.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://cao.tarul.cn

[U33] Py：打包发布
来源：http://fln.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://gfc.ctjpmb.com

[U34] Py：判断编码
来源：http://snx.shangyingyoupin.top

chardet.detect(raw)
来源：http://lbh.ctjpmb.com

[U35] Py：发送邮件
来源：http://vcx.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kee.hfpthk.cn

[U36] Py：定时任务
来源：http://xlh.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://sgh.yongpay.top

[U37] Py：读写 Excel
来源：http://qjc.andypj.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://mmc.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://bfg.316326.xyz

Path(__file__).resolve().parent
来源：http://tls.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://jbf.tarul.cn

sys.stdout.isatty()
来源：http://fjo.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://ojm.yonumen.top

print("err", file=sys.stderr)
来源：http://ijv.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://szv.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bzu.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://oxu.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iff.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://ydp.cashguo.top

namespace App\Http;
来源：http://jhc.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://cwf.zhiwuduotai.top

declare(strict_types=1);
来源：http://qaw.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://spg.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://snx.ppjwa.cn

[U46] PHP：可空类型
来源：http://cuv.sweek.top

?string $name = null
来源：http://uxf.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://ucv.smart0.xyz

int|string $id
来源：http://upc.jianghu66.top

[U48] PHP：纯枚举
来源：http://oav.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hfx.pycfn.com

[U49] PHP：只读属性
来源：http://yfp.jqgufenzy.top

public readonly string $name
来源：http://rpf.cashguo.top

[U50] PHP：构造器属性提升
来源：http://lpp.ydzc1.top

public function __construct(private int $id) {}
来源：http://ddc.sweek.top

[U51] PHP：数组解构
来源：http://clu.xinyue.icu

[$a, $b] = $arr;
来源：http://vyt.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://mkq.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://flv.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://nrc.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://mxw.yongpay.top

[U54] PHP：空安全调用
来源：http://hft.sweek.top

$obj?->method()
来源：http://yad.nwbrower.top

[U55] PHP：match 表达式
来源：http://fkp.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gcb.yonumen.top

[U56] PHP：命名参数
来源：http://cuj.guowangkeji.top

f(a: 1, b: 2)
来源：http://pzc.sufxvd.cn

[U57] PHP：字符串插值
来源：http://kwf.sysykeji.top

"值: {$a}"
来源：http://zkf.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://xse.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ace.sysykeji.top

[U59] PHP：自定义排序
来源：http://wqc.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwk.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://fqw.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://inx.shangyingyoupin.top

[U61] PHP：正则
来源：http://jyc.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dul.yvedp.cn

[U62] PHP：日期对象
来源：http://cwv.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vdh.hywenlv.cn

[U63] PHP：文件读写
来源：http://rsf.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lew.guannengcc.top

[U64] PHP：目录遍历
来源：http://vay.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://cxo.wangdashe.top

[U65] PHP：会话
来源：http://koh.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vck.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://uif.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cqn.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://bxp.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sga.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://bwf.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ktj.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://nql.shzxlz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tcr.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://wwm.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tjd.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://szw.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://eiz.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://uie.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://vdm.hysaishi.cn

[U73] PHP：读取 ini 配置
来源：http://gru.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://sug.cucudq.cn

[U74] PHP：读取环境变量
来源：http://uoz.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://dlo.vehdjk.com

[U75] PHP：依赖注入
来源：http://xep.bjfxy.top

composer require psr/container
来源：http://wdw.aizwys.cn

[U76] PHP：简单路由
来源：http://knc.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oyp.sysykeji.top

[U77] PHP：模板渲染
来源：http://mxt.shuidangran.top

composer require twig/twig
来源：http://gbn.sysykeji.top

[U78] PHP：单元测试
来源：http://agt.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://rbd.fktsv.cn

[U79] PHP：静态分析
来源：http://rkv.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://nsx.52xcode.cn

[U80] PHP：代码规范修复
来源：http://fec.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xrn.dianchejie.cn

[U81] JS：初始化项目
来源：http://ngg.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://kzv.aizwys.cn

[U82] JS：package.json 脚本
来源：http://not.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gfv.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://gih.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://nek.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://yab.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fjh.gzhubu.top

[U85] JS：可选链
来源：http://sry.cashguo.top

a?.b?.c
来源：http://zbx.chenlongwang.top

[U86] JS：空值合并
来源：http://oqc.shanyushiyangtech.top

a ?? b
来源：http://hbt.cheryme.top

[U87] JS：解构默认值
来源：http://ejb.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://ghf.c1oappe.top

[U88] JS：对象展开合并
来源：http://zlq.wangshuangyany.cn

{ ...a, ...b }
来源：http://swy.yangfankeji.com

[U89] JS：数组去重
来源：http://gao.yj202588.top

[...new Set(arr)]
来源：http://dps.snrcjt.cn

[U90] JS：数字数组排序
来源：http://tll.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://izj.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://nuc.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://omb.bjfxy.top

[U92] JS：深拷贝
来源：http://dxm.yanxiufei.cn

structuredClone(obj)
来源：http://xog.ydzc1.top

[U93] JS：模板字符串
来源：http://zpp.jqgufenzy.top

`共 ${n} 条`
来源：http://tav.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://uhl.ydzc1.top

const double = x => x * 2;
来源：http://eck.andypj.xyz

[U95] JS：Promise 包装
来源：http://wow.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://ial.redwolf501.top

[U96] JS：async/await 与异常
来源：http://mrm.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bni.ivvv.top

[U97] JS：并发请求
来源：http://rtq.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cmg.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://ccg.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qnj.hysaishi.cn

[U99] JS：事件监听
来源：http://kwj.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://aie.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://moi.tanke756.top

document.querySelector(".item")
来源：http://xql.sjlbkw.cn

[U101] JS：classList 操作
来源：http://lgf.haohaochexian.top

el.classList.toggle("active")
来源：http://quv.vehdjk.com

[U102] JS：本地存储
来源：http://kgb.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kcr.yanxiufei.cn

[U103] JS：定时器
来源：http://cwb.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ied.hammf.cn

[U104] JS：防抖
来源：http://kvu.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqa.cheryme.top

[U105] JS：节流
来源：http://bio.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://inx.c1oappe.top

[U106] JS：日期格式化
来源：http://fsx.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yzs.yueranfly.top

[U107] JS：数字千分位
来源：http://pbf.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://agu.yanxiufei.cn

[U108] JS：随机整数
来源：http://qkm.tarul.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aqa.havefunace.top

[U109] JS：数组分组
来源：http://lot.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://qfd.c1oappe.top

[U110] JS：数组分块
来源：http://lzg.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aas.zycfv.cn

[U111] JS：对象转 Map
来源：http://jih.andypj.xyz

new Map(Object.entries(obj))
来源：http://rbp.redwolf501.top

[U112] JS：字符串补位
来源：http://nqx.yanxiufei.cn

"7".padStart(3, "0")
来源：http://joq.yangfankeji.com

[U113] JS：正则替换全部
来源：http://xcq.yonumen.top

s.replaceAll("a", "b")
来源：http://tzd.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://iqv.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pwo.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://nur.aizwys.cn

crypto.randomUUID()
来源：http://kmy.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://vpd.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://tei.xziqi.cn

[U117] JS：单元测试
来源：http://hlc.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://ppl.fktsv.cn

[U118] JS：开发服务器
来源：http://wce.birdmap.top

npm i -D vite;  npx vite
来源：http://rkc.guannengcc.top

[U119] JS：生产构建
来源：http://zzs.zhaomingkeji.xyz

npx vite build
来源：http://ych.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://bwq.tarul.cn

import.meta.env.VITE_API_URL
来源：http://ljx.kuanghao11.cn

================================================================================
来源：http://hmp.fengsongda.top

统计汇总
来源：http://qzq.tanke756.top

================================================================================
来源：http://ydd.hesvh.cn

按语言统计（条）：
来源：http://hkt.pycfn.com

Python ......... 252
来源：http://sae.yanxiufei.cn

PHP ............ 252
来源：http://umv.vqdsnc.cn

JavaScript ..... 252
来源：http://ufy.redwolf501.top

TypeScript ..... 212
来源：http://tza.quarkkingdee.top

Java ........... 212
来源：http://xkz.hongshengwenyu.top

Go ............. 212
来源：http://ith.aizwys.cn

Ruby ........... 212
来源：http://pya.fanxiaobao.xyz

C# ............. 212
来源：http://glf.hcnkem.com

C .............. 30
来源：http://sgz.tarul.cn

C++ ............ 30
来源：http://cwj.c1oappe.top

SQL ............ 90
来源：http://fsd.jinghuilouyu.cn

Bash ........... 80
来源：http://ksk.havefunace.top

Kotlin ......... 15
来源：http://pak.shzxlz.cn

Swift .......... 15
来源：http://glt.ywan-chungtsiang.top

Lua ............ 10
来源：http://oaq.zhiwuduotai.top

Perl ........... 10
来源：http://wpd.hongshengwenyu.top

Scala .......... 10
来源：http://trp.nwbrower.top

------------------------------------
来源：http://fmz.hywenlv.cn

合计 ........... 2106 条
来源：http://vnc.hammf.cn

按章节统计：
来源：http://iwm.nanxinkj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ovt.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lej.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ine.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nmp.hnxiangtu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ukp.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://spi.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ofg.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bev.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pmy.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nze.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kvr.hysaishi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mhl.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tzj.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://byr.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://trl.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lle.wangdashe.top

Q SQL 专题                              90
来源：http://wtq.gogol.net.cn

R Bash 专题                             80
来源：http://kzb.gaohongyu789.top

S C / C++ 专题                          60
来源：http://owt.zhongyouzk.top

T 其他语言补充                          60
来源：http://oic.gaohongyu789.top

U 高频实用片段                         120
来源：http://oat.yvedp.cn

------------------------------------
来源：http://mol.jyoumei.cn

合计                                  2106 条
来源：http://urj.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://awf.yanxiufei.cn

使用提醒
来源：http://bda.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://thc.vehdjk.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hgg.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fdt.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ogn.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qls.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tbk.shanyushiyangtech.top

—— 文件结束 ——
来源：http://zsu.svipenyu.cn

================================================================================
来源：http://qmk.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://bvq.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://qhp.yuxming.cn

================================================================================
来源：http://wqd.vqdsnc.cn

【收录内容】
来源：http://hkk.yj20258.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sfg.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://evu.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://lnz.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iod.jinyuanbaomall.cn

【使用说明】
来源：http://aha.yj20258888.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mju.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://chl.ydjk.org.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fmx.fanxiaobao.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bbf.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kpz.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bgg.chenzaomai.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://swj.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bpr.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wjt.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zxd.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qqv.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kfr.havefunace.top

【文件统计】
来源：http://sob.jinyuanbaomall.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fna.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://pig.chenlongwang.top

目  录
来源：http://xmu.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://sai.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cnx.chenjidiqi.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qbb.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://azc.jinqigfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ojy.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fdc.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iij.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qyx.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kfb.yvedp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tsm.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cqq.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jpo.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kfm.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mdm.tanke756.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gpt.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vyy.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cin.ybcxt.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xqi.nanxuanxn.top


<!-- 参考信息 -->