代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zqn.chenlongwang.top

[S57] C++：编译期常量
来源：http://llk.dianchejie.cn

constexpr int N = 10;
来源：http://ykr.sxryk.cn

[S58] C++：命名空间
来源：http://vkg.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://mxq.sufxvd.cn

[S59] C++：静态断言
来源：http://mda.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vde.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://nvp.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jsz.guowangkeji.top

================================================================================
来源：http://dak.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mvd.zdbjq.cn

================================================================================
来源：http://ekl.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://gmd.aibaodan.cn

println("Hello")
来源：http://grk.yanxiufei.cn

[T02] Kotlin：变量
来源：http://rjj.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uzw.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://vjp.zhoulong.xyz

"值: $b"
来源：http://vbd.smart0.xyz

[T04] Kotlin：空安全
来源：http://ouw.hfpthk.cn

val n: String? = null;  n?.length
来源：http://wub.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://gwu.jinqigfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://umu.yuxming.cn

[T06] Kotlin：集合映射
来源：http://ggm.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vfd.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://kro.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nxi.fzhhl.top

[T08] Kotlin：数据类
来源：http://qvf.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://toh.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://edj.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://qqa.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://vyr.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oab.fktsv.cn

[T11] Kotlin：协程
来源：http://poq.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ndd.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://bat.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://fjn.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://xuq.c1oappe.top

val m = mapOf("a" to 1)
来源：http://svz.jinqigufen.top

[T14] Kotlin：循环
来源：http://ooc.cheryme.top

for (i in 1..10) println(i)
来源：http://nrz.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://nfj.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://qop.ppjwa.cn

[T16] Swift：Hello World
来源：http://mau.fengsongda.top

print("Hello")
来源：http://hvm.shuidangran.top

[T17] Swift：变量与常量
来源：http://axr.tarul.cn

var a = 1;  let b = 2
来源：http://bik.jiagoushi.top

[T18] Swift：字符串插值
来源：http://jlh.wangdashe.top

"值: \(b)"
来源：http://prt.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://obr.svipenyu.cn

if let n = opt { print(n) }
来源：http://eur.daria6918.cn

[T20] Swift：数组操作
来源：http://yit.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gsa.feifeiyinyue.top

[T21] Swift：遍历
来源：http://vdb.ctjpmb.com

for x in a { print(x) }
来源：http://buv.mhx1999.top

[T22] Swift：字典
来源：http://dly.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://vxr.ydjk.org.cn

[T23] Swift：函数
来源：http://oth.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zon.hysaishi.cn

[T24] Swift：闭包
来源：http://rdx.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://snk.hnqzz.top

[T25] Swift：结构体
来源：http://lem.kuanghao11.cn

struct P { var x: Int }
来源：http://dao.fehbvm.com

[T26] Swift：类与重写
来源：http://vbj.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://tkk.ctjpmb.com

[T27] Swift：错误处理
来源：http://vvq.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://sar.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://ins.zhoulong.xyz

enum Color { case red, green }
来源：http://fle.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://jtc.zhoulong.xyz

guard let x = opt else { return }
来源：http://mle.yueranfly.top

[T30] Swift：协议
来源：http://kit.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://ipt.xuanzx.com

[T31] Lua：Hello World
来源：http://itg.sjlbkw.cn

print("Hello")
来源：http://wli.meibo888.top

[T32] Lua：局部变量
来源：http://tcd.zdbjq.cn

local a = 1
来源：http://yhv.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://ice.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xdr.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://vtj.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bzt.nanxinkj.top

[T35] Lua：字典表
来源：http://tyo.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://sme.shanyushiyangtech.top

[T36] Lua：函数
来源：http://smh.sjlbkw.cn

function add(a, b) return a + b end
来源：http://swd.pycfn.com

[T37] Lua：字符串拼接
来源：http://rho.havefunace.top

"a" .. "b"
来源：http://jyb.birdmap.top

[T38] Lua：条件
来源：http://zmn.snrcjt.cn

if x > 0 then print("正") end
来源：http://ecq.yj20258.top

[T39] Lua：模式匹配
来源：http://zkv.fehbvm.com

string.find(s, "%d+")
来源：http://dpj.pycfn.com

[T40] Lua：元表
来源：http://ybo.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://brr.fehbvm.com

[T41] Perl：Hello World
来源：http://xoi.cashguo.top

print "Hello\n";
来源：http://ebn.dianchejie.cn

[T42] Perl：变量类型
来源：http://uzl.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yps.hammf.cn

[T43] Perl：字符串插值
来源：http://tbg.xuanzx.com

"值: $a"
来源：http://jhz.birdmap.top

[T44] Perl：条件
来源：http://xai.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://fat.ivvv.top

[T45] Perl：数组遍历
来源：http://oqv.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://ixd.sweek.top

[T46] Perl：哈希操作
来源：http://fdn.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zwr.ivvv.top

[T47] Perl：正则捕获
来源：http://scj.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sfe.cheryme.top

[T48] Perl：正则替换
来源：http://zxt.jianghu66.top

$s =~ s/old/new/g;
来源：http://jix.birdmap.top

[T49] Perl：函数
来源：http://lmj.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vlm.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://ovb.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hyv.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://axm.zhengqikj.top

[T51] Scala：Hello World
来源：http://pbl.guannengcc.top

println("Hello")
来源：http://rjv.yonumen.top

[T52] Scala：变量
来源：http://jjw.yonumen.top

val a = 1;  var b = 2
来源：http://qmt.hysaishi.cn

[T53] Scala：字符串插值
来源：http://jwf.yuxming.cn

s"值: $b"
来源：http://tkl.yj20258.top

[T54] Scala：集合映射
来源：http://eco.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://zrz.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://jwf.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://ren.cucudq.cn

[T56] Scala：样例类
来源：http://qzq.sweek.top

case class User(name: String, age: Int)
来源：http://qyr.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://hbd.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ggs.pycfn.com

[T58] Scala：函数定义
来源：http://bwf.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://hir.hesvh.cn

[T59] Scala：循环
来源：http://dbr.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://odk.0kj1m.cn

[T60] Scala：折叠
来源：http://oiq.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ffy.yuxming.cn

================================================================================
来源：http://njc.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ahl.hesvh.cn

================================================================================
来源：http://oej.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://zct.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://qqo.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://wmw.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://htv.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://bls.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gks.yj20258888.top

[U04] Py：变量调试打印
来源：http://mzc.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vup.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://qhq.hcnkem.com

list(dict.fromkeys(arr))
来源：http://qqv.hesvh.cn

[U06] Py：合并两个字典
来源：http://iav.sxryk.cn

{**a, **b}
来源：http://xxz.gzhubu.top

[U07] Py：反转字典键值
来源：http://vlk.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://hqr.wangdashe.top

[U08] Py：展平二维列表
来源：http://xvg.yuxming.cn

[y for x in nested for y in x]
来源：http://klh.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://bcf.gotoacloud.top

max(d, key=d.get)
来源：http://bja.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://pat.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hqw.zdbjq.cn

[U11] Py：生成器表达式
来源：http://qal.vehdjk.com

(x * 2 for x in arr)
来源：http://dqt.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fex.sufxvd.cn

Counter(arr).most_common(3)
来源：http://flj.cdnleiting.top

[U13] Py：固定长度队列
来源：http://anr.svipenyu.cn

deque(maxlen=10)
来源：http://dvb.sysykeji.top

[U14] Py：分组收集到列表
来源：http://qlt.chenlongwang.top

defaultdict(list)
来源：http://oji.ehwqpu.com

[U15] Py：高精度计时
来源：http://zbb.epnwcf.com

t = time.perf_counter()
来源：http://slh.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://ivl.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kgd.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://hzw.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://bjh.xylfe.cn

[U18] Py：预编译正则
来源：http://ugs.zycfv.cn

pat = re.compile(r"\d+")
来源：http://gvz.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://oue.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gsv.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://sbs.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://uye.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://czr.ivvv.top

@contextlib.contextmanager
来源：http://gyy.tanke756.top

[U22] Py：矩阵转置
来源：http://gtt.9152youxi.cn

list(zip(*m))
来源：http://yxs.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://xgc.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dlp.daxiang520.top

[U24] Py：路径操作
来源：http://cbw.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://shz.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://llo.ehwqpu.com

csv.DictReader(f)
来源：http://qbh.bbcook.cn

[U26] Py：并发下载
来源：http://hah.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://anx.yueranfly.top

[U27] Py：异步 HTTP
来源：http://hyf.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://cdr.andypj.xyz

[U28] Py：类型别名
来源：http://kgh.uphjek.com

UserId = int
来源：http://jmd.epnwcf.com

[U29] Py：属性校验
来源：http://kmp.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://zhw.tianlin.xyz

[U30] Py：数据类
来源：http://ygi.zhijiandao.cn

@dataclass(slots=True)
来源：http://kgj.andypj.xyz

[U31] Py：单测
来源：http://szv.ybcxt.top

python -m pytest -q
来源：http://fyc.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://pjf.hammf.cn

ruff format . && ruff check --fix .
来源：http://qir.andypj.xyz

[U33] Py：打包发布
来源：http://kdn.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://tgr.ydzc1.top

[U34] Py：判断编码
来源：http://fir.yanxiufei.cn

chardet.detect(raw)
来源：http://flc.gaohongyu789.top

[U35] Py：发送邮件
来源：http://fla.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://exc.hnqzz.top

[U36] Py：定时任务
来源：http://geh.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://kkr.daxiang520.top

[U37] Py：读写 Excel
来源：http://kwx.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kbu.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://xew.52xcode.cn

Path(__file__).resolve().parent
来源：http://cdy.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://nxk.xziqi.cn

sys.stdout.isatty()
来源：http://pcl.fzhhl.top

[U40] Py：打印到标准错误
来源：http://adk.andypj.xyz

print("err", file=sys.stderr)
来源：http://cgh.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://jgq.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://djc.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://jog.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ars.bjfxy.top

[U43] PHP：声明命名空间
来源：http://vwi.daria6918.cn

namespace App\Http;
来源：http://ypx.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://fwx.xuanzx.com

declare(strict_types=1);
来源：http://lif.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://qxj.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lcq.0kj1m.cn

[U46] PHP：可空类型
来源：http://aoi.ivvv.top

?string $name = null
来源：http://lgm.gotoacloud.top

[U47] PHP：联合类型
来源：http://uoi.jqgfzy.top

int|string $id
来源：http://awo.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://yts.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fpm.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://jjd.pycfn.com

public readonly string $name
来源：http://vka.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://peo.ctjpmb.com

public function __construct(private int $id) {}
来源：http://boa.jinqigfzy.top

[U51] PHP：数组解构
来源：http://wzz.ivvv.top

[$a, $b] = $arr;
来源：http://ytn.ydzc1.top

[U52] PHP：箭头函数
来源：http://tat.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://ybc.pycfn.com

[U53] PHP：空合并运算符
来源：http://dhg.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://llc.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://kse.pycfn.com

$obj?->method()
来源：http://vwq.yj202588.top

[U55] PHP：match 表达式
来源：http://kgx.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hzc.yueranfly.top

[U56] PHP：命名参数
来源：http://puj.tianlin.xyz

f(a: 1, b: 2)
来源：http://dqg.yvedp.cn

[U57] PHP：字符串插值
来源：http://rds.ctjpmb.com

"值: {$a}"
来源：http://jcr.daxiang520.top

[U58] PHP：数组三件套
来源：http://lnf.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hpx.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://rdk.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvl.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://ncv.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vsi.bjfxy.top

[U61] PHP：正则
来源：http://lmj.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://grn.cdnleiting.top

[U62] PHP：日期对象
来源：http://hyd.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uzb.sufxvd.cn

[U63] PHP：文件读写
来源：http://ilt.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://muk.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://qfu.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://mnk.dashuyun.cn

[U65] PHP：会话
来源：http://oiz.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uzr.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://puv.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hng.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://jpm.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xgb.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://kkq.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://trl.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://mkm.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gnu.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://mqf.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uso.epnwcf.com

[U71] PHP：抛出异常
来源：http://qxs.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://taw.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://lib.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://isy.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://rqk.tarul.cn

parse_ini_file("config.ini", true)
来源：http://rmz.ydzc1.top

[U74] PHP：读取环境变量
来源：http://inm.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://pbk.yj20258.top

[U75] PHP：依赖注入
来源：http://rsz.pycfn.com

composer require psr/container
来源：http://ssx.hnxiangtu.top

[U76] PHP：简单路由
来源：http://apf.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jay.hesvh.cn

[U77] PHP：模板渲染
来源：http://ckf.jiagoushi.top

composer require twig/twig
来源：http://afq.ppjwa.cn

[U78] PHP：单元测试
来源：http://mho.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://tew.gaohongyu789.top

[U79] PHP：静态分析
来源：http://hou.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://avr.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://oma.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qpe.aizwys.cn

[U81] JS：初始化项目
来源：http://kmc.aibaodan.cn

npm init -y;  npm i express
来源：http://mpf.tanke756.top

[U82] JS：package.json 脚本
来源：http://lzy.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lej.zdbjq.cn


<!-- 参考信息 -->