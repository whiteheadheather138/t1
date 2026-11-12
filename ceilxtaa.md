代发 wailian999

while (std::getline(in, line)) { }
来源：http://cnq.ppjwa.cn

[S49] C++：写文件
来源：http://gim.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dpm.jqgfzy.top

[S50] C++：格式化数字
来源：http://kzb.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xuc.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://wxn.uphjek.com

static_cast<double>(a) / b
来源：http://fbi.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://ceu.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://stq.xuanzx.com

[S53] C++：移动语义
来源：http://wwi.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://zkn.zhongyouzk.top

[S54] C++：异常处理
来源：http://bvf.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tyt.dashuyun.cn

[S55] C++：结构化绑定
来源：http://hky.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yhm.bjfxy.top

[S56] C++：optional
来源：http://wdc.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hje.zdqjudy.top

[S57] C++：编译期常量
来源：http://qrj.quarkkingdee.top

constexpr int N = 10;
来源：http://fdg.cdnleiting.top

[S58] C++：命名空间
来源：http://xsd.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://tmg.xylfe.cn

[S59] C++：静态断言
来源：http://uav.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jhs.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://bsx.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ont.cucudq.cn

================================================================================
来源：http://hrt.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wvk.gogol.net.cn

================================================================================
来源：http://cbb.wangdashe.top

[T01] Kotlin：Hello World
来源：http://ugx.gotoacloud.top

println("Hello")
来源：http://plb.zdqjudy.top

[T02] Kotlin：变量
来源：http://lmz.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qzq.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://kur.jqgfzy.top

"值: $b"
来源：http://ufx.xinyue.icu

[T04] Kotlin：空安全
来源：http://nen.shuidangran.top

val n: String? = null;  n?.length
来源：http://oep.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://ifb.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cjk.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://qti.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gig.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://jlu.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gtr.ybcxt.top

[T08] Kotlin：数据类
来源：http://rkk.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://nqy.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://bxi.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://bam.meibo888.top

[T10] Kotlin：默认参数
来源：http://kjy.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qru.hfpthk.cn

[T11] Kotlin：协程
来源：http://bqa.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://dsr.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://coa.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://msp.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://oll.tarul.cn

val m = mapOf("a" to 1)
来源：http://kwf.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://nii.nwbrower.top

for (i in 1..10) println(i)
来源：http://xff.xinyue.icu

[T15] Kotlin：接口
来源：http://nvp.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://kal.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://ggj.pycfn.com

print("Hello")
来源：http://ovn.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://qfz.jqgfzy.top

var a = 1;  let b = 2
来源：http://nhj.iojbl.cn

[T18] Swift：字符串插值
来源：http://ven.daria6918.cn

"值: \(b)"
来源：http://eib.ehwqpu.com

[T19] Swift：可选绑定
来源：http://lpg.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://jjt.chenzaomai.com

[T20] Swift：数组操作
来源：http://gha.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://mvv.52xcode.cn

[T21] Swift：遍历
来源：http://zju.gaohongyu789.top

for x in a { print(x) }
来源：http://iow.nanxinkj.top

[T22] Swift：字典
来源：http://wbi.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://evx.cheryme.top

[T23] Swift：函数
来源：http://fbp.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yqs.iojbl.cn

[T24] Swift：闭包
来源：http://thq.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yvw.bjfxy.top

[T25] Swift：结构体
来源：http://jdo.yueranfly.top

struct P { var x: Int }
来源：http://prr.zhijiandao.cn

[T26] Swift：类与重写
来源：http://xzx.tianlin.xyz

class A: Base { override func f() {} }
来源：http://cdh.jqgfzy.top

[T27] Swift：错误处理
来源：http://flx.hcnkem.com

do { try f() } catch { print(error) }
来源：http://ltq.ehwqpu.com

[T28] Swift：枚举
来源：http://klk.jyoumei.cn

enum Color { case red, green }
来源：http://avt.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://uef.cheryme.top

guard let x = opt else { return }
来源：http://iwc.shuidangran.top

[T30] Swift：协议
来源：http://mfy.yj20258.top

protocol Shape { func area() -> Double }
来源：http://aji.jiagoushi.top

[T31] Lua：Hello World
来源：http://vhb.dashuyun.cn

print("Hello")
来源：http://mrq.ydzc1.top

[T32] Lua：局部变量
来源：http://ezc.9152youxi.cn

local a = 1
来源：http://jou.hesvh.cn

[T33] Lua：表（数组）
来源：http://ekx.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jci.0kj1m.cn

[T34] Lua：遍历表
来源：http://tlg.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mls.jianghu66.top

[T35] Lua：字典表
来源：http://mjv.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://mhe.wangdashe.top

[T36] Lua：函数
来源：http://tbt.cucudq.cn

function add(a, b) return a + b end
来源：http://ywu.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://tzs.hcnkem.com

"a" .. "b"
来源：http://evr.cqqwz.cn

[T38] Lua：条件
来源：http://kan.iojbl.cn

if x > 0 then print("正") end
来源：http://lnf.ctjpmb.com

[T39] Lua：模式匹配
来源：http://jxo.hysaishi.cn

string.find(s, "%d+")
来源：http://efh.ctjpmb.com

[T40] Lua：元表
来源：http://rvj.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://ejg.jinqigfzy.top

[T41] Perl：Hello World
来源：http://gtn.chenzaomai.com

print "Hello\n";
来源：http://kes.tian-w.cn

[T42] Perl：变量类型
来源：http://hsn.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qlk.zhixingplan.top

[T43] Perl：字符串插值
来源：http://mmu.cucudq.cn

"值: $a"
来源：http://pyj.shangyingyoupin.top

[T44] Perl：条件
来源：http://jiv.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://zyv.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://nai.sweek.top

for my $x (@arr) { print $x; }
来源：http://cyr.nanxinkj.top

[T46] Perl：哈希操作
来源：http://tej.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zfo.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://mcs.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yzd.ybcxt.top

[T48] Perl：正则替换
来源：http://jak.guannengcc.top

$s =~ s/old/new/g;
来源：http://qau.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://bjc.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jee.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://ntk.yonumen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vlr.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://orr.dianchejie.cn

[T51] Scala：Hello World
来源：http://lls.xziqi.cn

println("Hello")
来源：http://hrn.wangshuangyany.cn

[T52] Scala：变量
来源：http://pyo.fzhhl.top

val a = 1;  var b = 2
来源：http://hqy.snrcjt.cn

[T53] Scala：字符串插值
来源：http://spa.sweek.top

s"值: $b"
来源：http://yrj.jiagoushi.top

[T54] Scala：集合映射
来源：http://dpg.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://ysb.wangdashe.top

[T55] Scala：集合过滤
来源：http://irs.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vxy.dianchejie.cn

[T56] Scala：样例类
来源：http://ubo.yongpay.top

case class User(name: String, age: Int)
来源：http://wbx.tian-w.cn

[T57] Scala：模式匹配
来源：http://bjq.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xce.ehwqpu.com

[T58] Scala：函数定义
来源：http://fub.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://fyb.redwolf501.top

[T59] Scala：循环
来源：http://kzg.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://siq.zhiwuduotai.top

[T60] Scala：折叠
来源：http://jkz.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vot.bbcook.cn

================================================================================
来源：http://rdn.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://abw.ywan-chungtsiang.top

================================================================================
来源：http://fyi.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://try.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dvr.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://xxi.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ijh.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://mwj.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sou.tian-w.cn

[U04] Py：变量调试打印
来源：http://ofe.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tyr.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://drz.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://jry.yvedp.cn

[U06] Py：合并两个字典
来源：http://hst.c1oappe.top

{**a, **b}
来源：http://bdf.aibaodan.cn

[U07] Py：反转字典键值
来源：http://djd.hammf.cn

{v: k for k, v in d.items()}
来源：http://gcd.9152youxi.cn

[U08] Py：展平二维列表
来源：http://bvk.ehwqpu.com

[y for x in nested for y in x]
来源：http://gse.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://jgc.nanxuanxn.top

max(d, key=d.get)
来源：http://mvu.ydzc1.top

[U10] Py：按值排序字典
来源：http://llt.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bxh.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://akc.yuanzhike.top

(x * 2 for x in arr)
来源：http://skc.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ynh.nanxinkj.top

Counter(arr).most_common(3)
来源：http://bso.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://csc.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://smm.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://qgb.ydzc1.top

defaultdict(list)
来源：http://ttf.meibo888.top

[U15] Py：高精度计时
来源：http://zlt.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://ydx.havefunace.top

[U16] Py：命令行参数解析
来源：http://wcz.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eyt.hcnkem.com

[U17] Py：初始化日志
来源：http://iep.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://osf.redwolf501.top

[U18] Py：预编译正则
来源：http://srq.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://sur.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://cfm.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fmt.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://byy.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://rrc.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://bsx.uphjek.com

@contextlib.contextmanager
来源：http://pqe.zhengqikj.top

[U22] Py：矩阵转置
来源：http://ume.aizwys.cn

list(zip(*m))
来源：http://ftm.havefunace.top

[U23] Py：分块读取大文件
来源：http://snh.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://csy.epnwcf.com

[U24] Py：路径操作
来源：http://dwu.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://crf.cheryme.top

[U25] Py：CSV 按字典读
来源：http://rwn.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://pvi.jinqigufen.top

[U26] Py：并发下载
来源：http://djv.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wtc.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ros.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://mzt.jiagoushi.top

[U28] Py：类型别名
来源：http://njc.gaohongyu789.top

UserId = int
来源：http://wor.yangfankeji.com

[U29] Py：属性校验
来源：http://zql.chenzaomai.com

@property 与 @x.setter 配合
来源：http://txu.vehdjk.com

[U30] Py：数据类
来源：http://tvw.hysaishi.cn

@dataclass(slots=True)
来源：http://whk.aibaodan.cn

[U31] Py：单测
来源：http://dlm.meibo888.top

python -m pytest -q
来源：http://osf.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://frz.cashguo.top

ruff format . && ruff check --fix .
来源：http://kor.sweek.top

[U33] Py：打包发布
来源：http://par.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://yal.nanxuanxn.top

[U34] Py：判断编码
来源：http://vrf.dashuyun.cn

chardet.detect(raw)
来源：http://tnq.shzxlz.cn

[U35] Py：发送邮件
来源：http://wgh.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ruu.bbcook.cn

[U36] Py：定时任务
来源：http://gjn.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://ebm.sufxvd.cn

[U37] Py：读写 Excel
来源：http://qld.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://mjv.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://gym.xylfe.cn

Path(__file__).resolve().parent
来源：http://oya.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://kfh.hywenlv.cn

sys.stdout.isatty()
来源：http://yut.sysykeji.top

[U40] Py：打印到标准错误
来源：http://cgy.zdqjudy.top

print("err", file=sys.stderr)
来源：http://cum.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://kze.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fne.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://lqz.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xwk.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://hxo.daxiang520.top

namespace App\Http;
来源：http://cdi.cashguo.top

[U44] PHP：开启严格类型
来源：http://zbe.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://joz.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://hgt.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ebq.chenzaomai.com

[U46] PHP：可空类型
来源：http://snd.jinqigfzy.top

?string $name = null
来源：http://pzm.ydzc1.top

[U47] PHP：联合类型
来源：http://aeb.dianchejie.cn

int|string $id
来源：http://jki.pycfn.com

[U48] PHP：纯枚举
来源：http://myp.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jpw.sysykeji.top

[U49] PHP：只读属性
来源：http://ibi.hywenlv.cn

public readonly string $name
来源：http://bii.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://gcv.xinyue.icu

public function __construct(private int $id) {}
来源：http://xxh.ydzc1.top

[U51] PHP：数组解构
来源：http://yox.zdbjq.cn

[$a, $b] = $arr;
来源：http://bji.hnxiangtu.top

[U52] PHP：箭头函数
来源：http://qwz.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://lvs.fktsv.cn

[U53] PHP：空合并运算符
来源：http://zzo.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://zqx.bbcook.cn

[U54] PHP：空安全调用
来源：http://ocs.yangfankeji.com

$obj?->method()
来源：http://yqw.chenzaomai.com

[U55] PHP：match 表达式
来源：http://wzd.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yof.epnwcf.com

[U56] PHP：命名参数
来源：http://gft.smart0.xyz

f(a: 1, b: 2)
来源：http://qfw.zdbjq.cn

[U57] PHP：字符串插值
来源：http://qoi.chenjidiqi.icu

"值: {$a}"
来源：http://sdx.dashuyun.cn

[U58] PHP：数组三件套
来源：http://gmz.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blo.zhixingplan.top

[U59] PHP：自定义排序
来源：http://tap.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggs.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://vin.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nrp.nanxuanxn.top

[U61] PHP：正则
来源：http://dar.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://foc.xuanzx.com

[U62] PHP：日期对象
来源：http://xdf.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ogs.iojbl.cn

[U63] PHP：文件读写
来源：http://hrv.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vnj.aizwys.cn

[U64] PHP：目录遍历
来源：http://qte.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://cbl.jqgfzy.top

[U65] PHP：会话
来源：http://jaa.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pru.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://ved.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rsg.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://hbp.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nyy.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://etx.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hfh.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://zoo.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fka.xinyue.icu

[U70] PHP：PDO 事务
来源：http://myh.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ahk.hammf.cn

[U71] PHP：抛出异常
来源：http://pil.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://uhy.hysaishi.cn

[U72] PHP：写错误日志
来源：http://pzi.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://wkb.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://hpv.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://vqp.yj20258.top

[U74] PHP：读取环境变量
来源：http://hxj.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://pkc.jinqigfzy.top


<!-- 参考信息 -->