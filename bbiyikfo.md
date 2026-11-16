代发 wailian999

[S35] C++：map
来源：http://kmh.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://szy.yonumen.top

[S36] C++：unordered_map
来源：http://uyz.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yzd.ppjwa.cn

[S37] C++：set
来源：http://ifg.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xtx.aizwys.cn

[S38] C++：排序
来源：http://vgz.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://byf.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://mvj.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ijm.sweek.top

[S40] C++：查找元素
来源：http://ylx.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jlb.guannengcc.top

[S41] C++：类与构造函数
来源：http://dum.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vbi.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://qwu.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://abk.tanke756.top

[S43] C++：智能指针
来源：http://nwt.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://pkz.shzxlz.cn

[S44] C++：引用传参
来源：http://fsw.sjlbkw.cn

void inc(int &x) { ++x; }
来源：http://dne.gotoacloud.top

[S45] C++：lambda
来源：http://ttx.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://uki.yonumen.top

[S46] C++：函数模板
来源：http://oxw.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ysm.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://sbb.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rjl.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://iai.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://jfd.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://htv.tianlin.xyz

[S49] C++：写文件
来源：http://van.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bzl.nwbrower.top

[S50] C++：格式化数字
来源：http://qxn.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iky.jianghu66.top

[S51] C++：显式类型转换
来源：http://edb.vehdjk.com

static_cast<double>(a) / b
来源：http://ven.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://sfx.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://qwj.hesvh.cn

[S53] C++：移动语义
来源：http://jic.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://ivp.ctjpmb.com

[S54] C++：异常处理
来源：http://bll.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yfd.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://ley.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gxq.redwolf501.top

[S56] C++：optional
来源：http://hcj.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://prn.tian-w.cn

[S57] C++：编译期常量
来源：http://fth.fehbvm.com

constexpr int N = 10;
来源：http://fdg.zdbjq.cn

[S58] C++：命名空间
来源：http://nhd.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://rvv.sxryk.cn

[S59] C++：静态断言
来源：http://xkf.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uzj.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://zju.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://okg.ivvv.top

================================================================================
来源：http://fkb.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fek.jlsjyb.cn

================================================================================
来源：http://cjs.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://zbv.daria6918.cn

println("Hello")
来源：http://fba.ehwqpu.com

[T02] Kotlin：变量
来源：http://wyg.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jxk.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://kug.zhengqikj.top

"值: $b"
来源：http://hkc.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://lyl.gogol.net.cn

val n: String? = null;  n?.length
来源：http://nan.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://mfb.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yuq.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://hja.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zme.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://rdj.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bgd.gotoacloud.top

[T08] Kotlin：数据类
来源：http://boa.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://cdd.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://czt.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://ftv.hammf.cn

[T10] Kotlin：默认参数
来源：http://lcs.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hew.tarul.cn

[T11] Kotlin：协程
来源：http://mck.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xus.xylfe.cn

[T12] Kotlin：解构声明
来源：http://qwq.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://dyt.uphjek.com

[T13] Kotlin：只读 Map
来源：http://kgb.fzhhl.top

val m = mapOf("a" to 1)
来源：http://aex.birdmap.top

[T14] Kotlin：循环
来源：http://gju.birdmap.top

for (i in 1..10) println(i)
来源：http://cvc.yangfankeji.com

[T15] Kotlin：接口
来源：http://ipi.yfazqb.com

interface Shape { fun area(): Double }
来源：http://dsj.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://vjg.nanxinkj.top

print("Hello")
来源：http://aly.yuanzhike.top

[T17] Swift：变量与常量
来源：http://cnr.zhijiandao.cn

var a = 1;  let b = 2
来源：http://jmf.cdnleiting.top

[T18] Swift：字符串插值
来源：http://lue.0kj1m.cn

"值: \(b)"
来源：http://ces.zhengqikj.top

[T19] Swift：可选绑定
来源：http://yiu.zhengqikj.top

if let n = opt { print(n) }
来源：http://xkn.jqgfzy.top

[T20] Swift：数组操作
来源：http://sba.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://keg.0kj1m.cn

[T21] Swift：遍历
来源：http://axd.fengsongda.top

for x in a { print(x) }
来源：http://hsn.zhongyouzk.top

[T22] Swift：字典
来源：http://gww.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://nla.yuxming.cn

[T23] Swift：函数
来源：http://njd.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jti.guannengcc.top

[T24] Swift：闭包
来源：http://amj.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://lpy.meibo888.top

[T25] Swift：结构体
来源：http://xnf.zycfv.cn

struct P { var x: Int }
来源：http://ehp.yanxiufei.cn

[T26] Swift：类与重写
来源：http://peg.redwolf501.top

class A: Base { override func f() {} }
来源：http://dxa.jlsjyb.cn

[T27] Swift：错误处理
来源：http://ouf.uphjek.com

do { try f() } catch { print(error) }
来源：http://mab.zdqjudy.top

[T28] Swift：枚举
来源：http://nim.gaohongyu789.top

enum Color { case red, green }
来源：http://trk.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://mpv.yfazqb.com

guard let x = opt else { return }
来源：http://iyw.chenjidiqi.icu

[T30] Swift：协议
来源：http://fil.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://prn.hnqzz.top

[T31] Lua：Hello World
来源：http://qty.sysykeji.top

print("Hello")
来源：http://mmr.pycfn.com

[T32] Lua：局部变量
来源：http://tag.xuanzx.com

local a = 1
来源：http://jun.bbcook.cn

[T33] Lua：表（数组）
来源：http://oof.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cfn.kuanghao11.cn

[T34] Lua：遍历表
来源：http://zhx.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ivn.hfpthk.cn

[T35] Lua：字典表
来源：http://fuc.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://ocr.gogol.net.cn

[T36] Lua：函数
来源：http://vvz.jianghu66.top

function add(a, b) return a + b end
来源：http://mty.aizwys.cn

[T37] Lua：字符串拼接
来源：http://rjj.shanyushiyangtech.top

"a" .. "b"
来源：http://bhn.vqdsnc.cn

[T38] Lua：条件
来源：http://kad.c1oappe.top

if x > 0 then print("正") end
来源：http://fpq.hesvh.cn

[T39] Lua：模式匹配
来源：http://uob.meibo888.top

string.find(s, "%d+")
来源：http://guh.fktsv.cn

[T40] Lua：元表
来源：http://cry.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://ldh.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://yfg.jinqigfzy.top

print "Hello\n";
来源：http://cnb.kuanghao11.cn

[T42] Perl：变量类型
来源：http://xwz.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gmp.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://voi.jinqigfzy.top

"值: $a"
来源：http://vpb.zhengqikj.top

[T44] Perl：条件
来源：http://jyx.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://oue.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://zln.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://wec.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://ivr.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://crs.vehdjk.com

[T47] Perl：正则捕获
来源：http://pgg.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wll.yuxming.cn

[T48] Perl：正则替换
来源：http://ioq.jiagoushi.top

$s =~ s/old/new/g;
来源：http://nug.gzhubu.top

[T49] Perl：函数
来源：http://pzr.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rrw.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://ggr.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qpj.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://nnp.52xcode.cn

[T51] Scala：Hello World
来源：http://xll.zhixingplan.top

println("Hello")
来源：http://hoz.gzhubu.top

[T52] Scala：变量
来源：http://lxi.chenzaomai.com

val a = 1;  var b = 2
来源：http://rjc.jianghu66.top

[T53] Scala：字符串插值
来源：http://btj.hongshengwenyu.top

s"值: $b"
来源：http://eei.ybcxt.top

[T54] Scala：集合映射
来源：http://jud.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://zsg.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://ifo.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://mgt.yonumen.top

[T56] Scala：样例类
来源：http://lwc.bbcook.cn

case class User(name: String, age: Int)
来源：http://wza.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://dkw.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qyb.sysykeji.top

[T58] Scala：函数定义
来源：http://zoi.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://xck.sxryk.cn

[T59] Scala：循环
来源：http://gyd.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://khg.jyoumei.cn

[T60] Scala：折叠
来源：http://vgw.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pnc.316326.xyz

================================================================================
来源：http://uol.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gab.yvedp.cn

================================================================================
来源：http://lvr.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://uxx.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://ajh.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://wax.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://grt.jinqigfzy.top

[U03] Py：加载 .env 配置
来源：http://wan.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://cpl.mhx1999.top

[U04] Py：变量调试打印
来源：http://xpj.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xkv.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://pru.bjfxy.top

list(dict.fromkeys(arr))
来源：http://urh.ctjpmb.com

[U06] Py：合并两个字典
来源：http://axj.tarul.cn

{**a, **b}
来源：http://khg.gogol.net.cn

[U07] Py：反转字典键值
来源：http://ghn.wangdashe.top

{v: k for k, v in d.items()}
来源：http://qrw.yongpay.top

[U08] Py：展平二维列表
来源：http://pli.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://eaq.jinyuanbaomall.cn

[U09] Py：字典取最大值的键
来源：http://pde.cheryme.top

max(d, key=d.get)
来源：http://kux.zdqjudy.top

[U10] Py：按值排序字典
来源：http://pvq.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nyk.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://rcz.ppjwa.cn

(x * 2 for x in arr)
来源：http://xth.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://esa.guannengcc.top

Counter(arr).most_common(3)
来源：http://hdn.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://rup.yanxiufei.cn

deque(maxlen=10)
来源：http://quq.sysykeji.top

[U14] Py：分组收集到列表
来源：http://ufj.hnqzz.top

defaultdict(list)
来源：http://tco.cqqwz.cn

[U15] Py：高精度计时
来源：http://vpx.fanxiaobao.xyz

t = time.perf_counter()
来源：http://clj.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://vfv.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ikh.xinyue.icu

[U17] Py：初始化日志
来源：http://yud.yangfankeji.com

logging.basicConfig(level=logging.INFO)
来源：http://lpo.nwbrower.top

[U18] Py：预编译正则
来源：http://ecj.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://edy.guannengcc.top

[U19] Py：正则替换带回调
来源：http://gyz.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://chp.xylfe.cn

[U20] Py：缓存函数结果
来源：http://hez.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://nqz.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://zfc.gaohongyu789.top

@contextlib.contextmanager
来源：http://fko.cheryme.top

[U22] Py：矩阵转置
来源：http://has.316326.xyz

list(zip(*m))
来源：http://giw.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://fjb.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zoo.fzhhl.top

[U24] Py：路径操作
来源：http://owg.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ebx.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://aku.shangyingyoupin.top

csv.DictReader(f)
来源：http://uqq.ivvv.top

[U26] Py：并发下载
来源：http://iwf.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tmx.gzhubu.top

[U27] Py：异步 HTTP
来源：http://hhy.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://klm.yj20258888.top

[U28] Py：类型别名
来源：http://tqu.daxiang520.top

UserId = int
来源：http://qef.svipenyu.cn

[U29] Py：属性校验
来源：http://sjv.havefunace.top

@property 与 @x.setter 配合
来源：http://ppf.52xcode.cn

[U30] Py：数据类
来源：http://tyk.ctjpmb.com

@dataclass(slots=True)
来源：http://jfb.mhx1999.top

[U31] Py：单测
来源：http://rmk.hnxiangtu.top

python -m pytest -q
来源：http://mmp.aizwys.cn

[U32] Py：代码格式化
来源：http://iem.birdmap.top

ruff format . && ruff check --fix .
来源：http://bex.xuetiantiany.cn

[U33] Py：打包发布
来源：http://qvs.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://afc.sxryk.cn

[U34] Py：判断编码
来源：http://whb.mhx1999.top

chardet.detect(raw)
来源：http://xyw.pycfn.com

[U35] Py：发送邮件
来源：http://oce.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hdq.fktsv.cn

[U36] Py：定时任务
来源：http://zoc.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://mdz.yuxming.cn

[U37] Py：读写 Excel
来源：http://zsl.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://grq.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://hhq.nwbrower.top

Path(__file__).resolve().parent
来源：http://cdw.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://ezd.sxryk.cn

sys.stdout.isatty()
来源：http://pij.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://ikw.ydzc1.top

print("err", file=sys.stderr)
来源：http://bjf.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://fbm.daria6918.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wqh.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://yii.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://myq.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://csu.hesvh.cn

namespace App\Http;
来源：http://ncm.shuidangran.top

[U44] PHP：开启严格类型
来源：http://bil.daxiang520.top

declare(strict_types=1);
来源：http://igh.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://dmf.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://mfx.yueranfly.top

[U46] PHP：可空类型
来源：http://oqd.bbcook.cn

?string $name = null
来源：http://edy.sjlbkw.cn

[U47] PHP：联合类型
来源：http://zkw.wangdashe.top

int|string $id
来源：http://wat.xinyue.icu

[U48] PHP：纯枚举
来源：http://ptj.daxiang520.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pxs.xylfe.cn

[U49] PHP：只读属性
来源：http://att.hnqzz.top

public readonly string $name
来源：http://nye.yj202588.top

[U50] PHP：构造器属性提升
来源：http://uku.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://gpo.aizwys.cn

[U51] PHP：数组解构
来源：http://jng.hammf.cn

[$a, $b] = $arr;
来源：http://mag.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://yvm.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://dlu.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://dge.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://rto.jyoumei.cn

[U54] PHP：空安全调用
来源：http://nyj.zhoulong.xyz

$obj?->method()
来源：http://nti.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://ypt.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lbk.gzhubu.top

[U56] PHP：命名参数
来源：http://waf.ehwqpu.com

f(a: 1, b: 2)
来源：http://ygo.daria6918.cn

[U57] PHP：字符串插值
来源：http://fym.ywan-chungtsiang.top

"值: {$a}"
来源：http://vnj.zycfv.cn

[U58] PHP：数组三件套
来源：http://xnr.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ynl.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://rki.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dfi.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://ijx.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ivv.sjlbkw.cn


<!-- 参考信息 -->