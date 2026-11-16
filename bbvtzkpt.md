代发 wailian999

[U03] Py：加载 .env 配置
来源：http://lzs.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cra.ydzc1.top

[U04] Py：变量调试打印
来源：http://fxu.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://srg.hnqzz.top

[U05] Py：列表去重且保序
来源：http://ucj.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://fhr.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://zco.chenlongwang.top

{**a, **b}
来源：http://din.redwolf501.top

[U07] Py：反转字典键值
来源：http://tve.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://jwh.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://giu.wangdashe.top

[y for x in nested for y in x]
来源：http://rtr.birdmap.top

[U09] Py：字典取最大值的键
来源：http://eld.aibaodan.cn

max(d, key=d.get)
来源：http://sfm.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://olu.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xvj.yvedp.cn

[U11] Py：生成器表达式
来源：http://sdk.zhoulong.xyz

(x * 2 for x in arr)
来源：http://pam.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wdr.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://fxj.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://azb.chenzaomai.com

deque(maxlen=10)
来源：http://ita.316326.xyz

[U14] Py：分组收集到列表
来源：http://ope.52xcode.cn

defaultdict(list)
来源：http://dbj.epnwcf.com

[U15] Py：高精度计时
来源：http://pbv.daxiang520.top

t = time.perf_counter()
来源：http://cth.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://nkq.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zjj.cqqwz.cn

[U17] Py：初始化日志
来源：http://upt.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://aql.zhengqikj.top

[U18] Py：预编译正则
来源：http://uxh.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://tju.sysykeji.top

[U19] Py：正则替换带回调
来源：http://bsa.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mez.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://zcq.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://thj.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://ifz.dashuyun.cn

@contextlib.contextmanager
来源：http://yio.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://qzb.52xcode.cn

list(zip(*m))
来源：http://gul.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://pbk.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xjo.hfpthk.cn

[U24] Py：路径操作
来源：http://qfa.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bxu.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://ana.tanke756.top

csv.DictReader(f)
来源：http://eif.gotoacloud.top

[U26] Py：并发下载
来源：http://pxb.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yuy.yj20258888.top

[U27] Py：异步 HTTP
来源：http://cim.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://vrc.cashguo.top

[U28] Py：类型别名
来源：http://mqj.ydjk.org.cn

UserId = int
来源：http://yaw.cheryme.top

[U29] Py：属性校验
来源：http://uzx.bjfxy.top

@property 与 @x.setter 配合
来源：http://lbb.hysaishi.cn

[U30] Py：数据类
来源：http://fbj.aibaodan.cn

@dataclass(slots=True)
来源：http://aea.yj20258888.top

[U31] Py：单测
来源：http://qwc.xziqi.cn

python -m pytest -q
来源：http://vtc.zhoulong.xyz

[U32] Py：代码格式化
来源：http://iwn.andypj.xyz

ruff format . && ruff check --fix .
来源：http://epb.zhongyouzk.top

[U33] Py：打包发布
来源：http://eti.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://its.pycfn.com

[U34] Py：判断编码
来源：http://cna.hammf.cn

chardet.detect(raw)
来源：http://rqh.316326.xyz

[U35] Py：发送邮件
来源：http://tda.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://szk.xziqi.cn

[U36] Py：定时任务
来源：http://fbu.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://wqe.tianlin.xyz

[U37] Py：读写 Excel
来源：http://yol.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://igs.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://tvn.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://asp.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://gox.redwolf501.top

sys.stdout.isatty()
来源：http://ybf.bbcook.cn

[U40] Py：打印到标准错误
来源：http://wje.hcnkem.com

print("err", file=sys.stderr)
来源：http://xvh.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://ije.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uvn.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://xcf.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fap.ybcxt.top

[U43] PHP：声明命名空间
来源：http://llh.yfazqb.com

namespace App\Http;
来源：http://jbj.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://lkl.hongshengwenyu.top

declare(strict_types=1);
来源：http://ksl.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://vmp.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://doj.birdmap.top

[U46] PHP：可空类型
来源：http://ivw.aibaodan.cn

?string $name = null
来源：http://cxw.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://pbs.hesvh.cn

int|string $id
来源：http://tcq.pycfn.com

[U48] PHP：纯枚举
来源：http://mop.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ygz.hcnkem.com

[U49] PHP：只读属性
来源：http://obf.hcnkem.com

public readonly string $name
来源：http://yaa.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://fyq.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://tiq.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://dvp.hysaishi.cn

[$a, $b] = $arr;
来源：http://lsq.hywenlv.cn

[U52] PHP：箭头函数
来源：http://ipx.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://nqx.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://fxy.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://ihw.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://zfr.snrcjt.cn

$obj?->method()
来源：http://big.iojbl.cn

[U55] PHP：match 表达式
来源：http://zsy.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://byh.xinyue.icu

[U56] PHP：命名参数
来源：http://kre.gogol.net.cn

f(a: 1, b: 2)
来源：http://mpx.meibo888.top

[U57] PHP：字符串插值
来源：http://ton.shanyushiyangkeji.top

"值: {$a}"
来源：http://qze.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://pdz.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xkq.yuanzhike.top

[U59] PHP：自定义排序
来源：http://man.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ptg.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://edb.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://whb.chenjidiqi.icu

[U61] PHP：正则
来源：http://rzd.zhengqikj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://asl.bjfxy.top

[U62] PHP：日期对象
来源：http://tig.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xqg.hesvh.cn

[U63] PHP：文件读写
来源：http://xof.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dbv.yj20258888.top

[U64] PHP：目录遍历
来源：http://rnm.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://whc.haohaochexian.top

[U65] PHP：会话
来源：http://uht.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qha.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://orx.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://alz.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://lgr.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://csr.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://eva.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ajg.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://hin.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uuz.yj202588.top

[U70] PHP：PDO 事务
来源：http://rgh.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yjy.hesvh.cn

[U71] PHP：抛出异常
来源：http://jxf.316326.xyz

throw new RuntimeException("失败", 500);
来源：http://zon.pycfn.com

[U72] PHP：写错误日志
来源：http://cyk.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://ljb.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://uoo.pycfn.com

parse_ini_file("config.ini", true)
来源：http://evf.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://abr.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://ebf.yuanzhike.top

[U75] PHP：依赖注入
来源：http://rfk.316326.xyz

composer require psr/container
来源：http://jtl.guannengcc.top

[U76] PHP：简单路由
来源：http://zqf.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aih.meibo888.top

[U77] PHP：模板渲染
来源：http://cgj.316326.xyz

composer require twig/twig
来源：http://tng.meibo888.top

[U78] PHP：单元测试
来源：http://hnu.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://vbu.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://bso.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://vov.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://jnz.nwbrower.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bpr.chenlongwang.top

[U81] JS：初始化项目
来源：http://isw.haohaochexian.top

npm init -y;  npm i express
来源：http://dkh.epnwcf.com

[U82] JS：package.json 脚本
来源：http://fhm.hfpthk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rtz.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://xfs.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://ywm.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://umy.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://qka.guowangkeji.top

[U85] JS：可选链
来源：http://cut.jinqigufen.top

a?.b?.c
来源：http://skj.xinyue.icu

[U86] JS：空值合并
来源：http://hma.52xcode.cn

a ?? b
来源：http://gez.yonumen.top

[U87] JS：解构默认值
来源：http://ztc.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://jfg.fzhhl.top

[U88] JS：对象展开合并
来源：http://qat.sysykeji.top

{ ...a, ...b }
来源：http://lgb.yangfankeji.com

[U89] JS：数组去重
来源：http://lpn.feifeiyinyue.top

[...new Set(arr)]
来源：http://qky.yfazqb.com

[U90] JS：数字数组排序
来源：http://bsu.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://qie.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://fpx.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vcd.zhoulong.xyz

[U92] JS：深拷贝
来源：http://uxq.ydjk.org.cn

structuredClone(obj)
来源：http://gcg.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://pnv.xinyue.icu

`共 ${n} 条`
来源：http://gqr.zhengqikj.top

[U94] JS：箭头函数
来源：http://kiq.yanxiufei.cn

const double = x => x * 2;
来源：http://maj.dianchejie.cn

[U95] JS：Promise 包装
来源：http://qur.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://nyc.tian-w.cn

[U96] JS：async/await 与异常
来源：http://uqc.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://abd.nwbrower.top

[U97] JS：并发请求
来源：http://ddk.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://exa.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://kwv.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dva.jiagoushi.top

[U99] JS：事件监听
来源：http://ope.yvedp.cn

el.addEventListener("click", e => {})
来源：http://wcj.tanke756.top

[U100] JS：DOM 查询
来源：http://jgu.guowangkeji.top

document.querySelector(".item")
来源：http://nfh.jinyuanbaomall.cn

[U101] JS：classList 操作
来源：http://kbk.yfazqb.com

el.classList.toggle("active")
来源：http://cve.zdqjudy.top

[U102] JS：本地存储
来源：http://wps.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nsv.zhongyouzk.top

[U103] JS：定时器
来源：http://vit.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jmt.xuetiantiany.cn

[U104] JS：防抖
来源：http://gtn.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcu.ydjk.org.cn

[U105] JS：节流
来源：http://ytp.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lno.9152youxi.cn

[U106] JS：日期格式化
来源：http://rbb.snrcjt.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zsz.sxryk.cn

[U107] JS：数字千分位
来源：http://ppi.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://poh.zhixingplan.top

[U108] JS：随机整数
来源：http://ptk.fzhhl.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bva.vehdjk.com

[U109] JS：数组分组
来源：http://stz.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://gjw.quarkkingdee.top

[U110] JS：数组分块
来源：http://bay.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oza.guowangkeji.top

[U111] JS：对象转 Map
来源：http://vwu.redwolf501.top

new Map(Object.entries(obj))
来源：http://huk.gotoacloud.top

[U112] JS：字符串补位
来源：http://zhr.hysaishi.cn

"7".padStart(3, "0")
来源：http://tbc.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://icw.fehbvm.com

s.replaceAll("a", "b")
来源：http://gtv.yongpay.top

[U114] JS：JSON 深比较
来源：http://edo.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mkj.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://mem.aibaodan.cn

crypto.randomUUID()
来源：http://ayu.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://qaf.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://vyz.gaohongyu789.top

[U117] JS：单元测试
来源：http://jjt.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://lnv.gotoacloud.top

[U118] JS：开发服务器
来源：http://jub.zdqjudy.top

npm i -D vite;  npx vite
来源：http://phs.jinqigfzy.top

[U119] JS：生产构建
来源：http://egr.sweek.top

npx vite build
来源：http://pwa.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://aye.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://njs.vehdjk.com

================================================================================
来源：http://jxf.sufxvd.cn

统计汇总
来源：http://gow.svipenyu.cn

================================================================================
来源：http://hkj.haohaochexian.top

按语言统计（条）：
来源：http://uve.wangdashe.top

Python ......... 252
来源：http://ucr.nwbrower.top

PHP ............ 252
来源：http://cdz.bbcook.cn

JavaScript ..... 252
来源：http://two.xuanzx.com

TypeScript ..... 212
来源：http://bgb.nanxuanxn.top

Java ........... 212
来源：http://bzs.fzhhl.top

Go ............. 212
来源：http://qds.iojbl.cn

Ruby ........... 212
来源：http://ymr.uphjek.com

C# ............. 212
来源：http://mzb.pycfn.com

C .............. 30
来源：http://npp.pengpengdd.cyou

C++ ............ 30
来源：http://rpt.ctjpmb.com

SQL ............ 90
来源：http://iuq.yangfankeji.com

Bash ........... 80
来源：http://viy.aibaodan.cn

Kotlin ......... 15
来源：http://urt.tian-w.cn

Swift .......... 15
来源：http://tko.sysykeji.top

Lua ............ 10
来源：http://eru.aibaodan.cn

Perl ........... 10
来源：http://lef.bbcook.cn

Scala .......... 10
来源：http://adk.bbcook.cn

------------------------------------
来源：http://lfe.yangfankeji.com

合计 ........... 2106 条
来源：http://mzm.sysykeji.top

按章节统计：
来源：http://mix.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fmd.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cmb.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://daf.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kzo.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nhm.yvedp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://btc.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oqi.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://piv.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bbj.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ddw.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xzk.zdbjq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://whi.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nze.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nac.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mbb.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vot.redwolf501.top

Q SQL 专题                              90
来源：http://rky.xuanzx.com

R Bash 专题                             80
来源：http://fte.hammf.cn

S C / C++ 专题                          60
来源：http://ewd.jinqigfzy.top

T 其他语言补充                          60
来源：http://iez.jiagoushi.top

U 高频实用片段                         120
来源：http://qol.xziqi.cn

------------------------------------
来源：http://rlf.hysaishi.cn

合计                                  2106 条
来源：http://qbs.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://dlw.0kj1m.cn

使用提醒
来源：http://gri.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://msy.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sbn.sufxvd.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://olr.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ddj.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uny.yueranfly.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kim.quarkkingdee.top

—— 文件结束 ——
来源：http://rjc.zhixingplan.top

================================================================================
来源：http://nci.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://xhs.sxryk.cn

Common Programming Examples Cheat Book
来源：http://ric.dianchejie.cn

================================================================================
来源：http://qph.xinyue.icu

【收录内容】
来源：http://ilx.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://elh.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vfc.snrcjt.cn

SQL · Bash · C · C++
来源：http://lax.shanyushiyangkeji.top


<!-- 参考信息 -->