代发 wailian999

[U19] Py：正则替换带回调
来源：http://rcg.xylfe.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://liz.smart0.xyz

[U20] Py：缓存函数结果
来源：http://arj.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://xyj.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://zot.fktsv.cn

@contextlib.contextmanager
来源：http://loa.sysykeji.top

[U22] Py：矩阵转置
来源：http://snq.ybcxt.top

list(zip(*m))
来源：http://mmm.cheryme.top

[U23] Py：分块读取大文件
来源：http://boh.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bho.9152youxi.cn

[U24] Py：路径操作
来源：http://bwr.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zum.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://pvm.yanxiufei.cn

csv.DictReader(f)
来源：http://tie.yongpay.top

[U26] Py：并发下载
来源：http://dfu.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nqg.316326.xyz

[U27] Py：异步 HTTP
来源：http://nqw.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://akm.mhx1999.top

[U28] Py：类型别名
来源：http://paj.ppjwa.cn

UserId = int
来源：http://oqr.sxryk.cn

[U29] Py：属性校验
来源：http://nli.birdmap.top

@property 与 @x.setter 配合
来源：http://nir.hesvh.cn

[U30] Py：数据类
来源：http://zyz.shanyushiyangtech.top

@dataclass(slots=True)
来源：http://ozw.sweek.top

[U31] Py：单测
来源：http://lxo.daxiang520.top

python -m pytest -q
来源：http://nae.quarkkingdee.top

[U32] Py：代码格式化
来源：http://hvy.52xcode.cn

ruff format . && ruff check --fix .
来源：http://ccm.xinyue.icu

[U33] Py：打包发布
来源：http://icn.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://pbm.tarul.cn

[U34] Py：判断编码
来源：http://dlk.wangdashe.top

chardet.detect(raw)
来源：http://igo.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://yje.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uuy.vehdjk.com

[U36] Py：定时任务
来源：http://qgq.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://hkk.hysaishi.cn

[U37] Py：读写 Excel
来源：http://nge.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://jwd.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://err.zhixingplan.top

Path(__file__).resolve().parent
来源：http://pyo.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://ajq.chenlongwang.top

sys.stdout.isatty()
来源：http://rfp.xziqi.cn

[U40] Py：打印到标准错误
来源：http://oln.bbcook.cn

print("err", file=sys.stderr)
来源：http://ytv.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://kww.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wdd.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://mbw.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ayh.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://smz.xziqi.cn

namespace App\Http;
来源：http://wzg.bjfxy.top

[U44] PHP：开启严格类型
来源：http://gie.ivvv.top

declare(strict_types=1);
来源：http://gxu.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://iyr.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uws.pycfn.com

[U46] PHP：可空类型
来源：http://aks.nanxuanxn.top

?string $name = null
来源：http://ilm.jqgufenzy.top

[U47] PHP：联合类型
来源：http://gyr.yj202588.top

int|string $id
来源：http://cnx.yj202588.top

[U48] PHP：纯枚举
来源：http://olq.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ohu.yueranfly.top

[U49] PHP：只读属性
来源：http://emi.wangdashe.top

public readonly string $name
来源：http://cve.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://wjc.tianlin.xyz

public function __construct(private int $id) {}
来源：http://pwa.jiagoushi.top

[U51] PHP：数组解构
来源：http://nsm.fzhhl.top

[$a, $b] = $arr;
来源：http://gpr.316326.xyz

[U52] PHP：箭头函数
来源：http://yao.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://tyo.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://elq.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://rdd.hfpthk.cn

[U54] PHP：空安全调用
来源：http://age.hammf.cn

$obj?->method()
来源：http://nvw.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://nku.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iqw.xylfe.cn

[U56] PHP：命名参数
来源：http://qgs.redwolf501.top

f(a: 1, b: 2)
来源：http://jlq.aibaodan.cn

[U57] PHP：字符串插值
来源：http://lce.zhongyouzk.top

"值: {$a}"
来源：http://qxr.9152youxi.cn

[U58] PHP：数组三件套
来源：http://etr.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eok.dashuyun.cn

[U59] PHP：自定义排序
来源：http://ctd.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujb.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://irv.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hff.chenzaomai.com

[U61] PHP：正则
来源：http://bnq.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kqb.sxryk.cn

[U62] PHP：日期对象
来源：http://cjx.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://brv.iojbl.cn

[U63] PHP：文件读写
来源：http://yys.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sqh.ctjpmb.com

[U64] PHP：目录遍历
来源：http://wtt.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://vfk.gaohongyu789.top

[U65] PHP：会话
来源：http://fbr.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jpf.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://ejl.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dqv.tarul.cn

[U67] PHP：处理文件上传
来源：http://vhy.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pyk.bbcook.cn

[U68] PHP：PDO 连接
来源：http://ybc.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blz.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://upg.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kwq.fzhhl.top

[U70] PHP：PDO 事务
来源：http://fwa.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xwe.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://qzy.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://drl.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://xww.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://hsk.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://wgk.havefunace.top

parse_ini_file("config.ini", true)
来源：http://mbw.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://met.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://zwi.daria6918.cn

[U75] PHP：依赖注入
来源：http://wnz.hesvh.cn

composer require psr/container
来源：http://yaj.aibaodan.cn

[U76] PHP：简单路由
来源：http://fkg.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vbc.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://zqh.ivvv.top

composer require twig/twig
来源：http://cgn.vqdsnc.cn

[U78] PHP：单元测试
来源：http://bfa.havefunace.top

composer require --dev phpunit/phpunit
来源：http://ngm.hesvh.cn

[U79] PHP：静态分析
来源：http://atx.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://oqh.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://szd.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hmq.chenzaomai.com

[U81] JS：初始化项目
来源：http://lgb.zhongyouzk.top

npm init -y;  npm i express
来源：http://sza.fehbvm.com

[U82] JS：package.json 脚本
来源：http://vea.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://woc.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://zfj.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://ben.hammf.cn

[U84] JS：CommonJS 写法
来源：http://pzy.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://lvb.zhengqikj.top

[U85] JS：可选链
来源：http://vou.quarkkingdee.top

a?.b?.c
来源：http://iko.sxryk.cn

[U86] JS：空值合并
来源：http://eta.chenjidiqi.icu

a ?? b
来源：http://asz.jinqigufen.top

[U87] JS：解构默认值
来源：http://hnt.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://kyb.yuanzhike.top

[U88] JS：对象展开合并
来源：http://sfo.hesvh.cn

{ ...a, ...b }
来源：http://qks.c1oappe.top

[U89] JS：数组去重
来源：http://aqa.svipenyu.cn

[...new Set(arr)]
来源：http://agy.tarul.cn

[U90] JS：数字数组排序
来源：http://fun.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://qha.52xcode.cn

[U91] JS：对象键值遍历
来源：http://ddi.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bdq.zdqjudy.top

[U92] JS：深拷贝
来源：http://bzu.yvedp.cn

structuredClone(obj)
来源：http://wcf.chenlongwang.top

[U93] JS：模板字符串
来源：http://opt.dianchejie.cn

`共 ${n} 条`
来源：http://iro.zdqjudy.top

[U94] JS：箭头函数
来源：http://waz.chenzaomai.com

const double = x => x * 2;
来源：http://vqw.cqqwz.cn

[U95] JS：Promise 包装
来源：http://hcj.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://qhq.uphjek.com

[U96] JS：async/await 与异常
来源：http://qao.ybcxt.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rxn.tarul.cn

[U97] JS：并发请求
来源：http://wjv.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bbj.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://gdy.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://grv.ydjk.org.cn

[U99] JS：事件监听
来源：http://dtn.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://iet.yj202588.top

[U100] JS：DOM 查询
来源：http://rfs.quarkkingdee.top

document.querySelector(".item")
来源：http://ylg.yueranfly.top

[U101] JS：classList 操作
来源：http://syd.fehbvm.com

el.classList.toggle("active")
来源：http://vfv.snrcjt.cn

[U102] JS：本地存储
来源：http://iny.nwbrower.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vwg.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://bbi.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fwu.jiagoushi.top

[U104] JS：防抖
来源：http://vbj.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvi.yanxiufei.cn

[U105] JS：节流
来源：http://hjv.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://exe.yangfankeji.com

[U106] JS：日期格式化
来源：http://lfm.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qjf.redwolf501.top

[U107] JS：数字千分位
来源：http://ibt.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yqm.havefunace.top

[U108] JS：随机整数
来源：http://mab.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lxr.sweek.top

[U109] JS：数组分组
来源：http://ckr.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://zhy.zhengqikj.top

[U110] JS：数组分块
来源：http://yzz.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tfz.aizwys.cn

[U111] JS：对象转 Map
来源：http://bkr.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://wyi.hammf.cn

[U112] JS：字符串补位
来源：http://moh.quarkkingdee.top

"7".padStart(3, "0")
来源：http://vml.vehdjk.com

[U113] JS：正则替换全部
来源：http://mvp.cqqwz.cn

s.replaceAll("a", "b")
来源：http://cty.yvedp.cn

[U114] JS：JSON 深比较
来源：http://ztc.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://auq.yj202588.top

[U115] JS：生成 UUID
来源：http://tik.kuanghao11.cn

crypto.randomUUID()
来源：http://qyn.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://hgu.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://bxk.xylfe.cn

[U117] JS：单元测试
来源：http://obp.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://rpw.ydjk.org.cn

[U118] JS：开发服务器
来源：http://aer.zycfv.cn

npm i -D vite;  npx vite
来源：http://ypz.fktsv.cn

[U119] JS：生产构建
来源：http://yea.vehdjk.com

npx vite build
来源：http://vfq.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://cwo.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://bqr.fehbvm.com

================================================================================
来源：http://jtt.shangyingyoupin.top

统计汇总
来源：http://kuz.yuxming.cn

================================================================================
来源：http://azh.jlsjyb.cn

按语言统计（条）：
来源：http://qqb.gotoacloud.top

Python ......... 252
来源：http://fsd.xuetiantiany.cn

PHP ............ 252
来源：http://dyt.meibo888.top

JavaScript ..... 252
来源：http://haa.daria6918.cn

TypeScript ..... 212
来源：http://jsz.chenjidiqi.icu

Java ........... 212
来源：http://eqr.ydzc1.top

Go ............. 212
来源：http://lhb.xziqi.cn

Ruby ........... 212
来源：http://pop.hcnkem.com

C# ............. 212
来源：http://oxo.cdnleiting.top

C .............. 30
来源：http://blr.nwbrower.top

C++ ............ 30
来源：http://ncv.gotoacloud.top

SQL ............ 90
来源：http://lyq.c1oappe.top

Bash ........... 80
来源：http://jup.zhengqikj.top

Kotlin ......... 15
来源：http://cqa.ehwqpu.com

Swift .......... 15
来源：http://bbf.316326.xyz

Lua ............ 10
来源：http://emh.snrcjt.cn

Perl ........... 10
来源：http://dbc.tian-w.cn

Scala .......... 10
来源：http://lei.dashuyun.cn

------------------------------------
来源：http://wbf.9152youxi.cn

合计 ........... 2106 条
来源：http://jmt.havefunace.top

按章节统计：
来源：http://oro.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rnz.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ese.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ldt.fengsongda.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uip.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fws.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cxz.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eco.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://whp.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bsf.ydjk.org.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fow.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xib.316326.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://riz.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yzt.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lqk.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xpc.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fyx.chenzaomai.com

Q SQL 专题                              90
来源：http://etv.hongshengwenyu.top

R Bash 专题                             80
来源：http://aik.jyoumei.cn

S C / C++ 专题                          60
来源：http://syp.meibo888.top

T 其他语言补充                          60
来源：http://oty.fktsv.cn

U 高频实用片段                         120
来源：http://aze.0kj1m.cn

------------------------------------
来源：http://dwp.dashuyun.cn

合计                                  2106 条
来源：http://dbs.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://xgk.pycfn.com

使用提醒
来源：http://lcr.ydzc1.top

--------------------------------------------------------------------------------
来源：http://ohf.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lqi.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qkr.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xqx.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://djh.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://isn.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://vse.dashuyun.cn

================================================================================
来源：http://rrj.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://shm.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://cka.cqqwz.cn

================================================================================
来源：http://bnp.bbcook.cn

【收录内容】
来源：http://gwc.hfpthk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ssv.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://aql.c1oappe.top

SQL · Bash · C · C++
来源：http://rbv.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ouk.sxryk.cn

【使用说明】
来源：http://gkl.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lwc.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xjf.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mkm.chenlongwang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oik.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uwt.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dwo.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jum.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hyo.zhongyouzk.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://onc.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xte.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ewc.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iav.ydzc1.top

【文件统计】
来源：http://mbd.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://okl.aizwys.cn

--------------------------------------------------------------------------------
来源：http://gac.haohaochexian.top

目  录
来源：http://mhn.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://jab.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dnp.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gef.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fys.guannengcc.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://swv.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://myr.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ksp.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mvk.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hmh.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nwi.jinghuilouyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jfp.ydzc1.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://csm.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ffo.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://exs.uphjek.com


<!-- 参考信息 -->