代发 wailian999

[S33] C++：vector 增删
来源：http://yfv.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mcv.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://uod.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://zxd.hammf.cn

[S35] C++：map
来源：http://tme.hesvh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jkt.jyoumei.cn

[S36] C++：unordered_map
来源：http://unb.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ioa.zdbjq.cn

[S37] C++：set
来源：http://qod.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rzm.gotoacloud.top

[S38] C++：排序
来源：http://ykz.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://esu.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://kzt.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kpf.nwbrower.top

[S40] C++：查找元素
来源：http://isx.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ybj.ctjpmb.com

[S41] C++：类与构造函数
来源：http://otm.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hvs.bjfxy.top

[S42] C++：继承与虚函数
来源：http://yqr.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://bti.sweek.top

[S43] C++：智能指针
来源：http://tbc.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://wvx.zhijiandao.cn

[S44] C++：引用传参
来源：http://ngq.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://osk.cheryme.top

[S45] C++：lambda
来源：http://vbr.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://epe.chenlongwang.top

[S46] C++：函数模板
来源：http://kfk.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zht.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://zkr.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fur.jyoumei.cn

[S48] C++：逐行读文件
来源：http://uhf.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jkp.jianghu66.top

while (std::getline(in, line)) { }
来源：http://axo.sysykeji.top

[S49] C++：写文件
来源：http://ctj.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mjs.gogol.net.cn

[S50] C++：格式化数字
来源：http://aet.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ttx.svipenyu.cn

[S51] C++：显式类型转换
来源：http://dkt.yueranfly.top

static_cast<double>(a) / b
来源：http://bas.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://cgf.sweek.top

int size() const noexcept { return n_; }
来源：http://pij.sjlbkw.cn

[S53] C++：移动语义
来源：http://fin.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://tzq.aibaodan.cn

[S54] C++：异常处理
来源：http://xdd.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ptn.zhixingplan.top

[S55] C++：结构化绑定
来源：http://qya.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eew.vehdjk.com

[S56] C++：optional
来源：http://ekp.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ull.zhengqikj.top

[S57] C++：编译期常量
来源：http://dnq.haohaochexian.top

constexpr int N = 10;
来源：http://ihz.gzhubu.top

[S58] C++：命名空间
来源：http://ovp.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://yil.redwolf501.top

[S59] C++：静态断言
来源：http://duu.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qiy.uphjek.com

[S60] C++：遍历并删除元素
来源：http://amh.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ihx.jinghuilouyu.cn

================================================================================
来源：http://gtc.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rdh.hfpthk.cn

================================================================================
来源：http://xkn.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://zkl.pycfn.com

println("Hello")
来源：http://pyf.kuanghao11.cn

[T02] Kotlin：变量
来源：http://tby.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uqb.cashguo.top

[T03] Kotlin：字符串模板
来源：http://mbl.guannengcc.top

"值: $b"
来源：http://wly.zdbjq.cn

[T04] Kotlin：空安全
来源：http://pje.hcnkem.com

val n: String? = null;  n?.length
来源：http://urd.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://frw.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://evn.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://cbc.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aef.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://bvm.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jsl.0kj1m.cn

[T08] Kotlin：数据类
来源：http://uha.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://tmp.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://opw.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://vlh.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://vac.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bdk.0kj1m.cn

[T11] Kotlin：协程
来源：http://kwi.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://dnm.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://kgt.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://tue.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://oza.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://ddt.xziqi.cn

[T14] Kotlin：循环
来源：http://zwv.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://hjq.jianghu66.top

[T15] Kotlin：接口
来源：http://nnh.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://bms.smart0.xyz

[T16] Swift：Hello World
来源：http://xwa.ywan-chungtsiang.top

print("Hello")
来源：http://zaq.guowangkeji.top

[T17] Swift：变量与常量
来源：http://tcn.vehdjk.com

var a = 1;  let b = 2
来源：http://prx.cheryme.top

[T18] Swift：字符串插值
来源：http://dqr.jiagoushi.top

"值: \(b)"
来源：http://vyj.havefunace.top

[T19] Swift：可选绑定
来源：http://azr.yueranfly.top

if let n = opt { print(n) }
来源：http://bxx.jianghu66.top

[T20] Swift：数组操作
来源：http://cif.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qph.fehbvm.com

[T21] Swift：遍历
来源：http://rvi.jinghuilouyu.cn

for x in a { print(x) }
来源：http://sei.mhx1999.top

[T22] Swift：字典
来源：http://abe.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://foy.yongpay.top

[T23] Swift：函数
来源：http://yol.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cme.hesvh.cn

[T24] Swift：闭包
来源：http://qnr.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://svf.0kj1m.cn

[T25] Swift：结构体
来源：http://pjy.zhengqikj.top

struct P { var x: Int }
来源：http://uqe.jlsjyb.cn

[T26] Swift：类与重写
来源：http://rsc.cashguo.top

class A: Base { override func f() {} }
来源：http://fmc.cheryme.top

[T27] Swift：错误处理
来源：http://eua.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://vbw.snrcjt.cn

[T28] Swift：枚举
来源：http://imr.hongshengwenyu.top

enum Color { case red, green }
来源：http://sgl.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://wng.gogol.net.cn

guard let x = opt else { return }
来源：http://voi.epnwcf.com

[T30] Swift：协议
来源：http://hey.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://ajf.chenlongwang.top

[T31] Lua：Hello World
来源：http://fyi.yj20258888.top

print("Hello")
来源：http://gro.cdnleiting.top

[T32] Lua：局部变量
来源：http://aay.vqdsnc.cn

local a = 1
来源：http://lod.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://zeh.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://blk.jinqigufen.top

[T34] Lua：遍历表
来源：http://uaw.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://auo.316326.xyz

[T35] Lua：字典表
来源：http://isb.wangdashe.top

local d = { a = 1 };  d.b = 2
来源：http://yml.fanxiaobao.xyz

[T36] Lua：函数
来源：http://gcl.yuxming.cn

function add(a, b) return a + b end
来源：http://aeu.cucudq.cn

[T37] Lua：字符串拼接
来源：http://efy.hfpthk.cn

"a" .. "b"
来源：http://dpa.sjlbkw.cn

[T38] Lua：条件
来源：http://dic.gzhubu.top

if x > 0 then print("正") end
来源：http://ces.jiagoushi.top

[T39] Lua：模式匹配
来源：http://stx.zhiwuduotai.top

string.find(s, "%d+")
来源：http://eed.sxryk.cn

[T40] Lua：元表
来源：http://cxr.cucudq.cn

setmetatable({}, { __index = base })
来源：http://ius.hnqzz.top

[T41] Perl：Hello World
来源：http://gaj.zhaomingkeji.xyz

print "Hello\n";
来源：http://rhq.andypj.xyz

[T42] Perl：变量类型
来源：http://yxo.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hid.316326.xyz

[T43] Perl：字符串插值
来源：http://btw.mhx1999.top

"值: $a"
来源：http://kcp.mhx1999.top

[T44] Perl：条件
来源：http://ngi.meibo888.top

if ($a > 0) { print "正"; }
来源：http://fxl.guannengcc.top

[T45] Perl：数组遍历
来源：http://vtu.meibo888.top

for my $x (@arr) { print $x; }
来源：http://eia.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://cob.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sto.tian-w.cn

[T47] Perl：正则捕获
来源：http://chd.xylfe.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mpk.snrcjt.cn

[T48] Perl：正则替换
来源：http://mvo.tianlin.xyz

$s =~ s/old/new/g;
来源：http://wxz.aizwys.cn

[T49] Perl：函数
来源：http://bsp.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dbh.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://stq.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://khh.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://kve.chenlongwang.top

[T51] Scala：Hello World
来源：http://vmu.fengsongda.top

println("Hello")
来源：http://whu.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://jiq.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://mvm.hnqzz.top

[T53] Scala：字符串插值
来源：http://ijl.yangfankeji.com

s"值: $b"
来源：http://ack.yangfankeji.com

[T54] Scala：集合映射
来源：http://pgl.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://izs.ctjpmb.com

[T55] Scala：集合过滤
来源：http://oiu.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://gdn.bbcook.cn

[T56] Scala：样例类
来源：http://wxv.xinyue.icu

case class User(name: String, age: Int)
来源：http://hky.epnwcf.com

[T57] Scala：模式匹配
来源：http://zbr.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://msb.smart0.xyz

[T58] Scala：函数定义
来源：http://huc.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wfw.yuanzhike.top

[T59] Scala：循环
来源：http://zuj.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://vss.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://fbh.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cic.daxiang520.top

================================================================================
来源：http://aaz.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mdv.ydzc1.top

================================================================================
来源：http://cjg.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://zcn.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://wvr.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://rfh.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zkc.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://hzn.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dma.cdnleiting.top

[U04] Py：变量调试打印
来源：http://pes.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rwb.meibo888.top

[U05] Py：列表去重且保序
来源：http://huz.wangdashe.top

list(dict.fromkeys(arr))
来源：http://fae.fzhhl.top

[U06] Py：合并两个字典
来源：http://rxd.xylfe.cn

{**a, **b}
来源：http://urj.tianlin.xyz

[U07] Py：反转字典键值
来源：http://vnh.nwbrower.top

{v: k for k, v in d.items()}
来源：http://hfv.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://sut.tian-w.cn

[y for x in nested for y in x]
来源：http://hoq.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://ftc.yuxming.cn

max(d, key=d.get)
来源：http://wur.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://hgw.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bup.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://ana.shzxlz.cn

(x * 2 for x in arr)
来源：http://fen.sxryk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lnk.zycfv.cn

Counter(arr).most_common(3)
来源：http://eng.shuidangran.top

[U13] Py：固定长度队列
来源：http://psz.zhiwuduotai.top

deque(maxlen=10)
来源：http://qfa.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://hnn.jyoumei.cn

defaultdict(list)
来源：http://hrd.jianghu66.top

[U15] Py：高精度计时
来源：http://jce.jqgufenzy.top

t = time.perf_counter()
来源：http://vxm.mhx1999.top

[U16] Py：命令行参数解析
来源：http://pup.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gwc.tianlin.xyz

[U17] Py：初始化日志
来源：http://lvz.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://req.9152youxi.cn

[U18] Py：预编译正则
来源：http://eld.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://eyp.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://aan.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cgu.ivvv.top

[U20] Py：缓存函数结果
来源：http://dly.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://sju.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://iua.yj202588.top

@contextlib.contextmanager
来源：http://vhh.shuidangran.top

[U22] Py：矩阵转置
来源：http://fzc.gaohongyu789.top

list(zip(*m))
来源：http://evi.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://wgf.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://exo.epnwcf.com

[U24] Py：路径操作
来源：http://hzw.gogol.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://muf.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://guq.yangfankeji.com

csv.DictReader(f)
来源：http://weq.52xcode.cn

[U26] Py：并发下载
来源：http://wuj.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tie.redwolf501.top

[U27] Py：异步 HTTP
来源：http://dpc.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://lwc.shzxlz.cn

[U28] Py：类型别名
来源：http://nzz.ydjk.org.cn

UserId = int
来源：http://xty.zhijiandao.cn

[U29] Py：属性校验
来源：http://lxv.smart0.xyz

@property 与 @x.setter 配合
来源：http://cpd.uphjek.com

[U30] Py：数据类
来源：http://uay.c1oappe.top

@dataclass(slots=True)
来源：http://pvc.meibo888.top

[U31] Py：单测
来源：http://gra.52xcode.cn

python -m pytest -q
来源：http://vkv.ivvv.top

[U32] Py：代码格式化
来源：http://lkx.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://dtc.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://zsb.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://uda.shangyingyoupin.top

[U34] Py：判断编码
来源：http://jst.0kj1m.cn

chardet.detect(raw)
来源：http://vre.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://whg.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://egy.gaohongyu789.top

[U36] Py：定时任务
来源：http://zex.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://lui.yj20258.top

[U37] Py：读写 Excel
来源：http://vzx.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://coq.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://aqm.jianghu66.top

Path(__file__).resolve().parent
来源：http://zfx.sweek.top

[U39] Py：判断是否在交互环境
来源：http://sxb.fehbvm.com

sys.stdout.isatty()
来源：http://shx.bjfxy.top

[U40] Py：打印到标准错误
来源：http://dxk.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://mra.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://qdm.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://brx.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://kau.guannengcc.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ptw.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://hlf.snrcjt.cn

namespace App\Http;
来源：http://cek.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://qat.hywenlv.cn

declare(strict_types=1);
来源：http://qzg.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://jgx.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://egd.zhoulong.xyz

[U46] PHP：可空类型
来源：http://mia.yanxiufei.cn

?string $name = null
来源：http://pjs.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://qjh.xingfuxueyuan.xyz

int|string $id
来源：http://joq.wangdashe.top

[U48] PHP：纯枚举
来源：http://kic.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tqo.cdnleiting.top

[U49] PHP：只读属性
来源：http://adt.birdmap.top

public readonly string $name
来源：http://qsh.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://oij.xylfe.cn

public function __construct(private int $id) {}
来源：http://cqx.zdqjudy.top

[U51] PHP：数组解构
来源：http://cdz.jinqigufen.top

[$a, $b] = $arr;
来源：http://xoe.hnqzz.top

[U52] PHP：箭头函数
来源：http://lqr.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://vww.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://iye.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://eed.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://rqc.vqdsnc.cn

$obj?->method()
来源：http://shr.tanke756.top

[U55] PHP：match 表达式
来源：http://ndb.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wyk.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://imy.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://eaj.cheryme.top

[U57] PHP：字符串插值
来源：http://gdt.ybcxt.top

"值: {$a}"
来源：http://dxz.ybcxt.top

[U58] PHP：数组三件套
来源：http://maq.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ddc.zdbjq.cn


<!-- 参考信息 -->