代发 wailian999

[S43] C++：智能指针
来源：http://zgf.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://bvt.tian-w.cn

[S44] C++：引用传参
来源：http://ley.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://epc.hongshengwenyu.top

[S45] C++：lambda
来源：http://udf.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://okg.xziqi.cn

[S46] C++：函数模板
来源：http://tlo.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hxu.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://hpc.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wxj.fzhhl.top

[S48] C++：逐行读文件
来源：http://bkv.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://irp.fzhhl.top

while (std::getline(in, line)) { }
来源：http://ixx.gotoacloud.top

[S49] C++：写文件
来源：http://eky.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lep.xziqi.cn

[S50] C++：格式化数字
来源：http://nba.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xcp.yongpay.top

[S51] C++：显式类型转换
来源：http://ubh.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://qpi.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://txy.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://dzj.jiagoushi.top

[S53] C++：移动语义
来源：http://ozd.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://oyl.birdmap.top

[S54] C++：异常处理
来源：http://gpr.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sgs.hesvh.cn

[S55] C++：结构化绑定
来源：http://eqy.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gjo.ppjwa.cn

[S56] C++：optional
来源：http://ben.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bft.zdqjudy.top

[S57] C++：编译期常量
来源：http://qfm.yvedp.cn

constexpr int N = 10;
来源：http://wlq.aizwys.cn

[S58] C++：命名空间
来源：http://jhk.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://brs.316326.xyz

[S59] C++：静态断言
来源：http://gzi.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aom.uphjek.com

[S60] C++：遍历并删除元素
来源：http://elw.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pwi.ctjpmb.com

================================================================================
来源：http://ycf.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ixg.yueranfly.top

================================================================================
来源：http://yam.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://fgi.yuxming.cn

println("Hello")
来源：http://svb.xylfe.cn

[T02] Kotlin：变量
来源：http://tjy.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sur.sweek.top

[T03] Kotlin：字符串模板
来源：http://qam.daria6918.cn

"值: $b"
来源：http://rus.jinqigufen.top

[T04] Kotlin：空安全
来源：http://lxr.zdqjudy.top

val n: String? = null;  n?.length
来源：http://yye.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://zfc.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hvq.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://ucg.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://amr.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://xvb.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mil.dashuyun.cn

[T08] Kotlin：数据类
来源：http://wfe.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://agc.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://ybg.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://fai.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://vzi.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://suf.nanxinkj.top

[T11] Kotlin：协程
来源：http://uuw.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://atu.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://ezb.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://jmj.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://crg.tarul.cn

val m = mapOf("a" to 1)
来源：http://bdq.xuanzx.com

[T14] Kotlin：循环
来源：http://vqw.dashuyun.cn

for (i in 1..10) println(i)
来源：http://utr.meibo888.top

[T15] Kotlin：接口
来源：http://yta.ivvv.top

interface Shape { fun area(): Double }
来源：http://mfi.xylfe.cn

[T16] Swift：Hello World
来源：http://hfo.bjfxy.top

print("Hello")
来源：http://slo.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://jbi.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://yci.iojbl.cn

[T18] Swift：字符串插值
来源：http://vsj.xinyue.icu

"值: \(b)"
来源：http://lfj.sxryk.cn

[T19] Swift：可选绑定
来源：http://xmn.bjfxy.top

if let n = opt { print(n) }
来源：http://rer.zhixingplan.top

[T20] Swift：数组操作
来源：http://qut.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://lqh.hnqzz.top

[T21] Swift：遍历
来源：http://crh.redwolf501.top

for x in a { print(x) }
来源：http://mxi.pycfn.com

[T22] Swift：字典
来源：http://dqa.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://azs.shanyushiyangkeji.top

[T23] Swift：函数
来源：http://wpq.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://the.yfazqb.com

[T24] Swift：闭包
来源：http://fsc.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yhy.redwolf501.top

[T25] Swift：结构体
来源：http://bmw.jqgufenzy.top

struct P { var x: Int }
来源：http://wlz.sysykeji.top

[T26] Swift：类与重写
来源：http://dhv.mhx1999.top

class A: Base { override func f() {} }
来源：http://saf.yj202588.top

[T27] Swift：错误处理
来源：http://axz.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://lnx.gotoacloud.top

[T28] Swift：枚举
来源：http://gfh.shangyingyoupin.top

enum Color { case red, green }
来源：http://iub.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://ghr.wangdashe.top

guard let x = opt else { return }
来源：http://xon.wangdashe.top

[T30] Swift：协议
来源：http://pod.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://scw.chenzaomai.com

[T31] Lua：Hello World
来源：http://ncr.jqgufenzy.top

print("Hello")
来源：http://nbn.birdmap.top

[T32] Lua：局部变量
来源：http://vzd.316326.xyz

local a = 1
来源：http://bor.shzxlz.cn

[T33] Lua：表（数组）
来源：http://urs.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sbw.hesvh.cn

[T34] Lua：遍历表
来源：http://ivd.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cea.zhengqikj.top

[T35] Lua：字典表
来源：http://nfe.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://tuu.vehdjk.com

[T36] Lua：函数
来源：http://trj.bjfxy.top

function add(a, b) return a + b end
来源：http://nxl.hammf.cn

[T37] Lua：字符串拼接
来源：http://tlf.gotoacloud.top

"a" .. "b"
来源：http://njx.birdmap.top

[T38] Lua：条件
来源：http://fjw.haohaochexian.top

if x > 0 then print("正") end
来源：http://cwd.redwolf501.top

[T39] Lua：模式匹配
来源：http://leh.epnwcf.com

string.find(s, "%d+")
来源：http://wrp.andypj.xyz

[T40] Lua：元表
来源：http://rxh.sysykeji.top

setmetatable({}, { __index = base })
来源：http://teb.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://fby.zdqjudy.top

print "Hello\n";
来源：http://tsi.havefunace.top

[T42] Perl：变量类型
来源：http://gbe.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ygx.nwbrower.top

[T43] Perl：字符串插值
来源：http://dcp.vqdsnc.cn

"值: $a"
来源：http://pou.hcnkem.com

[T44] Perl：条件
来源：http://kqf.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://apf.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://yeb.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://zjc.hammf.cn

[T46] Perl：哈希操作
来源：http://xng.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tyq.dashuyun.cn

[T47] Perl：正则捕获
来源：http://qjg.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lit.yanxiufei.cn

[T48] Perl：正则替换
来源：http://hvf.zdqjudy.top

$s =~ s/old/new/g;
来源：http://rjg.52xcode.cn

[T49] Perl：函数
来源：http://huz.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sdw.havefunace.top

[T50] Perl：逐行读文件
来源：http://age.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://maa.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://zit.yfazqb.com

[T51] Scala：Hello World
来源：http://tuv.cashguo.top

println("Hello")
来源：http://uco.havefunace.top

[T52] Scala：变量
来源：http://icb.0kj1m.cn

val a = 1;  var b = 2
来源：http://ait.ehwqpu.com

[T53] Scala：字符串插值
来源：http://noo.xziqi.cn

s"值: $b"
来源：http://mtr.daria6918.cn

[T54] Scala：集合映射
来源：http://xuu.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://koo.gzhubu.top

[T55] Scala：集合过滤
来源：http://cfa.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://ndy.hfpthk.cn

[T56] Scala：样例类
来源：http://pti.daria6918.cn

case class User(name: String, age: Int)
来源：http://czw.yongpay.top

[T57] Scala：模式匹配
来源：http://jur.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zit.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://jjm.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gfe.fanxiaobao.xyz

[T59] Scala：循环
来源：http://wjd.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://fyp.0kj1m.cn

[T60] Scala：折叠
来源：http://fsf.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xac.shanyushiyangkeji.top

================================================================================
来源：http://kzy.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rzc.hcnkem.com

================================================================================
来源：http://azm.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://rlk.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://hnb.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://pph.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hll.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://ewq.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vlv.pycfn.com

[U04] Py：变量调试打印
来源：http://cbz.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vet.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://gxj.wangdashe.top

list(dict.fromkeys(arr))
来源：http://kux.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://rsd.ehwqpu.com

{**a, **b}
来源：http://idw.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://axn.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://qtn.gogol.net.cn

[U08] Py：展平二维列表
来源：http://wvi.aizwys.cn

[y for x in nested for y in x]
来源：http://oqw.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://auq.chenzaomai.com

max(d, key=d.get)
来源：http://zak.ydzc1.top

[U10] Py：按值排序字典
来源：http://fqy.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pyz.xylfe.cn

[U11] Py：生成器表达式
来源：http://qjf.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://vot.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cng.yfazqb.com

Counter(arr).most_common(3)
来源：http://wln.xziqi.cn

[U13] Py：固定长度队列
来源：http://kdw.fehbvm.com

deque(maxlen=10)
来源：http://rdx.andypj.xyz

[U14] Py：分组收集到列表
来源：http://lqf.hysaishi.cn

defaultdict(list)
来源：http://wbf.fktsv.cn

[U15] Py：高精度计时
来源：http://dxs.hongshengwenyu.top

t = time.perf_counter()
来源：http://nzf.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://vhf.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sqy.yanxiufei.cn

[U17] Py：初始化日志
来源：http://eif.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://xoa.52xcode.cn

[U18] Py：预编译正则
来源：http://pxq.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://vow.316326.xyz

[U19] Py：正则替换带回调
来源：http://mnz.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hji.cucudq.cn

[U20] Py：缓存函数结果
来源：http://lbk.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://isu.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://fow.gaohongyu789.top

@contextlib.contextmanager
来源：http://ind.9152youxi.cn

[U22] Py：矩阵转置
来源：http://ejs.ydzc1.top

list(zip(*m))
来源：http://kmy.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://zgf.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fua.nwbrower.top

[U24] Py：路径操作
来源：http://boq.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://azi.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://vgm.jqgufenzy.top

csv.DictReader(f)
来源：http://suw.sjlbkw.cn

[U26] Py：并发下载
来源：http://yfj.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://chi.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://pet.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://xpf.fktsv.cn

[U28] Py：类型别名
来源：http://fut.yanxiufei.cn

UserId = int
来源：http://hvg.fzhhl.top

[U29] Py：属性校验
来源：http://gsa.316326.xyz

@property 与 @x.setter 配合
来源：http://yvw.ctjpmb.com

[U30] Py：数据类
来源：http://aty.sxryk.cn

@dataclass(slots=True)
来源：http://trn.yj202588.top

[U31] Py：单测
来源：http://iac.hongshengwenyu.top

python -m pytest -q
来源：http://tms.yueranfly.top

[U32] Py：代码格式化
来源：http://avw.sweek.top

ruff format . && ruff check --fix .
来源：http://ido.tianlin.xyz

[U33] Py：打包发布
来源：http://evp.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://yvo.cqqwz.cn

[U34] Py：判断编码
来源：http://ciu.daria6918.cn

chardet.detect(raw)
来源：http://apl.hnxiangtu.top

[U35] Py：发送邮件
来源：http://mnk.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kxx.jyoumei.cn

[U36] Py：定时任务
来源：http://ckp.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://wox.yvedp.cn

[U37] Py：读写 Excel
来源：http://efp.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mat.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://sgr.hammf.cn

Path(__file__).resolve().parent
来源：http://cro.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://tzd.vehdjk.com

sys.stdout.isatty()
来源：http://qua.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://mfx.smart0.xyz

print("err", file=sys.stderr)
来源：http://eem.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://rkr.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://maz.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://heg.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tfj.fzhhl.top

[U43] PHP：声明命名空间
来源：http://ubn.gaohongyu789.top

namespace App\Http;
来源：http://yea.xylfe.cn

[U44] PHP：开启严格类型
来源：http://pqk.ivvv.top

declare(strict_types=1);
来源：http://brf.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://lsq.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ics.ehwqpu.com

[U46] PHP：可空类型
来源：http://qez.hnxiangtu.top

?string $name = null
来源：http://yix.yonumen.top

[U47] PHP：联合类型
来源：http://ztj.ydjk.org.cn

int|string $id
来源：http://xpl.zhixingplan.top

[U48] PHP：纯枚举
来源：http://byx.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://icf.sxryk.cn

[U49] PHP：只读属性
来源：http://jsd.guowangkeji.top

public readonly string $name
来源：http://fbd.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://mgb.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://bpl.sjlbkw.cn

[U51] PHP：数组解构
来源：http://vis.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://xpu.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://cba.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://kmd.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://ccz.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://ubm.mhx1999.top

[U54] PHP：空安全调用
来源：http://hoe.vqdsnc.cn

$obj?->method()
来源：http://eho.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://sel.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qxa.pycfn.com

[U56] PHP：命名参数
来源：http://lpx.fengsongda.top

f(a: 1, b: 2)
来源：http://ytq.ctjpmb.com

[U57] PHP：字符串插值
来源：http://vtf.guannengcc.top

"值: {$a}"
来源：http://ngj.ybcxt.top

[U58] PHP：数组三件套
来源：http://dus.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rof.tanke756.top

[U59] PHP：自定义排序
来源：http://vbd.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://usj.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://wjq.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hdf.feifeiyinyue.top

[U61] PHP：正则
来源：http://rrs.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dii.fzhhl.top

[U62] PHP：日期对象
来源：http://ics.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wyi.vqdsnc.cn

[U63] PHP：文件读写
来源：http://hgv.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://krh.wangdashe.top

[U64] PHP：目录遍历
来源：http://ygz.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://rcz.52xcode.cn

[U65] PHP：会话
来源：http://asg.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://utd.yj202588.top

[U66] PHP：设置 Cookie
来源：http://wus.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ttf.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://abr.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://brn.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://oah.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oqs.pengpengdd.cyou


<!-- 参考信息 -->