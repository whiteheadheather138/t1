代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://omw.shuidangran.top

[S51] C++：显式类型转换
来源：http://nrt.sweek.top

static_cast<double>(a) / b
来源：http://vcw.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://kli.sxryk.cn

int size() const noexcept { return n_; }
来源：http://ntd.ctjpmb.com

[S53] C++：移动语义
来源：http://vmx.ivvv.top

std::vector<int> w = std::move(v);
来源：http://nbx.svipenyu.cn

[S54] C++：异常处理
来源：http://fle.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qpq.jyoumei.cn

[S55] C++：结构化绑定
来源：http://nwp.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vic.dashuyun.cn

[S56] C++：optional
来源：http://wul.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ncq.daria6918.cn

[S57] C++：编译期常量
来源：http://lwl.guannengcc.top

constexpr int N = 10;
来源：http://wqa.zhijiandao.cn

[S58] C++：命名空间
来源：http://eff.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://amg.daria6918.cn

[S59] C++：静态断言
来源：http://ggl.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fin.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://xjr.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://icb.hesvh.cn

================================================================================
来源：http://ake.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qif.fzhhl.top

================================================================================
来源：http://bbz.hammf.cn

[T01] Kotlin：Hello World
来源：http://vma.ppjwa.cn

println("Hello")
来源：http://kbi.guowangkeji.top

[T02] Kotlin：变量
来源：http://srq.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bsc.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://ayc.52xcode.cn

"值: $b"
来源：http://kxk.vehdjk.com

[T04] Kotlin：空安全
来源：http://erd.zdqjudy.top

val n: String? = null;  n?.length
来源：http://ciq.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://ixi.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hcq.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://auw.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qpl.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://mse.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ajb.jiagoushi.top

[T08] Kotlin：数据类
来源：http://jas.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://ihl.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://mux.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://qlu.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://cii.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iae.yj202588.top

[T11] Kotlin：协程
来源：http://woo.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wdz.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://kbz.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://oaf.jinghuilouyu.cn

[T13] Kotlin：只读 Map
来源：http://etj.jianghu66.top

val m = mapOf("a" to 1)
来源：http://gzi.nanxuanxn.top

[T14] Kotlin：循环
来源：http://ksi.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://ppb.hfpthk.cn

[T15] Kotlin：接口
来源：http://zvp.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://imp.sweek.top

[T16] Swift：Hello World
来源：http://ftj.tianlin.xyz

print("Hello")
来源：http://ayq.snrcjt.cn

[T17] Swift：变量与常量
来源：http://okl.daxiang520.top

var a = 1;  let b = 2
来源：http://aka.yuanzhike.top

[T18] Swift：字符串插值
来源：http://vza.52xcode.cn

"值: \(b)"
来源：http://bjx.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://rmn.cucudq.cn

if let n = opt { print(n) }
来源：http://gdv.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://pxs.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sao.sysykeji.top

[T21] Swift：遍历
来源：http://eak.wangshuangyany.cn

for x in a { print(x) }
来源：http://jkn.jinqigfzy.top

[T22] Swift：字典
来源：http://irv.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nrr.cheryme.top

[T23] Swift：函数
来源：http://ira.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jqo.mhx1999.top

[T24] Swift：闭包
来源：http://igz.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://bzk.yuanzhike.top

[T25] Swift：结构体
来源：http://hwa.bjfxy.top

struct P { var x: Int }
来源：http://vbs.chenlongwang.top

[T26] Swift：类与重写
来源：http://umc.cqqwz.cn

class A: Base { override func f() {} }
来源：http://oub.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://imj.bbcook.cn

do { try f() } catch { print(error) }
来源：http://bwu.zdbjq.cn

[T28] Swift：枚举
来源：http://fmz.ehwqpu.com

enum Color { case red, green }
来源：http://hle.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://jev.yfazqb.com

guard let x = opt else { return }
来源：http://evj.cucudq.cn

[T30] Swift：协议
来源：http://ibl.zycfv.cn

protocol Shape { func area() -> Double }
来源：http://dsg.chenzaomai.com

[T31] Lua：Hello World
来源：http://wcb.hongshengwenyu.top

print("Hello")
来源：http://hwf.hysaishi.cn

[T32] Lua：局部变量
来源：http://buy.jianghu66.top

local a = 1
来源：http://ayr.hammf.cn

[T33] Lua：表（数组）
来源：http://nmv.wangdashe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vfj.cashguo.top

[T34] Lua：遍历表
来源：http://wfp.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cbx.jinqigfzy.top

[T35] Lua：字典表
来源：http://cmn.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://jke.zdbjq.cn

[T36] Lua：函数
来源：http://avk.birdmap.top

function add(a, b) return a + b end
来源：http://tsp.guannengcc.top

[T37] Lua：字符串拼接
来源：http://gxw.mhx1999.top

"a" .. "b"
来源：http://qcs.chenjidiqi.icu

[T38] Lua：条件
来源：http://fvs.ppjwa.cn

if x > 0 then print("正") end
来源：http://wpm.fengsongda.top

[T39] Lua：模式匹配
来源：http://stf.cucudq.cn

string.find(s, "%d+")
来源：http://zli.aibaodan.cn

[T40] Lua：元表
来源：http://crj.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://ndb.jqgfzy.top

[T41] Perl：Hello World
来源：http://fsy.hywenlv.cn

print "Hello\n";
来源：http://rdl.sxryk.cn

[T42] Perl：变量类型
来源：http://epp.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mqz.sysykeji.top

[T43] Perl：字符串插值
来源：http://mqd.wangshuangyany.cn

"值: $a"
来源：http://wht.cashguo.top

[T44] Perl：条件
来源：http://tsw.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://qmn.yuxming.cn

[T45] Perl：数组遍历
来源：http://vmo.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://fjb.jianghu66.top

[T46] Perl：哈希操作
来源：http://waz.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eer.shuidangran.top

[T47] Perl：正则捕获
来源：http://rth.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jqe.sweek.top

[T48] Perl：正则替换
来源：http://qum.redwolf501.top

$s =~ s/old/new/g;
来源：http://vwy.jinqigufen.top

[T49] Perl：函数
来源：http://fbx.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ocd.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://hol.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://bsm.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://xof.zhengqikj.top

[T51] Scala：Hello World
来源：http://uoq.xziqi.cn

println("Hello")
来源：http://pks.sufxvd.cn

[T52] Scala：变量
来源：http://wmf.vehdjk.com

val a = 1;  var b = 2
来源：http://mtg.uphjek.com

[T53] Scala：字符串插值
来源：http://jrq.yuxming.cn

s"值: $b"
来源：http://ftz.chenzaomai.com

[T54] Scala：集合映射
来源：http://kza.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://cmk.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://hha.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://yuu.chenlongwang.top

[T56] Scala：样例类
来源：http://dlt.yangfankeji.com

case class User(name: String, age: Int)
来源：http://oxz.xziqi.cn

[T57] Scala：模式匹配
来源：http://yzp.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://spk.bjfxy.top

[T58] Scala：函数定义
来源：http://zyx.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://ixc.hammf.cn

[T59] Scala：循环
来源：http://igs.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://kwc.guowangkeji.top

[T60] Scala：折叠
来源：http://yyp.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rsu.zhongyouzk.top

================================================================================
来源：http://ptq.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bcm.yongpay.top

================================================================================
来源：http://dkm.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://cel.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://qrw.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://ftz.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mnf.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://dif.yuxming.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ezy.9152youxi.cn

[U04] Py：变量调试打印
来源：http://ocw.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rsp.shuidangran.top

[U05] Py：列表去重且保序
来源：http://kcl.yuxming.cn

list(dict.fromkeys(arr))
来源：http://kbo.pycfn.com

[U06] Py：合并两个字典
来源：http://hef.meibo888.top

{**a, **b}
来源：http://nac.yueranfly.top

[U07] Py：反转字典键值
来源：http://lfh.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://iam.shuidangran.top

[U08] Py：展平二维列表
来源：http://qbo.gotoacloud.top

[y for x in nested for y in x]
来源：http://stb.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://dbe.dianchejie.cn

max(d, key=d.get)
来源：http://feo.xuanzx.com

[U10] Py：按值排序字典
来源：http://sev.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lmi.guannengcc.top

[U11] Py：生成器表达式
来源：http://hzv.zhixingplan.top

(x * 2 for x in arr)
来源：http://hgw.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oef.c1oappe.top

Counter(arr).most_common(3)
来源：http://cic.guowangkeji.top

[U13] Py：固定长度队列
来源：http://xqk.aizwys.cn

deque(maxlen=10)
来源：http://yyp.52xcode.cn

[U14] Py：分组收集到列表
来源：http://hxs.yangfankeji.com

defaultdict(list)
来源：http://tdj.yj202588.top

[U15] Py：高精度计时
来源：http://hmw.xziqi.cn

t = time.perf_counter()
来源：http://ftp.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://wrs.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nln.kuanghao11.cn

[U17] Py：初始化日志
来源：http://gzw.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://vdd.zhixingplan.top

[U18] Py：预编译正则
来源：http://xdv.andypj.xyz

pat = re.compile(r"\d+")
来源：http://dyx.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://lnd.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xoy.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://lui.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://pab.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://xxg.nanxinkj.top

@contextlib.contextmanager
来源：http://jcq.jinqigufen.top

[U22] Py：矩阵转置
来源：http://xrp.zhijiandao.cn

list(zip(*m))
来源：http://ewx.bjfxy.top

[U23] Py：分块读取大文件
来源：http://qro.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://upm.fktsv.cn

[U24] Py：路径操作
来源：http://hlr.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sap.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://qyo.iojbl.cn

csv.DictReader(f)
来源：http://mve.daxiang520.top

[U26] Py：并发下载
来源：http://fvq.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lci.iojbl.cn

[U27] Py：异步 HTTP
来源：http://oxu.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://idw.fktsv.cn

[U28] Py：类型别名
来源：http://afn.yj20258.top

UserId = int
来源：http://rob.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://gpr.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://gma.yj20258.top

[U30] Py：数据类
来源：http://haj.jinqigfzy.top

@dataclass(slots=True)
来源：http://xdd.nanxinkj.top

[U31] Py：单测
来源：http://yao.birdmap.top

python -m pytest -q
来源：http://bjy.iojbl.cn

[U32] Py：代码格式化
来源：http://ebb.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://lcl.birdmap.top

[U33] Py：打包发布
来源：http://ivj.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://omh.gogol.net.cn

[U34] Py：判断编码
来源：http://mlw.dianchejie.cn

chardet.detect(raw)
来源：http://mud.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://wck.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://din.nwbrower.top

[U36] Py：定时任务
来源：http://hgp.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://wbi.zdqjudy.top

[U37] Py：读写 Excel
来源：http://abt.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://psz.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://wuh.jinqigufen.top

Path(__file__).resolve().parent
来源：http://gma.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://dnt.daxiang520.top

sys.stdout.isatty()
来源：http://zum.mhx1999.top

[U40] Py：打印到标准错误
来源：http://ssb.zycfv.cn

print("err", file=sys.stderr)
来源：http://coe.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://ywx.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hrj.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://fxc.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cfm.wangdashe.top

[U43] PHP：声明命名空间
来源：http://lqb.hywenlv.cn

namespace App\Http;
来源：http://pnv.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://god.jinyuanbaomall.cn

declare(strict_types=1);
来源：http://sxb.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://ucl.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jgx.xuanzx.com

[U46] PHP：可空类型
来源：http://yip.hysaishi.cn

?string $name = null
来源：http://tmi.snrcjt.cn

[U47] PHP：联合类型
来源：http://qkf.shuidangran.top

int|string $id
来源：http://cbv.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://vyo.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ksh.0kj1m.cn

[U49] PHP：只读属性
来源：http://egm.zhengqikj.top

public readonly string $name
来源：http://jds.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://xuu.birdmap.top

public function __construct(private int $id) {}
来源：http://tyn.nwbrower.top

[U51] PHP：数组解构
来源：http://uth.cdnleiting.top

[$a, $b] = $arr;
来源：http://ewq.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://dgz.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://hfv.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://xop.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://cyp.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://xou.ydjk.org.cn

$obj?->method()
来源：http://zen.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://zah.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zfk.jinqigufen.top

[U56] PHP：命名参数
来源：http://gfi.hnqzz.top

f(a: 1, b: 2)
来源：http://ika.aibaodan.cn

[U57] PHP：字符串插值
来源：http://uol.kuanghao11.cn

"值: {$a}"
来源：http://ezf.ivvv.top

[U58] PHP：数组三件套
来源：http://hbz.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hdu.mhx1999.top

[U59] PHP：自定义排序
来源：http://pud.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jju.shzxlz.cn

[U60] PHP：JSON 编解码
来源：http://enz.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://edt.shanyushiyangtech.top

[U61] PHP：正则
来源：http://cpz.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wmn.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://bws.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mke.gotoacloud.top

[U63] PHP：文件读写
来源：http://qfw.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://shb.dashuyun.cn

[U64] PHP：目录遍历
来源：http://san.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://uxt.gzhubu.top

[U65] PHP：会话
来源：http://qhr.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://dsb.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://sha.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mwe.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://rtc.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wop.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://hpu.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vop.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://cid.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cfh.xinyue.icu

[U70] PHP：PDO 事务
来源：http://ukh.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://beh.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://dox.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://ksu.chenzaomai.com

[U72] PHP：写错误日志
来源：http://nkz.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://dpr.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://jgd.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://pdi.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://prg.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://odx.hesvh.cn

[U75] PHP：依赖注入
来源：http://oxj.zhengqikj.top

composer require psr/container
来源：http://utk.gzhubu.top

[U76] PHP：简单路由
来源：http://nsz.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rxs.yonumen.top


<!-- 参考信息 -->