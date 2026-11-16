代发 wailian999

[U19] Py：正则替换带回调
来源：http://opw.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xmt.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://trz.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://yfn.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://gxq.svipenyu.cn

@contextlib.contextmanager
来源：http://cve.snrcjt.cn

[U22] Py：矩阵转置
来源：http://ean.guowangkeji.top

list(zip(*m))
来源：http://jgz.bjfxy.top

[U23] Py：分块读取大文件
来源：http://kba.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cwm.yuanzhike.top

[U24] Py：路径操作
来源：http://fbe.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://asm.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://tst.nanxuanxn.top

csv.DictReader(f)
来源：http://opk.vehdjk.com

[U26] Py：并发下载
来源：http://irt.316326.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yho.yongpay.top

[U27] Py：异步 HTTP
来源：http://kkn.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://dtt.feifeiyinyue.top

[U28] Py：类型别名
来源：http://ihc.xziqi.cn

UserId = int
来源：http://hip.sysykeji.top

[U29] Py：属性校验
来源：http://irp.tanke756.top

@property 与 @x.setter 配合
来源：http://yry.yongpay.top

[U30] Py：数据类
来源：http://glg.tanke756.top

@dataclass(slots=True)
来源：http://gcj.chenjidiqi.icu

[U31] Py：单测
来源：http://uzj.yangfankeji.com

python -m pytest -q
来源：http://aui.yangfankeji.com

[U32] Py：代码格式化
来源：http://eol.fzhhl.top

ruff format . && ruff check --fix .
来源：http://zrl.chenjidiqi.icu

[U33] Py：打包发布
来源：http://cub.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://xxn.zycfv.cn

[U34] Py：判断编码
来源：http://fup.wangdashe.top

chardet.detect(raw)
来源：http://dgd.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://qsa.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqo.zdqjudy.top

[U36] Py：定时任务
来源：http://cjc.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://fyr.haohaochexian.top

[U37] Py：读写 Excel
来源：http://zip.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vcb.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://vwp.daria6918.cn

Path(__file__).resolve().parent
来源：http://cbi.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://dyd.yj20258888.top

sys.stdout.isatty()
来源：http://jqn.daxiang520.top

[U40] Py：打印到标准错误
来源：http://aby.nanxuanxn.top

print("err", file=sys.stderr)
来源：http://wbd.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://nbp.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://obd.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://nka.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bfr.hnqzz.top

[U43] PHP：声明命名空间
来源：http://lxc.yangfankeji.com

namespace App\Http;
来源：http://gwl.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://nlm.ppjwa.cn

declare(strict_types=1);
来源：http://hvx.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://brg.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oew.gzhubu.top

[U46] PHP：可空类型
来源：http://ase.vqdsnc.cn

?string $name = null
来源：http://joe.hesvh.cn

[U47] PHP：联合类型
来源：http://kzr.nanxuanxn.top

int|string $id
来源：http://kqj.havefunace.top

[U48] PHP：纯枚举
来源：http://luh.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eqf.gotoacloud.top

[U49] PHP：只读属性
来源：http://fxe.dianchejie.cn

public readonly string $name
来源：http://dkp.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://sdm.316326.xyz

public function __construct(private int $id) {}
来源：http://zux.zhengqikj.top

[U51] PHP：数组解构
来源：http://pac.cdnleiting.top

[$a, $b] = $arr;
来源：http://dvi.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://atr.316326.xyz

$double = fn($x) => $x * 2;
来源：http://xjm.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://ovf.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://sdq.sxryk.cn

[U54] PHP：空安全调用
来源：http://nwx.ppjwa.cn

$obj?->method()
来源：http://fro.jqgfzy.top

[U55] PHP：match 表达式
来源：http://rzy.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://epv.yongpay.top

[U56] PHP：命名参数
来源：http://oig.yonumen.top

f(a: 1, b: 2)
来源：http://xzt.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://ype.jyoumei.cn

"值: {$a}"
来源：http://rye.daria6918.cn

[U58] PHP：数组三件套
来源：http://hmv.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lva.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://ugp.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrh.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://gin.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uyb.zdqjudy.top

[U61] PHP：正则
来源：http://thd.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eno.nanxuanxn.top

[U62] PHP：日期对象
来源：http://qec.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xww.chenlongwang.top

[U63] PHP：文件读写
来源：http://vkn.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cxz.c1oappe.top

[U64] PHP：目录遍历
来源：http://fae.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://zkm.zhijiandao.cn

[U65] PHP：会话
来源：http://ddy.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qmd.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://bae.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://auh.zhongyouzk.top

[U67] PHP：处理文件上传
来源：http://sos.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cmw.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://xnw.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://efg.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://ppw.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://duy.jianghu66.top

[U70] PHP：PDO 事务
来源：http://pmv.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iqb.shanyushiyangtech.top

[U71] PHP：抛出异常
来源：http://ksm.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://lkl.cheryme.top

[U72] PHP：写错误日志
来源：http://mhw.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://vhv.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://kni.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://ezy.mhx1999.top

[U74] PHP：读取环境变量
来源：http://uti.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://cce.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://rhr.ydzc1.top

composer require psr/container
来源：http://zel.smart0.xyz

[U76] PHP：简单路由
来源：http://nuw.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iey.yuanzhike.top

[U77] PHP：模板渲染
来源：http://hgy.jianghu66.top

composer require twig/twig
来源：http://ihx.bjfxy.top

[U78] PHP：单元测试
来源：http://xmn.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://kux.xylfe.cn

[U79] PHP：静态分析
来源：http://ltf.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://ikz.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://odt.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dnh.yonumen.top

[U81] JS：初始化项目
来源：http://buv.aizwys.cn

npm init -y;  npm i express
来源：http://bnf.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://usl.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cve.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://uor.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jwi.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://tcj.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://snd.cheryme.top

[U85] JS：可选链
来源：http://iec.yj20258.top

a?.b?.c
来源：http://ckt.nanxinkj.top

[U86] JS：空值合并
来源：http://fsq.yj20258888.top

a ?? b
来源：http://akg.andypj.xyz

[U87] JS：解构默认值
来源：http://wim.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://bbc.cucudq.cn

[U88] JS：对象展开合并
来源：http://mif.jinghuilouyu.cn

{ ...a, ...b }
来源：http://ogs.andypj.xyz

[U89] JS：数组去重
来源：http://rbb.shzxlz.cn

[...new Set(arr)]
来源：http://hxu.cqqwz.cn

[U90] JS：数字数组排序
来源：http://oov.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://lyy.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://bwg.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oxq.jinqigfzy.top

[U92] JS：深拷贝
来源：http://rla.xylfe.cn

structuredClone(obj)
来源：http://nec.guannengcc.top

[U93] JS：模板字符串
来源：http://rqg.iojbl.cn

`共 ${n} 条`
来源：http://bro.zhengqikj.top

[U94] JS：箭头函数
来源：http://puk.yj20258.top

const double = x => x * 2;
来源：http://xdh.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://eue.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://ugs.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://puq.hywenlv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xim.9152youxi.cn

[U97] JS：并发请求
来源：http://wnd.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rtf.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://wne.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iht.yonumen.top

[U99] JS：事件监听
来源：http://kkf.yongpay.top

el.addEventListener("click", e => {})
来源：http://pqq.daria6918.cn

[U100] JS：DOM 查询
来源：http://fbw.dianchejie.cn

document.querySelector(".item")
来源：http://kpg.hammf.cn

[U101] JS：classList 操作
来源：http://aej.chenlongwang.top

el.classList.toggle("active")
来源：http://ftb.jianghu66.top

[U102] JS：本地存储
来源：http://dkb.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://txi.guannengcc.top

[U103] JS：定时器
来源：http://mrp.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cnt.yvedp.cn

[U104] JS：防抖
来源：http://gnb.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kix.shuidangran.top

[U105] JS：节流
来源：http://zfx.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bwt.epnwcf.com

[U106] JS：日期格式化
来源：http://lmh.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vfp.iojbl.cn

[U107] JS：数字千分位
来源：http://lkl.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ebc.aibaodan.cn

[U108] JS：随机整数
来源：http://pvb.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://byi.fehbvm.com

[U109] JS：数组分组
来源：http://hoo.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://vve.jyoumei.cn

[U110] JS：数组分块
来源：http://djo.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hzt.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://duk.birdmap.top

new Map(Object.entries(obj))
来源：http://xud.yj202588.top

[U112] JS：字符串补位
来源：http://nnt.meibo888.top

"7".padStart(3, "0")
来源：http://owm.jinqigufen.top

[U113] JS：正则替换全部
来源：http://wif.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://vqt.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://qlf.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rwz.shuidangran.top

[U115] JS：生成 UUID
来源：http://ezu.tanke756.top

crypto.randomUUID()
来源：http://qst.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://vvw.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://bzp.sweek.top

[U117] JS：单元测试
来源：http://zrx.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://cgs.ppjwa.cn

[U118] JS：开发服务器
来源：http://xif.daria6918.cn

npm i -D vite;  npx vite
来源：http://dvk.jqgfzy.top

[U119] JS：生产构建
来源：http://dac.gotoacloud.top

npx vite build
来源：http://sqi.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://ltn.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://peq.uphjek.com

================================================================================
来源：http://hmx.ehwqpu.com

统计汇总
来源：http://yme.jqgufenzy.top

================================================================================
来源：http://osy.yj202588.top

按语言统计（条）：
来源：http://szc.gogol.net.cn

Python ......... 252
来源：http://fmf.shzxlz.cn

PHP ............ 252
来源：http://tdv.gzhubu.top

JavaScript ..... 252
来源：http://zrt.andypj.xyz

TypeScript ..... 212
来源：http://rqm.svipenyu.cn

Java ........... 212
来源：http://dch.dashuyun.cn

Go ............. 212
来源：http://cea.jqgufenzy.top

Ruby ........... 212
来源：http://svx.xinyue.icu

C# ............. 212
来源：http://jti.jqgufenzy.top

C .............. 30
来源：http://xwz.havefunace.top

C++ ............ 30
来源：http://szi.cheryme.top

SQL ............ 90
来源：http://epc.xuetiantiany.cn

Bash ........... 80
来源：http://tpv.pycfn.com

Kotlin ......... 15
来源：http://omg.shanyushiyangkeji.top

Swift .......... 15
来源：http://zah.zhongyouzk.top

Lua ............ 10
来源：http://hqn.jyoumei.cn

Perl ........... 10
来源：http://bts.jinyuanbaomall.cn

Scala .......... 10
来源：http://uzx.yuxming.cn

------------------------------------
来源：http://fqt.sysykeji.top

合计 ........... 2106 条
来源：http://kct.mhx1999.top

按章节统计：
来源：http://cve.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zxv.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dum.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://flk.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://grg.yuanzhike.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ibw.sysykeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pzx.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uvs.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jus.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sur.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ech.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hkb.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fge.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://asm.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://azh.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tyb.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://czx.bjfxy.top

Q SQL 专题                              90
来源：http://tcg.xuetiantiany.cn

R Bash 专题                             80
来源：http://yuk.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://vtk.hysaishi.cn

T 其他语言补充                          60
来源：http://klm.wangdashe.top

U 高频实用片段                         120
来源：http://srz.ehwqpu.com

------------------------------------
来源：http://cur.hysaishi.cn

合计                                  2106 条
来源：http://xev.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://okq.c1oappe.top

使用提醒
来源：http://drv.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://qki.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fyp.52xcode.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yqv.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lcz.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nss.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zva.yj20258.top

—— 文件结束 ——
来源：http://wtd.hesvh.cn

================================================================================
来源：http://ecc.wangshuangyany.cn

程序语言常见例子速查手册（2024 版）
来源：http://eee.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://fld.zdqjudy.top

================================================================================
来源：http://har.zhoulong.xyz

【收录内容】
来源：http://pkw.0kj1m.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://onf.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mww.sjlbkw.cn

SQL · Bash · C · C++
来源：http://owu.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wca.hywenlv.cn

【使用说明】
来源：http://slg.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kno.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hkd.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qko.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rtm.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ufk.sweek.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zht.zhongyouzk.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zvc.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uba.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ryq.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xey.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://usl.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yir.feifeiyinyue.top

【文件统计】
来源：http://vfr.0kj1m.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eof.iojbl.cn

--------------------------------------------------------------------------------
来源：http://utj.aibaodan.cn

目  录
来源：http://oev.birdmap.top

--------------------------------------------------------------------------------
来源：http://znr.xuanzx.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yip.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eti.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mfy.chenjidiqi.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fez.mhx1999.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vwx.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vad.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iox.mhx1999.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kav.xinyue.icu

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xbd.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://klg.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gpa.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dvo.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ilj.fzhhl.top


<!-- 参考信息 -->