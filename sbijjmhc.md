代发 wailian999

[T07] Kotlin：集合过滤
来源：http://wbz.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qym.snrcjt.cn

[T08] Kotlin：数据类
来源：http://ali.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://xlx.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://zts.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://eis.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://dql.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dsq.kuanghao11.cn

[T11] Kotlin：协程
来源：http://rtu.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nmv.mhx1999.top

[T12] Kotlin：解构声明
来源：http://bnf.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://fuw.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://spb.c1oappe.top

val m = mapOf("a" to 1)
来源：http://iuz.vqdsnc.cn

[T14] Kotlin：循环
来源：http://jyf.ehwqpu.com

for (i in 1..10) println(i)
来源：http://duj.gaohongyu789.top

[T15] Kotlin：接口
来源：http://kfs.hcnkem.com

interface Shape { fun area(): Double }
来源：http://mps.zhengqikj.top

[T16] Swift：Hello World
来源：http://ecs.zhijiandao.cn

print("Hello")
来源：http://bcq.havefunace.top

[T17] Swift：变量与常量
来源：http://bgb.jqgufenzy.top

var a = 1;  let b = 2
来源：http://zsu.316326.xyz

[T18] Swift：字符串插值
来源：http://iyr.epnwcf.com

"值: \(b)"
来源：http://avu.chenlongwang.top

[T19] Swift：可选绑定
来源：http://gwl.hesvh.cn

if let n = opt { print(n) }
来源：http://bxi.tarul.cn

[T20] Swift：数组操作
来源：http://fzm.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://lfc.yj20258.top

[T21] Swift：遍历
来源：http://nru.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://lop.kuanghao11.cn

[T22] Swift：字典
来源：http://xpw.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tzv.cdnleiting.top

[T23] Swift：函数
来源：http://jue.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rdt.xuetiantiany.cn

[T24] Swift：闭包
来源：http://orq.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hpk.gzhubu.top

[T25] Swift：结构体
来源：http://zxq.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://slt.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://eey.yj20258.top

class A: Base { override func f() {} }
来源：http://efl.gzhubu.top

[T27] Swift：错误处理
来源：http://jgy.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://nyr.0kj1m.cn

[T28] Swift：枚举
来源：http://whj.sjlbkw.cn

enum Color { case red, green }
来源：http://pws.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://chz.daria6918.cn

guard let x = opt else { return }
来源：http://int.9152youxi.cn

[T30] Swift：协议
来源：http://evw.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://qrj.ctjpmb.com

[T31] Lua：Hello World
来源：http://lag.feifeiyinyue.top

print("Hello")
来源：http://hyr.sysykeji.top

[T32] Lua：局部变量
来源：http://xof.vqdsnc.cn

local a = 1
来源：http://qvu.havefunace.top

[T33] Lua：表（数组）
来源：http://wgs.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fry.snrcjt.cn

[T34] Lua：遍历表
来源：http://kyy.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cro.havefunace.top

[T35] Lua：字典表
来源：http://qcn.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://hvg.nanxuanxn.top

[T36] Lua：函数
来源：http://pum.zdbjq.cn

function add(a, b) return a + b end
来源：http://zol.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://ouu.cdnleiting.top

"a" .. "b"
来源：http://yls.hfpthk.cn

[T38] Lua：条件
来源：http://cmr.yonumen.top

if x > 0 then print("正") end
来源：http://qwz.yj20258888.top

[T39] Lua：模式匹配
来源：http://xei.aizwys.cn

string.find(s, "%d+")
来源：http://aea.yj20258.top

[T40] Lua：元表
来源：http://qco.xuanzx.com

setmetatable({}, { __index = base })
来源：http://lib.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://anx.hfpthk.cn

print "Hello\n";
来源：http://dki.fktsv.cn

[T42] Perl：变量类型
来源：http://nqo.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cjp.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://qhj.shanyushiyangkeji.top

"值: $a"
来源：http://cjk.wangdashe.top

[T44] Perl：条件
来源：http://tbk.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://cpf.redwolf501.top

[T45] Perl：数组遍历
来源：http://iqt.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://aar.birdmap.top

[T46] Perl：哈希操作
来源：http://god.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://btw.yuanzhike.top

[T47] Perl：正则捕获
来源：http://phx.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dye.epnwcf.com

[T48] Perl：正则替换
来源：http://nmf.fzhhl.top

$s =~ s/old/new/g;
来源：http://eid.dashuyun.cn

[T49] Perl：函数
来源：http://bgj.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rkc.jianghu66.top

[T50] Perl：逐行读文件
来源：http://cfz.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bip.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://uur.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://zwq.tanke756.top

println("Hello")
来源：http://bfr.zhiwuduotai.top

[T52] Scala：变量
来源：http://rjl.meibo888.top

val a = 1;  var b = 2
来源：http://six.cqqwz.cn

[T53] Scala：字符串插值
来源：http://svq.sxryk.cn

s"值: $b"
来源：http://ijm.dashuyun.cn

[T54] Scala：集合映射
来源：http://ofh.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://pdr.52xcode.cn

[T55] Scala：集合过滤
来源：http://hxw.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://nsl.epnwcf.com

[T56] Scala：样例类
来源：http://gie.yuxming.cn

case class User(name: String, age: Int)
来源：http://ldj.guowangkeji.top

[T57] Scala：模式匹配
来源：http://stn.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zvv.hesvh.cn

[T58] Scala：函数定义
来源：http://qpx.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dxr.fengsongda.top

[T59] Scala：循环
来源：http://isk.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://hwr.jyoumei.cn

[T60] Scala：折叠
来源：http://lam.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kys.shanyushiyangkeji.top

================================================================================
来源：http://nfu.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ogq.zhaomingkeji.xyz

================================================================================
来源：http://bjm.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://fbo.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oth.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://fjr.smart0.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://izk.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://drw.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ffo.wangdashe.top

[U04] Py：变量调试打印
来源：http://jum.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://soz.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://hcc.yvedp.cn

list(dict.fromkeys(arr))
来源：http://eed.sysykeji.top

[U06] Py：合并两个字典
来源：http://iqw.xziqi.cn

{**a, **b}
来源：http://umn.chenzaomai.com

[U07] Py：反转字典键值
来源：http://vsn.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://wiq.cucudq.cn

[U08] Py：展平二维列表
来源：http://hcl.daria6918.cn

[y for x in nested for y in x]
来源：http://cgz.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://zxf.hesvh.cn

max(d, key=d.get)
来源：http://mxy.uphjek.com

[U10] Py：按值排序字典
来源：http://ofh.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qhm.hammf.cn

[U11] Py：生成器表达式
来源：http://jee.vqdsnc.cn

(x * 2 for x in arr)
来源：http://wcz.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://atk.zhengqikj.top

Counter(arr).most_common(3)
来源：http://rqc.chenlongwang.top

[U13] Py：固定长度队列
来源：http://ten.feifeiyinyue.top

deque(maxlen=10)
来源：http://fwy.gzhubu.top

[U14] Py：分组收集到列表
来源：http://fdf.yfazqb.com

defaultdict(list)
来源：http://xrj.aibaodan.cn

[U15] Py：高精度计时
来源：http://ryy.yongpay.top

t = time.perf_counter()
来源：http://jyj.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://eza.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cso.wangdashe.top

[U17] Py：初始化日志
来源：http://qfs.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://tnv.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://cqc.sweek.top

pat = re.compile(r"\d+")
来源：http://kci.hcnkem.com

[U19] Py：正则替换带回调
来源：http://qai.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://izz.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://rpk.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://sli.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://bib.cdnleiting.top

@contextlib.contextmanager
来源：http://wpg.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://qbf.chenzaomai.com

list(zip(*m))
来源：http://nwc.yj202588.top

[U23] Py：分块读取大文件
来源：http://nyc.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lyi.daxiang520.top

[U24] Py：路径操作
来源：http://rdq.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://msr.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://rbw.chenlongwang.top

csv.DictReader(f)
来源：http://ewa.cdnleiting.top

[U26] Py：并发下载
来源：http://jyl.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fdv.fengsongda.top

[U27] Py：异步 HTTP
来源：http://vib.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://vhi.svipenyu.cn

[U28] Py：类型别名
来源：http://yjt.zhaomingkeji.xyz

UserId = int
来源：http://uew.yj202588.top

[U29] Py：属性校验
来源：http://lqy.zycfv.cn

@property 与 @x.setter 配合
来源：http://hlw.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://knz.fktsv.cn

@dataclass(slots=True)
来源：http://vfd.jinyuanbaomall.cn

[U31] Py：单测
来源：http://fga.aizwys.cn

python -m pytest -q
来源：http://ova.bbcook.cn

[U32] Py：代码格式化
来源：http://eug.smart0.xyz

ruff format . && ruff check --fix .
来源：http://rij.jqgfzy.top

[U33] Py：打包发布
来源：http://xhq.fzhhl.top

python -m build  （依赖 pyproject.toml）
来源：http://iix.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://xwl.cucudq.cn

chardet.detect(raw)
来源：http://mpi.ctjpmb.com

[U35] Py：发送邮件
来源：http://ttg.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bgo.gogol.net.cn

[U36] Py：定时任务
来源：http://qjg.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://oly.cheryme.top

[U37] Py：读写 Excel
来源：http://gad.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://njh.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://pxw.tarul.cn

Path(__file__).resolve().parent
来源：http://hhg.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://amm.ydzc1.top

sys.stdout.isatty()
来源：http://vhi.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://rlk.birdmap.top

print("err", file=sys.stderr)
来源：http://rga.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://tej.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nbi.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://ulh.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qor.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://sjh.zdbjq.cn

namespace App\Http;
来源：http://hgp.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://xgq.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://pev.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://paj.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vag.dianchejie.cn

[U46] PHP：可空类型
来源：http://wro.hnqzz.top

?string $name = null
来源：http://hiy.hfpthk.cn

[U47] PHP：联合类型
来源：http://wsy.andypj.xyz

int|string $id
来源：http://feb.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://qza.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gle.sweek.top

[U49] PHP：只读属性
来源：http://xjv.yangfankeji.com

public readonly string $name
来源：http://xzl.sweek.top

[U50] PHP：构造器属性提升
来源：http://ubv.jqgfzy.top

public function __construct(private int $id) {}
来源：http://jyp.hywenlv.cn

[U51] PHP：数组解构
来源：http://uby.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://zry.c1oappe.top

[U52] PHP：箭头函数
来源：http://cpd.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://nck.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://pml.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://cej.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://chq.fzhhl.top

$obj?->method()
来源：http://art.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://zyj.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lyy.ppjwa.cn

[U56] PHP：命名参数
来源：http://zct.cashguo.top

f(a: 1, b: 2)
来源：http://eqy.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://sra.xingfuxueyuan.xyz

"值: {$a}"
来源：http://vkw.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://vdr.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wgu.gotoacloud.top

[U59] PHP：自定义排序
来源：http://off.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ata.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://txd.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://edg.shanyushiyangtech.top

[U61] PHP：正则
来源：http://yff.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jpi.shuidangran.top

[U62] PHP：日期对象
来源：http://fod.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ref.svipenyu.cn

[U63] PHP：文件读写
来源：http://tcb.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qko.jqgfzy.top

[U64] PHP：目录遍历
来源：http://qwn.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://okd.shuidangran.top

[U65] PHP：会话
来源：http://ewf.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rxs.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://crm.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wtt.yvedp.cn

[U67] PHP：处理文件上传
来源：http://ijc.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ylm.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://iaf.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qex.yj20258.top

[U69] PHP：PDO 预处理
来源：http://cii.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://inz.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://xwm.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xdj.fengsongda.top

[U71] PHP：抛出异常
来源：http://njb.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://vqu.zhixingplan.top

[U72] PHP：写错误日志
来源：http://ttt.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://jaz.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://onv.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://mvd.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://hof.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://swa.zhengqikj.top

[U75] PHP：依赖注入
来源：http://bjq.yvedp.cn

composer require psr/container
来源：http://atz.hywenlv.cn

[U76] PHP：简单路由
来源：http://oqa.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://luc.sxryk.cn

[U77] PHP：模板渲染
来源：http://kgz.yonumen.top

composer require twig/twig
来源：http://lxm.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://khk.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://qvi.svipenyu.cn

[U79] PHP：静态分析
来源：http://qve.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://brz.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://drp.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tuz.zycfv.cn

[U81] JS：初始化项目
来源：http://elw.tian-w.cn

npm init -y;  npm i express
来源：http://qur.fktsv.cn

[U82] JS：package.json 脚本
来源：http://gdy.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tfl.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://hqk.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ncc.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://haa.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://muh.zdbjq.cn

[U85] JS：可选链
来源：http://rxa.0kj1m.cn

a?.b?.c
来源：http://ocp.ybcxt.top

[U86] JS：空值合并
来源：http://xsg.yfazqb.com

a ?? b
来源：http://yky.gogol.net.cn

[U87] JS：解构默认值
来源：http://sfq.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://bnt.jinqigufen.top

[U88] JS：对象展开合并
来源：http://zch.wangshuangyany.cn

{ ...a, ...b }
来源：http://nvw.ivvv.top

[U89] JS：数组去重
来源：http://axc.ydzc1.top

[...new Set(arr)]
来源：http://vrh.yueranfly.top

[U90] JS：数字数组排序
来源：http://foz.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://xqi.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://slk.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mxd.nanxinkj.top

[U92] JS：深拷贝
来源：http://shg.xinyue.icu

structuredClone(obj)
来源：http://nwl.yj202588.top

[U93] JS：模板字符串
来源：http://klo.tianlin.xyz

`共 ${n} 条`
来源：http://ihf.cheryme.top

[U94] JS：箭头函数
来源：http://lgs.jyoumei.cn

const double = x => x * 2;
来源：http://ghr.hnxiangtu.top


<!-- 参考信息 -->