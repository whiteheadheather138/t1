代发 wailian999

[U17] Py：初始化日志
来源：http://cqr.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://baa.yfazqb.com

[U18] Py：预编译正则
来源：http://obj.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://mmk.ybcxt.top

[U19] Py：正则替换带回调
来源：http://kzo.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lmz.tarul.cn

[U20] Py：缓存函数结果
来源：http://nca.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://uxl.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://exk.sjlbkw.cn

@contextlib.contextmanager
来源：http://phm.birdmap.top

[U22] Py：矩阵转置
来源：http://qvn.wangshuangyany.cn

list(zip(*m))
来源：http://yhx.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://avj.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sbq.gzhubu.top

[U24] Py：路径操作
来源：http://oxa.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qqa.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://tnt.9152youxi.cn

csv.DictReader(f)
来源：http://ejt.yuxming.cn

[U26] Py：并发下载
来源：http://ala.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fbe.sxryk.cn

[U27] Py：异步 HTTP
来源：http://ljl.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://byu.snrcjt.cn

[U28] Py：类型别名
来源：http://zof.shangyingyoupin.top

UserId = int
来源：http://nig.jlsjyb.cn

[U29] Py：属性校验
来源：http://hfp.jqgfzy.top

@property 与 @x.setter 配合
来源：http://wkr.hcnkem.com

[U30] Py：数据类
来源：http://flj.pycfn.com

@dataclass(slots=True)
来源：http://ary.fengsongda.top

[U31] Py：单测
来源：http://hnc.gaohongyu789.top

python -m pytest -q
来源：http://ppu.zhijiandao.cn

[U32] Py：代码格式化
来源：http://lqu.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://vdt.hnqzz.top

[U33] Py：打包发布
来源：http://dac.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://psj.hnqzz.top

[U34] Py：判断编码
来源：http://mmc.yueranfly.top

chardet.detect(raw)
来源：http://vwq.tanke756.top

[U35] Py：发送邮件
来源：http://eay.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://imd.aibaodan.cn

[U36] Py：定时任务
来源：http://etb.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://nmk.yuanzhike.top

[U37] Py：读写 Excel
来源：http://cgm.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://qvj.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://ilo.birdmap.top

Path(__file__).resolve().parent
来源：http://wsc.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://jna.yonumen.top

sys.stdout.isatty()
来源：http://bee.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://mms.xinyue.icu

print("err", file=sys.stderr)
来源：http://cxm.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://igz.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zys.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://ess.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gyw.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://bni.xingfuxueyuan.xyz

namespace App\Http;
来源：http://uqw.hammf.cn

[U44] PHP：开启严格类型
来源：http://nxi.zdqjudy.top

declare(strict_types=1);
来源：http://ihj.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://mkp.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zsi.bjfxy.top

[U46] PHP：可空类型
来源：http://age.nanxuanxn.top

?string $name = null
来源：http://yuf.aibaodan.cn

[U47] PHP：联合类型
来源：http://xex.fzhhl.top

int|string $id
来源：http://kyw.wangdashe.top

[U48] PHP：纯枚举
来源：http://rfk.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gxv.yvedp.cn

[U49] PHP：只读属性
来源：http://tai.chenjidiqi.icu

public readonly string $name
来源：http://obb.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://wls.fktsv.cn

public function __construct(private int $id) {}
来源：http://dev.xylfe.cn

[U51] PHP：数组解构
来源：http://sxv.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://ynh.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://qza.tarul.cn

$double = fn($x) => $x * 2;
来源：http://vpm.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://egd.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://bhk.yonumen.top

[U54] PHP：空安全调用
来源：http://bce.smart0.xyz

$obj?->method()
来源：http://mdi.c1oappe.top

[U55] PHP：match 表达式
来源：http://xvy.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cdu.sweek.top

[U56] PHP：命名参数
来源：http://oia.fengsongda.top

f(a: 1, b: 2)
来源：http://obj.shzxlz.cn

[U57] PHP：字符串插值
来源：http://vln.jianghu66.top

"值: {$a}"
来源：http://lmy.yongpay.top

[U58] PHP：数组三件套
来源：http://ttb.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jjv.redwolf501.top

[U59] PHP：自定义排序
来源：http://yll.zhiwuduotai.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rks.jqgufenzy.top

[U60] PHP：JSON 编解码
来源：http://sjt.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rfe.hcnkem.com

[U61] PHP：正则
来源：http://drt.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wwb.hammf.cn

[U62] PHP：日期对象
来源：http://oxg.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hsw.jqgfzy.top

[U63] PHP：文件读写
来源：http://dzo.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hea.hywenlv.cn

[U64] PHP：目录遍历
来源：http://tij.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://vuf.cashguo.top

[U65] PHP：会话
来源：http://mex.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bgv.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://myt.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lux.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://liw.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jtj.xuanzx.com

[U68] PHP：PDO 连接
来源：http://ifv.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ouj.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://jpi.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ipe.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://zaw.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fnb.zdqjudy.top

[U71] PHP：抛出异常
来源：http://qjl.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://lhq.shzxlz.cn

[U72] PHP：写错误日志
来源：http://ebb.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://vzs.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://urv.cashguo.top

parse_ini_file("config.ini", true)
来源：http://vbc.cheryme.top

[U74] PHP：读取环境变量
来源：http://ynj.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://cts.jqgfzy.top

[U75] PHP：依赖注入
来源：http://uwa.zhijiandao.cn

composer require psr/container
来源：http://bwa.ppjwa.cn

[U76] PHP：简单路由
来源：http://egm.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tyg.zhixingplan.top

[U77] PHP：模板渲染
来源：http://yii.chenlongwang.top

composer require twig/twig
来源：http://hjn.vehdjk.com

[U78] PHP：单元测试
来源：http://qud.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://zgt.havefunace.top

[U79] PHP：静态分析
来源：http://tez.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://iic.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://vae.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://thp.ctjpmb.com

[U81] JS：初始化项目
来源：http://osd.yj20258888.top

npm init -y;  npm i express
来源：http://vvr.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://vgj.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gef.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://myn.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://isz.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://mwz.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://wio.cashguo.top

[U85] JS：可选链
来源：http://ebs.yongpay.top

a?.b?.c
来源：http://tti.yongpay.top

[U86] JS：空值合并
来源：http://fjf.52xcode.cn

a ?? b
来源：http://oqj.yangfankeji.com

[U87] JS：解构默认值
来源：http://mje.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://hzo.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://gno.uphjek.com

{ ...a, ...b }
来源：http://css.sjlbkw.cn

[U89] JS：数组去重
来源：http://fwl.meibo888.top

[...new Set(arr)]
来源：http://hrw.0kj1m.cn

[U90] JS：数字数组排序
来源：http://cad.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://bbr.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://vup.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kuq.jinqigufen.top

[U92] JS：深拷贝
来源：http://tdn.shanyushiyangkeji.top

structuredClone(obj)
来源：http://olv.52xcode.cn

[U93] JS：模板字符串
来源：http://nlm.yj20258.top

`共 ${n} 条`
来源：http://tdy.yuanzhike.top

[U94] JS：箭头函数
来源：http://olq.feifeiyinyue.top

const double = x => x * 2;
来源：http://axq.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://ftt.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://knl.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://bpw.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uai.snrcjt.cn

[U97] JS：并发请求
来源：http://knj.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ner.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://otx.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tcj.gogol.net.cn

[U99] JS：事件监听
来源：http://eav.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://stv.yj20258.top

[U100] JS：DOM 查询
来源：http://uhe.zhengqikj.top

document.querySelector(".item")
来源：http://udi.nwbrower.top

[U101] JS：classList 操作
来源：http://ccp.gotoacloud.top

el.classList.toggle("active")
来源：http://vci.ppjwa.cn

[U102] JS：本地存储
来源：http://sne.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://icl.hammf.cn

[U103] JS：定时器
来源：http://gxf.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bfb.tian-w.cn

[U104] JS：防抖
来源：http://pum.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://acu.xylfe.cn

[U105] JS：节流
来源：http://wmc.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cgw.jqgufenzy.top

[U106] JS：日期格式化
来源：http://kiw.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jgg.yongpay.top

[U107] JS：数字千分位
来源：http://vui.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://puu.gotoacloud.top

[U108] JS：随机整数
来源：http://pic.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lnx.gzhubu.top

[U109] JS：数组分组
来源：http://jpx.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://doq.zhongyouzk.top

[U110] JS：数组分块
来源：http://adv.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zih.cqqwz.cn

[U111] JS：对象转 Map
来源：http://hiz.sxryk.cn

new Map(Object.entries(obj))
来源：http://oge.yvedp.cn

[U112] JS：字符串补位
来源：http://oab.epnwcf.com

"7".padStart(3, "0")
来源：http://tpp.jinqigufen.top

[U113] JS：正则替换全部
来源：http://uuy.guannengcc.top

s.replaceAll("a", "b")
来源：http://qiu.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://eqn.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://twe.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://wgs.daria6918.cn

crypto.randomUUID()
来源：http://oxa.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://utv.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://llr.zhijiandao.cn

[U117] JS：单元测试
来源：http://wok.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://ftb.nanxuanxn.top

[U118] JS：开发服务器
来源：http://hit.zhengqikj.top

npm i -D vite;  npx vite
来源：http://oel.jqgufenzy.top

[U119] JS：生产构建
来源：http://erj.gogol.net.cn

npx vite build
来源：http://zot.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://zsq.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://bnz.sxryk.cn

================================================================================
来源：http://amz.wangdashe.top

统计汇总
来源：http://itd.hnqzz.top

================================================================================
来源：http://rdi.pengpengdd.cyou

按语言统计（条）：
来源：http://kta.kuanghao11.cn

Python ......... 252
来源：http://zsz.wangshuangyany.cn

PHP ............ 252
来源：http://mea.xinyue.icu

JavaScript ..... 252
来源：http://yld.nanxuanxn.top

TypeScript ..... 212
来源：http://der.pycfn.com

Java ........... 212
来源：http://oge.zhengqikj.top

Go ............. 212
来源：http://rlu.fzhhl.top

Ruby ........... 212
来源：http://wvh.iojbl.cn

C# ............. 212
来源：http://fyw.zhoulong.xyz

C .............. 30
来源：http://wtb.ydjk.org.cn

C++ ............ 30
来源：http://mcy.zhengqikj.top

SQL ............ 90
来源：http://zat.fengsongda.top

Bash ........... 80
来源：http://jxt.ywan-chungtsiang.top

Kotlin ......... 15
来源：http://snc.chenlongwang.top

Swift .......... 15
来源：http://xwj.hfpthk.cn

Lua ............ 10
来源：http://nws.ctjpmb.com

Perl ........... 10
来源：http://zcy.smart0.xyz

Scala .......... 10
来源：http://mrb.jinqigufen.top

------------------------------------
来源：http://nyn.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://mda.yanxiufei.cn

按章节统计：
来源：http://yla.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://epr.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://soy.tian-w.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pmr.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aun.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sgo.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zae.tarul.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tvw.jiagoushi.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gbw.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ous.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jjg.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://web.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://edq.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ksh.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oaj.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cqp.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wmb.meibo888.top

Q SQL 专题                              90
来源：http://gwp.cucudq.cn

R Bash 专题                             80
来源：http://rqs.bbcook.cn

S C / C++ 专题                          60
来源：http://mtq.nwbrower.top

T 其他语言补充                          60
来源：http://rnv.nanxuanxn.top

U 高频实用片段                         120
来源：http://uml.tarul.cn

------------------------------------
来源：http://fho.aizwys.cn

合计                                  2106 条
来源：http://sxp.havefunace.top

--------------------------------------------------------------------------------
来源：http://znv.dianchejie.cn

使用提醒
来源：http://kyd.meibo888.top

--------------------------------------------------------------------------------
来源：http://pvi.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://clc.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wyw.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nja.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mpv.ivvv.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxs.zhoulong.xyz

—— 文件结束 ——
来源：http://klo.zhongyouzk.top

================================================================================
来源：http://qgm.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://cle.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://mot.bbcook.cn

================================================================================
来源：http://imm.epnwcf.com

【收录内容】
来源：http://dfy.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qvw.fzhhl.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wmp.gogol.net.cn

SQL · Bash · C · C++
来源：http://bzj.ybcxt.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pws.jinqigufen.top

【使用说明】
来源：http://hul.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pev.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rlr.havefunace.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jvb.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vnl.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://emg.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lif.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://azg.jqgufenzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://now.pengpengdd.cyou

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iqu.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gao.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mye.gzhubu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jxc.jianghu66.top

【文件统计】
来源：http://ybl.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ceh.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://boz.smart0.xyz

目  录
来源：http://nra.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://tbu.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ccn.epnwcf.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yqs.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dap.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nhc.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://grw.zhengqikj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jtt.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sly.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://edi.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ghw.yj202588.top


<!-- 参考信息 -->