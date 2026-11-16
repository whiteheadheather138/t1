代发 wailian999

[T41] Perl：Hello World
来源：http://tgv.mhx1999.top

print "Hello\n";
来源：http://gnh.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://lql.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xch.epnwcf.com

[T43] Perl：字符串插值
来源：http://cwu.yueranfly.top

"值: $a"
来源：http://rwi.bjfxy.top

[T44] Perl：条件
来源：http://xpk.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://bti.zhengqikj.top

[T45] Perl：数组遍历
来源：http://mub.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://esd.hammf.cn

[T46] Perl：哈希操作
来源：http://rnc.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vbe.gzhubu.top

[T47] Perl：正则捕获
来源：http://ddu.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ftp.smart0.xyz

[T48] Perl：正则替换
来源：http://ybz.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://bfu.ybcxt.top

[T49] Perl：函数
来源：http://uqh.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pqt.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://qgh.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://jqf.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://nmu.yvedp.cn

[T51] Scala：Hello World
来源：http://jpp.tianlin.xyz

println("Hello")
来源：http://pgj.hesvh.cn

[T52] Scala：变量
来源：http://bls.tianlin.xyz

val a = 1;  var b = 2
来源：http://bjz.tanke756.top

[T53] Scala：字符串插值
来源：http://eqj.zhaomingkeji.xyz

s"值: $b"
来源：http://kkf.xuanzx.com

[T54] Scala：集合映射
来源：http://qvi.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://sfp.nanxinkj.top

[T55] Scala：集合过滤
来源：http://yig.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://brl.yangfankeji.com

[T56] Scala：样例类
来源：http://okk.fzhhl.top

case class User(name: String, age: Int)
来源：http://nbx.bjfxy.top

[T57] Scala：模式匹配
来源：http://rkj.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://mfk.daxiang520.top

[T58] Scala：函数定义
来源：http://ods.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://hkp.ppjwa.cn

[T59] Scala：循环
来源：http://mvq.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://ows.ivvv.top

[T60] Scala：折叠
来源：http://wvr.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kpn.ywan-chungtsiang.top

================================================================================
来源：http://rhh.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nhk.ivvv.top

================================================================================
来源：http://zhb.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://odf.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tdv.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://qez.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qmf.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://loi.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bnz.redwolf501.top

[U04] Py：变量调试打印
来源：http://jhu.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ipj.yueranfly.top

[U05] Py：列表去重且保序
来源：http://agb.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://prt.xuanzx.com

[U06] Py：合并两个字典
来源：http://uho.hysaishi.cn

{**a, **b}
来源：http://gwi.yj20258.top

[U07] Py：反转字典键值
来源：http://pik.cashguo.top

{v: k for k, v in d.items()}
来源：http://rdc.zhixingplan.top

[U08] Py：展平二维列表
来源：http://kpd.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://gck.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://wdy.xuanzx.com

max(d, key=d.get)
来源：http://alm.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://vvp.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bkt.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://umq.fzhhl.top

(x * 2 for x in arr)
来源：http://mts.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kpa.tianlin.xyz

Counter(arr).most_common(3)
来源：http://zmi.redwolf501.top

[U13] Py：固定长度队列
来源：http://ayy.jinqigfzy.top

deque(maxlen=10)
来源：http://qcp.xylfe.cn

[U14] Py：分组收集到列表
来源：http://vpv.haohaochexian.top

defaultdict(list)
来源：http://yul.yuanzhike.top

[U15] Py：高精度计时
来源：http://tmn.yuxming.cn

t = time.perf_counter()
来源：http://jsa.aibaodan.cn

[U16] Py：命令行参数解析
来源：http://hei.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://luz.yongpay.top

[U17] Py：初始化日志
来源：http://vjy.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://tym.jianghu66.top

[U18] Py：预编译正则
来源：http://cvk.tian-w.cn

pat = re.compile(r"\d+")
来源：http://cun.yj20258888.top

[U19] Py：正则替换带回调
来源：http://cug.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gce.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://map.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://lsz.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://twq.zhijiandao.cn

@contextlib.contextmanager
来源：http://yac.pycfn.com

[U22] Py：矩阵转置
来源：http://pxc.tanke756.top

list(zip(*m))
来源：http://gtq.xinyue.icu

[U23] Py：分块读取大文件
来源：http://brh.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://twv.shzxlz.cn

[U24] Py：路径操作
来源：http://snj.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zrj.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://opc.ydjk.org.cn

csv.DictReader(f)
来源：http://glx.yanxiufei.cn

[U26] Py：并发下载
来源：http://xzn.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mpb.yj202588.top

[U27] Py：异步 HTTP
来源：http://uhm.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://lzi.hysaishi.cn

[U28] Py：类型别名
来源：http://olv.jianghu66.top

UserId = int
来源：http://tsu.tianlin.xyz

[U29] Py：属性校验
来源：http://kuh.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://ngj.cdnleiting.top

[U30] Py：数据类
来源：http://xnn.jianghu66.top

@dataclass(slots=True)
来源：http://rgk.bbcook.cn

[U31] Py：单测
来源：http://wrw.vqdsnc.cn

python -m pytest -q
来源：http://xec.316326.xyz

[U32] Py：代码格式化
来源：http://won.meibo888.top

ruff format . && ruff check --fix .
来源：http://vsd.bjfxy.top

[U33] Py：打包发布
来源：http://uux.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://uxt.uphjek.com

[U34] Py：判断编码
来源：http://hwg.uphjek.com

chardet.detect(raw)
来源：http://yrn.sysykeji.top

[U35] Py：发送邮件
来源：http://lxb.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wtf.9152youxi.cn

[U36] Py：定时任务
来源：http://wwj.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://xbn.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://iea.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://tct.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://zxv.jiagoushi.top

Path(__file__).resolve().parent
来源：http://vpw.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://mcq.feifeiyinyue.top

sys.stdout.isatty()
来源：http://esg.gzhubu.top

[U40] Py：打印到标准错误
来源：http://doo.hammf.cn

print("err", file=sys.stderr)
来源：http://myr.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://qbd.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yny.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://uyg.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iec.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://ure.yongpay.top

namespace App\Http;
来源：http://vxd.aizwys.cn

[U44] PHP：开启严格类型
来源：http://hle.yj20258888.top

declare(strict_types=1);
来源：http://mgb.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://lny.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ygh.aizwys.cn

[U46] PHP：可空类型
来源：http://pfa.zhongyouzk.top

?string $name = null
来源：http://aio.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://qsb.jinqigfzy.top

int|string $id
来源：http://enj.ehwqpu.com

[U48] PHP：纯枚举
来源：http://jru.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qpr.cashguo.top

[U49] PHP：只读属性
来源：http://fde.shanyushiyangtech.top

public readonly string $name
来源：http://ovm.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://oat.yuanzhike.top

public function __construct(private int $id) {}
来源：http://zjm.jinqigfzy.top

[U51] PHP：数组解构
来源：http://odd.kuanghao11.cn

[$a, $b] = $arr;
来源：http://egr.cheryme.top

[U52] PHP：箭头函数
来源：http://sop.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://wng.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://hgf.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://mur.hcnkem.com

[U54] PHP：空安全调用
来源：http://ahx.birdmap.top

$obj?->method()
来源：http://kfs.yangfankeji.com

[U55] PHP：match 表达式
来源：http://qym.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ing.zhixingplan.top

[U56] PHP：命名参数
来源：http://wmg.cdnleiting.top

f(a: 1, b: 2)
来源：http://uyz.yj202588.top

[U57] PHP：字符串插值
来源：http://mce.yangfankeji.com

"值: {$a}"
来源：http://pqu.snrcjt.cn

[U58] PHP：数组三件套
来源：http://jzr.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gqf.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://uwg.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://srm.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://xrr.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dfs.cqqwz.cn

[U61] PHP：正则
来源：http://zot.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://geg.tian-w.cn

[U62] PHP：日期对象
来源：http://tzz.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yal.sxryk.cn

[U63] PHP：文件读写
来源：http://aga.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hug.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://irr.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://jch.yanxiufei.cn

[U65] PHP：会话
来源：http://rii.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://hor.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://cda.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fym.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://owb.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aql.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://ofd.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rxe.316326.xyz

[U69] PHP：PDO 预处理
来源：http://ctb.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mfk.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://tkv.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gbu.yfazqb.com

[U71] PHP：抛出异常
来源：http://nxg.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://aga.jqgfzy.top

[U72] PHP：写错误日志
来源：http://prc.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://jhg.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://zhr.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://srn.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://tcf.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://nzj.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://ggi.chenjidiqi.icu

composer require psr/container
来源：http://qrt.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://jhi.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://epk.yueranfly.top

[U77] PHP：模板渲染
来源：http://oeq.nwbrower.top

composer require twig/twig
来源：http://jmv.sxryk.cn

[U78] PHP：单元测试
来源：http://qqz.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://mhy.hammf.cn

[U79] PHP：静态分析
来源：http://ceg.hammf.cn

composer require --dev phpstan/phpstan
来源：http://vtu.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://rss.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://glk.chenzaomai.com

[U81] JS：初始化项目
来源：http://mxg.cqqwz.cn

npm init -y;  npm i express
来源：http://tkn.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://myx.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yho.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://ymu.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://ljg.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://jpl.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://kip.ppjwa.cn

[U85] JS：可选链
来源：http://cjk.yonumen.top

a?.b?.c
来源：http://fli.zycfv.cn

[U86] JS：空值合并
来源：http://djl.cucudq.cn

a ?? b
来源：http://hmh.ydzc1.top

[U87] JS：解构默认值
来源：http://qxy.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://mqx.birdmap.top

[U88] JS：对象展开合并
来源：http://wzj.mhx1999.top

{ ...a, ...b }
来源：http://clm.sweek.top

[U89] JS：数组去重
来源：http://rrd.jqgfzy.top

[...new Set(arr)]
来源：http://ypg.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://mxz.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://zfk.cheryme.top

[U91] JS：对象键值遍历
来源：http://dbw.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xto.cucudq.cn

[U92] JS：深拷贝
来源：http://hnb.cdnleiting.top

structuredClone(obj)
来源：http://wsr.sxryk.cn

[U93] JS：模板字符串
来源：http://tfh.shangyingyoupin.top

`共 ${n} 条`
来源：http://jpg.sxryk.cn

[U94] JS：箭头函数
来源：http://wyc.jinqigufen.top

const double = x => x * 2;
来源：http://rsn.birdmap.top

[U95] JS：Promise 包装
来源：http://vnx.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://yed.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://brj.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://chq.yfazqb.com

[U97] JS：并发请求
来源：http://bux.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kuh.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://tmm.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rli.ydzc1.top

[U99] JS：事件监听
来源：http://dem.meibo888.top

el.addEventListener("click", e => {})
来源：http://nhz.havefunace.top

[U100] JS：DOM 查询
来源：http://wwb.cdnleiting.top

document.querySelector(".item")
来源：http://ghe.zhixingplan.top

[U101] JS：classList 操作
来源：http://qep.xuetiantiany.cn

el.classList.toggle("active")
来源：http://nfp.hammf.cn

[U102] JS：本地存储
来源：http://djp.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jjc.gotoacloud.top

[U103] JS：定时器
来源：http://qsk.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zls.ybcxt.top

[U104] JS：防抖
来源：http://ldt.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://udd.vehdjk.com

[U105] JS：节流
来源：http://smx.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wxm.iojbl.cn

[U106] JS：日期格式化
来源：http://zjc.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gum.hcnkem.com

[U107] JS：数字千分位
来源：http://xlf.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zug.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://hdw.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iep.iojbl.cn

[U109] JS：数组分组
来源：http://mgt.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://mke.guowangkeji.top

[U110] JS：数组分块
来源：http://prj.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hwq.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://vvw.pycfn.com

new Map(Object.entries(obj))
来源：http://wja.guannengcc.top

[U112] JS：字符串补位
来源：http://qcp.hnxiangtu.top

"7".padStart(3, "0")
来源：http://xej.chenlongwang.top

[U113] JS：正则替换全部
来源：http://vpf.aibaodan.cn

s.replaceAll("a", "b")
来源：http://mak.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://jwg.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qow.xinyue.icu

[U115] JS：生成 UUID
来源：http://ndc.jqgfzy.top

crypto.randomUUID()
来源：http://jmy.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://hqe.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://axd.smart0.xyz

[U117] JS：单元测试
来源：http://ldv.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://gvz.pycfn.com

[U118] JS：开发服务器
来源：http://wpw.chenjidiqi.icu

npm i -D vite;  npx vite
来源：http://cpf.vqdsnc.cn

[U119] JS：生产构建
来源：http://cbz.svipenyu.cn

npx vite build
来源：http://glh.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://ywh.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://jsq.yuxming.cn

================================================================================
来源：http://sit.yj202588.top

统计汇总
来源：http://kvz.shzxlz.cn

================================================================================
来源：http://qhj.ydjk.org.cn

按语言统计（条）：
来源：http://atn.hammf.cn

Python ......... 252
来源：http://wdz.redwolf501.top

PHP ............ 252
来源：http://iag.guowangkeji.top

JavaScript ..... 252
来源：http://gvc.kuanghao11.cn

TypeScript ..... 212
来源：http://day.yangfankeji.com

Java ........... 212
来源：http://gyj.yonumen.top

Go ............. 212
来源：http://avy.zhengqikj.top

Ruby ........... 212
来源：http://hvv.ydjk.org.cn

C# ............. 212
来源：http://ayl.xylfe.cn

C .............. 30
来源：http://uxv.shuidangran.top

C++ ............ 30
来源：http://uqu.xuanzx.com

SQL ............ 90
来源：http://fki.fktsv.cn

Bash ........... 80
来源：http://ohg.daxiang520.top


<!-- 参考信息 -->