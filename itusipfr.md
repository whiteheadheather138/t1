代发 wailian999

[U03] Py：加载 .env 配置
来源：http://tsy.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://erd.bbcook.cn

[U04] Py：变量调试打印
来源：http://vbm.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kwm.bbcook.cn

[U05] Py：列表去重且保序
来源：http://loa.sweek.top

list(dict.fromkeys(arr))
来源：http://ijm.hammf.cn

[U06] Py：合并两个字典
来源：http://yss.birdmap.top

{**a, **b}
来源：http://xjz.tianlin.xyz

[U07] Py：反转字典键值
来源：http://koo.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://rbx.chenlongwang.top

[U08] Py：展平二维列表
来源：http://vbj.xziqi.cn

[y for x in nested for y in x]
来源：http://xwn.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://vro.9152youxi.cn

max(d, key=d.get)
来源：http://xsz.0kj1m.cn

[U10] Py：按值排序字典
来源：http://dup.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fit.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://wvg.iojbl.cn

(x * 2 for x in arr)
来源：http://uhs.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iuc.fengsongda.top

Counter(arr).most_common(3)
来源：http://tae.jiagoushi.top

[U13] Py：固定长度队列
来源：http://lzw.52xcode.cn

deque(maxlen=10)
来源：http://urh.yj20258888.top

[U14] Py：分组收集到列表
来源：http://qah.aizwys.cn

defaultdict(list)
来源：http://jdj.cdnleiting.top

[U15] Py：高精度计时
来源：http://plr.cashguo.top

t = time.perf_counter()
来源：http://yuh.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://fks.daria6918.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uag.yvedp.cn

[U17] Py：初始化日志
来源：http://api.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://jwx.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://hfg.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://iom.daxiang520.top

[U19] Py：正则替换带回调
来源：http://cly.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://psd.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://wjw.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://tob.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://rcm.yfazqb.com

@contextlib.contextmanager
来源：http://wjm.zycfv.cn

[U22] Py：矩阵转置
来源：http://njb.hongshengwenyu.top

list(zip(*m))
来源：http://mvz.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://lob.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://icp.zhixingplan.top

[U24] Py：路径操作
来源：http://bbl.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bin.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://wjn.pycfn.com

csv.DictReader(f)
来源：http://dpc.redwolf501.top

[U26] Py：并发下载
来源：http://yef.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://myc.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://sue.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://cgg.cheryme.top

[U28] Py：类型别名
来源：http://kpk.fzhhl.top

UserId = int
来源：http://feb.chenzaomai.com

[U29] Py：属性校验
来源：http://edk.yongpay.top

@property 与 @x.setter 配合
来源：http://rwt.iojbl.cn

[U30] Py：数据类
来源：http://jbo.iojbl.cn

@dataclass(slots=True)
来源：http://pxk.yvedp.cn

[U31] Py：单测
来源：http://cnf.zhiwuduotai.top

python -m pytest -q
来源：http://jpu.uphjek.com

[U32] Py：代码格式化
来源：http://xll.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://qiv.cashguo.top

[U33] Py：打包发布
来源：http://mni.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://cos.yfazqb.com

[U34] Py：判断编码
来源：http://otm.aizwys.cn

chardet.detect(raw)
来源：http://gjo.jinqigufen.top

[U35] Py：发送邮件
来源：http://rsg.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://heh.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://iyy.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://jgp.sysykeji.top

[U37] Py：读写 Excel
来源：http://ivu.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://alx.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://xyx.yj202588.top

Path(__file__).resolve().parent
来源：http://qik.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://wkz.wangshuangyany.cn

sys.stdout.isatty()
来源：http://abk.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://hie.bjfxy.top

print("err", file=sys.stderr)
来源：http://hij.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://anl.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ezq.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://gnk.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bjd.tanke756.top

[U43] PHP：声明命名空间
来源：http://cpr.zhaomingkeji.xyz

namespace App\Http;
来源：http://gdl.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://phu.tian-w.cn

declare(strict_types=1);
来源：http://aid.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://sap.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yxs.c1oappe.top

[U46] PHP：可空类型
来源：http://jbe.sufxvd.cn

?string $name = null
来源：http://idj.jinqigufen.top

[U47] PHP：联合类型
来源：http://qcv.tian-w.cn

int|string $id
来源：http://sax.meibo888.top

[U48] PHP：纯枚举
来源：http://jkl.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://txu.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://kvf.hywenlv.cn

public readonly string $name
来源：http://cuo.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://sll.cheryme.top

public function __construct(private int $id) {}
来源：http://nsg.sxryk.cn

[U51] PHP：数组解构
来源：http://sih.jlsjyb.cn

[$a, $b] = $arr;
来源：http://hrc.fktsv.cn

[U52] PHP：箭头函数
来源：http://wnq.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://sxf.bbcook.cn

[U53] PHP：空合并运算符
来源：http://zgg.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://erx.ehwqpu.com

[U54] PHP：空安全调用
来源：http://odt.cheryme.top

$obj?->method()
来源：http://aiy.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://rgq.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://trx.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://ybq.havefunace.top

f(a: 1, b: 2)
来源：http://fue.nwbrower.top

[U57] PHP：字符串插值
来源：http://atp.sysykeji.top

"值: {$a}"
来源：http://rrh.zdbjq.cn

[U58] PHP：数组三件套
来源：http://fce.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cyn.xuanzx.com

[U59] PHP：自定义排序
来源：http://kxn.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uly.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://sgl.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://srq.bbcook.cn

[U61] PHP：正则
来源：http://ldp.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://whz.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://tnv.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hml.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://brs.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ipy.gogol.net.cn

[U64] PHP：目录遍历
来源：http://ltb.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://qfl.hywenlv.cn

[U65] PHP：会话
来源：http://yye.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://upp.sysykeji.top

[U66] PHP：设置 Cookie
来源：http://qyi.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mzt.cucudq.cn

[U67] PHP：处理文件上传
来源：http://exa.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ivd.shuidangran.top

[U68] PHP：PDO 连接
来源：http://eqj.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tdi.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://kpi.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kqh.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://bzd.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hyn.dianchejie.cn

[U71] PHP：抛出异常
来源：http://dbu.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://ulh.yj20258.top

[U72] PHP：写错误日志
来源：http://jpi.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://bfg.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://qnu.havefunace.top

parse_ini_file("config.ini", true)
来源：http://mvh.c1oappe.top

[U74] PHP：读取环境变量
来源：http://rna.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://dxh.tarul.cn

[U75] PHP：依赖注入
来源：http://bwn.aizwys.cn

composer require psr/container
来源：http://ioa.aibaodan.cn

[U76] PHP：简单路由
来源：http://nvg.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dek.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://zfy.jinqigfzy.top

composer require twig/twig
来源：http://bfl.bbcook.cn

[U78] PHP：单元测试
来源：http://ohh.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://dts.fzhhl.top

[U79] PHP：静态分析
来源：http://woy.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://qrj.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://rlb.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cno.dashuyun.cn

[U81] JS：初始化项目
来源：http://qdw.ehwqpu.com

npm init -y;  npm i express
来源：http://zcc.yvedp.cn

[U82] JS：package.json 脚本
来源：http://thx.dashuyun.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sre.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://gcp.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://yql.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://rsg.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://njz.52xcode.cn

[U85] JS：可选链
来源：http://vyh.316326.xyz

a?.b?.c
来源：http://mun.zdqjudy.top

[U86] JS：空值合并
来源：http://kji.jiagoushi.top

a ?? b
来源：http://rda.tarul.cn

[U87] JS：解构默认值
来源：http://det.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://hor.52xcode.cn

[U88] JS：对象展开合并
来源：http://bmt.aizwys.cn

{ ...a, ...b }
来源：http://bzb.cheryme.top

[U89] JS：数组去重
来源：http://pql.yonumen.top

[...new Set(arr)]
来源：http://bxz.jyoumei.cn

[U90] JS：数字数组排序
来源：http://aak.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://hvx.yueranfly.top

[U91] JS：对象键值遍历
来源：http://pai.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dhr.fktsv.cn

[U92] JS：深拷贝
来源：http://rnb.jlsjyb.cn

structuredClone(obj)
来源：http://fxe.birdmap.top

[U93] JS：模板字符串
来源：http://ylv.jiagoushi.top

`共 ${n} 条`
来源：http://szd.zycfv.cn

[U94] JS：箭头函数
来源：http://kbt.ydzc1.top

const double = x => x * 2;
来源：http://sys.gogol.net.cn

[U95] JS：Promise 包装
来源：http://zdf.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://jov.meibo888.top

[U96] JS：async/await 与异常
来源：http://vke.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://css.vehdjk.com

[U97] JS：并发请求
来源：http://ilb.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uny.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://zxj.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nnr.ivvv.top

[U99] JS：事件监听
来源：http://atz.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://unk.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://fei.epnwcf.com

document.querySelector(".item")
来源：http://mip.hcnkem.com

[U101] JS：classList 操作
来源：http://saz.xziqi.cn

el.classList.toggle("active")
来源：http://lvs.svipenyu.cn

[U102] JS：本地存储
来源：http://ozj.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vdi.nanxuanxn.top

[U103] JS：定时器
来源：http://tgl.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://glx.svipenyu.cn

[U104] JS：防抖
来源：http://gzr.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://whj.0kj1m.cn

[U105] JS：节流
来源：http://otd.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://edy.hcnkem.com

[U106] JS：日期格式化
来源：http://ndo.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sxk.zdqjudy.top

[U107] JS：数字千分位
来源：http://waf.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hmb.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://fbw.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dyx.sufxvd.cn

[U109] JS：数组分组
来源：http://cgp.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://gso.gotoacloud.top

[U110] JS：数组分块
来源：http://mck.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bqb.guowangkeji.top

[U111] JS：对象转 Map
来源：http://lya.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://yjq.hysaishi.cn

[U112] JS：字符串补位
来源：http://kkv.hnqzz.top

"7".padStart(3, "0")
来源：http://yfd.jianghu66.top

[U113] JS：正则替换全部
来源：http://xfu.cqqwz.cn

s.replaceAll("a", "b")
来源：http://gkp.aizwys.cn

[U114] JS：JSON 深比较
来源：http://xdi.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wnx.sufxvd.cn

[U115] JS：生成 UUID
来源：http://uyp.hcnkem.com

crypto.randomUUID()
来源：http://qvd.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://guu.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://jkp.jyoumei.cn

[U117] JS：单元测试
来源：http://reh.jqgufenzy.top

npm i -D vitest;  npx vitest
来源：http://yui.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://mxc.jiagoushi.top

npm i -D vite;  npx vite
来源：http://ilz.chenzaomai.com

[U119] JS：生产构建
来源：http://sff.316326.xyz

npx vite build
来源：http://jsb.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://ykn.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://gnt.chenjidiqi.icu

================================================================================
来源：http://wvh.chenlongwang.top

统计汇总
来源：http://frx.yj20258888.top

================================================================================
来源：http://qtx.nanxuanxn.top

按语言统计（条）：
来源：http://ohg.epnwcf.com

Python ......... 252
来源：http://yuo.nanxinkj.top

PHP ............ 252
来源：http://blw.sxryk.cn

JavaScript ..... 252
来源：http://gap.havefunace.top

TypeScript ..... 212
来源：http://ysv.cqqwz.cn

Java ........... 212
来源：http://zvb.yuxming.cn

Go ............. 212
来源：http://zpy.andypj.xyz

Ruby ........... 212
来源：http://pox.yj202588.top

C# ............. 212
来源：http://wyk.chenzaomai.com

C .............. 30
来源：http://dtw.sjlbkw.cn

C++ ............ 30
来源：http://qor.zycfv.cn

SQL ............ 90
来源：http://mlg.jinghuilouyu.cn

Bash ........... 80
来源：http://ebf.shangyingyoupin.top

Kotlin ......... 15
来源：http://xqq.zdqjudy.top

Swift .......... 15
来源：http://hpv.hfpthk.cn

Lua ............ 10
来源：http://auu.52xcode.cn

Perl ........... 10
来源：http://lrx.9152youxi.cn

Scala .......... 10
来源：http://xal.chenlongwang.top

------------------------------------
来源：http://aip.52xcode.cn

合计 ........... 2106 条
来源：http://kwd.haohaochexian.top

按章节统计：
来源：http://ebv.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://orr.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://akh.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bka.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gup.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gnq.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aif.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oml.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://utr.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rdi.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wzd.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zfy.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bzp.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://khn.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dgx.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aiv.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oze.fehbvm.com

Q SQL 专题                              90
来源：http://qzc.chenzaomai.com

R Bash 专题                             80
来源：http://ugn.tian-w.cn

S C / C++ 专题                          60
来源：http://rvx.jiagoushi.top

T 其他语言补充                          60
来源：http://ucp.gogol.net.cn

U 高频实用片段                         120
来源：http://rgg.ppjwa.cn

------------------------------------
来源：http://tvd.shuidangran.top

合计                                  2106 条
来源：http://mqr.nwbrower.top

--------------------------------------------------------------------------------
来源：http://nsk.haohaochexian.top

使用提醒
来源：http://jlq.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://uzg.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xua.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cuw.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fgw.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jqv.zhixingplan.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bsc.316326.xyz

—— 文件结束 ——
来源：http://wmq.jinghuilouyu.cn

================================================================================
来源：http://flq.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://zjf.pycfn.com

Common Programming Examples Cheat Book
来源：http://uao.shanyushiyangkeji.top

================================================================================
来源：http://nic.zhongyouzk.top

【收录内容】
来源：http://ujy.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ffe.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hvv.haohaochexian.top

SQL · Bash · C · C++
来源：http://bwo.birdmap.top


<!-- 参考信息 -->