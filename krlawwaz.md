代发 wailian999

[S45] C++：lambda
来源：http://iot.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://bap.yangfankeji.com

[S46] C++：函数模板
来源：http://kuv.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whe.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://kvx.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iux.xinyue.icu

[S48] C++：逐行读文件
来源：http://zlj.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://bnh.aizwys.cn

while (std::getline(in, line)) { }
来源：http://kwd.jinqigufen.top

[S49] C++：写文件
来源：http://zyc.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nlc.fehbvm.com

[S50] C++：格式化数字
来源：http://dkn.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vtb.0kj1m.cn

[S51] C++：显式类型转换
来源：http://jfg.cqqwz.cn

static_cast<double>(a) / b
来源：http://lxc.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://bvh.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://biq.ybcxt.top

[S53] C++：移动语义
来源：http://qel.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://vkg.yj20258888.top

[S54] C++：异常处理
来源：http://eyd.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eah.cheryme.top

[S55] C++：结构化绑定
来源：http://llw.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nxv.zhengqikj.top

[S56] C++：optional
来源：http://xnt.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vyu.xinyue.icu

[S57] C++：编译期常量
来源：http://doa.uphjek.com

constexpr int N = 10;
来源：http://bta.haohaochexian.top

[S58] C++：命名空间
来源：http://wdz.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://vep.fengsongda.top

[S59] C++：静态断言
来源：http://fqu.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wso.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://paj.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kkx.tanke756.top

================================================================================
来源：http://tee.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://muu.hnqzz.top

================================================================================
来源：http://ixl.yj202588.top

[T01] Kotlin：Hello World
来源：http://nwp.mhx1999.top

println("Hello")
来源：http://itg.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://kgz.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://umy.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://puw.yvedp.cn

"值: $b"
来源：http://mre.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://wnj.yangfankeji.com

val n: String? = null;  n?.length
来源：http://iaq.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://ijo.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ijq.sxryk.cn

[T06] Kotlin：集合映射
来源：http://ojp.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kyg.cashguo.top

[T07] Kotlin：集合过滤
来源：http://hzs.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://fba.jinqigufen.top

[T08] Kotlin：数据类
来源：http://tku.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://mvh.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://bjr.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://zzm.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://lej.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://qer.yj20258.top

[T11] Kotlin：协程
来源：http://zye.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uzd.yvedp.cn

[T12] Kotlin：解构声明
来源：http://cxz.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://zpm.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://mua.bjfxy.top

val m = mapOf("a" to 1)
来源：http://crs.jinqigufen.top

[T14] Kotlin：循环
来源：http://bob.yonumen.top

for (i in 1..10) println(i)
来源：http://lvs.fengsongda.top

[T15] Kotlin：接口
来源：http://aaz.52xcode.cn

interface Shape { fun area(): Double }
来源：http://byr.tian-w.cn

[T16] Swift：Hello World
来源：http://pxg.hysaishi.cn

print("Hello")
来源：http://ukk.dashuyun.cn

[T17] Swift：变量与常量
来源：http://vjf.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://odf.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://hfn.yuxming.cn

"值: \(b)"
来源：http://ddq.yfazqb.com

[T19] Swift：可选绑定
来源：http://lgm.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://hzo.mhx1999.top

[T20] Swift：数组操作
来源：http://ihd.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://htj.zhongyouzk.top

[T21] Swift：遍历
来源：http://kaf.jinqigfzy.top

for x in a { print(x) }
来源：http://shv.yuanzhike.top

[T22] Swift：字典
来源：http://lcv.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://exy.xuetiantiany.cn

[T23] Swift：函数
来源：http://rec.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fwz.tanke756.top

[T24] Swift：闭包
来源：http://eat.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://teb.mhx1999.top

[T25] Swift：结构体
来源：http://bcd.dianchejie.cn

struct P { var x: Int }
来源：http://dks.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://mtc.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://kbw.jqgfzy.top

[T27] Swift：错误处理
来源：http://xgn.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://jhc.zhoulong.xyz

[T28] Swift：枚举
来源：http://lty.yuxming.cn

enum Color { case red, green }
来源：http://wrg.meibo888.top

[T29] Swift：guard 提前返回
来源：http://nwq.kuanghao11.cn

guard let x = opt else { return }
来源：http://iij.aibaodan.cn

[T30] Swift：协议
来源：http://rlk.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://sag.aizwys.cn

[T31] Lua：Hello World
来源：http://oxp.daxiang520.top

print("Hello")
来源：http://kba.jqgufenzy.top

[T32] Lua：局部变量
来源：http://dfo.yanxiufei.cn

local a = 1
来源：http://stc.ydzc1.top

[T33] Lua：表（数组）
来源：http://zjl.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wzb.epnwcf.com

[T34] Lua：遍历表
来源：http://oep.fzhhl.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oja.svipenyu.cn

[T35] Lua：字典表
来源：http://asy.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://spk.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://ors.shuidangran.top

function add(a, b) return a + b end
来源：http://fem.tanke756.top

[T37] Lua：字符串拼接
来源：http://lps.vehdjk.com

"a" .. "b"
来源：http://xty.jiagoushi.top

[T38] Lua：条件
来源：http://dfr.svipenyu.cn

if x > 0 then print("正") end
来源：http://akw.chenlongwang.top

[T39] Lua：模式匹配
来源：http://myn.ydjk.org.cn

string.find(s, "%d+")
来源：http://cmc.gogol.net.cn

[T40] Lua：元表
来源：http://ppy.fktsv.cn

setmetatable({}, { __index = base })
来源：http://fvn.mhx1999.top

[T41] Perl：Hello World
来源：http://uqt.nwbrower.top

print "Hello\n";
来源：http://tto.nanxuanxn.top

[T42] Perl：变量类型
来源：http://ham.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rjz.hnqzz.top

[T43] Perl：字符串插值
来源：http://rkb.yuxming.cn

"值: $a"
来源：http://bat.pengpengdd.cyou

[T44] Perl：条件
来源：http://znf.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://ges.nwbrower.top

[T45] Perl：数组遍历
来源：http://iwz.316326.xyz

for my $x (@arr) { print $x; }
来源：http://sfb.cucudq.cn

[T46] Perl：哈希操作
来源：http://vgh.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qlz.zdqjudy.top

[T47] Perl：正则捕获
来源：http://jwh.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://auf.sufxvd.cn

[T48] Perl：正则替换
来源：http://grv.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://cik.shangyingyoupin.top

[T49] Perl：函数
来源：http://oxy.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://owo.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://dsh.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zch.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://rmc.chenzaomai.com

[T51] Scala：Hello World
来源：http://eom.gaohongyu789.top

println("Hello")
来源：http://qrp.chenjidiqi.icu

[T52] Scala：变量
来源：http://zky.yj20258888.top

val a = 1;  var b = 2
来源：http://fub.iojbl.cn

[T53] Scala：字符串插值
来源：http://yrt.hysaishi.cn

s"值: $b"
来源：http://twi.yj202588.top

[T54] Scala：集合映射
来源：http://wff.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://suh.hesvh.cn

[T55] Scala：集合过滤
来源：http://grt.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vza.wangshuangyany.cn

[T56] Scala：样例类
来源：http://cll.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://byd.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://rgk.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fly.meibo888.top

[T58] Scala：函数定义
来源：http://wrk.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gvx.fanxiaobao.xyz

[T59] Scala：循环
来源：http://ogs.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://npa.nanxinkj.top

[T60] Scala：折叠
来源：http://doc.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pfx.jinqigfzy.top

================================================================================
来源：http://eyk.hammf.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kcy.c1oappe.top

================================================================================
来源：http://odc.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://ncs.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://sfx.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://suf.fzhhl.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lqb.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://xic.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://phz.xuanzx.com

[U04] Py：变量调试打印
来源：http://hxx.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ulc.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://ahf.hnqzz.top

list(dict.fromkeys(arr))
来源：http://ium.hammf.cn

[U06] Py：合并两个字典
来源：http://cjw.xylfe.cn

{**a, **b}
来源：http://qhs.zhengqikj.top

[U07] Py：反转字典键值
来源：http://shv.c1oappe.top

{v: k for k, v in d.items()}
来源：http://erp.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://qlw.xuanzx.com

[y for x in nested for y in x]
来源：http://xdu.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://wqv.yongpay.top

max(d, key=d.get)
来源：http://ezn.zdbjq.cn

[U10] Py：按值排序字典
来源：http://eym.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmb.ctjpmb.com

[U11] Py：生成器表达式
来源：http://hqe.daxiang520.top

(x * 2 for x in arr)
来源：http://ccp.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://kfo.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://izl.xziqi.cn

[U13] Py：固定长度队列
来源：http://hyn.fehbvm.com

deque(maxlen=10)
来源：http://uwr.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://ppp.cucudq.cn

defaultdict(list)
来源：http://aqp.svipenyu.cn

[U15] Py：高精度计时
来源：http://xir.jianghu66.top

t = time.perf_counter()
来源：http://bvw.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://gib.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qnz.guannengcc.top

[U17] Py：初始化日志
来源：http://qeu.yanxiufei.cn

logging.basicConfig(level=logging.INFO)
来源：http://tfc.jinqigfzy.top

[U18] Py：预编译正则
来源：http://qnp.zycfv.cn

pat = re.compile(r"\d+")
来源：http://dtw.wangdashe.top

[U19] Py：正则替换带回调
来源：http://kdd.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://inj.xuanzx.com

[U20] Py：缓存函数结果
来源：http://zsa.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://sek.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://axo.tarul.cn

@contextlib.contextmanager
来源：http://nua.hfpthk.cn

[U22] Py：矩阵转置
来源：http://vwj.bbcook.cn

list(zip(*m))
来源：http://blu.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://qyq.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dfa.guowangkeji.top

[U24] Py：路径操作
来源：http://wus.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dzb.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://gqr.zdbjq.cn

csv.DictReader(f)
来源：http://gpq.hcnkem.com

[U26] Py：并发下载
来源：http://ros.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hkk.yongpay.top

[U27] Py：异步 HTTP
来源：http://ymy.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://srj.yj20258.top

[U28] Py：类型别名
来源：http://moh.zdqjudy.top

UserId = int
来源：http://nte.tanke756.top

[U29] Py：属性校验
来源：http://rnf.zhengqikj.top

@property 与 @x.setter 配合
来源：http://wmg.daria6918.cn

[U30] Py：数据类
来源：http://wco.jlsjyb.cn

@dataclass(slots=True)
来源：http://elh.ehwqpu.com

[U31] Py：单测
来源：http://tpd.zhiwuduotai.top

python -m pytest -q
来源：http://lkk.iojbl.cn

[U32] Py：代码格式化
来源：http://kdu.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://izb.quarkkingdee.top

[U33] Py：打包发布
来源：http://ndl.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://pbr.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://han.iojbl.cn

chardet.detect(raw)
来源：http://cba.daxiang520.top

[U35] Py：发送邮件
来源：http://ape.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nwn.havefunace.top

[U36] Py：定时任务
来源：http://pjf.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://jgm.yj202588.top

[U37] Py：读写 Excel
来源：http://wso.jqgufenzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://phe.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://dkw.fehbvm.com

Path(__file__).resolve().parent
来源：http://pxu.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://vzb.sjlbkw.cn

sys.stdout.isatty()
来源：http://vud.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://xcb.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://ciq.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://thx.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://gpm.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://rsv.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ywo.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://rxm.yangfankeji.com

namespace App\Http;
来源：http://jes.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://gss.cqqwz.cn

declare(strict_types=1);
来源：http://yeg.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://ilm.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://onn.yvedp.cn

[U46] PHP：可空类型
来源：http://cno.zhongyouzk.top

?string $name = null
来源：http://gzv.dashuyun.cn

[U47] PHP：联合类型
来源：http://uhj.hammf.cn

int|string $id
来源：http://mng.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://gsb.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fjt.gzhubu.top

[U49] PHP：只读属性
来源：http://ahf.c1oappe.top

public readonly string $name
来源：http://doi.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://xdk.daxiang520.top

public function __construct(private int $id) {}
来源：http://vzh.zhoulong.xyz

[U51] PHP：数组解构
来源：http://rjo.zhoulong.xyz

[$a, $b] = $arr;
来源：http://nef.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://mjf.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://qhn.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://gfr.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://goe.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://svh.gaohongyu789.top

$obj?->method()
来源：http://stt.guowangkeji.top

[U55] PHP：match 表达式
来源：http://xdm.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://igb.xziqi.cn

[U56] PHP：命名参数
来源：http://uzu.hysaishi.cn

f(a: 1, b: 2)
来源：http://mvi.shuidangran.top

[U57] PHP：字符串插值
来源：http://wow.guowangkeji.top

"值: {$a}"
来源：http://per.pycfn.com

[U58] PHP：数组三件套
来源：http://ydi.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fuc.ppjwa.cn

[U59] PHP：自定义排序
来源：http://mrw.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsd.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://tox.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vuy.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://umt.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dna.fktsv.cn

[U62] PHP：日期对象
来源：http://syy.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dmk.gotoacloud.top

[U63] PHP：文件读写
来源：http://wqh.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pzn.xylfe.cn

[U64] PHP：目录遍历
来源：http://wcd.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://taq.dashuyun.cn

[U65] PHP：会话
来源：http://udb.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jib.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://rpu.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mid.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://trs.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dzv.yuxming.cn

[U68] PHP：PDO 连接
来源：http://wse.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://foo.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://rbx.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lol.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://zsx.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lka.yuanzhike.top


<!-- 参考信息 -->