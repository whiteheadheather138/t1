代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nzf.chenjidiqi.icu

================================================================================
来源：http://nru.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eku.hammf.cn

================================================================================
来源：http://xie.fehbvm.com

[T01] Kotlin：Hello World
来源：http://tae.mhx1999.top

println("Hello")
来源：http://kgn.zhijiandao.cn

[T02] Kotlin：变量
来源：http://soc.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bqy.shzxlz.cn

[T03] Kotlin：字符串模板
来源：http://wih.shanyushiyangtech.top

"值: $b"
来源：http://adr.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://cyp.ppjwa.cn

val n: String? = null;  n?.length
来源：http://ans.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://lcb.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wvg.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://vkq.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://osd.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://vfs.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hrh.tianlin.xyz

[T08] Kotlin：数据类
来源：http://fsk.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://kbu.hammf.cn

[T09] Kotlin：扩展函数
来源：http://rce.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://lux.tian-w.cn

[T10] Kotlin：默认参数
来源：http://zff.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rmw.yanxiufei.cn

[T11] Kotlin：协程
来源：http://fwz.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qwp.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://dnx.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://owr.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://aov.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://tuc.zhixingplan.top

[T14] Kotlin：循环
来源：http://csy.tarul.cn

for (i in 1..10) println(i)
来源：http://bnb.ydjk.org.cn

[T15] Kotlin：接口
来源：http://lxg.zycfv.cn

interface Shape { fun area(): Double }
来源：http://qkb.zhijiandao.cn

[T16] Swift：Hello World
来源：http://uzl.yangfankeji.com

print("Hello")
来源：http://ysu.chenzaomai.com

[T17] Swift：变量与常量
来源：http://mhd.tanke756.top

var a = 1;  let b = 2
来源：http://wvj.uphjek.com

[T18] Swift：字符串插值
来源：http://ifv.cucudq.cn

"值: \(b)"
来源：http://gvm.zycfv.cn

[T19] Swift：可选绑定
来源：http://spw.ivvv.top

if let n = opt { print(n) }
来源：http://aez.yj202588.top

[T20] Swift：数组操作
来源：http://tbm.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://klr.fehbvm.com

[T21] Swift：遍历
来源：http://qfo.9152youxi.cn

for x in a { print(x) }
来源：http://uzy.fengsongda.top

[T22] Swift：字典
来源：http://pdf.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://gst.tarul.cn

[T23] Swift：函数
来源：http://tye.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zpl.nwbrower.top

[T24] Swift：闭包
来源：http://xlg.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://cmp.aibaodan.cn

[T25] Swift：结构体
来源：http://vjt.yuxming.cn

struct P { var x: Int }
来源：http://kzo.316326.xyz

[T26] Swift：类与重写
来源：http://ovx.fehbvm.com

class A: Base { override func f() {} }
来源：http://xiq.jlsjyb.cn

[T27] Swift：错误处理
来源：http://awd.redwolf501.top

do { try f() } catch { print(error) }
来源：http://ojf.sweek.top

[T28] Swift：枚举
来源：http://kxc.hammf.cn

enum Color { case red, green }
来源：http://gdb.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://kbt.jinqigfzy.top

guard let x = opt else { return }
来源：http://zaq.yj202588.top

[T30] Swift：协议
来源：http://ahk.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://ted.ctjpmb.com

[T31] Lua：Hello World
来源：http://gph.zdqjudy.top

print("Hello")
来源：http://lvf.meibo888.top

[T32] Lua：局部变量
来源：http://qtu.iojbl.cn

local a = 1
来源：http://taw.ctjpmb.com

[T33] Lua：表（数组）
来源：http://ozo.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pma.cashguo.top

[T34] Lua：遍历表
来源：http://hns.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fng.tianlin.xyz

[T35] Lua：字典表
来源：http://ovq.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://elf.cqqwz.cn

[T36] Lua：函数
来源：http://abs.sjlbkw.cn

function add(a, b) return a + b end
来源：http://ktj.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://hxf.aibaodan.cn

"a" .. "b"
来源：http://nso.fanxiaobao.xyz

[T38] Lua：条件
来源：http://dvw.wangdashe.top

if x > 0 then print("正") end
来源：http://dcy.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://hiu.nwbrower.top

string.find(s, "%d+")
来源：http://zom.yongpay.top

[T40] Lua：元表
来源：http://gpc.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://mbs.yj20258.top

[T41] Perl：Hello World
来源：http://qsz.yfazqb.com

print "Hello\n";
来源：http://ykc.hywenlv.cn

[T42] Perl：变量类型
来源：http://gkt.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jhj.guowangkeji.top

[T43] Perl：字符串插值
来源：http://qrt.hywenlv.cn

"值: $a"
来源：http://jhv.fehbvm.com

[T44] Perl：条件
来源：http://tdo.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://ixk.haohaochexian.top

[T45] Perl：数组遍历
来源：http://stw.uphjek.com

for my $x (@arr) { print $x; }
来源：http://jpx.cucudq.cn

[T46] Perl：哈希操作
来源：http://isl.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zfj.yangfankeji.com

[T47] Perl：正则捕获
来源：http://pvj.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gtj.yuxming.cn

[T48] Perl：正则替换
来源：http://juk.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://kiq.snrcjt.cn

[T49] Perl：函数
来源：http://ugw.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hjq.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://fiw.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lse.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://rdx.redwolf501.top

[T51] Scala：Hello World
来源：http://ojk.yj202588.top

println("Hello")
来源：http://xmw.zdqjudy.top

[T52] Scala：变量
来源：http://gdf.hammf.cn

val a = 1;  var b = 2
来源：http://acv.tian-w.cn

[T53] Scala：字符串插值
来源：http://bez.yonumen.top

s"值: $b"
来源：http://iok.ehwqpu.com

[T54] Scala：集合映射
来源：http://qgb.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://jgq.havefunace.top

[T55] Scala：集合过滤
来源：http://kwa.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://daq.zycfv.cn

[T56] Scala：样例类
来源：http://xdi.sysykeji.top

case class User(name: String, age: Int)
来源：http://ftc.yfazqb.com

[T57] Scala：模式匹配
来源：http://jof.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eox.epnwcf.com

[T58] Scala：函数定义
来源：http://bqd.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://xfc.shuidangran.top

[T59] Scala：循环
来源：http://dox.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://kla.hammf.cn

[T60] Scala：折叠
来源：http://tcz.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hvv.jinyuanbaomall.cn

================================================================================
来源：http://ggm.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rjr.hywenlv.cn

================================================================================
来源：http://chm.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://bsa.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://mwn.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://uow.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ncu.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://xmf.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://abe.ydzc1.top

[U04] Py：变量调试打印
来源：http://dlo.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://otd.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://rpp.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://zky.yvedp.cn

[U06] Py：合并两个字典
来源：http://kvh.hnqzz.top

{**a, **b}
来源：http://lue.haohaochexian.top

[U07] Py：反转字典键值
来源：http://yzy.fktsv.cn

{v: k for k, v in d.items()}
来源：http://xjk.yueranfly.top

[U08] Py：展平二维列表
来源：http://wng.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://kwc.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://gpx.yj20258888.top

max(d, key=d.get)
来源：http://hyi.xziqi.cn

[U10] Py：按值排序字典
来源：http://hxr.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://org.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://sha.cdnleiting.top

(x * 2 for x in arr)
来源：http://nfh.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://tyo.ehwqpu.com

Counter(arr).most_common(3)
来源：http://jhm.vehdjk.com

[U13] Py：固定长度队列
来源：http://dtj.yj20258888.top

deque(maxlen=10)
来源：http://atv.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://dao.kuanghao11.cn

defaultdict(list)
来源：http://rxh.bjfxy.top

[U15] Py：高精度计时
来源：http://rlo.jqgufenzy.top

t = time.perf_counter()
来源：http://oua.ivvv.top

[U16] Py：命令行参数解析
来源：http://xap.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://owd.cheryme.top

[U17] Py：初始化日志
来源：http://sib.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://svt.birdmap.top

[U18] Py：预编译正则
来源：http://wtz.316326.xyz

pat = re.compile(r"\d+")
来源：http://ifq.316326.xyz

[U19] Py：正则替换带回调
来源：http://end.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dha.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://epj.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://zlo.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://qix.jinqigufen.top

@contextlib.contextmanager
来源：http://tdh.hysaishi.cn

[U22] Py：矩阵转置
来源：http://ixm.zdbjq.cn

list(zip(*m))
来源：http://dxu.daria6918.cn

[U23] Py：分块读取大文件
来源：http://qgv.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://smy.316326.xyz

[U24] Py：路径操作
来源：http://bqi.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vml.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://jxl.jinghuilouyu.cn

csv.DictReader(f)
来源：http://aml.nanxuanxn.top

[U26] Py：并发下载
来源：http://oee.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xtp.yj20258888.top

[U27] Py：异步 HTTP
来源：http://ain.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://vpb.cqqwz.cn

[U28] Py：类型别名
来源：http://rhy.hongshengwenyu.top

UserId = int
来源：http://mti.xuetiantiany.cn

[U29] Py：属性校验
来源：http://jrv.xziqi.cn

@property 与 @x.setter 配合
来源：http://xef.zycfv.cn

[U30] Py：数据类
来源：http://pfp.jlsjyb.cn

@dataclass(slots=True)
来源：http://ejd.yuanzhike.top

[U31] Py：单测
来源：http://vpt.ivvv.top

python -m pytest -q
来源：http://riz.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://ydc.yvedp.cn

ruff format . && ruff check --fix .
来源：http://nwr.cheryme.top

[U33] Py：打包发布
来源：http://kap.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://vkc.bjfxy.top

[U34] Py：判断编码
来源：http://tge.daxiang520.top

chardet.detect(raw)
来源：http://psr.zhongyouzk.top

[U35] Py：发送邮件
来源：http://sqn.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pof.shangyingyoupin.top

[U36] Py：定时任务
来源：http://tym.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://olm.sysykeji.top

[U37] Py：读写 Excel
来源：http://yec.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://tdz.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://lbl.jiagoushi.top

Path(__file__).resolve().parent
来源：http://lsm.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://jfu.sufxvd.cn

sys.stdout.isatty()
来源：http://axd.guannengcc.top

[U40] Py：打印到标准错误
来源：http://tlh.sweek.top

print("err", file=sys.stderr)
来源：http://acy.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://epk.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tnb.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://blw.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aew.ydzc1.top

[U43] PHP：声明命名空间
来源：http://leu.wangshuangyany.cn

namespace App\Http;
来源：http://qri.bjfxy.top

[U44] PHP：开启严格类型
来源：http://jzm.vqdsnc.cn

declare(strict_types=1);
来源：http://jnv.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://bjg.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ejj.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://uss.ehwqpu.com

?string $name = null
来源：http://kxi.zhongyouzk.top

[U47] PHP：联合类型
来源：http://vda.redwolf501.top

int|string $id
来源：http://wqs.yangfankeji.com

[U48] PHP：纯枚举
来源：http://vtl.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pva.ydjk.org.cn

[U49] PHP：只读属性
来源：http://enf.cqqwz.cn

public readonly string $name
来源：http://zvb.yj20258.top

[U50] PHP：构造器属性提升
来源：http://tjq.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://cem.kuanghao11.cn

[U51] PHP：数组解构
来源：http://cji.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://wuu.havefunace.top

[U52] PHP：箭头函数
来源：http://bkn.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://cqf.sweek.top

[U53] PHP：空合并运算符
来源：http://msi.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://abd.andypj.xyz

[U54] PHP：空安全调用
来源：http://tfk.mhx1999.top

$obj?->method()
来源：http://ans.zhixingplan.top

[U55] PHP：match 表达式
来源：http://fpp.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qsq.mhx1999.top

[U56] PHP：命名参数
来源：http://xut.hfpthk.cn

f(a: 1, b: 2)
来源：http://tcj.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://kjk.vqdsnc.cn

"值: {$a}"
来源：http://tlv.nwbrower.top

[U58] PHP：数组三件套
来源：http://idd.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sou.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://uga.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyb.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://oos.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dmc.yj20258.top

[U61] PHP：正则
来源：http://zbs.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rie.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://pgs.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jai.hammf.cn

[U63] PHP：文件读写
来源：http://umb.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://asq.cqqwz.cn

[U64] PHP：目录遍历
来源：http://hba.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://jyb.cqqwz.cn

[U65] PHP：会话
来源：http://rrz.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yka.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://cof.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qie.daria6918.cn

[U67] PHP：处理文件上传
来源：http://bow.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eha.yongpay.top

[U68] PHP：PDO 连接
来源：http://yny.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jcu.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://stn.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dpu.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://dui.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eor.zycfv.cn

[U71] PHP：抛出异常
来源：http://zzx.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://qsr.chenjidiqi.icu

[U72] PHP：写错误日志
来源：http://uyp.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://zpi.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://bfy.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://ehv.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://xfc.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://rpz.sufxvd.cn

[U75] PHP：依赖注入
来源：http://yha.smart0.xyz

composer require psr/container
来源：http://rhj.vehdjk.com

[U76] PHP：简单路由
来源：http://uva.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://efi.tanke756.top

[U77] PHP：模板渲染
来源：http://svz.aizwys.cn

composer require twig/twig
来源：http://saw.guowangkeji.top

[U78] PHP：单元测试
来源：http://sma.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://gfd.bbcook.cn

[U79] PHP：静态分析
来源：http://ttj.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://csp.ybcxt.top

[U80] PHP：代码规范修复
来源：http://ltt.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uxq.xziqi.cn

[U81] JS：初始化项目
来源：http://eqe.yj20258888.top

npm init -y;  npm i express
来源：http://iqp.xziqi.cn

[U82] JS：package.json 脚本
来源：http://wxs.zdbjq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wqs.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://qyi.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://ppc.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://yyb.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://wyi.aibaodan.cn

[U85] JS：可选链
来源：http://ocu.zhijiandao.cn

a?.b?.c
来源：http://hfr.316326.xyz

[U86] JS：空值合并
来源：http://pqk.yueranfly.top

a ?? b
来源：http://cuq.yuanzhike.top


<!-- 参考信息 -->