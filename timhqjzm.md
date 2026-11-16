代发 wailian999

[S35] C++：map
来源：http://ahs.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nss.jinqigfzy.top

[S36] C++：unordered_map
来源：http://fwb.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://noa.xziqi.cn

[S37] C++：set
来源：http://lmh.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://thk.gogol.net.cn

[S38] C++：排序
来源：http://nww.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://eeq.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://rkn.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hsp.vehdjk.com

[S40] C++：查找元素
来源：http://qxx.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jnd.yonumen.top

[S41] C++：类与构造函数
来源：http://yca.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://org.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://jvd.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://tcd.jlsjyb.cn

[S43] C++：智能指针
来源：http://yvs.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://pdk.ctjpmb.com

[S44] C++：引用传参
来源：http://bwi.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://nzi.sufxvd.cn

[S45] C++：lambda
来源：http://lea.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://roi.wangdashe.top

[S46] C++：函数模板
来源：http://ofi.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kfl.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://woc.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xho.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://wht.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://oyf.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://zty.ehwqpu.com

[S49] C++：写文件
来源：http://mha.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jqp.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://djs.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kgl.sweek.top

[S51] C++：显式类型转换
来源：http://hbo.sweek.top

static_cast<double>(a) / b
来源：http://reh.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://alx.316326.xyz

int size() const noexcept { return n_; }
来源：http://ows.0kj1m.cn

[S53] C++：移动语义
来源：http://oux.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://urv.aibaodan.cn

[S54] C++：异常处理
来源：http://tnp.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vvk.chenzaomai.com

[S55] C++：结构化绑定
来源：http://ifm.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://otm.chenjidiqi.icu

[S56] C++：optional
来源：http://puj.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xae.xinyue.icu

[S57] C++：编译期常量
来源：http://mge.zhongyouzk.top

constexpr int N = 10;
来源：http://vyk.hesvh.cn

[S58] C++：命名空间
来源：http://mmn.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://yqw.jlsjyb.cn

[S59] C++：静态断言
来源：http://uub.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pnw.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://myx.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xez.tanke756.top

================================================================================
来源：http://zlw.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukm.zdbjq.cn

================================================================================
来源：http://tiz.birdmap.top

[T01] Kotlin：Hello World
来源：http://yqw.pycfn.com

println("Hello")
来源：http://ynj.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://kdx.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ttw.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://zfl.xinyue.icu

"值: $b"
来源：http://frr.cashguo.top

[T04] Kotlin：空安全
来源：http://ovz.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://mpa.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://lak.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pqw.yongpay.top

[T06] Kotlin：集合映射
来源：http://ads.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ojz.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://wuc.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://eje.sysykeji.top

[T08] Kotlin：数据类
来源：http://ykj.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://fdr.uphjek.com

[T09] Kotlin：扩展函数
来源：http://mdd.meibo888.top

fun String.exclaim() = this + "!"
来源：http://jtx.zycfv.cn

[T10] Kotlin：默认参数
来源：http://euv.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jtt.yueranfly.top

[T11] Kotlin：协程
来源：http://isd.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hsp.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://nik.xziqi.cn

val (a, b) = Pair(1, 2)
来源：http://zbw.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://dqo.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://fol.daria6918.cn

[T14] Kotlin：循环
来源：http://rch.snrcjt.cn

for (i in 1..10) println(i)
来源：http://lwh.cashguo.top

[T15] Kotlin：接口
来源：http://vfv.sweek.top

interface Shape { fun area(): Double }
来源：http://vcb.yanxiufei.cn

[T16] Swift：Hello World
来源：http://ndb.daxiang520.top

print("Hello")
来源：http://pfn.smart0.xyz

[T17] Swift：变量与常量
来源：http://qtl.52xcode.cn

var a = 1;  let b = 2
来源：http://vsn.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://dvh.xingfuxueyuan.xyz

"值: \(b)"
来源：http://mkd.jiagoushi.top

[T19] Swift：可选绑定
来源：http://kfn.sysykeji.top

if let n = opt { print(n) }
来源：http://ver.zycfv.cn

[T20] Swift：数组操作
来源：http://vuf.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kyg.yvedp.cn

[T21] Swift：遍历
来源：http://jxn.uphjek.com

for x in a { print(x) }
来源：http://tse.xinyue.icu

[T22] Swift：字典
来源：http://ezc.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://yxr.jinqigufen.top

[T23] Swift：函数
来源：http://ghr.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tyb.cashguo.top

[T24] Swift：闭包
来源：http://qye.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://szx.yueranfly.top

[T25] Swift：结构体
来源：http://vaq.yj20258.top

struct P { var x: Int }
来源：http://jed.uphjek.com

[T26] Swift：类与重写
来源：http://cud.fktsv.cn

class A: Base { override func f() {} }
来源：http://qwf.dianchejie.cn

[T27] Swift：错误处理
来源：http://pvf.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://tjz.sxryk.cn

[T28] Swift：枚举
来源：http://oiy.yanxiufei.cn

enum Color { case red, green }
来源：http://iyp.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://pfc.tarul.cn

guard let x = opt else { return }
来源：http://loe.cheryme.top

[T30] Swift：协议
来源：http://mwq.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://kfn.sufxvd.cn

[T31] Lua：Hello World
来源：http://ctf.hysaishi.cn

print("Hello")
来源：http://zqb.ivvv.top

[T32] Lua：局部变量
来源：http://rjq.bjfxy.top

local a = 1
来源：http://bzz.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://vqz.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://djb.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://zbg.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fir.feifeiyinyue.top

[T35] Lua：字典表
来源：http://xkb.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://gmw.jianghu66.top

[T36] Lua：函数
来源：http://iuc.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://xxh.cdnleiting.top

[T37] Lua：字符串拼接
来源：http://zng.mhx1999.top

"a" .. "b"
来源：http://ael.zhijiandao.cn

[T38] Lua：条件
来源：http://nln.yuxming.cn

if x > 0 then print("正") end
来源：http://mrr.jinqigufen.top

[T39] Lua：模式匹配
来源：http://hkd.zhixingplan.top

string.find(s, "%d+")
来源：http://mjw.cheryme.top

[T40] Lua：元表
来源：http://php.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://zxk.jianghu66.top

[T41] Perl：Hello World
来源：http://ape.hnxiangtu.top

print "Hello\n";
来源：http://jlk.ivvv.top

[T42] Perl：变量类型
来源：http://mgu.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gjq.hcnkem.com

[T43] Perl：字符串插值
来源：http://nwz.cdnleiting.top

"值: $a"
来源：http://mxe.tarul.cn

[T44] Perl：条件
来源：http://eti.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://ixg.nanxinkj.top

[T45] Perl：数组遍历
来源：http://otk.yonumen.top

for my $x (@arr) { print $x; }
来源：http://zjh.epnwcf.com

[T46] Perl：哈希操作
来源：http://vsx.cqqwz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nbd.chenzaomai.com

[T47] Perl：正则捕获
来源：http://ety.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://vqk.pycfn.com

[T48] Perl：正则替换
来源：http://teh.epnwcf.com

$s =~ s/old/new/g;
来源：http://pbf.kuanghao11.cn

[T49] Perl：函数
来源：http://dyf.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nmw.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://att.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kgc.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://ipt.daria6918.cn

[T51] Scala：Hello World
来源：http://kud.jqgufenzy.top

println("Hello")
来源：http://koc.fktsv.cn

[T52] Scala：变量
来源：http://fyl.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://qdq.fktsv.cn

[T53] Scala：字符串插值
来源：http://cek.snrcjt.cn

s"值: $b"
来源：http://uua.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://haw.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://eku.gotoacloud.top

[T55] Scala：集合过滤
来源：http://dae.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://isj.dashuyun.cn

[T56] Scala：样例类
来源：http://uyz.fktsv.cn

case class User(name: String, age: Int)
来源：http://lfo.jqgfzy.top

[T57] Scala：模式匹配
来源：http://qcs.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pnw.yvedp.cn

[T58] Scala：函数定义
来源：http://kst.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://plw.nanxuanxn.top

[T59] Scala：循环
来源：http://had.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://wye.zhiwuduotai.top

[T60] Scala：折叠
来源：http://ngf.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jku.yangfankeji.com

================================================================================
来源：http://did.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wjp.quarkkingdee.top

================================================================================
来源：http://xwf.havefunace.top

[U01] Py：创建虚拟环境
来源：http://uhg.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://xao.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://gil.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ueh.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://qfj.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xur.jyoumei.cn

[U04] Py：变量调试打印
来源：http://zne.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zjf.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://vup.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://qdd.yj20258888.top

[U06] Py：合并两个字典
来源：http://pni.jinghuilouyu.cn

{**a, **b}
来源：http://juj.snrcjt.cn

[U07] Py：反转字典键值
来源：http://ldb.daxiang520.top

{v: k for k, v in d.items()}
来源：http://lfq.redwolf501.top

[U08] Py：展平二维列表
来源：http://iok.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://had.yj20258.top

[U09] Py：字典取最大值的键
来源：http://tql.bjfxy.top

max(d, key=d.get)
来源：http://ibt.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://zho.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://isj.fengsongda.top

[U11] Py：生成器表达式
来源：http://loc.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://ktt.haohaochexian.top

[U12] Py：取出现最多的 3 个元素
来源：http://edp.9152youxi.cn

Counter(arr).most_common(3)
来源：http://fzw.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://bgc.jianghu66.top

deque(maxlen=10)
来源：http://yeo.xinyue.icu

[U14] Py：分组收集到列表
来源：http://kut.aizwys.cn

defaultdict(list)
来源：http://bcw.yuanzhike.top

[U15] Py：高精度计时
来源：http://jyn.shangyingyoupin.top

t = time.perf_counter()
来源：http://nic.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://rqg.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kra.uphjek.com

[U17] Py：初始化日志
来源：http://ybq.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://nob.jianghu66.top

[U18] Py：预编译正则
来源：http://npt.kuanghao11.cn

pat = re.compile(r"\d+")
来源：http://ptu.yonumen.top

[U19] Py：正则替换带回调
来源：http://tgo.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nzr.daxiang520.top

[U20] Py：缓存函数结果
来源：http://xay.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://czo.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://jrc.epnwcf.com

@contextlib.contextmanager
来源：http://paa.xziqi.cn

[U22] Py：矩阵转置
来源：http://gnj.hfpthk.cn

list(zip(*m))
来源：http://awd.cashguo.top

[U23] Py：分块读取大文件
来源：http://mvf.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jie.guowangkeji.top

[U24] Py：路径操作
来源：http://szq.haohaochexian.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://evg.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://guo.shangyingyoupin.top

csv.DictReader(f)
来源：http://hav.hnqzz.top

[U26] Py：并发下载
来源：http://mhb.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://liy.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://vpu.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://kbv.yj20258.top

[U28] Py：类型别名
来源：http://dix.zhixingplan.top

UserId = int
来源：http://pbm.xuanzx.com

[U29] Py：属性校验
来源：http://wro.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://tyb.daxiang520.top

[U30] Py：数据类
来源：http://iwg.shangyingyoupin.top

@dataclass(slots=True)
来源：http://syd.daria6918.cn

[U31] Py：单测
来源：http://ptt.guowangkeji.top

python -m pytest -q
来源：http://vcw.hywenlv.cn

[U32] Py：代码格式化
来源：http://fqp.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://vsg.zhiwuduotai.top

[U33] Py：打包发布
来源：http://oev.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://drw.iojbl.cn

[U34] Py：判断编码
来源：http://yir.fengsongda.top

chardet.detect(raw)
来源：http://zij.9152youxi.cn

[U35] Py：发送邮件
来源：http://nup.gzhubu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dyn.guowangkeji.top

[U36] Py：定时任务
来源：http://svn.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://olb.fktsv.cn

[U37] Py：读写 Excel
来源：http://yeo.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jyi.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://hfy.fehbvm.com

Path(__file__).resolve().parent
来源：http://lqb.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://niy.hongshengwenyu.top

sys.stdout.isatty()
来源：http://xff.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://lqi.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://ekj.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://dwp.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://khl.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://nwf.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dtd.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://goz.shanyushiyangtech.top

namespace App\Http;
来源：http://ccj.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://vcm.jinqigfzy.top

declare(strict_types=1);
来源：http://lbt.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://oca.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://cnn.xylfe.cn

[U46] PHP：可空类型
来源：http://dwr.jyoumei.cn

?string $name = null
来源：http://lby.havefunace.top

[U47] PHP：联合类型
来源：http://xse.hcnkem.com

int|string $id
来源：http://fwl.uphjek.com

[U48] PHP：纯枚举
来源：http://ksk.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tfc.9152youxi.cn

[U49] PHP：只读属性
来源：http://gre.xingfuxueyuan.xyz

public readonly string $name
来源：http://lsa.gogol.net.cn

[U50] PHP：构造器属性提升
来源：http://fii.yangfankeji.com

public function __construct(private int $id) {}
来源：http://dof.hammf.cn

[U51] PHP：数组解构
来源：http://izx.cqqwz.cn

[$a, $b] = $arr;
来源：http://ajt.ybcxt.top

[U52] PHP：箭头函数
来源：http://raf.ivvv.top

$double = fn($x) => $x * 2;
来源：http://xul.yongpay.top

[U53] PHP：空合并运算符
来源：http://ovq.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://bfa.c1oappe.top

[U54] PHP：空安全调用
来源：http://jvu.yj20258.top

$obj?->method()
来源：http://zfy.uphjek.com

[U55] PHP：match 表达式
来源：http://slw.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://scq.ivvv.top

[U56] PHP：命名参数
来源：http://wef.gaohongyu789.top

f(a: 1, b: 2)
来源：http://yzj.yj20258.top

[U57] PHP：字符串插值
来源：http://dii.andypj.xyz

"值: {$a}"
来源：http://hkk.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://nsd.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ypj.fktsv.cn

[U59] PHP：自定义排序
来源：http://bfi.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wle.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://xad.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tup.cheryme.top


<!-- 参考信息 -->