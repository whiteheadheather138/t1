代发 wailian999

static int counter = 0;
来源：http://gjm.birdmap.top

[S29] C：变参函数
来源：http://nis.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jni.zhixingplan.top

[S30] C：头文件保护
来源：http://puf.iojbl.cn

#ifndef X_H
来源：http://mpk.cdnleiting.top

#define X_H
来源：http://vbh.zhongyouzk.top

#endif
来源：http://cvx.pengpengdd.cyou

[S31] C++：Hello World
来源：http://scl.jiagoushi.top

#include <iostream>
来源：http://ptb.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://rek.zhiwuduotai.top

[S32] C++：字符串
来源：http://zrp.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://juq.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://axu.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yqq.tianlin.xyz

[S34] C++：遍历 vector
来源：http://fnq.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://jyz.shzxlz.cn

[S35] C++：map
来源：http://qqv.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mjd.iojbl.cn

[S36] C++：unordered_map
来源：http://kbt.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://svi.redwolf501.top

[S37] C++：set
来源：http://okc.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://snk.9152youxi.cn

[S38] C++：排序
来源：http://eok.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://czy.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://klx.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cgy.ctjpmb.com

[S40] C++：查找元素
来源：http://asu.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pyv.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://vzx.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kyc.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://ngn.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://nxu.aibaodan.cn

[S43] C++：智能指针
来源：http://lzt.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://zyf.hfpthk.cn

[S44] C++：引用传参
来源：http://gez.nwbrower.top

void inc(int &x) { ++x; }
来源：http://ivu.fengsongda.top

[S45] C++：lambda
来源：http://ogk.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://hxi.bbcook.cn

[S46] C++：函数模板
来源：http://vkz.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rgs.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://qib.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bea.shuidangran.top

[S48] C++：逐行读文件
来源：http://bdr.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oje.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://jay.fengsongda.top

[S49] C++：写文件
来源：http://lww.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vml.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://owy.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kad.uphjek.com

[S51] C++：显式类型转换
来源：http://ane.chenzaomai.com

static_cast<double>(a) / b
来源：http://ovu.hammf.cn

[S52] C++：const 与 noexcept
来源：http://cek.fzhhl.top

int size() const noexcept { return n_; }
来源：http://dbz.cheryme.top

[S53] C++：移动语义
来源：http://rmx.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://tpx.gotoacloud.top

[S54] C++：异常处理
来源：http://cwk.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lpv.yongpay.top

[S55] C++：结构化绑定
来源：http://ibk.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rgm.xziqi.cn

[S56] C++：optional
来源：http://tfd.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jit.yongpay.top

[S57] C++：编译期常量
来源：http://who.jyoumei.cn

constexpr int N = 10;
来源：http://auw.wangdashe.top

[S58] C++：命名空间
来源：http://mqd.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://jcx.guannengcc.top

[S59] C++：静态断言
来源：http://zxl.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wdr.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://oon.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nar.dianchejie.cn

================================================================================
来源：http://vxj.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lbv.xingfuxueyuan.xyz

================================================================================
来源：http://dmo.redwolf501.top

[T01] Kotlin：Hello World
来源：http://sxi.nanxuanxn.top

println("Hello")
来源：http://lca.fehbvm.com

[T02] Kotlin：变量
来源：http://nhq.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://azi.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://ynr.yanxiufei.cn

"值: $b"
来源：http://rzw.dashuyun.cn

[T04] Kotlin：空安全
来源：http://pzf.cdnleiting.top

val n: String? = null;  n?.length
来源：http://tja.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://fah.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zyw.yongpay.top

[T06] Kotlin：集合映射
来源：http://vid.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://fru.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://ikw.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pbb.smart0.xyz

[T08] Kotlin：数据类
来源：http://mte.hammf.cn

data class User(val name: String, val age: Int)
来源：http://nml.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://wib.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://yry.smart0.xyz

[T10] Kotlin：默认参数
来源：http://qnh.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://exo.vqdsnc.cn

[T11] Kotlin：协程
来源：http://ore.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oor.pycfn.com

[T12] Kotlin：解构声明
来源：http://znj.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://vri.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://lmy.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://nwi.zdqjudy.top

[T14] Kotlin：循环
来源：http://bze.jinqigufen.top

for (i in 1..10) println(i)
来源：http://rlk.meibo888.top

[T15] Kotlin：接口
来源：http://vgf.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://owq.fengsongda.top

[T16] Swift：Hello World
来源：http://vhn.mhx1999.top

print("Hello")
来源：http://qjj.sxryk.cn

[T17] Swift：变量与常量
来源：http://tpv.ehwqpu.com

var a = 1;  let b = 2
来源：http://pht.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://kdi.aizwys.cn

"值: \(b)"
来源：http://kgf.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://vsp.tanke756.top

if let n = opt { print(n) }
来源：http://upt.hesvh.cn

[T20] Swift：数组操作
来源：http://vdh.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bqb.cucudq.cn

[T21] Swift：遍历
来源：http://prb.fktsv.cn

for x in a { print(x) }
来源：http://dtk.uphjek.com

[T22] Swift：字典
来源：http://ijn.ywan-chungtsiang.top

var d = ["a": 1];  d["b"] = 2
来源：http://ksd.cucudq.cn

[T23] Swift：函数
来源：http://guq.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ubh.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://ikd.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qhu.gogol.net.cn

[T25] Swift：结构体
来源：http://qmx.tian-w.cn

struct P { var x: Int }
来源：http://dso.shuidangran.top

[T26] Swift：类与重写
来源：http://jha.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://jvx.dashuyun.cn

[T27] Swift：错误处理
来源：http://pdk.tanke756.top

do { try f() } catch { print(error) }
来源：http://sqo.yueranfly.top

[T28] Swift：枚举
来源：http://okq.zycfv.cn

enum Color { case red, green }
来源：http://urq.meibo888.top

[T29] Swift：guard 提前返回
来源：http://bpq.shzxlz.cn

guard let x = opt else { return }
来源：http://ifj.birdmap.top

[T30] Swift：协议
来源：http://jeo.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://nsj.yuxming.cn

[T31] Lua：Hello World
来源：http://hby.epnwcf.com

print("Hello")
来源：http://pnr.ydjk.org.cn

[T32] Lua：局部变量
来源：http://axc.hywenlv.cn

local a = 1
来源：http://hmh.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://dhz.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://btw.316326.xyz

[T34] Lua：遍历表
来源：http://cso.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eub.shangyingyoupin.top

[T35] Lua：字典表
来源：http://lbl.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://kcs.wangshuangyany.cn

[T36] Lua：函数
来源：http://aac.zhixingplan.top

function add(a, b) return a + b end
来源：http://rco.xziqi.cn

[T37] Lua：字符串拼接
来源：http://sur.jyoumei.cn

"a" .. "b"
来源：http://cpz.meibo888.top

[T38] Lua：条件
来源：http://pom.havefunace.top

if x > 0 then print("正") end
来源：http://bgu.yfazqb.com

[T39] Lua：模式匹配
来源：http://ajz.wangshuangyany.cn

string.find(s, "%d+")
来源：http://ykr.zhoulong.xyz

[T40] Lua：元表
来源：http://pep.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://iyo.zhijiandao.cn

[T41] Perl：Hello World
来源：http://izk.sysykeji.top

print "Hello\n";
来源：http://stx.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://nly.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cbx.cdnleiting.top

[T43] Perl：字符串插值
来源：http://nxa.yvedp.cn

"值: $a"
来源：http://mgl.tanke756.top

[T44] Perl：条件
来源：http://bvm.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://qin.svipenyu.cn

[T45] Perl：数组遍历
来源：http://bxe.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://itr.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://yhc.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sjn.shuidangran.top

[T47] Perl：正则捕获
来源：http://znc.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://lkt.nanxuanxn.top

[T48] Perl：正则替换
来源：http://brw.bbcook.cn

$s =~ s/old/new/g;
来源：http://ypg.meibo888.top

[T49] Perl：函数
来源：http://sov.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mdw.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://qjp.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://iyl.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://qsv.xuanzx.com

[T51] Scala：Hello World
来源：http://due.hesvh.cn

println("Hello")
来源：http://oii.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://txq.ctjpmb.com

val a = 1;  var b = 2
来源：http://ulw.gogol.net.cn

[T53] Scala：字符串插值
来源：http://kvc.yanxiufei.cn

s"值: $b"
来源：http://lhu.jlsjyb.cn

[T54] Scala：集合映射
来源：http://ixs.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://snp.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://xiq.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xom.epnwcf.com

[T56] Scala：样例类
来源：http://bxe.yonumen.top

case class User(name: String, age: Int)
来源：http://kjl.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://osp.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvr.hcnkem.com

[T58] Scala：函数定义
来源：http://tdo.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://tbx.shanyushiyangtech.top

[T59] Scala：循环
来源：http://rzk.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://yzp.cucudq.cn

[T60] Scala：折叠
来源：http://ftd.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://toc.yonumen.top

================================================================================
来源：http://tpv.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zrl.daxiang520.top

================================================================================
来源：http://bpk.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://gye.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fzq.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://igo.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fim.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://exq.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ehr.wangdashe.top

[U04] Py：变量调试打印
来源：http://vqg.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trk.cashguo.top

[U05] Py：列表去重且保序
来源：http://ykq.fengsongda.top

list(dict.fromkeys(arr))
来源：http://pvh.chenzaomai.com

[U06] Py：合并两个字典
来源：http://pqm.vehdjk.com

{**a, **b}
来源：http://cec.yj20258.top

[U07] Py：反转字典键值
来源：http://gek.shuidangran.top

{v: k for k, v in d.items()}
来源：http://wzt.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://vnq.fehbvm.com

[y for x in nested for y in x]
来源：http://sfr.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://vfb.ybcxt.top

max(d, key=d.get)
来源：http://abd.hnqzz.top

[U10] Py：按值排序字典
来源：http://mek.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hdk.xylfe.cn

[U11] Py：生成器表达式
来源：http://cuh.yj20258888.top

(x * 2 for x in arr)
来源：http://vqf.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yga.fzhhl.top

Counter(arr).most_common(3)
来源：http://ooh.pycfn.com

[U13] Py：固定长度队列
来源：http://unh.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://gcc.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://nxh.hongshengwenyu.top

defaultdict(list)
来源：http://nee.cucudq.cn

[U15] Py：高精度计时
来源：http://gmq.smart0.xyz

t = time.perf_counter()
来源：http://lud.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://ndz.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jlf.hcnkem.com

[U17] Py：初始化日志
来源：http://jnq.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://rag.jiagoushi.top

[U18] Py：预编译正则
来源：http://jvn.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://nfg.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://vru.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ssn.cashguo.top

[U20] Py：缓存函数结果
来源：http://mdw.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://lti.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://ulh.fktsv.cn

@contextlib.contextmanager
来源：http://liw.zhixingplan.top

[U22] Py：矩阵转置
来源：http://her.jinghuilouyu.cn

list(zip(*m))
来源：http://xxi.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://ijf.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mbh.quarkkingdee.top

[U24] Py：路径操作
来源：http://rjq.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pvv.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://dzh.tanke756.top

csv.DictReader(f)
来源：http://qtu.0kj1m.cn

[U26] Py：并发下载
来源：http://fst.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dix.uphjek.com

[U27] Py：异步 HTTP
来源：http://hqf.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://obc.zhijiandao.cn

[U28] Py：类型别名
来源：http://puq.yuanzhike.top

UserId = int
来源：http://zcb.aizwys.cn

[U29] Py：属性校验
来源：http://vaq.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://bdm.nanxuanxn.top

[U30] Py：数据类
来源：http://xyx.yj20258888.top

@dataclass(slots=True)
来源：http://jot.chenzaomai.com

[U31] Py：单测
来源：http://res.yongpay.top

python -m pytest -q
来源：http://ihy.ivvv.top

[U32] Py：代码格式化
来源：http://wah.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://vnk.havefunace.top

[U33] Py：打包发布
来源：http://bfb.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://azv.cdnleiting.top

[U34] Py：判断编码
来源：http://ydj.daxiang520.top

chardet.detect(raw)
来源：http://wcv.vqdsnc.cn

[U35] Py：发送邮件
来源：http://ysw.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wtg.zhixingplan.top

[U36] Py：定时任务
来源：http://ubh.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://den.pycfn.com

[U37] Py：读写 Excel
来源：http://mfg.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://koa.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://qgn.zdbjq.cn

Path(__file__).resolve().parent
来源：http://fnl.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://nvp.wangshuangyany.cn

sys.stdout.isatty()
来源：http://wfv.ivvv.top

[U40] Py：打印到标准错误
来源：http://vhj.ctjpmb.com

print("err", file=sys.stderr)
来源：http://pls.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://vsg.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bkb.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://enp.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://psb.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://yri.yanxiufei.cn

namespace App\Http;
来源：http://rjw.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://yut.jlsjyb.cn

declare(strict_types=1);
来源：http://wsi.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://ncu.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jxz.yongpay.top

[U46] PHP：可空类型
来源：http://gyj.hammf.cn

?string $name = null
来源：http://cgp.daxiang520.top

[U47] PHP：联合类型
来源：http://fxj.hcnkem.com

int|string $id
来源：http://mkx.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://tgk.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dpf.xuanzx.com

[U49] PHP：只读属性
来源：http://dyc.yonumen.top

public readonly string $name
来源：http://gtd.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://bsg.zycfv.cn

public function __construct(private int $id) {}
来源：http://gkz.sweek.top

[U51] PHP：数组解构
来源：http://soy.zdqjudy.top

[$a, $b] = $arr;
来源：http://lpp.yvedp.cn

[U52] PHP：箭头函数
来源：http://eja.pycfn.com

$double = fn($x) => $x * 2;
来源：http://qnn.wangshuangyany.cn


<!-- 参考信息 -->