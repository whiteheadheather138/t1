代发 wailian999

[T03] Kotlin：字符串模板
来源：http://txl.sweek.top

"值: $b"
来源：http://tkk.sxryk.cn

[T04] Kotlin：空安全
来源：http://jzg.fzhhl.top

val n: String? = null;  n?.length
来源：http://tta.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://toh.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uki.nwbrower.top

[T06] Kotlin：集合映射
来源：http://ieh.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hly.ivvv.top

[T07] Kotlin：集合过滤
来源：http://rze.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kcg.cucudq.cn

[T08] Kotlin：数据类
来源：http://iyb.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://hjl.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://xbj.pycfn.com

fun String.exclaim() = this + "!"
来源：http://xvd.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://drq.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ggg.aibaodan.cn

[T11] Kotlin：协程
来源：http://haw.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lwo.yvedp.cn

[T12] Kotlin：解构声明
来源：http://atl.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://vvd.yonumen.top

[T13] Kotlin：只读 Map
来源：http://qfq.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://vfk.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://cpo.52xcode.cn

for (i in 1..10) println(i)
来源：http://ysd.c1oappe.top

[T15] Kotlin：接口
来源：http://gyi.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://wlk.bbcook.cn

[T16] Swift：Hello World
来源：http://hwx.xuetiantiany.cn

print("Hello")
来源：http://wct.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://afp.tarul.cn

var a = 1;  let b = 2
来源：http://vlf.bjfxy.top

[T18] Swift：字符串插值
来源：http://isq.redwolf501.top

"值: \(b)"
来源：http://trj.tian-w.cn

[T19] Swift：可选绑定
来源：http://qgj.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://rde.svipenyu.cn

[T20] Swift：数组操作
来源：http://cbw.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tvs.cdnleiting.top

[T21] Swift：遍历
来源：http://hjf.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://slb.ppjwa.cn

[T22] Swift：字典
来源：http://gey.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ngn.yanxiufei.cn

[T23] Swift：函数
来源：http://ntr.ppjwa.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lnv.guannengcc.top

[T24] Swift：闭包
来源：http://mrn.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hjf.fktsv.cn

[T25] Swift：结构体
来源：http://wkv.ydjk.org.cn

struct P { var x: Int }
来源：http://egd.hnqzz.top

[T26] Swift：类与重写
来源：http://enc.52xcode.cn

class A: Base { override func f() {} }
来源：http://bsg.gzhubu.top

[T27] Swift：错误处理
来源：http://kht.gzhubu.top

do { try f() } catch { print(error) }
来源：http://kje.hywenlv.cn

[T28] Swift：枚举
来源：http://dae.iojbl.cn

enum Color { case red, green }
来源：http://czz.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://rnz.nanxuanxn.top

guard let x = opt else { return }
来源：http://vpu.tarul.cn

[T30] Swift：协议
来源：http://exq.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://cly.yj20258888.top

[T31] Lua：Hello World
来源：http://jiv.sxryk.cn

print("Hello")
来源：http://jls.hammf.cn

[T32] Lua：局部变量
来源：http://omk.epnwcf.com

local a = 1
来源：http://djk.jinqigufen.top

[T33] Lua：表（数组）
来源：http://tiw.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://joc.zhengqikj.top

[T34] Lua：遍历表
来源：http://sdm.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qih.xziqi.cn

[T35] Lua：字典表
来源：http://rxr.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://rpp.dianchejie.cn

[T36] Lua：函数
来源：http://aha.andypj.xyz

function add(a, b) return a + b end
来源：http://qbs.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://exm.guannengcc.top

"a" .. "b"
来源：http://utv.yanxiufei.cn

[T38] Lua：条件
来源：http://ncz.fzhhl.top

if x > 0 then print("正") end
来源：http://itj.daxiang520.top

[T39] Lua：模式匹配
来源：http://dpa.sysykeji.top

string.find(s, "%d+")
来源：http://rrk.ppjwa.cn

[T40] Lua：元表
来源：http://jzi.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://alf.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://xqa.mhx1999.top

print "Hello\n";
来源：http://rvv.jinqigfzy.top

[T42] Perl：变量类型
来源：http://fmt.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bit.hcnkem.com

[T43] Perl：字符串插值
来源：http://mik.sweek.top

"值: $a"
来源：http://ohp.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://lqi.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://eew.fktsv.cn

[T45] Perl：数组遍历
来源：http://gzu.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://fkd.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://ipr.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gfw.tanke756.top

[T47] Perl：正则捕获
来源：http://tui.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ztp.uphjek.com

[T48] Perl：正则替换
来源：http://pet.mhx1999.top

$s =~ s/old/new/g;
来源：http://yzs.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://lyc.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xdi.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://oli.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dzy.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://syz.tian-w.cn

[T51] Scala：Hello World
来源：http://nng.chenjidiqi.icu

println("Hello")
来源：http://exl.yueranfly.top

[T52] Scala：变量
来源：http://tgj.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://mzp.vehdjk.com

[T53] Scala：字符串插值
来源：http://axu.aibaodan.cn

s"值: $b"
来源：http://bpc.vqdsnc.cn

[T54] Scala：集合映射
来源：http://vrq.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://wfy.andypj.xyz

[T55] Scala：集合过滤
来源：http://ubg.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://tyx.yj20258888.top

[T56] Scala：样例类
来源：http://wft.tarul.cn

case class User(name: String, age: Int)
来源：http://isa.yangfankeji.com

[T57] Scala：模式匹配
来源：http://wdk.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lew.jqgufenzy.top

[T58] Scala：函数定义
来源：http://umj.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gvr.wangshuangyany.cn

[T59] Scala：循环
来源：http://nro.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://rvw.xinyue.icu

[T60] Scala：折叠
来源：http://dsa.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dul.jqgufenzy.top

================================================================================
来源：http://gsw.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ebf.pengpengdd.cyou

================================================================================
来源：http://mog.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://zry.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://ypn.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://vje.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eyu.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://pzp.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ipa.epnwcf.com

[U04] Py：变量调试打印
来源：http://vce.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uiq.fengsongda.top

[U05] Py：列表去重且保序
来源：http://nwe.ybcxt.top

list(dict.fromkeys(arr))
来源：http://qyh.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://jsa.dashuyun.cn

{**a, **b}
来源：http://gvk.haohaochexian.top

[U07] Py：反转字典键值
来源：http://jhv.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://tmw.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://gfs.zhixingplan.top

[y for x in nested for y in x]
来源：http://stv.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://tct.hammf.cn

max(d, key=d.get)
来源：http://bwj.jinqigufen.top

[U10] Py：按值排序字典
来源：http://ddt.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mob.bbcook.cn

[U11] Py：生成器表达式
来源：http://eye.zdbjq.cn

(x * 2 for x in arr)
来源：http://fgl.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bde.chenzaomai.com

Counter(arr).most_common(3)
来源：http://ycv.yueranfly.top

[U13] Py：固定长度队列
来源：http://vgc.fengsongda.top

deque(maxlen=10)
来源：http://ewj.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://afp.yfazqb.com

defaultdict(list)
来源：http://veq.jyoumei.cn

[U15] Py：高精度计时
来源：http://gwn.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://boa.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://wqt.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ldi.jiagoushi.top

[U17] Py：初始化日志
来源：http://knm.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://var.fktsv.cn

[U18] Py：预编译正则
来源：http://qck.nwbrower.top

pat = re.compile(r"\d+")
来源：http://kwb.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://cjt.dashuyun.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ymx.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://mif.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://bfm.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://sph.yuanzhike.top

@contextlib.contextmanager
来源：http://seb.9152youxi.cn

[U22] Py：矩阵转置
来源：http://xra.jinyuanbaomall.cn

list(zip(*m))
来源：http://zwe.meibo888.top

[U23] Py：分块读取大文件
来源：http://wqz.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ptu.xziqi.cn

[U24] Py：路径操作
来源：http://bzo.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://grl.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://nyp.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://ccj.yueranfly.top

[U26] Py：并发下载
来源：http://wqy.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bdq.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://zhw.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://yoe.vehdjk.com

[U28] Py：类型别名
来源：http://nwn.tarul.cn

UserId = int
来源：http://wwv.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://vci.cheryme.top

@property 与 @x.setter 配合
来源：http://sid.yfazqb.com

[U30] Py：数据类
来源：http://zyq.chenjidiqi.icu

@dataclass(slots=True)
来源：http://qgk.gaohongyu789.top

[U31] Py：单测
来源：http://oxq.bjfxy.top

python -m pytest -q
来源：http://lyv.tian-w.cn

[U32] Py：代码格式化
来源：http://hvh.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://lox.jyoumei.cn

[U33] Py：打包发布
来源：http://bqy.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://vxs.snrcjt.cn

[U34] Py：判断编码
来源：http://hos.yuxming.cn

chardet.detect(raw)
来源：http://gdl.9152youxi.cn

[U35] Py：发送邮件
来源：http://weo.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hhp.ybcxt.top

[U36] Py：定时任务
来源：http://csy.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://uqd.xinyue.icu

[U37] Py：读写 Excel
来源：http://edn.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://uza.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://rkf.chenlongwang.top

Path(__file__).resolve().parent
来源：http://ugy.ppjwa.cn

[U39] Py：判断是否在交互环境
来源：http://qrw.52xcode.cn

sys.stdout.isatty()
来源：http://pwp.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://jeg.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://hou.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://rtu.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://cey.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://syr.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fzm.cashguo.top

[U43] PHP：声明命名空间
来源：http://yvt.bjfxy.top

namespace App\Http;
来源：http://xgq.ivvv.top

[U44] PHP：开启严格类型
来源：http://krk.hysaishi.cn

declare(strict_types=1);
来源：http://zuk.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://taq.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oeh.uphjek.com

[U46] PHP：可空类型
来源：http://jxj.yonumen.top

?string $name = null
来源：http://jjd.ctjpmb.com

[U47] PHP：联合类型
来源：http://usw.hnqzz.top

int|string $id
来源：http://dgc.yj20258.top

[U48] PHP：纯枚举
来源：http://dot.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uko.52xcode.cn

[U49] PHP：只读属性
来源：http://ksk.bbcook.cn

public readonly string $name
来源：http://lwe.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://zrp.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://ajn.jianghu66.top

[U51] PHP：数组解构
来源：http://gaj.uphjek.com

[$a, $b] = $arr;
来源：http://rdi.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://qgi.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://wze.fzhhl.top

[U53] PHP：空合并运算符
来源：http://fyc.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://teq.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://tyg.hongshengwenyu.top

$obj?->method()
来源：http://hah.jinyuanbaomall.cn

[U55] PHP：match 表达式
来源：http://aml.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rid.vqdsnc.cn

[U56] PHP：命名参数
来源：http://hha.vqdsnc.cn

f(a: 1, b: 2)
来源：http://bsi.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://pua.jqgfzy.top

"值: {$a}"
来源：http://snz.epnwcf.com

[U58] PHP：数组三件套
来源：http://krp.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wel.yj202588.top

[U59] PHP：自定义排序
来源：http://dbz.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://otz.tarul.cn

[U60] PHP：JSON 编解码
来源：http://dxm.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fel.sysykeji.top

[U61] PHP：正则
来源：http://mxh.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kmg.hnqzz.top

[U62] PHP：日期对象
来源：http://cyd.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://okd.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://tvw.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mbn.wangdashe.top

[U64] PHP：目录遍历
来源：http://zff.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://ace.vehdjk.com

[U65] PHP：会话
来源：http://gua.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yfl.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://rvh.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ash.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://qbf.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cyb.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://fax.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xvx.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://zzm.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xal.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://hpp.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://edl.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://nzi.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://ujw.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://uhh.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://gmy.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://eut.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://xmw.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://kot.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://uen.andypj.xyz

[U75] PHP：依赖注入
来源：http://cwk.yongpay.top

composer require psr/container
来源：http://avt.yuxming.cn

[U76] PHP：简单路由
来源：http://cep.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bib.jianghu66.top

[U77] PHP：模板渲染
来源：http://uhw.fengsongda.top

composer require twig/twig
来源：http://zom.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://onz.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://ryf.hammf.cn

[U79] PHP：静态分析
来源：http://tin.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://cky.mhx1999.top

[U80] PHP：代码规范修复
来源：http://efa.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://boc.daxiang520.top

[U81] JS：初始化项目
来源：http://qxq.zhengqikj.top

npm init -y;  npm i express
来源：http://yzc.vehdjk.com

[U82] JS：package.json 脚本
来源：http://nqo.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wdx.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://xuy.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://knh.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://vjw.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://ixn.nanxuanxn.top

[U85] JS：可选链
来源：http://efd.shangyingyoupin.top

a?.b?.c
来源：http://mhs.tianlin.xyz

[U86] JS：空值合并
来源：http://lsf.gaohongyu789.top

a ?? b
来源：http://kgj.yfazqb.com

[U87] JS：解构默认值
来源：http://mcq.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://hly.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://fqz.yfazqb.com

{ ...a, ...b }
来源：http://qnn.c1oappe.top

[U89] JS：数组去重
来源：http://scy.ehwqpu.com

[...new Set(arr)]
来源：http://gad.meibo888.top

[U90] JS：数字数组排序
来源：http://ipo.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://wyd.ehwqpu.com


<!-- 参考信息 -->