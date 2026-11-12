代发 wailian999

[S35] C++：map
来源：http://gby.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mff.zdqjudy.top

[S36] C++：unordered_map
来源：http://tiz.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cqj.hongshengwenyu.top

[S37] C++：set
来源：http://tjr.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aia.xuanzx.com

[S38] C++：排序
来源：http://ywm.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://fwf.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://lri.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xod.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://wln.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ebx.ybcxt.top

[S41] C++：类与构造函数
来源：http://qvo.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ygw.xinyue.icu

[S42] C++：继承与虚函数
来源：http://vvl.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://org.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://oyy.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://hur.zycfv.cn

[S44] C++：引用传参
来源：http://jyn.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://cll.hcnkem.com

[S45] C++：lambda
来源：http://yrk.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bue.daria6918.cn

[S46] C++：函数模板
来源：http://sae.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hum.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://snr.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hrw.nanxinkj.top

[S48] C++：逐行读文件
来源：http://fea.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://een.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://pik.jinghuilouyu.cn

[S49] C++：写文件
来源：http://mzr.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://awj.jyoumei.cn

[S50] C++：格式化数字
来源：http://pug.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tfb.guannengcc.top

[S51] C++：显式类型转换
来源：http://wkx.xuanzx.com

static_cast<double>(a) / b
来源：http://fhc.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://imq.ydzc1.top

int size() const noexcept { return n_; }
来源：http://nnw.gaohongyu789.top

[S53] C++：移动语义
来源：http://cdt.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://kpn.fehbvm.com

[S54] C++：异常处理
来源：http://scx.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vcy.yfazqb.com

[S55] C++：结构化绑定
来源：http://lom.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kzt.aibaodan.cn

[S56] C++：optional
来源：http://ukc.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ngo.snrcjt.cn

[S57] C++：编译期常量
来源：http://uac.fengsongda.top

constexpr int N = 10;
来源：http://ahf.sweek.top

[S58] C++：命名空间
来源：http://sel.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://edq.zhengqikj.top

[S59] C++：静态断言
来源：http://eol.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fao.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://csa.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://btt.fanxiaobao.xyz

================================================================================
来源：http://xyk.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ieb.yangfankeji.com

================================================================================
来源：http://cix.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://llp.9152youxi.cn

println("Hello")
来源：http://pvp.yuxming.cn

[T02] Kotlin：变量
来源：http://qkn.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mab.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://zht.gaohongyu789.top

"值: $b"
来源：http://gll.jianghu66.top

[T04] Kotlin：空安全
来源：http://ftj.haohaochexian.top

val n: String? = null;  n?.length
来源：http://vfa.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://fov.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://csw.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://dfe.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lfn.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://zub.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://btn.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://bsy.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://csg.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://nkk.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://dal.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://bzd.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://doe.aibaodan.cn

[T11] Kotlin：协程
来源：http://mux.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jxg.birdmap.top

[T12] Kotlin：解构声明
来源：http://fis.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://xbt.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://tra.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://xkc.dashuyun.cn

[T14] Kotlin：循环
来源：http://cnn.iojbl.cn

for (i in 1..10) println(i)
来源：http://zix.jyoumei.cn

[T15] Kotlin：接口
来源：http://ati.cashguo.top

interface Shape { fun area(): Double }
来源：http://fgl.vqdsnc.cn

[T16] Swift：Hello World
来源：http://hcx.svipenyu.cn

print("Hello")
来源：http://cmz.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://jrl.xinyue.icu

var a = 1;  let b = 2
来源：http://ehk.jinqigufen.top

[T18] Swift：字符串插值
来源：http://zdh.gotoacloud.top

"值: \(b)"
来源：http://qkn.ehwqpu.com

[T19] Swift：可选绑定
来源：http://hyp.redwolf501.top

if let n = opt { print(n) }
来源：http://awt.shzxlz.cn

[T20] Swift：数组操作
来源：http://xjp.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://pod.cdnleiting.top

[T21] Swift：遍历
来源：http://ctu.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://qvr.meibo888.top

[T22] Swift：字典
来源：http://gjf.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lkk.yuanzhike.top

[T23] Swift：函数
来源：http://nqv.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jzu.jiagoushi.top

[T24] Swift：闭包
来源：http://fzg.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rin.xuanzx.com

[T25] Swift：结构体
来源：http://mib.sxryk.cn

struct P { var x: Int }
来源：http://ant.xziqi.cn

[T26] Swift：类与重写
来源：http://lus.nanxinkj.top

class A: Base { override func f() {} }
来源：http://lmh.vehdjk.com

[T27] Swift：错误处理
来源：http://cbk.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://gxs.ybcxt.top

[T28] Swift：枚举
来源：http://eft.daxiang520.top

enum Color { case red, green }
来源：http://djr.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://gfv.hcnkem.com

guard let x = opt else { return }
来源：http://phv.yangfankeji.com

[T30] Swift：协议
来源：http://qwl.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://piz.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://aab.wangdashe.top

print("Hello")
来源：http://ena.ivvv.top

[T32] Lua：局部变量
来源：http://ycd.yvedp.cn

local a = 1
来源：http://wao.zhengqikj.top

[T33] Lua：表（数组）
来源：http://ouq.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tzi.guowangkeji.top

[T34] Lua：遍历表
来源：http://pzw.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tbv.jiagoushi.top

[T35] Lua：字典表
来源：http://vgl.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://gcl.shuidangran.top

[T36] Lua：函数
来源：http://uul.hfpthk.cn

function add(a, b) return a + b end
来源：http://nyt.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://lvw.zhengqikj.top

"a" .. "b"
来源：http://idg.nanxinkj.top

[T38] Lua：条件
来源：http://cpz.aibaodan.cn

if x > 0 then print("正") end
来源：http://nax.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://seo.jinqigufen.top

string.find(s, "%d+")
来源：http://qts.xinyue.icu

[T40] Lua：元表
来源：http://paq.yfazqb.com

setmetatable({}, { __index = base })
来源：http://tnk.zhijiandao.cn

[T41] Perl：Hello World
来源：http://wdl.iojbl.cn

print "Hello\n";
来源：http://ebe.c1oappe.top

[T42] Perl：变量类型
来源：http://sji.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fyo.yj202588.top

[T43] Perl：字符串插值
来源：http://rgl.yuxming.cn

"值: $a"
来源：http://ljz.andypj.xyz

[T44] Perl：条件
来源：http://otr.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://hak.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://jzw.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://yfp.svipenyu.cn

[T46] Perl：哈希操作
来源：http://qxo.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hgj.jiagoushi.top

[T47] Perl：正则捕获
来源：http://ume.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://yky.hywenlv.cn

[T48] Perl：正则替换
来源：http://edy.tanke756.top

$s =~ s/old/new/g;
来源：http://nqx.zycfv.cn

[T49] Perl：函数
来源：http://vev.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qvc.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://owc.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fbd.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://yda.vehdjk.com

[T51] Scala：Hello World
来源：http://piz.bjfxy.top

println("Hello")
来源：http://sgs.hnqzz.top

[T52] Scala：变量
来源：http://upb.chenzaomai.com

val a = 1;  var b = 2
来源：http://irr.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://bxm.tian-w.cn

s"值: $b"
来源：http://zuo.zhengqikj.top

[T54] Scala：集合映射
来源：http://odz.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://pjl.xziqi.cn

[T55] Scala：集合过滤
来源：http://cki.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tqq.hysaishi.cn

[T56] Scala：样例类
来源：http://qlb.redwolf501.top

case class User(name: String, age: Int)
来源：http://hrs.hfpthk.cn

[T57] Scala：模式匹配
来源：http://xkz.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://lfa.ctjpmb.com

[T58] Scala：函数定义
来源：http://ckn.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://akr.kuanghao11.cn

[T59] Scala：循环
来源：http://crb.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://bvu.aibaodan.cn

[T60] Scala：折叠
来源：http://rne.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hbd.vehdjk.com

================================================================================
来源：http://ibz.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hyn.tanke756.top

================================================================================
来源：http://zxs.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://eop.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zpe.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://dsv.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://goo.ivvv.top

[U03] Py：加载 .env 配置
来源：http://ybw.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lkl.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://vmu.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wph.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://zvq.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://pvv.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://jqx.yongpay.top

{**a, **b}
来源：http://nsk.cheryme.top

[U07] Py：反转字典键值
来源：http://pkl.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://ghn.tian-w.cn

[U08] Py：展平二维列表
来源：http://nbi.ehwqpu.com

[y for x in nested for y in x]
来源：http://aeh.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://qud.zhijiandao.cn

max(d, key=d.get)
来源：http://tan.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://hdj.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://teu.yangfankeji.com

[U11] Py：生成器表达式
来源：http://eyq.ppjwa.cn

(x * 2 for x in arr)
来源：http://cql.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://czf.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://pxp.wangdashe.top

[U13] Py：固定长度队列
来源：http://hnz.cashguo.top

deque(maxlen=10)
来源：http://net.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://cly.yuanzhike.top

defaultdict(list)
来源：http://kte.sufxvd.cn

[U15] Py：高精度计时
来源：http://rlp.hesvh.cn

t = time.perf_counter()
来源：http://omp.mhx1999.top

[U16] Py：命令行参数解析
来源：http://zot.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tha.yanxiufei.cn

[U17] Py：初始化日志
来源：http://daz.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://dch.hammf.cn

[U18] Py：预编译正则
来源：http://ghy.yongpay.top

pat = re.compile(r"\d+")
来源：http://sie.tanke756.top

[U19] Py：正则替换带回调
来源：http://jyz.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aip.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://eyv.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://khe.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://htd.fehbvm.com

@contextlib.contextmanager
来源：http://mdg.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://kgx.cheryme.top

list(zip(*m))
来源：http://uwq.yueranfly.top

[U23] Py：分块读取大文件
来源：http://oie.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rwq.birdmap.top

[U24] Py：路径操作
来源：http://ais.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://apk.meibo888.top

[U25] Py：CSV 按字典读
来源：http://vmh.52xcode.cn

csv.DictReader(f)
来源：http://cde.bbcook.cn

[U26] Py：并发下载
来源：http://ifc.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qzf.yj20258.top

[U27] Py：异步 HTTP
来源：http://exr.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://wmn.jlsjyb.cn

[U28] Py：类型别名
来源：http://cvt.jinghuilouyu.cn

UserId = int
来源：http://pdb.vqdsnc.cn

[U29] Py：属性校验
来源：http://ave.xylfe.cn

@property 与 @x.setter 配合
来源：http://pry.ydjk.org.cn

[U30] Py：数据类
来源：http://vdf.guannengcc.top

@dataclass(slots=True)
来源：http://xtc.yueranfly.top

[U31] Py：单测
来源：http://blm.316326.xyz

python -m pytest -q
来源：http://lhe.xylfe.cn

[U32] Py：代码格式化
来源：http://qzb.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://oxr.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://oen.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://cby.jyoumei.cn

[U34] Py：判断编码
来源：http://xio.hfpthk.cn

chardet.detect(raw)
来源：http://bni.gogol.net.cn

[U35] Py：发送邮件
来源：http://chh.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ijo.ydjk.org.cn

[U36] Py：定时任务
来源：http://ndp.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://jko.nwbrower.top

[U37] Py：读写 Excel
来源：http://mor.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bcc.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://zep.sysykeji.top

Path(__file__).resolve().parent
来源：http://ojb.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://ywc.hongshengwenyu.top

sys.stdout.isatty()
来源：http://wkd.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://fqy.yj20258888.top

print("err", file=sys.stderr)
来源：http://hsj.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://eqy.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://aps.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://lvd.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://arz.iojbl.cn

[U43] PHP：声明命名空间
来源：http://hgy.shzxlz.cn

namespace App\Http;
来源：http://syi.yfazqb.com

[U44] PHP：开启严格类型
来源：http://xqv.hywenlv.cn

declare(strict_types=1);
来源：http://zte.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://cnd.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gll.cucudq.cn

[U46] PHP：可空类型
来源：http://tfm.nanxuanxn.top

?string $name = null
来源：http://zqt.xuanzx.com

[U47] PHP：联合类型
来源：http://xqt.chenlongwang.top

int|string $id
来源：http://nvf.guannengcc.top

[U48] PHP：纯枚举
来源：http://dsf.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zrj.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://nxd.jinghuilouyu.cn

public readonly string $name
来源：http://pot.ivvv.top

[U50] PHP：构造器属性提升
来源：http://qzh.aizwys.cn

public function __construct(private int $id) {}
来源：http://pme.bjfxy.top

[U51] PHP：数组解构
来源：http://pmw.zhijiandao.cn

[$a, $b] = $arr;
来源：http://lxw.sysykeji.top

[U52] PHP：箭头函数
来源：http://edd.yonumen.top

$double = fn($x) => $x * 2;
来源：http://pjw.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://icw.haohaochexian.top

$v = $a ?? $b ?? "default";
来源：http://swj.9152youxi.cn

[U54] PHP：空安全调用
来源：http://avs.xziqi.cn

$obj?->method()
来源：http://doj.yueranfly.top

[U55] PHP：match 表达式
来源：http://utp.kuanghao11.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uuk.snrcjt.cn

[U56] PHP：命名参数
来源：http://gen.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://rlq.hcnkem.com

[U57] PHP：字符串插值
来源：http://ffq.yonumen.top

"值: {$a}"
来源：http://wnh.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://hai.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jdi.bbcook.cn

[U59] PHP：自定义排序
来源：http://aii.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://slv.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://bbh.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rkg.vqdsnc.cn


<!-- 参考信息 -->