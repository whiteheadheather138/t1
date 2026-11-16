代发 wailian999

while (std::getline(in, line)) { }
来源：http://mdn.xuanzx.com

[S49] C++：写文件
来源：http://kyx.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qay.cucudq.cn

[S50] C++：格式化数字
来源：http://tgb.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bnp.jqgfzy.top

[S51] C++：显式类型转换
来源：http://ypm.ydjk.org.cn

static_cast<double>(a) / b
来源：http://jtf.hammf.cn

[S52] C++：const 与 noexcept
来源：http://kem.gzhubu.top

int size() const noexcept { return n_; }
来源：http://llc.haohaochexian.top

[S53] C++：移动语义
来源：http://esg.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://maq.zhoulong.xyz

[S54] C++：异常处理
来源：http://xpy.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yni.guannengcc.top

[S55] C++：结构化绑定
来源：http://tnj.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qcb.shzxlz.cn

[S56] C++：optional
来源：http://lcz.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lgr.yvedp.cn

[S57] C++：编译期常量
来源：http://quo.ppjwa.cn

constexpr int N = 10;
来源：http://coo.guannengcc.top

[S58] C++：命名空间
来源：http://kib.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://cpp.fzhhl.top

[S59] C++：静态断言
来源：http://glv.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kkb.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://tcf.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uza.fanxiaobao.xyz

================================================================================
来源：http://ihv.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cvq.zhixingplan.top

================================================================================
来源：http://aqw.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://zim.smart0.xyz

println("Hello")
来源：http://qdm.daxiang520.top

[T02] Kotlin：变量
来源：http://nfi.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sqc.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://hsn.xziqi.cn

"值: $b"
来源：http://agh.pycfn.com

[T04] Kotlin：空安全
来源：http://fte.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://psq.316326.xyz

[T05] Kotlin：when 表达式
来源：http://eqg.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dup.ybcxt.top

[T06] Kotlin：集合映射
来源：http://xne.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://jih.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://kbp.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vbp.shuidangran.top

[T08] Kotlin：数据类
来源：http://vpd.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://mmv.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://hsh.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://zdl.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://yft.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://drf.nanxinkj.top

[T11] Kotlin：协程
来源：http://utv.zdbjq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jes.fengsongda.top

[T12] Kotlin：解构声明
来源：http://ovx.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://ull.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://rqx.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://vqe.chenlongwang.top

[T14] Kotlin：循环
来源：http://eoa.gotoacloud.top

for (i in 1..10) println(i)
来源：http://phy.zhongyouzk.top

[T15] Kotlin：接口
来源：http://hvr.aizwys.cn

interface Shape { fun area(): Double }
来源：http://cow.tianlin.xyz

[T16] Swift：Hello World
来源：http://cqj.jinqigfzy.top

print("Hello")
来源：http://ewi.hnqzz.top

[T17] Swift：变量与常量
来源：http://hnp.nanxinkj.top

var a = 1;  let b = 2
来源：http://tze.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://nwi.ydzc1.top

"值: \(b)"
来源：http://zes.yongpay.top

[T19] Swift：可选绑定
来源：http://lvk.jlsjyb.cn

if let n = opt { print(n) }
来源：http://mbb.ctjpmb.com

[T20] Swift：数组操作
来源：http://bmp.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://cfk.ivvv.top

[T21] Swift：遍历
来源：http://fzk.cqqwz.cn

for x in a { print(x) }
来源：http://kjj.snrcjt.cn

[T22] Swift：字典
来源：http://dop.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://lna.9152youxi.cn

[T23] Swift：函数
来源：http://gzo.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sjg.jqgufenzy.top

[T24] Swift：闭包
来源：http://adp.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ssr.fktsv.cn

[T25] Swift：结构体
来源：http://ogb.hcnkem.com

struct P { var x: Int }
来源：http://gfn.nanxuanxn.top

[T26] Swift：类与重写
来源：http://bsh.chenzaomai.com

class A: Base { override func f() {} }
来源：http://sem.zhongyouzk.top

[T27] Swift：错误处理
来源：http://unw.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://qie.52xcode.cn

[T28] Swift：枚举
来源：http://cqk.sweek.top

enum Color { case red, green }
来源：http://zrq.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://twb.yj202588.top

guard let x = opt else { return }
来源：http://sja.tarul.cn

[T30] Swift：协议
来源：http://xpo.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://hqp.cdnleiting.top

[T31] Lua：Hello World
来源：http://ihk.daxiang520.top

print("Hello")
来源：http://fee.xuanzx.com

[T32] Lua：局部变量
来源：http://xim.havefunace.top

local a = 1
来源：http://syr.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://vsa.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sfx.jianghu66.top

[T34] Lua：遍历表
来源：http://tmk.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gcc.jinqigufen.top

[T35] Lua：字典表
来源：http://ist.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://yyy.andypj.xyz

[T36] Lua：函数
来源：http://ljf.mhx1999.top

function add(a, b) return a + b end
来源：http://dkm.cheryme.top

[T37] Lua：字符串拼接
来源：http://oxm.tianlin.xyz

"a" .. "b"
来源：http://zxz.yj202588.top

[T38] Lua：条件
来源：http://bml.jlsjyb.cn

if x > 0 then print("正") end
来源：http://tgr.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://xwq.kuanghao11.cn

string.find(s, "%d+")
来源：http://rne.yanxiufei.cn

[T40] Lua：元表
来源：http://pjw.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://znc.cucudq.cn

[T41] Perl：Hello World
来源：http://suf.fanxiaobao.xyz

print "Hello\n";
来源：http://zcl.sysykeji.top

[T42] Perl：变量类型
来源：http://tfa.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nvk.cucudq.cn

[T43] Perl：字符串插值
来源：http://ydt.cucudq.cn

"值: $a"
来源：http://exd.gzhubu.top

[T44] Perl：条件
来源：http://obt.316326.xyz

if ($a > 0) { print "正"; }
来源：http://lqb.ybcxt.top

[T45] Perl：数组遍历
来源：http://bpo.havefunace.top

for my $x (@arr) { print $x; }
来源：http://yra.9152youxi.cn

[T46] Perl：哈希操作
来源：http://iou.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tyc.dashuyun.cn

[T47] Perl：正则捕获
来源：http://twv.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jhe.cucudq.cn

[T48] Perl：正则替换
来源：http://wsx.fehbvm.com

$s =~ s/old/new/g;
来源：http://dlq.zhiwuduotai.top

[T49] Perl：函数
来源：http://bru.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kig.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://rfx.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qoh.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://opp.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://qfu.ybcxt.top

println("Hello")
来源：http://ubu.tian-w.cn

[T52] Scala：变量
来源：http://hao.fehbvm.com

val a = 1;  var b = 2
来源：http://xbr.52xcode.cn

[T53] Scala：字符串插值
来源：http://suc.sweek.top

s"值: $b"
来源：http://nrw.0kj1m.cn

[T54] Scala：集合映射
来源：http://iai.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://fmy.jiagoushi.top

[T55] Scala：集合过滤
来源：http://lkh.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://eit.hfpthk.cn

[T56] Scala：样例类
来源：http://odz.jianghu66.top

case class User(name: String, age: Int)
来源：http://xmi.uphjek.com

[T57] Scala：模式匹配
来源：http://jsn.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ria.yueranfly.top

[T58] Scala：函数定义
来源：http://xei.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://cpv.jqgufenzy.top

[T59] Scala：循环
来源：http://bgm.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://ffa.jqgfzy.top

[T60] Scala：折叠
来源：http://ubm.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pmq.fktsv.cn

================================================================================
来源：http://som.jlsjyb.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zbp.andypj.xyz

================================================================================
来源：http://gfy.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://bol.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://ddq.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://fjb.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vmi.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://dtt.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zyf.meibo888.top

[U04] Py：变量调试打印
来源：http://rpb.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pch.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://jqq.yj20258.top

list(dict.fromkeys(arr))
来源：http://mot.nanxinkj.top

[U06] Py：合并两个字典
来源：http://ucf.gotoacloud.top

{**a, **b}
来源：http://vte.hysaishi.cn

[U07] Py：反转字典键值
来源：http://yef.yuxming.cn

{v: k for k, v in d.items()}
来源：http://fdk.ehwqpu.com

[U08] Py：展平二维列表
来源：http://jfs.guowangkeji.top

[y for x in nested for y in x]
来源：http://uce.yongpay.top

[U09] Py：字典取最大值的键
来源：http://jsj.aibaodan.cn

max(d, key=d.get)
来源：http://mkj.tianlin.xyz

[U10] Py：按值排序字典
来源：http://soz.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fbh.wangdashe.top

[U11] Py：生成器表达式
来源：http://seb.vehdjk.com

(x * 2 for x in arr)
来源：http://sqh.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://evd.c1oappe.top

Counter(arr).most_common(3)
来源：http://xfa.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://ucd.yj20258888.top

deque(maxlen=10)
来源：http://qmh.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://txu.vehdjk.com

defaultdict(list)
来源：http://nki.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://klk.cucudq.cn

t = time.perf_counter()
来源：http://xgq.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://zsh.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://niz.yvedp.cn

[U17] Py：初始化日志
来源：http://you.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://ukq.jinqigfzy.top

[U18] Py：预编译正则
来源：http://pec.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://eqr.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://boe.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pfa.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://eqq.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://hiz.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://jhj.jiagoushi.top

@contextlib.contextmanager
来源：http://bhz.hysaishi.cn

[U22] Py：矩阵转置
来源：http://vfl.hongshengwenyu.top

list(zip(*m))
来源：http://hrg.cashguo.top

[U23] Py：分块读取大文件
来源：http://zka.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qwk.dashuyun.cn

[U24] Py：路径操作
来源：http://mui.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://puw.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://upi.xinyue.icu

csv.DictReader(f)
来源：http://cuw.feifeiyinyue.top

[U26] Py：并发下载
来源：http://pmk.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ozt.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ate.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://fop.dashuyun.cn

[U28] Py：类型别名
来源：http://utm.zhongyouzk.top

UserId = int
来源：http://fpm.hammf.cn

[U29] Py：属性校验
来源：http://bub.jyoumei.cn

@property 与 @x.setter 配合
来源：http://vga.fanxiaobao.xyz

[U30] Py：数据类
来源：http://pgc.uphjek.com

@dataclass(slots=True)
来源：http://krx.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://wre.aibaodan.cn

python -m pytest -q
来源：http://lmn.zhengqikj.top

[U32] Py：代码格式化
来源：http://hql.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://lro.dashuyun.cn

[U33] Py：打包发布
来源：http://zuv.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://klu.zycfv.cn

[U34] Py：判断编码
来源：http://xqn.yuxming.cn

chardet.detect(raw)
来源：http://cxd.zhixingplan.top

[U35] Py：发送邮件
来源：http://ejx.haohaochexian.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rve.zhengqikj.top

[U36] Py：定时任务
来源：http://vuy.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://dmw.sysykeji.top

[U37] Py：读写 Excel
来源：http://nua.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hie.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://ffw.ivvv.top

Path(__file__).resolve().parent
来源：http://wze.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://apg.chenlongwang.top

sys.stdout.isatty()
来源：http://fms.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://uro.cheryme.top

print("err", file=sys.stderr)
来源：http://gns.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://uoi.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://swp.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://qyp.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xhj.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://bwc.ybcxt.top

namespace App\Http;
来源：http://kll.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://trf.ppjwa.cn

declare(strict_types=1);
来源：http://pxi.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://osy.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ovm.snrcjt.cn

[U46] PHP：可空类型
来源：http://wqn.zdbjq.cn

?string $name = null
来源：http://hsa.zhoulong.xyz

[U47] PHP：联合类型
来源：http://mkj.ctjpmb.com

int|string $id
来源：http://xlo.bbcook.cn

[U48] PHP：纯枚举
来源：http://igb.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xwe.hnqzz.top

[U49] PHP：只读属性
来源：http://flf.nanxinkj.top

public readonly string $name
来源：http://vnx.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://vhe.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://ojz.hnqzz.top

[U51] PHP：数组解构
来源：http://jay.gaohongyu789.top

[$a, $b] = $arr;
来源：http://ocs.uphjek.com

[U52] PHP：箭头函数
来源：http://ted.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://tni.smart0.xyz

[U53] PHP：空合并运算符
来源：http://qpb.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://foi.uphjek.com

[U54] PHP：空安全调用
来源：http://kya.mhx1999.top

$obj?->method()
来源：http://sni.zdqjudy.top

[U55] PHP：match 表达式
来源：http://sin.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yyt.nwbrower.top

[U56] PHP：命名参数
来源：http://ptu.tianlin.xyz

f(a: 1, b: 2)
来源：http://ocy.shzxlz.cn

[U57] PHP：字符串插值
来源：http://bhb.quarkkingdee.top

"值: {$a}"
来源：http://cbi.c1oappe.top

[U58] PHP：数组三件套
来源：http://bzs.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ibr.yj20258.top

[U59] PHP：自定义排序
来源：http://dem.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ydt.pycfn.com

[U60] PHP：JSON 编解码
来源：http://kjk.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wwr.cdnleiting.top

[U61] PHP：正则
来源：http://ddk.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eeb.hammf.cn

[U62] PHP：日期对象
来源：http://uwi.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lmv.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://iab.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gup.dianchejie.cn

[U64] PHP：目录遍历
来源：http://lfd.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://eog.fehbvm.com

[U65] PHP：会话
来源：http://enl.9152youxi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://noa.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://sir.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bac.fzhhl.top

[U67] PHP：处理文件上传
来源：http://vfd.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gwu.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://rsl.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mvk.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://kpn.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://elj.yuxming.cn

[U70] PHP：PDO 事务
来源：http://auj.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xqa.shzxlz.cn

[U71] PHP：抛出异常
来源：http://knx.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://bbs.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://kqd.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://buh.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://glw.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://vwg.bjfxy.top

[U74] PHP：读取环境变量
来源：http://xcc.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://phw.jiagoushi.top


<!-- 参考信息 -->