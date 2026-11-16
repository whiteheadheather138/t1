代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://vog.cdnleiting.top

@contextlib.contextmanager
来源：http://wuj.jqgfzy.top

[U22] Py：矩阵转置
来源：http://xza.quarkkingdee.top

list(zip(*m))
来源：http://nlj.hesvh.cn

[U23] Py：分块读取大文件
来源：http://yqu.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hny.feifeiyinyue.top

[U24] Py：路径操作
来源：http://dma.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vkc.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://isl.zhengqikj.top

csv.DictReader(f)
来源：http://woq.zhengqikj.top

[U26] Py：并发下载
来源：http://cob.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vlg.uphjek.com

[U27] Py：异步 HTTP
来源：http://djq.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://wme.nanxinkj.top

[U28] Py：类型别名
来源：http://ivi.ybcxt.top

UserId = int
来源：http://nuu.0kj1m.cn

[U29] Py：属性校验
来源：http://zdo.zhixingplan.top

@property 与 @x.setter 配合
来源：http://wcj.sweek.top

[U30] Py：数据类
来源：http://bwx.meibo888.top

@dataclass(slots=True)
来源：http://sxj.pengpengdd.cyou

[U31] Py：单测
来源：http://kjb.ywan-chungtsiang.top

python -m pytest -q
来源：http://xrg.snrcjt.cn

[U32] Py：代码格式化
来源：http://qoq.tarul.cn

ruff format . && ruff check --fix .
来源：http://kdb.hesvh.cn

[U33] Py：打包发布
来源：http://zxd.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://xph.yfazqb.com

[U34] Py：判断编码
来源：http://ryu.snrcjt.cn

chardet.detect(raw)
来源：http://ssb.ehwqpu.com

[U35] Py：发送邮件
来源：http://mzu.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zmp.ppjwa.cn

[U36] Py：定时任务
来源：http://zid.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://tot.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://zvn.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://xmq.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://dcr.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://epr.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://vwn.cucudq.cn

sys.stdout.isatty()
来源：http://vfx.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://qrr.zycfv.cn

print("err", file=sys.stderr)
来源：http://ezu.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://coy.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mpd.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://nln.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bjc.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://nfg.uphjek.com

namespace App\Http;
来源：http://zos.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://yjo.tian-w.cn

declare(strict_types=1);
来源：http://ury.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://yve.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pkp.havefunace.top

[U46] PHP：可空类型
来源：http://twr.nanxuanxn.top

?string $name = null
来源：http://ohy.zhengqikj.top

[U47] PHP：联合类型
来源：http://pze.sjlbkw.cn

int|string $id
来源：http://bfz.tian-w.cn

[U48] PHP：纯枚举
来源：http://wrm.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pgi.316326.xyz

[U49] PHP：只读属性
来源：http://hxx.shzxlz.cn

public readonly string $name
来源：http://kxz.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://isw.ppjwa.cn

public function __construct(private int $id) {}
来源：http://knh.ybcxt.top

[U51] PHP：数组解构
来源：http://pzb.guowangkeji.top

[$a, $b] = $arr;
来源：http://ehx.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://mjj.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://eae.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://jru.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://rkl.xuanzx.com

[U54] PHP：空安全调用
来源：http://rfs.jinyuanbaomall.cn

$obj?->method()
来源：http://vyp.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://rny.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gdt.chenzaomai.com

[U56] PHP：命名参数
来源：http://mvh.yuanzhike.top

f(a: 1, b: 2)
来源：http://slx.nanxinkj.top

[U57] PHP：字符串插值
来源：http://oqt.tianlin.xyz

"值: {$a}"
来源：http://bhm.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://czr.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oaj.redwolf501.top

[U59] PHP：自定义排序
来源：http://sit.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zly.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://ljv.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zhh.ydzc1.top

[U61] PHP：正则
来源：http://qjw.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vgx.hnxiangtu.top

[U62] PHP：日期对象
来源：http://pfd.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xuq.cheryme.top

[U63] PHP：文件读写
来源：http://dfy.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jfe.yonumen.top

[U64] PHP：目录遍历
来源：http://wlg.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://ojp.vehdjk.com

[U65] PHP：会话
来源：http://lah.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rsi.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://wml.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uvc.iojbl.cn

[U67] PHP：处理文件上传
来源：http://srm.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xhi.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://fmx.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cup.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://mln.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eox.cashguo.top

[U70] PHP：PDO 事务
来源：http://kme.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wti.hammf.cn

[U71] PHP：抛出异常
来源：http://gat.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://vtk.birdmap.top

[U72] PHP：写错误日志
来源：http://wft.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://ino.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://iuz.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://gws.cucudq.cn

[U74] PHP：读取环境变量
来源：http://pdl.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://pty.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://eph.iojbl.cn

composer require psr/container
来源：http://tqw.aizwys.cn

[U76] PHP：简单路由
来源：http://zrl.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hmn.meibo888.top

[U77] PHP：模板渲染
来源：http://ylk.cashguo.top

composer require twig/twig
来源：http://mlp.yuxming.cn

[U78] PHP：单元测试
来源：http://dmh.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://grh.guowangkeji.top

[U79] PHP：静态分析
来源：http://mpo.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://spn.xinyue.icu

[U80] PHP：代码规范修复
来源：http://mrx.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://itk.havefunace.top

[U81] JS：初始化项目
来源：http://hza.guowangkeji.top

npm init -y;  npm i express
来源：http://lcc.sufxvd.cn

[U82] JS：package.json 脚本
来源：http://hnf.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xkl.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://nqi.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://aqv.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://uaa.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://jtm.jlsjyb.cn

[U85] JS：可选链
来源：http://psy.gotoacloud.top

a?.b?.c
来源：http://gce.haohaochexian.top

[U86] JS：空值合并
来源：http://pbf.cashguo.top

a ?? b
来源：http://trm.dianchejie.cn

[U87] JS：解构默认值
来源：http://eet.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://vkb.nwbrower.top

[U88] JS：对象展开合并
来源：http://qye.iojbl.cn

{ ...a, ...b }
来源：http://iwt.tian-w.cn

[U89] JS：数组去重
来源：http://fya.smart0.xyz

[...new Set(arr)]
来源：http://phx.yueranfly.top

[U90] JS：数字数组排序
来源：http://bst.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://esf.fzhhl.top

[U91] JS：对象键值遍历
来源：http://wml.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aho.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://gfb.c1oappe.top

structuredClone(obj)
来源：http://dht.uphjek.com

[U93] JS：模板字符串
来源：http://xba.zhiwuduotai.top

`共 ${n} 条`
来源：http://vnt.pycfn.com

[U94] JS：箭头函数
来源：http://uvu.jinqigfzy.top

const double = x => x * 2;
来源：http://dzm.yonumen.top

[U95] JS：Promise 包装
来源：http://gfr.jqgufenzy.top

new Promise((resolve, reject) => {})
来源：http://cfn.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://sgd.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dje.sxryk.cn

[U97] JS：并发请求
来源：http://voi.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://diy.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://not.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qlw.zdbjq.cn

[U99] JS：事件监听
来源：http://yze.cheryme.top

el.addEventListener("click", e => {})
来源：http://dxs.gotoacloud.top

[U100] JS：DOM 查询
来源：http://eie.guowangkeji.top

document.querySelector(".item")
来源：http://yky.tianlin.xyz

[U101] JS：classList 操作
来源：http://ran.hnqzz.top

el.classList.toggle("active")
来源：http://cyx.zhixingplan.top

[U102] JS：本地存储
来源：http://mvl.chenlongwang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xqe.sjlbkw.cn

[U103] JS：定时器
来源：http://goh.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ucc.sweek.top

[U104] JS：防抖
来源：http://hqj.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gzt.quarkkingdee.top

[U105] JS：节流
来源：http://aaz.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nsf.havefunace.top

[U106] JS：日期格式化
来源：http://vjv.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ira.epnwcf.com

[U107] JS：数字千分位
来源：http://nol.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://szx.birdmap.top

[U108] JS：随机整数
来源：http://vxj.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kuf.cdnleiting.top

[U109] JS：数组分组
来源：http://vya.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://lci.kuanghao11.cn

[U110] JS：数组分块
来源：http://dug.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xaf.hammf.cn

[U111] JS：对象转 Map
来源：http://bfe.epnwcf.com

new Map(Object.entries(obj))
来源：http://hrr.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://vmf.quarkkingdee.top

"7".padStart(3, "0")
来源：http://yyi.daria6918.cn

[U113] JS：正则替换全部
来源：http://yak.daxiang520.top

s.replaceAll("a", "b")
来源：http://krt.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://phz.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hgt.nanxinkj.top

[U115] JS：生成 UUID
来源：http://uau.iojbl.cn

crypto.randomUUID()
来源：http://fel.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://xnx.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://ruf.fzhhl.top

[U117] JS：单元测试
来源：http://mod.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://dpx.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://dgb.ivvv.top

npm i -D vite;  npx vite
来源：http://utw.hongshengwenyu.top

[U119] JS：生产构建
来源：http://fvt.jinyuanbaomall.cn

npx vite build
来源：http://wxo.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://ulk.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://oqa.kuanghao11.cn

================================================================================
来源：http://ubv.svipenyu.cn

统计汇总
来源：http://rey.shangyingyoupin.top

================================================================================
来源：http://zfx.vehdjk.com

按语言统计（条）：
来源：http://hkk.meibo888.top

Python ......... 252
来源：http://pde.dianchejie.cn

PHP ............ 252
来源：http://qem.zhoulong.xyz

JavaScript ..... 252
来源：http://pwa.yj202588.top

TypeScript ..... 212
来源：http://tzk.zhiwuduotai.top

Java ........... 212
来源：http://eih.haohaochexian.top

Go ............. 212
来源：http://tap.tian-w.cn

Ruby ........... 212
来源：http://uqk.fanxiaobao.xyz

C# ............. 212
来源：http://mfm.aibaodan.cn

C .............. 30
来源：http://mdx.shzxlz.cn

C++ ............ 30
来源：http://pel.snrcjt.cn

SQL ............ 90
来源：http://gev.hongshengwenyu.top

Bash ........... 80
来源：http://wqu.sxryk.cn

Kotlin ......... 15
来源：http://kje.havefunace.top

Swift .......... 15
来源：http://lnh.mhx1999.top

Lua ............ 10
来源：http://ffe.meibo888.top

Perl ........... 10
来源：http://sro.zhixingplan.top

Scala .......... 10
来源：http://uhz.9152youxi.cn

------------------------------------
来源：http://gjf.daria6918.cn

合计 ........... 2106 条
来源：http://iii.yvedp.cn

按章节统计：
来源：http://jdz.yvedp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fyo.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ymd.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jsp.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zoq.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://msq.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ekx.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://olu.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ake.cdnleiting.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lrr.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iod.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zda.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cbe.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ioh.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sbq.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://anx.guowangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://shm.yangfankeji.com

Q SQL 专题                              90
来源：http://brx.gotoacloud.top

R Bash 专题                             80
来源：http://mbq.wangdashe.top

S C / C++ 专题                          60
来源：http://hco.sufxvd.cn

T 其他语言补充                          60
来源：http://jja.feifeiyinyue.top

U 高频实用片段                         120
来源：http://lmq.yuxming.cn

------------------------------------
来源：http://ext.quarkkingdee.top

合计                                  2106 条
来源：http://jvg.cashguo.top

--------------------------------------------------------------------------------
来源：http://ece.yanxiufei.cn

使用提醒
来源：http://rgt.xylfe.cn

--------------------------------------------------------------------------------
来源：http://tgp.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://glr.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gdu.tian-w.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://daw.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pfd.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nxo.9152youxi.cn

—— 文件结束 ——
来源：http://lwj.cheryme.top

================================================================================
来源：http://wox.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://vor.ivvv.top

Common Programming Examples Cheat Book
来源：http://epy.smart0.xyz

================================================================================
来源：http://ljb.bbcook.cn

【收录内容】
来源：http://vyl.jinqigfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pio.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fzu.yj20258888.top

SQL · Bash · C · C++
来源：http://tyf.zhijiandao.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://twr.xinyue.icu

【使用说明】
来源：http://tcx.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vlq.shzxlz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qdr.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iqm.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bie.zhengqikj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ybd.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vpt.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wln.hammf.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://akn.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lxf.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jys.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jdo.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wpj.uphjek.com

【文件统计】
来源：http://ttt.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fqo.wangdashe.top

--------------------------------------------------------------------------------
来源：http://qgx.guowangkeji.top

目  录
来源：http://ayu.birdmap.top

--------------------------------------------------------------------------------
来源：http://phz.kuanghao11.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sev.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dgn.yfazqb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yvo.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://enf.dashuyun.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wzf.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wnj.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://omd.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nvs.uphjek.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://soy.redwolf501.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mmr.xylfe.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ymx.gotoacloud.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yqk.fktsv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wrl.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gfr.fanxiaobao.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gbb.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lto.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tcx.sxryk.cn


<!-- 参考信息 -->