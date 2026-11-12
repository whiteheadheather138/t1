代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://waq.nwbrower.top

[T51] Scala：Hello World
来源：http://ngh.wangshuangyany.cn

println("Hello")
来源：http://fid.0kj1m.cn

[T52] Scala：变量
来源：http://jfm.hysaishi.cn

val a = 1;  var b = 2
来源：http://nzc.dashuyun.cn

[T53] Scala：字符串插值
来源：http://zjf.xuetiantiany.cn

s"值: $b"
来源：http://lxf.guannengcc.top

[T54] Scala：集合映射
来源：http://cky.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://cxc.dashuyun.cn

[T55] Scala：集合过滤
来源：http://gcu.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://lji.guannengcc.top

[T56] Scala：样例类
来源：http://iyh.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://kzr.xziqi.cn

[T57] Scala：模式匹配
来源：http://gzb.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hko.hnxiangtu.top

[T58] Scala：函数定义
来源：http://twm.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bvu.snrcjt.cn

[T59] Scala：循环
来源：http://sdo.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://jlu.zhijiandao.cn

[T60] Scala：折叠
来源：http://fts.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xeg.tianlin.xyz

================================================================================
来源：http://eua.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://edv.guannengcc.top

================================================================================
来源：http://fnx.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://mja.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://sgr.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://hhf.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ecz.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://glm.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vxf.gzhubu.top

[U04] Py：变量调试打印
来源：http://cah.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mcw.sysykeji.top

[U05] Py：列表去重且保序
来源：http://npe.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://mwy.ppjwa.cn

[U06] Py：合并两个字典
来源：http://jis.bbcook.cn

{**a, **b}
来源：http://vjx.ydzc1.top

[U07] Py：反转字典键值
来源：http://uux.guannengcc.top

{v: k for k, v in d.items()}
来源：http://pyk.smart0.xyz

[U08] Py：展平二维列表
来源：http://tyq.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://wqi.meibo888.top

[U09] Py：字典取最大值的键
来源：http://wzq.zhongyouzk.top

max(d, key=d.get)
来源：http://hlz.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://rjp.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://umc.tanke756.top

[U11] Py：生成器表达式
来源：http://svp.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://mxa.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://gci.meibo888.top

Counter(arr).most_common(3)
来源：http://yut.hfpthk.cn

[U13] Py：固定长度队列
来源：http://goj.fengsongda.top

deque(maxlen=10)
来源：http://iov.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://xrk.ctjpmb.com

defaultdict(list)
来源：http://rci.0kj1m.cn

[U15] Py：高精度计时
来源：http://utd.hammf.cn

t = time.perf_counter()
来源：http://unz.cucudq.cn

[U16] Py：命令行参数解析
来源：http://wen.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://trx.dianchejie.cn

[U17] Py：初始化日志
来源：http://jxr.ybcxt.top

logging.basicConfig(level=logging.INFO)
来源：http://tau.guannengcc.top

[U18] Py：预编译正则
来源：http://vul.yonumen.top

pat = re.compile(r"\d+")
来源：http://xra.guannengcc.top

[U19] Py：正则替换带回调
来源：http://ogk.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aui.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://gij.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://afs.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://ztd.yangfankeji.com

@contextlib.contextmanager
来源：http://nfd.tanke756.top

[U22] Py：矩阵转置
来源：http://rbi.tarul.cn

list(zip(*m))
来源：http://zui.ivvv.top

[U23] Py：分块读取大文件
来源：http://rzb.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://txu.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://vmf.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fee.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://hte.shangyingyoupin.top

csv.DictReader(f)
来源：http://wuf.shzxlz.cn

[U26] Py：并发下载
来源：http://hyt.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dpx.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://hwh.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://myf.yj20258888.top

[U28] Py：类型别名
来源：http://ajo.wangshuangyany.cn

UserId = int
来源：http://psb.hnxiangtu.top

[U29] Py：属性校验
来源：http://ftm.yj202588.top

@property 与 @x.setter 配合
来源：http://nfy.ybcxt.top

[U30] Py：数据类
来源：http://jbw.tianlin.xyz

@dataclass(slots=True)
来源：http://sxg.xuetiantiany.cn

[U31] Py：单测
来源：http://xjn.52xcode.cn

python -m pytest -q
来源：http://agg.52xcode.cn

[U32] Py：代码格式化
来源：http://mbx.cashguo.top

ruff format . && ruff check --fix .
来源：http://zvs.jinqigfzy.top

[U33] Py：打包发布
来源：http://sht.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://vvy.feifeiyinyue.top

[U34] Py：判断编码
来源：http://jsm.fzhhl.top

chardet.detect(raw)
来源：http://rfp.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://rxd.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ofe.iojbl.cn

[U36] Py：定时任务
来源：http://fvc.gotoacloud.top

schedule.every(10).minutes.do(job)
来源：http://mlr.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://yvn.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://jfm.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://pmx.yj20258888.top

Path(__file__).resolve().parent
来源：http://uzo.gotoacloud.top

[U39] Py：判断是否在交互环境
来源：http://vjq.shangyingyoupin.top

sys.stdout.isatty()
来源：http://ddm.yonumen.top

[U40] Py：打印到标准错误
来源：http://onf.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://oth.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://biw.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://qjx.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://dgb.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xgt.aizwys.cn

[U43] PHP：声明命名空间
来源：http://xei.daria6918.cn

namespace App\Http;
来源：http://vaw.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://lae.316326.xyz

declare(strict_types=1);
来源：http://cze.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://bah.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://axv.shuidangran.top

[U46] PHP：可空类型
来源：http://wri.zhengqikj.top

?string $name = null
来源：http://tjl.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://jgi.yj20258888.top

int|string $id
来源：http://kiw.dianchejie.cn

[U48] PHP：纯枚举
来源：http://rze.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://khk.iojbl.cn

[U49] PHP：只读属性
来源：http://erq.zycfv.cn

public readonly string $name
来源：http://mwd.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://lxo.smart0.xyz

public function __construct(private int $id) {}
来源：http://new.bbcook.cn

[U51] PHP：数组解构
来源：http://wui.redwolf501.top

[$a, $b] = $arr;
来源：http://chc.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://bzd.uphjek.com

$double = fn($x) => $x * 2;
来源：http://xzh.fktsv.cn

[U53] PHP：空合并运算符
来源：http://poy.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://uic.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://got.vqdsnc.cn

$obj?->method()
来源：http://zox.chenlongwang.top

[U55] PHP：match 表达式
来源：http://wdb.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kbp.quarkkingdee.top

[U56] PHP：命名参数
来源：http://dul.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://nnw.zhengqikj.top

[U57] PHP：字符串插值
来源：http://etf.zhijiandao.cn

"值: {$a}"
来源：http://dwi.sweek.top

[U58] PHP：数组三件套
来源：http://ukd.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aot.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://pzy.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxy.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://xsh.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wik.shanyushiyangtech.top

[U61] PHP：正则
来源：http://kvr.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zlm.bjfxy.top

[U62] PHP：日期对象
来源：http://lrm.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zgx.cqqwz.cn

[U63] PHP：文件读写
来源：http://fdo.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dsw.uphjek.com

[U64] PHP：目录遍历
来源：http://qnr.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://pmq.xuetiantiany.cn

[U65] PHP：会话
来源：http://gjm.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hrj.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://svz.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wts.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://ewa.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wcg.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://pkl.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rpm.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://bld.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cpi.jianghu66.top

[U70] PHP：PDO 事务
来源：http://nwk.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jhv.xinyue.icu

[U71] PHP：抛出异常
来源：http://kyp.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://rng.hcnkem.com

[U72] PHP：写错误日志
来源：http://fdf.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://zix.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://ybv.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://lde.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://sdx.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://oim.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://gzr.jianghu66.top

composer require psr/container
来源：http://ciq.guannengcc.top

[U76] PHP：简单路由
来源：http://aoo.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vyn.fzhhl.top

[U77] PHP：模板渲染
来源：http://hdg.xuetiantiany.cn

composer require twig/twig
来源：http://zyt.316326.xyz

[U78] PHP：单元测试
来源：http://cfi.yj202588.top

composer require --dev phpunit/phpunit
来源：http://xhx.52xcode.cn

[U79] PHP：静态分析
来源：http://gnz.hammf.cn

composer require --dev phpstan/phpstan
来源：http://rue.hnqzz.top

[U80] PHP：代码规范修复
来源：http://vsj.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iff.pycfn.com

[U81] JS：初始化项目
来源：http://dsr.gaohongyu789.top

npm init -y;  npm i express
来源：http://kos.uphjek.com

[U82] JS：package.json 脚本
来源：http://bkm.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mjc.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://czu.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://nin.jyoumei.cn

[U84] JS：CommonJS 写法
来源：http://cjr.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vmg.yj20258.top

[U85] JS：可选链
来源：http://mvd.hfpthk.cn

a?.b?.c
来源：http://wff.andypj.xyz

[U86] JS：空值合并
来源：http://swx.uphjek.com

a ?? b
来源：http://kib.iojbl.cn

[U87] JS：解构默认值
来源：http://vnu.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://qdy.nwbrower.top

[U88] JS：对象展开合并
来源：http://zwp.chenlongwang.top

{ ...a, ...b }
来源：http://ksv.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://pbw.tanke756.top

[...new Set(arr)]
来源：http://fei.jyoumei.cn

[U90] JS：数字数组排序
来源：http://zeo.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://trq.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://elc.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ffu.jiagoushi.top

[U92] JS：深拷贝
来源：http://zus.guowangkeji.top

structuredClone(obj)
来源：http://ydg.jianghu66.top

[U93] JS：模板字符串
来源：http://abt.shzxlz.cn

`共 ${n} 条`
来源：http://zqa.ehwqpu.com

[U94] JS：箭头函数
来源：http://tcy.epnwcf.com

const double = x => x * 2;
来源：http://hfj.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://uwy.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://aqc.smart0.xyz

[U96] JS：async/await 与异常
来源：http://tjx.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iwh.meibo888.top

[U97] JS：并发请求
来源：http://lys.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kgq.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://jts.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqm.sweek.top

[U99] JS：事件监听
来源：http://znu.cheryme.top

el.addEventListener("click", e => {})
来源：http://wzv.hnqzz.top

[U100] JS：DOM 查询
来源：http://vll.mhx1999.top

document.querySelector(".item")
来源：http://tqf.uphjek.com

[U101] JS：classList 操作
来源：http://jrz.pycfn.com

el.classList.toggle("active")
来源：http://vch.zhixingplan.top

[U102] JS：本地存储
来源：http://nkl.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bsd.vehdjk.com

[U103] JS：定时器
来源：http://xrw.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eix.zhoulong.xyz

[U104] JS：防抖
来源：http://ant.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcb.zdbjq.cn

[U105] JS：节流
来源：http://ctq.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zwm.tanke756.top

[U106] JS：日期格式化
来源：http://tri.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nan.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://aup.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ttt.andypj.xyz

[U108] JS：随机整数
来源：http://pvg.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sdp.ehwqpu.com

[U109] JS：数组分组
来源：http://zvb.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://xfs.xylfe.cn

[U110] JS：数组分块
来源：http://xlu.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kzj.bbcook.cn

[U111] JS：对象转 Map
来源：http://eun.shzxlz.cn

new Map(Object.entries(obj))
来源：http://puc.jinyuanbaomall.cn

[U112] JS：字符串补位
来源：http://bmu.guannengcc.top

"7".padStart(3, "0")
来源：http://jzh.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://kiz.tarul.cn

s.replaceAll("a", "b")
来源：http://teu.ybcxt.top

[U114] JS：JSON 深比较
来源：http://ekb.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://etp.gotoacloud.top

[U115] JS：生成 UUID
来源：http://zjk.redwolf501.top

crypto.randomUUID()
来源：http://rgm.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://fms.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://elc.shangyingyoupin.top

[U117] JS：单元测试
来源：http://fsv.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://fvo.redwolf501.top

[U118] JS：开发服务器
来源：http://scu.cqqwz.cn

npm i -D vite;  npx vite
来源：http://cvr.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://fdx.meibo888.top

npx vite build
来源：http://iay.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://gyu.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://xxv.sxryk.cn

================================================================================
来源：http://dbp.sufxvd.cn

统计汇总
来源：http://siu.jlsjyb.cn

================================================================================
来源：http://owy.daxiang520.top

按语言统计（条）：
来源：http://xcz.jiagoushi.top

Python ......... 252
来源：http://nhj.xuanzx.com

PHP ............ 252
来源：http://vse.ivvv.top

JavaScript ..... 252
来源：http://abl.yuxming.cn

TypeScript ..... 212
来源：http://wfi.zdbjq.cn

Java ........... 212
来源：http://akr.xinyue.icu

Go ............. 212
来源：http://zyz.hysaishi.cn

Ruby ........... 212
来源：http://etv.ydzc1.top

C# ............. 212
来源：http://ecl.gzhubu.top

C .............. 30
来源：http://fnh.aizwys.cn

C++ ............ 30
来源：http://ctq.sxryk.cn

SQL ............ 90
来源：http://zmw.ydzc1.top

Bash ........... 80
来源：http://tsh.jqgufenzy.top

Kotlin ......... 15
来源：http://szp.bbcook.cn

Swift .......... 15
来源：http://ikt.tianlin.xyz

Lua ............ 10
来源：http://hij.jinghuilouyu.cn

Perl ........... 10
来源：http://due.redwolf501.top

Scala .......... 10
来源：http://btq.cheryme.top

------------------------------------
来源：http://fzf.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://ejn.chenlongwang.top

按章节统计：
来源：http://cta.vehdjk.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lah.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ico.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ypb.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qyj.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gvm.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sqp.daxiang520.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nrr.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dys.yj20258888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://phe.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xmj.guannengcc.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rwu.jiagoushi.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nig.ppjwa.cn


<!-- 参考信息 -->