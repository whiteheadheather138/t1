代发 wailian999

#ifndef X_H
来源：http://zzy.vqdsnc.cn

#define X_H
来源：http://pkk.mhx1999.top

#endif
来源：http://ubq.sysykeji.top

[S31] C++：Hello World
来源：http://rlh.cdnleiting.top

#include <iostream>
来源：http://pfe.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://uaz.xinyue.icu

[S32] C++：字符串
来源：http://pgk.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://upe.sufxvd.cn

[S33] C++：vector 增删
来源：http://utb.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zfy.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://fvd.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://kiu.cucudq.cn

[S35] C++：map
来源：http://wvb.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jks.0kj1m.cn

[S36] C++：unordered_map
来源：http://flk.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nvx.jiagoushi.top

[S37] C++：set
来源：http://lfb.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://brt.ehwqpu.com

[S38] C++：排序
来源：http://ojh.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://czs.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://ruv.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bni.zhiwuduotai.top

[S40] C++：查找元素
来源：http://yff.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kdx.sweek.top

[S41] C++：类与构造函数
来源：http://ial.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://loz.cheryme.top

[S42] C++：继承与虚函数
来源：http://nxc.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://sji.andypj.xyz

[S43] C++：智能指针
来源：http://hxp.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://exu.pycfn.com

[S44] C++：引用传参
来源：http://lwc.hnqzz.top

void inc(int &x) { ++x; }
来源：http://xgn.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://jqz.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://pgs.ydjk.org.cn

[S46] C++：函数模板
来源：http://zjg.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kit.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://tzs.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lsd.zhixingplan.top

[S48] C++：逐行读文件
来源：http://xof.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://nfw.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://qjc.hfpthk.cn

[S49] C++：写文件
来源：http://tmt.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kgf.sweek.top

[S50] C++：格式化数字
来源：http://fee.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sng.bbcook.cn

[S51] C++：显式类型转换
来源：http://lvw.cheryme.top

static_cast<double>(a) / b
来源：http://kzk.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://wsw.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://xdp.yonumen.top

[S53] C++：移动语义
来源：http://awo.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://rhq.redwolf501.top

[S54] C++：异常处理
来源：http://tyn.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kpt.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://gzi.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zsz.gotoacloud.top

[S56] C++：optional
来源：http://oqr.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zfx.chenzaomai.com

[S57] C++：编译期常量
来源：http://hvx.snrcjt.cn

constexpr int N = 10;
来源：http://uzv.guowangkeji.top

[S58] C++：命名空间
来源：http://pkb.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://ogy.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://gxb.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sdt.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://tpf.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qjb.jiagoushi.top

================================================================================
来源：http://xbw.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xqz.shanyushiyangkeji.top

================================================================================
来源：http://puv.daxiang520.top

[T01] Kotlin：Hello World
来源：http://zrw.gaohongyu789.top

println("Hello")
来源：http://zzv.redwolf501.top

[T02] Kotlin：变量
来源：http://axd.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zhw.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://xsq.dianchejie.cn

"值: $b"
来源：http://uvo.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://ptp.tianlin.xyz

val n: String? = null;  n?.length
来源：http://woo.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://iin.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vmn.yonumen.top

[T06] Kotlin：集合映射
来源：http://mfr.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qev.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://hnl.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lpt.svipenyu.cn

[T08] Kotlin：数据类
来源：http://zvb.yj202588.top

data class User(val name: String, val age: Int)
来源：http://did.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://xmy.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://ecc.yj20258.top

[T10] Kotlin：默认参数
来源：http://xqy.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qkj.smart0.xyz

[T11] Kotlin：协程
来源：http://cvy.yuanzhike.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yxd.wangdashe.top

[T12] Kotlin：解构声明
来源：http://hwo.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://pwm.yongpay.top

[T13] Kotlin：只读 Map
来源：http://oax.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://oxl.sysykeji.top

[T14] Kotlin：循环
来源：http://jjj.dianchejie.cn

for (i in 1..10) println(i)
来源：http://zag.daria6918.cn

[T15] Kotlin：接口
来源：http://ttm.jianghu66.top

interface Shape { fun area(): Double }
来源：http://qru.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://kvk.andypj.xyz

print("Hello")
来源：http://kjv.epnwcf.com

[T17] Swift：变量与常量
来源：http://ybr.tianlin.xyz

var a = 1;  let b = 2
来源：http://dii.cdnleiting.top

[T18] Swift：字符串插值
来源：http://nht.zhoulong.xyz

"值: \(b)"
来源：http://xgg.cqqwz.cn

[T19] Swift：可选绑定
来源：http://bfq.redwolf501.top

if let n = opt { print(n) }
来源：http://zij.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://tke.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hvq.gotoacloud.top

[T21] Swift：遍历
来源：http://bdr.zhijiandao.cn

for x in a { print(x) }
来源：http://ime.smart0.xyz

[T22] Swift：字典
来源：http://qyf.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pil.hongshengwenyu.top

[T23] Swift：函数
来源：http://eou.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rho.sysykeji.top

[T24] Swift：闭包
来源：http://lch.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://jiz.ybcxt.top

[T25] Swift：结构体
来源：http://ixq.xylfe.cn

struct P { var x: Int }
来源：http://toq.mhx1999.top

[T26] Swift：类与重写
来源：http://arg.ivvv.top

class A: Base { override func f() {} }
来源：http://uxx.chenzaomai.com

[T27] Swift：错误处理
来源：http://ztm.c1oappe.top

do { try f() } catch { print(error) }
来源：http://wsm.jlsjyb.cn

[T28] Swift：枚举
来源：http://bac.chenzaomai.com

enum Color { case red, green }
来源：http://wye.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://zco.havefunace.top

guard let x = opt else { return }
来源：http://nag.yfazqb.com

[T30] Swift：协议
来源：http://cvh.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://dto.pengpengdd.cyou

[T31] Lua：Hello World
来源：http://dqw.pycfn.com

print("Hello")
来源：http://pvm.gotoacloud.top

[T32] Lua：局部变量
来源：http://axy.jianghu66.top

local a = 1
来源：http://unq.cashguo.top

[T33] Lua：表（数组）
来源：http://sjk.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://lhs.vehdjk.com

[T34] Lua：遍历表
来源：http://xlp.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zxg.pycfn.com

[T35] Lua：字典表
来源：http://akr.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://ysc.0kj1m.cn

[T36] Lua：函数
来源：http://tea.haohaochexian.top

function add(a, b) return a + b end
来源：http://teb.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://zbj.quarkkingdee.top

"a" .. "b"
来源：http://upo.tian-w.cn

[T38] Lua：条件
来源：http://dju.hcnkem.com

if x > 0 then print("正") end
来源：http://gun.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://wlh.tian-w.cn

string.find(s, "%d+")
来源：http://fsd.xuanzx.com

[T40] Lua：元表
来源：http://xbf.xziqi.cn

setmetatable({}, { __index = base })
来源：http://doa.hfpthk.cn

[T41] Perl：Hello World
来源：http://byc.guowangkeji.top

print "Hello\n";
来源：http://crg.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://knt.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gsg.chenzaomai.com

[T43] Perl：字符串插值
来源：http://acy.zhongyouzk.top

"值: $a"
来源：http://vue.ivvv.top

[T44] Perl：条件
来源：http://rfn.havefunace.top

if ($a > 0) { print "正"; }
来源：http://icc.c1oappe.top

[T45] Perl：数组遍历
来源：http://abg.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://mmu.zhengqikj.top

[T46] Perl：哈希操作
来源：http://mtf.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xuu.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://lae.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kws.mhx1999.top

[T48] Perl：正则替换
来源：http://goz.sufxvd.cn

$s =~ s/old/new/g;
来源：http://pjf.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://jmd.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wqg.xylfe.cn

[T50] Perl：逐行读文件
来源：http://mrs.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://trg.meibo888.top

while (my $line = <$fh>) { print $line; }
来源：http://fhs.xinyue.icu

[T51] Scala：Hello World
来源：http://lvx.fehbvm.com

println("Hello")
来源：http://mgs.uphjek.com

[T52] Scala：变量
来源：http://djy.tarul.cn

val a = 1;  var b = 2
来源：http://trb.ehwqpu.com

[T53] Scala：字符串插值
来源：http://tcg.dashuyun.cn

s"值: $b"
来源：http://ukz.hammf.cn

[T54] Scala：集合映射
来源：http://rvp.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://jab.tanke756.top

[T55] Scala：集合过滤
来源：http://qaf.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://xjn.tarul.cn

[T56] Scala：样例类
来源：http://fkr.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://gds.jinqigufen.top

[T57] Scala：模式匹配
来源：http://qrl.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uof.snrcjt.cn

[T58] Scala：函数定义
来源：http://jmu.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://vos.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://gmr.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://vdf.yueranfly.top

[T60] Scala：折叠
来源：http://yrn.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kva.chenlongwang.top

================================================================================
来源：http://wrp.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pbz.svipenyu.cn

================================================================================
来源：http://hge.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://vri.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lsl.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://uil.gotoacloud.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jlj.yj202588.top

[U03] Py：加载 .env 配置
来源：http://llc.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kzd.yvedp.cn

[U04] Py：变量调试打印
来源：http://eus.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://znd.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://inf.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://uuc.aizwys.cn

[U06] Py：合并两个字典
来源：http://umj.chenlongwang.top

{**a, **b}
来源：http://xqe.cucudq.cn

[U07] Py：反转字典键值
来源：http://bfr.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://bzd.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://nyw.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://hif.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://gfd.yj202588.top

max(d, key=d.get)
来源：http://dkf.nanxinkj.top

[U10] Py：按值排序字典
来源：http://lok.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pqe.smart0.xyz

[U11] Py：生成器表达式
来源：http://jqw.tanke756.top

(x * 2 for x in arr)
来源：http://zib.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://wmh.yj20258.top

Counter(arr).most_common(3)
来源：http://sjo.fengsongda.top

[U13] Py：固定长度队列
来源：http://aui.chenzaomai.com

deque(maxlen=10)
来源：http://qwx.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://uua.sweek.top

defaultdict(list)
来源：http://pip.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://kve.smart0.xyz

t = time.perf_counter()
来源：http://mex.pycfn.com

[U16] Py：命令行参数解析
来源：http://kyh.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://euc.yj202588.top

[U17] Py：初始化日志
来源：http://irr.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://hcl.hcnkem.com

[U18] Py：预编译正则
来源：http://cet.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://yht.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://mdi.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sxp.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://wox.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://baq.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://tvp.hnqzz.top

@contextlib.contextmanager
来源：http://ctm.cucudq.cn

[U22] Py：矩阵转置
来源：http://wun.jinyuanbaomall.cn

list(zip(*m))
来源：http://tyw.52xcode.cn

[U23] Py：分块读取大文件
来源：http://zky.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mbb.andypj.xyz

[U24] Py：路径操作
来源：http://jyi.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qsg.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://eba.gaohongyu789.top

csv.DictReader(f)
来源：http://wrr.kuanghao11.cn

[U26] Py：并发下载
来源：http://aju.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tzm.yj202588.top

[U27] Py：异步 HTTP
来源：http://gyx.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://kya.gaohongyu789.top

[U28] Py：类型别名
来源：http://tza.shangyingyoupin.top

UserId = int
来源：http://vst.snrcjt.cn

[U29] Py：属性校验
来源：http://vdm.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://due.yonumen.top

[U30] Py：数据类
来源：http://jro.yanxiufei.cn

@dataclass(slots=True)
来源：http://ihk.smart0.xyz

[U31] Py：单测
来源：http://fhp.wangshuangyany.cn

python -m pytest -q
来源：http://qco.xylfe.cn

[U32] Py：代码格式化
来源：http://wgl.ivvv.top

ruff format . && ruff check --fix .
来源：http://wmk.c1oappe.top

[U33] Py：打包发布
来源：http://dzl.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://ylw.yongpay.top

[U34] Py：判断编码
来源：http://zze.yj202588.top

chardet.detect(raw)
来源：http://rpj.snrcjt.cn

[U35] Py：发送邮件
来源：http://mmh.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tui.yonumen.top

[U36] Py：定时任务
来源：http://rti.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://gdr.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://uwb.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://mvd.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://wpf.jianghu66.top

Path(__file__).resolve().parent
来源：http://mii.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://lng.sxryk.cn

sys.stdout.isatty()
来源：http://oue.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://cqi.sysykeji.top

print("err", file=sys.stderr)
来源：http://byv.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://sjr.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dae.fktsv.cn

[U42] PHP：PSR-4 自动加载
来源：http://uzp.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mhs.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://xxt.havefunace.top

namespace App\Http;
来源：http://fzr.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://jjt.xziqi.cn

declare(strict_types=1);
来源：http://jwg.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://vxj.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://udq.xuanzx.com

[U46] PHP：可空类型
来源：http://qct.zhengqikj.top

?string $name = null
来源：http://rku.hnqzz.top

[U47] PHP：联合类型
来源：http://exl.hesvh.cn

int|string $id
来源：http://brj.aizwys.cn

[U48] PHP：纯枚举
来源：http://nvs.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ftd.hywenlv.cn

[U49] PHP：只读属性
来源：http://aek.epnwcf.com

public readonly string $name
来源：http://oou.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://coc.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://kfh.hfpthk.cn

[U51] PHP：数组解构
来源：http://lzq.jyoumei.cn

[$a, $b] = $arr;
来源：http://xhp.smart0.xyz

[U52] PHP：箭头函数
来源：http://ype.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://guv.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://jhz.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://aqx.c1oappe.top

[U54] PHP：空安全调用
来源：http://tlu.guowangkeji.top

$obj?->method()
来源：http://gwk.guannengcc.top


<!-- 参考信息 -->