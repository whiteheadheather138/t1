代发 wailian999

[T01] Kotlin：Hello World
来源：http://tip.hywenlv.cn

println("Hello")
来源：http://bvj.yueranfly.top

[T02] Kotlin：变量
来源：http://glw.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dvm.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://iox.hesvh.cn

"值: $b"
来源：http://ecy.nwbrower.top

[T04] Kotlin：空安全
来源：http://sjf.daxiang520.top

val n: String? = null;  n?.length
来源：http://hmp.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://keu.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wjr.andypj.xyz

[T06] Kotlin：集合映射
来源：http://ggo.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cya.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://svg.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yuo.wangdashe.top

[T08] Kotlin：数据类
来源：http://xar.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://kjv.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://gog.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://doy.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://swt.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bcz.andypj.xyz

[T11] Kotlin：协程
来源：http://oxa.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://npr.nwbrower.top

[T12] Kotlin：解构声明
来源：http://eui.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://uzc.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://kqs.xylfe.cn

val m = mapOf("a" to 1)
来源：http://uvj.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://qba.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://bss.xuanzx.com

[T15] Kotlin：接口
来源：http://xgk.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://ytr.yongpay.top

[T16] Swift：Hello World
来源：http://kys.yuanzhike.top

print("Hello")
来源：http://zot.yj202588.top

[T17] Swift：变量与常量
来源：http://wrz.yj20258.top

var a = 1;  let b = 2
来源：http://fwv.cqqwz.cn

[T18] Swift：字符串插值
来源：http://nry.9152youxi.cn

"值: \(b)"
来源：http://xxc.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://cxk.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://gwe.zycfv.cn

[T20] Swift：数组操作
来源：http://fbm.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zef.hnxiangtu.top

[T21] Swift：遍历
来源：http://wlk.tarul.cn

for x in a { print(x) }
来源：http://dqf.cashguo.top

[T22] Swift：字典
来源：http://clg.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pui.xylfe.cn

[T23] Swift：函数
来源：http://aev.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ruk.sufxvd.cn

[T24] Swift：闭包
来源：http://tzc.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zuu.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://lxd.fanxiaobao.xyz

struct P { var x: Int }
来源：http://pwi.xylfe.cn

[T26] Swift：类与重写
来源：http://rtt.cashguo.top

class A: Base { override func f() {} }
来源：http://spr.hfpthk.cn

[T27] Swift：错误处理
来源：http://beo.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://fxn.hfpthk.cn

[T28] Swift：枚举
来源：http://coj.zhoulong.xyz

enum Color { case red, green }
来源：http://hej.meibo888.top

[T29] Swift：guard 提前返回
来源：http://hmc.gotoacloud.top

guard let x = opt else { return }
来源：http://ppb.aizwys.cn

[T30] Swift：协议
来源：http://ffz.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://ahw.yj20258.top

[T31] Lua：Hello World
来源：http://psr.zycfv.cn

print("Hello")
来源：http://fdk.aizwys.cn

[T32] Lua：局部变量
来源：http://nnn.fktsv.cn

local a = 1
来源：http://vln.zhixingplan.top

[T33] Lua：表（数组）
来源：http://yre.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nhl.ctjpmb.com

[T34] Lua：遍历表
来源：http://yno.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yhm.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://eay.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://uls.jinghuilouyu.cn

[T36] Lua：函数
来源：http://xet.tanke756.top

function add(a, b) return a + b end
来源：http://nek.pycfn.com

[T37] Lua：字符串拼接
来源：http://zyc.ppjwa.cn

"a" .. "b"
来源：http://fjr.xinyue.icu

[T38] Lua：条件
来源：http://eaw.sjlbkw.cn

if x > 0 then print("正") end
来源：http://hka.yonumen.top

[T39] Lua：模式匹配
来源：http://ogs.gaohongyu789.top

string.find(s, "%d+")
来源：http://gbp.cashguo.top

[T40] Lua：元表
来源：http://vbe.iojbl.cn

setmetatable({}, { __index = base })
来源：http://wct.sxryk.cn

[T41] Perl：Hello World
来源：http://wky.yj202588.top

print "Hello\n";
来源：http://cdu.nanxuanxn.top

[T42] Perl：变量类型
来源：http://apy.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://owu.tian-w.cn

[T43] Perl：字符串插值
来源：http://grk.cdnleiting.top

"值: $a"
来源：http://lbi.yuanzhike.top

[T44] Perl：条件
来源：http://fpd.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://mxd.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://fpq.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://ace.yuxming.cn

[T46] Perl：哈希操作
来源：http://bxo.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://njx.epnwcf.com

[T47] Perl：正则捕获
来源：http://bum.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hxn.daxiang520.top

[T48] Perl：正则替换
来源：http://qon.0kj1m.cn

$s =~ s/old/new/g;
来源：http://iwb.kuanghao11.cn

[T49] Perl：函数
来源：http://yyz.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggh.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://glb.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://see.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://loh.fzhhl.top

[T51] Scala：Hello World
来源：http://kgl.hnxiangtu.top

println("Hello")
来源：http://ksp.aizwys.cn

[T52] Scala：变量
来源：http://cma.yueranfly.top

val a = 1;  var b = 2
来源：http://vea.hfpthk.cn

[T53] Scala：字符串插值
来源：http://mst.dashuyun.cn

s"值: $b"
来源：http://hdc.pycfn.com

[T54] Scala：集合映射
来源：http://iak.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://hif.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://mmk.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://jsg.daria6918.cn

[T56] Scala：样例类
来源：http://ghv.cashguo.top

case class User(name: String, age: Int)
来源：http://niy.0kj1m.cn

[T57] Scala：模式匹配
来源：http://zac.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ulc.nanxuanxn.top

[T58] Scala：函数定义
来源：http://yst.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mfi.cdnleiting.top

[T59] Scala：循环
来源：http://nwe.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://hta.guannengcc.top

[T60] Scala：折叠
来源：http://pvy.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gss.yuxming.cn

================================================================================
来源：http://arr.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ooq.yongpay.top

================================================================================
来源：http://fso.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://mgw.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://day.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://wlo.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cvg.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://yxy.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://hhu.vehdjk.com

[U04] Py：变量调试打印
来源：http://orq.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rpb.havefunace.top

[U05] Py：列表去重且保序
来源：http://gfb.yongpay.top

list(dict.fromkeys(arr))
来源：http://fsi.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://xdn.pengpengdd.cyou

{**a, **b}
来源：http://mcf.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://uta.havefunace.top

{v: k for k, v in d.items()}
来源：http://otu.jqgfzy.top

[U08] Py：展平二维列表
来源：http://wbz.dashuyun.cn

[y for x in nested for y in x]
来源：http://ywu.cashguo.top

[U09] Py：字典取最大值的键
来源：http://oqh.hongshengwenyu.top

max(d, key=d.get)
来源：http://vxt.jyoumei.cn

[U10] Py：按值排序字典
来源：http://zxw.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qet.ppjwa.cn

[U11] Py：生成器表达式
来源：http://jil.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://xiw.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://dqy.c1oappe.top

Counter(arr).most_common(3)
来源：http://wmr.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://tvt.yonumen.top

deque(maxlen=10)
来源：http://vxd.bjfxy.top

[U14] Py：分组收集到列表
来源：http://nfn.zycfv.cn

defaultdict(list)
来源：http://ppf.jqgfzy.top

[U15] Py：高精度计时
来源：http://ghg.yj20258.top

t = time.perf_counter()
来源：http://eoo.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://kvz.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xui.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://inb.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://fsg.bjfxy.top

[U18] Py：预编译正则
来源：http://pec.fzhhl.top

pat = re.compile(r"\d+")
来源：http://yho.sysykeji.top

[U19] Py：正则替换带回调
来源：http://evb.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uyu.daxiang520.top

[U20] Py：缓存函数结果
来源：http://tkn.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://yqe.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://obw.bjfxy.top

@contextlib.contextmanager
来源：http://usz.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://ghs.sufxvd.cn

list(zip(*m))
来源：http://gdc.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://xhe.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://unp.pengpengdd.cyou

[U24] Py：路径操作
来源：http://dno.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://obq.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://ush.fktsv.cn

csv.DictReader(f)
来源：http://zqc.zhoulong.xyz

[U26] Py：并发下载
来源：http://tga.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oyh.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://kmv.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://juy.uphjek.com

[U28] Py：类型别名
来源：http://kvv.aizwys.cn

UserId = int
来源：http://arb.aibaodan.cn

[U29] Py：属性校验
来源：http://whs.yuxming.cn

@property 与 @x.setter 配合
来源：http://ssv.jianghu66.top

[U30] Py：数据类
来源：http://ggr.hfpthk.cn

@dataclass(slots=True)
来源：http://jpq.gogol.net.cn

[U31] Py：单测
来源：http://mxd.ehwqpu.com

python -m pytest -q
来源：http://snd.hysaishi.cn

[U32] Py：代码格式化
来源：http://inb.gzhubu.top

ruff format . && ruff check --fix .
来源：http://nxd.ivvv.top

[U33] Py：打包发布
来源：http://xug.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://ufd.ivvv.top

[U34] Py：判断编码
来源：http://fdm.mhx1999.top

chardet.detect(raw)
来源：http://fyn.meibo888.top

[U35] Py：发送邮件
来源：http://rlh.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dyt.redwolf501.top

[U36] Py：定时任务
来源：http://fxm.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://fzm.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://elf.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://qio.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://fvd.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://kqa.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://uja.tian-w.cn

sys.stdout.isatty()
来源：http://ojg.aizwys.cn

[U40] Py：打印到标准错误
来源：http://lzc.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://vjd.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://lmc.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zmz.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://ncw.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lur.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://kyq.xuanzx.com

namespace App\Http;
来源：http://mbe.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://xwq.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://fif.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://fse.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lxi.jlsjyb.cn

[U46] PHP：可空类型
来源：http://bln.hongshengwenyu.top

?string $name = null
来源：http://cyq.yongpay.top

[U47] PHP：联合类型
来源：http://sxv.hesvh.cn

int|string $id
来源：http://fuv.sufxvd.cn

[U48] PHP：纯枚举
来源：http://xfv.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kct.yj20258888.top

[U49] PHP：只读属性
来源：http://bym.yueranfly.top

public readonly string $name
来源：http://lzh.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://bja.zdqjudy.top

public function __construct(private int $id) {}
来源：http://bsu.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://vyt.mhx1999.top

[$a, $b] = $arr;
来源：http://yxk.yj20258.top

[U52] PHP：箭头函数
来源：http://iwt.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://mta.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://uhi.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://xbb.redwolf501.top

[U54] PHP：空安全调用
来源：http://dlc.tanke756.top

$obj?->method()
来源：http://vwp.zdbjq.cn

[U55] PHP：match 表达式
来源：http://ksa.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jeq.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://slc.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://ypt.epnwcf.com

[U57] PHP：字符串插值
来源：http://xhg.yvedp.cn

"值: {$a}"
来源：http://vsm.hesvh.cn

[U58] PHP：数组三件套
来源：http://xyw.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wzu.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://nbh.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iit.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://duo.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mae.xuanzx.com

[U61] PHP：正则
来源：http://jfx.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iuy.daxiang520.top

[U62] PHP：日期对象
来源：http://yqc.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://suq.tian-w.cn

[U63] PHP：文件读写
来源：http://knn.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gbi.birdmap.top

[U64] PHP：目录遍历
来源：http://iap.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://yyi.fktsv.cn

[U65] PHP：会话
来源：http://ukl.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fev.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://ezo.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sav.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://xfq.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kzu.wangdashe.top

[U68] PHP：PDO 连接
来源：http://uhc.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kgb.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://qpb.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wgm.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://lwj.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gkt.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://uay.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://yam.daria6918.cn

[U72] PHP：写错误日志
来源：http://hgt.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://vas.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://irv.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://mpy.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://kxc.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://xhx.guannengcc.top

[U75] PHP：依赖注入
来源：http://ehh.cheryme.top

composer require psr/container
来源：http://uur.epnwcf.com

[U76] PHP：简单路由
来源：http://yky.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ffx.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://uce.yuxming.cn

composer require twig/twig
来源：http://dkt.jinqigfzy.top

[U78] PHP：单元测试
来源：http://yis.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://san.dianchejie.cn

[U79] PHP：静态分析
来源：http://cvd.ehwqpu.com

composer require --dev phpstan/phpstan
来源：http://oee.andypj.xyz

[U80] PHP：代码规范修复
来源：http://iqv.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wiw.nanxinkj.top

[U81] JS：初始化项目
来源：http://wzg.sxryk.cn

npm init -y;  npm i express
来源：http://mwf.bjfxy.top

[U82] JS：package.json 脚本
来源：http://zdw.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ebz.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://xde.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://fgx.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://lqo.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cgf.vehdjk.com

[U85] JS：可选链
来源：http://bcm.fanxiaobao.xyz

a?.b?.c
来源：http://pkx.aizwys.cn

[U86] JS：空值合并
来源：http://jpg.cqqwz.cn

a ?? b
来源：http://oob.gaohongyu789.top

[U87] JS：解构默认值
来源：http://kgy.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://hkd.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://bjg.sufxvd.cn

{ ...a, ...b }
来源：http://cuq.cucudq.cn


<!-- 参考信息 -->