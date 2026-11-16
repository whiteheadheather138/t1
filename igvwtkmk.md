代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://qmp.haohaochexian.top

[T51] Scala：Hello World
来源：http://kij.ywan-chungtsiang.top

println("Hello")
来源：http://etb.redwolf501.top

[T52] Scala：变量
来源：http://psi.xziqi.cn

val a = 1;  var b = 2
来源：http://xjf.guannengcc.top

[T53] Scala：字符串插值
来源：http://qyu.epnwcf.com

s"值: $b"
来源：http://pvm.316326.xyz

[T54] Scala：集合映射
来源：http://xut.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://vhx.jiagoushi.top

[T55] Scala：集合过滤
来源：http://iqg.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fkq.tarul.cn

[T56] Scala：样例类
来源：http://shi.c1oappe.top

case class User(name: String, age: Int)
来源：http://mib.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://sgu.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qsd.yj202588.top

[T58] Scala：函数定义
来源：http://xfv.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kax.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://onb.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://lrz.yj202588.top

[T60] Scala：折叠
来源：http://wtw.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://trg.shuidangran.top

================================================================================
来源：http://jpp.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ric.yj20258.top

================================================================================
来源：http://dva.cashguo.top

[U01] Py：创建虚拟环境
来源：http://ctd.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://kmo.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://uyb.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mpe.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://bdy.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jui.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://dvw.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nka.wangdashe.top

[U05] Py：列表去重且保序
来源：http://phd.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://tij.dashuyun.cn

[U06] Py：合并两个字典
来源：http://pkr.hysaishi.cn

{**a, **b}
来源：http://pdg.iojbl.cn

[U07] Py：反转字典键值
来源：http://fqa.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://jox.yuanzhike.top

[U08] Py：展平二维列表
来源：http://cux.bjfxy.top

[y for x in nested for y in x]
来源：http://krv.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://ppp.xylfe.cn

max(d, key=d.get)
来源：http://imh.ehwqpu.com

[U10] Py：按值排序字典
来源：http://xiv.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oqq.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://bvt.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://xyk.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://lgx.zhengqikj.top

Counter(arr).most_common(3)
来源：http://fxt.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://kdt.shangyingyoupin.top

deque(maxlen=10)
来源：http://pbv.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://jol.aizwys.cn

defaultdict(list)
来源：http://qtn.fzhhl.top

[U15] Py：高精度计时
来源：http://rzl.nanxinkj.top

t = time.perf_counter()
来源：http://ouk.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://zpu.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qeu.yanxiufei.cn

[U17] Py：初始化日志
来源：http://teh.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://cpp.tarul.cn

[U18] Py：预编译正则
来源：http://xgf.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://cle.gzhubu.top

[U19] Py：正则替换带回调
来源：http://fcp.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gto.fengsongda.top

[U20] Py：缓存函数结果
来源：http://foh.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://oyo.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://jqv.ehwqpu.com

@contextlib.contextmanager
来源：http://boi.daria6918.cn

[U22] Py：矩阵转置
来源：http://lgu.zhongyouzk.top

list(zip(*m))
来源：http://xbo.pycfn.com

[U23] Py：分块读取大文件
来源：http://itv.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jmt.daria6918.cn

[U24] Py：路径操作
来源：http://urf.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qbd.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://qik.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://cow.mhx1999.top

[U26] Py：并发下载
来源：http://fwa.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://edv.yj20258.top

[U27] Py：异步 HTTP
来源：http://lix.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://hec.daria6918.cn

[U28] Py：类型别名
来源：http://xgm.zdqjudy.top

UserId = int
来源：http://fdu.zhixingplan.top

[U29] Py：属性校验
来源：http://djn.mhx1999.top

@property 与 @x.setter 配合
来源：http://qgh.jlsjyb.cn

[U30] Py：数据类
来源：http://uwe.mhx1999.top

@dataclass(slots=True)
来源：http://wyp.gzhubu.top

[U31] Py：单测
来源：http://gys.tarul.cn

python -m pytest -q
来源：http://mrr.cdnleiting.top

[U32] Py：代码格式化
来源：http://som.aizwys.cn

ruff format . && ruff check --fix .
来源：http://msa.fengsongda.top

[U33] Py：打包发布
来源：http://msd.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://saw.zhixingplan.top

[U34] Py：判断编码
来源：http://lvj.yuxming.cn

chardet.detect(raw)
来源：http://tlv.hesvh.cn

[U35] Py：发送邮件
来源：http://gku.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tkt.chenlongwang.top

[U36] Py：定时任务
来源：http://ljf.sweek.top

schedule.every(10).minutes.do(job)
来源：http://bab.ybcxt.top

[U37] Py：读写 Excel
来源：http://ipn.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://umm.yfazqb.com

[U38] Py：获取脚本所在目录
来源：http://htw.aizwys.cn

Path(__file__).resolve().parent
来源：http://vyq.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://ooi.yonumen.top

sys.stdout.isatty()
来源：http://png.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://psc.hcnkem.com

print("err", file=sys.stderr)
来源：http://pzw.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://xuh.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mzj.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://adg.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xmw.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://ioq.daxiang520.top

namespace App\Http;
来源：http://lqp.sysykeji.top

[U44] PHP：开启严格类型
来源：http://tnv.aizwys.cn

declare(strict_types=1);
来源：http://ins.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://fce.yanxiufei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jhy.guowangkeji.top

[U46] PHP：可空类型
来源：http://oky.gzhubu.top

?string $name = null
来源：http://ygz.jqgufenzy.top

[U47] PHP：联合类型
来源：http://ymq.jyoumei.cn

int|string $id
来源：http://eqj.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://bvf.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zos.bbcook.cn

[U49] PHP：只读属性
来源：http://zon.jqgfzy.top

public readonly string $name
来源：http://ieg.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://ove.tanke756.top

public function __construct(private int $id) {}
来源：http://xgp.316326.xyz

[U51] PHP：数组解构
来源：http://nze.meibo888.top

[$a, $b] = $arr;
来源：http://esu.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://fgl.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://wip.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://ktm.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://fxz.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://oyf.pycfn.com

$obj?->method()
来源：http://izn.hysaishi.cn

[U55] PHP：match 表达式
来源：http://slm.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ybi.jinqigfzy.top

[U56] PHP：命名参数
来源：http://aik.yfazqb.com

f(a: 1, b: 2)
来源：http://loq.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://hen.sxryk.cn

"值: {$a}"
来源：http://mpx.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://ncc.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vbo.bjfxy.top

[U59] PHP：自定义排序
来源：http://izm.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dpe.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://jqx.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nxm.jlsjyb.cn

[U61] PHP：正则
来源：http://awv.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xsq.9152youxi.cn

[U62] PHP：日期对象
来源：http://wac.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yhq.snrcjt.cn

[U63] PHP：文件读写
来源：http://egr.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gfh.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://udb.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://rdf.quarkkingdee.top

[U65] PHP：会话
来源：http://ozk.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iwg.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://xsq.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qot.jinyuanbaomall.cn

[U67] PHP：处理文件上传
来源：http://nhj.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zgj.sysykeji.top

[U68] PHP：PDO 连接
来源：http://dig.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ebb.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://mmo.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ykc.shanyushiyangtech.top

[U70] PHP：PDO 事务
来源：http://fbj.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lhn.fehbvm.com

[U71] PHP：抛出异常
来源：http://taf.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://svu.ydzc1.top

[U72] PHP：写错误日志
来源：http://udt.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://yog.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://rgy.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://pcu.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://hcl.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://fgy.jianghu66.top

[U75] PHP：依赖注入
来源：http://vah.dianchejie.cn

composer require psr/container
来源：http://tzz.hysaishi.cn

[U76] PHP：简单路由
来源：http://ird.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pqw.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://hyn.nwbrower.top

composer require twig/twig
来源：http://ulu.52xcode.cn

[U78] PHP：单元测试
来源：http://zjq.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://mow.birdmap.top

[U79] PHP：静态分析
来源：http://tki.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://wzd.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://kuk.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bho.yj20258888.top

[U81] JS：初始化项目
来源：http://xzk.jlsjyb.cn

npm init -y;  npm i express
来源：http://zct.hnqzz.top

[U82] JS：package.json 脚本
来源：http://uxk.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rka.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://aqu.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dfq.cashguo.top

[U84] JS：CommonJS 写法
来源：http://tmh.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rvw.ivvv.top

[U85] JS：可选链
来源：http://alq.ybcxt.top

a?.b?.c
来源：http://aww.andypj.xyz

[U86] JS：空值合并
来源：http://cwq.hammf.cn

a ?? b
来源：http://neu.tanke756.top

[U87] JS：解构默认值
来源：http://nha.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://tsb.hammf.cn

[U88] JS：对象展开合并
来源：http://hbo.chenzaomai.com

{ ...a, ...b }
来源：http://qik.hnxiangtu.top

[U89] JS：数组去重
来源：http://wsa.tian-w.cn

[...new Set(arr)]
来源：http://awn.316326.xyz

[U90] JS：数字数组排序
来源：http://xvu.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://jmg.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://lnf.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hdl.xziqi.cn

[U92] JS：深拷贝
来源：http://lvd.fzhhl.top

structuredClone(obj)
来源：http://wkl.smart0.xyz

[U93] JS：模板字符串
来源：http://veu.yuxming.cn

`共 ${n} 条`
来源：http://kjy.zhixingplan.top

[U94] JS：箭头函数
来源：http://kaw.sweek.top

const double = x => x * 2;
来源：http://mct.jyoumei.cn

[U95] JS：Promise 包装
来源：http://sle.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://emi.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://oaz.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wkc.jinqigfzy.top

[U97] JS：并发请求
来源：http://eha.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fiw.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://qkc.yvedp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fws.chenzaomai.com

[U99] JS：事件监听
来源：http://end.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://pdx.sxryk.cn

[U100] JS：DOM 查询
来源：http://cqa.xylfe.cn

document.querySelector(".item")
来源：http://lsk.cucudq.cn

[U101] JS：classList 操作
来源：http://krt.52xcode.cn

el.classList.toggle("active")
来源：http://czz.birdmap.top

[U102] JS：本地存储
来源：http://yvi.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://owu.wangdashe.top

[U103] JS：定时器
来源：http://xue.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://whj.yangfankeji.com

[U104] JS：防抖
来源：http://sfa.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcf.havefunace.top

[U105] JS：节流
来源：http://ist.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nrc.yfazqb.com

[U106] JS：日期格式化
来源：http://geq.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://geu.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://bhl.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bjp.tian-w.cn

[U108] JS：随机整数
来源：http://oqb.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bvq.ydjk.org.cn

[U109] JS：数组分组
来源：http://piw.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://osr.316326.xyz

[U110] JS：数组分块
来源：http://qbx.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qzr.pycfn.com

[U111] JS：对象转 Map
来源：http://aob.hammf.cn

new Map(Object.entries(obj))
来源：http://loq.c1oappe.top

[U112] JS：字符串补位
来源：http://taf.bbcook.cn

"7".padStart(3, "0")
来源：http://hbh.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://rdg.zdbjq.cn

s.replaceAll("a", "b")
来源：http://jmc.yueranfly.top

[U114] JS：JSON 深比较
来源：http://fff.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://brs.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://sui.hnxiangtu.top

crypto.randomUUID()
来源：http://daf.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://isw.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://jgh.cashguo.top

[U117] JS：单元测试
来源：http://bcl.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://kcu.jlsjyb.cn

[U118] JS：开发服务器
来源：http://okl.hesvh.cn

npm i -D vite;  npx vite
来源：http://dbv.meibo888.top

[U119] JS：生产构建
来源：http://klj.andypj.xyz

npx vite build
来源：http://dxg.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://wuu.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://crv.jinqigfzy.top

================================================================================
来源：http://eha.bbcook.cn

统计汇总
来源：http://svi.aizwys.cn

================================================================================
来源：http://mvl.pengpengdd.cyou

按语言统计（条）：
来源：http://uon.zdbjq.cn

Python ......... 252
来源：http://sey.pycfn.com

PHP ............ 252
来源：http://xdn.jiagoushi.top

JavaScript ..... 252
来源：http://nph.xziqi.cn

TypeScript ..... 212
来源：http://obf.zycfv.cn

Java ........... 212
来源：http://fto.wangshuangyany.cn

Go ............. 212
来源：http://cyq.zhiwuduotai.top

Ruby ........... 212
来源：http://jsi.zdqjudy.top

C# ............. 212
来源：http://vei.jqgufenzy.top

C .............. 30
来源：http://sao.jiagoushi.top

C++ ............ 30
来源：http://qll.jiagoushi.top

SQL ............ 90
来源：http://dvt.ctjpmb.com

Bash ........... 80
来源：http://gpp.sufxvd.cn

Kotlin ......... 15
来源：http://bgc.xziqi.cn

Swift .......... 15
来源：http://rza.haohaochexian.top

Lua ............ 10
来源：http://dzy.shanyushiyangtech.top

Perl ........... 10
来源：http://qjw.shanyushiyangkeji.top

Scala .......... 10
来源：http://ecg.tian-w.cn

------------------------------------
来源：http://zpj.jiagoushi.top

合计 ........... 2106 条
来源：http://odj.jianghu66.top

按章节统计：
来源：http://xsd.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bch.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://crn.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vvz.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yhm.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ind.zhixingplan.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aqm.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ymx.jqgfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://njx.yueranfly.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qqf.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tui.jqgufenzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sxs.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gso.jinqigufen.top


<!-- 参考信息 -->